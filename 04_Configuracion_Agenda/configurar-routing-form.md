# Automatizar la calificación con Calendly Routing Forms — GEOSOM

Mismo mecanismo que en [SOLUT](https://github.com/Fmatamalaa/SOLUT/blob/main/04_Configuracion_Agenda/configurar-routing-form.md): el prospecto responde un formulario corto y Calendly lo redirige solo, replicando `03_Flujo_Conversacional/guion-calificacion-prospectos.md` sección 3.

## Pasos para crearlo

1. En Calendly → **Routing** → **Create routing form**.
2. Nombre: **"Calificación de proyecto - GEOSOM"**.
3. Preguntas (multiple choice salvo la última):

   **P1 — ¿Con cuál de estas opciones te identificas?**
   - Inmobiliaria / Constructora
   - Municipio / sector público
   - Arquitecto / oficina de ingeniería
   - Empresa de perforación
   - Empresa con edificio propio (oficina, colegio, hospital, etc.)
   - Fondo de inversión / inversionista climático
   - Persona particular (vivienda propia)
   - Otro

   **P2 — ¿En qué etapa está tu proyecto?**
   - Idea / evaluando factibilidad
   - En diseño (aún no hay obra)
   - En construcción
   - Ya construido / operando

   **P3 — ¿Para cuándo te gustaría avanzar?**
   - Urgente (próximas semanas)
   - Este trimestre
   - Este año
   - Aún explorando, sin fecha

   **P4 — Datos de contacto** (short answer / email / phone)
   - Nombre y apellido
   - Empresa / organización
   - Email
   - Teléfono
   - Comuna/región del proyecto

4. **Routing logic**, en este orden de prioridad:

   | Regla | Condición | Acción |
   |---|---|---|
   | 1 | P1 = "Persona particular (vivienda propia)" | Redirigir al evento **Llamada corta**: `https://calendly.com/fmatamala-solut/30min` |
   | 2 | P2 = "Idea / evaluando factibilidad" **Y** P3 = "Aún explorando, sin fecha" | Mostrar **mensaje personalizado** (texto abajo) |
   | 3 | Cualquier otro caso | Redirigir al evento **Reunión técnica y evaluación económica**: `https://calendly.com/fmatamala-solut/new-meeting` |

   > Nota de orden: la regla 1 va primero porque una persona natural siempre se deriva a la llamada corta, sin importar la etapa o urgencia (así está definido en el guion, sección 3).

5. Texto del mensaje personalizado (regla 2):

```
¡Gracias por contarme sobre tu proyecto! Por ahora parece que están en una etapa temprana, así que te dejo contenido para que conozcas mejor cómo funciona GEOSOM:

- GEOSOM transforma el calor del subsuelo en energía limpia comercializable y 100% trazable, con simulación previa (gemelos digitales + BIM) antes de excavar.
- Contamos con respaldo de CORFO (programa Semilla Inicia).
- Aplica a viviendas, edificios, colegios, hospitales y proyectos de distrito.

Cuando tengas más definido el proyecto, contáctanos directo: +56 9 3006 2244 / contacto@geosom.cl / www.geosom.cl
```

6. **Publica** y copia el link del formulario.

## Dónde usar el link

- Reemplaza el link de **Featured/Destacado** en LinkedIn cuando publiques contenido de GEOSOM (en vez del link directo del evento).
- Actualiza `03_Flujo_Conversacional/guion-calificacion-prospectos.md` con el link publicado, igual como se hizo en el repo SOLUT.

## Pendiente

- [ ] Crear el formulario en Calendly con las reglas de arriba
- [ ] Publicar y devolver el link
- [ ] Preparar el próximo post de LinkedIn para GEOSOM (contenido ya disponible en `02_Marketing/resumen-grilla-contenido.md`)
