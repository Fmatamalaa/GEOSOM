# Configurar agenda virtual con Calendly — GEOSOM

Reemplaza el intento de usar "Programación de citas" de Google Calendar (no disponible con el plan de Workspace actual — ver `configurar-cita-programable-google-calendar.md`, queda como referencia histórica).

## Por qué Calendly

- No depende del plan de Google Workspace — funciona con cualquier cuenta.
- Se conecta a Google Calendar solo para **leer disponibilidad y evitar dobles reservas** (esto sí funciona en el plan gratuito de Calendly, es una conexión estándar de OAuth).

## Plan necesario

GEOSOM necesita **2 tipos de evento** (reunión técnica completa + llamada corta, ver `03_Flujo_Conversacional/guion-calificacion-prospectos.md` sección 4). El plan **gratuito de Calendly solo permite 1 tipo de evento activo**. Para tener los 2, se necesita el plan **Standard** (~US$10-12/mes).

> Si se va a usar la misma cuenta de Calendly para GEOSOM y SOLUT juntos (3 tipos de evento en total: 2 de GEOSOM + 1 de SOLUT), también se necesita el plan Standard.

## Pasos

1. Entra a [calendly.com](https://calendly.com) y crea una cuenta con `fmatamala@solut.cl` (o el correo que administrará las reuniones).
2. Conecta tu Google Calendar: *Account* → *Connected Calendars* → agregar `fmatamala@solut.cl`. Esto sincroniza tu disponibilidad real.
3. Si necesitas los 2 tipos de evento, activa el plan **Standard** (prueba gratuita disponible).
4. Crea el primer tipo de evento: **"Reunión técnica y evaluación económica"**
   - Duración: 45–60 min
   - Disponibilidad: los bloques reales del equipo técnico, con buffer de 15 min
   - Preguntas del formulario de reserva (además de nombre/email/teléfono que pide Calendly por defecto):
     - Empresa / organización
     - Tipo de proyecto
     - Etapa del proyecto
   - Notificaciones/recordatorios: activar email 24h y 1h antes
5. Crea el segundo tipo de evento: **"Llamada corta"**
   - Duración: 15–20 min
   - Formulario más simple (nombre, teléfono, email)
6. Cada tipo de evento genera su propia URL pública (ej. `calendly.com/fmatamala-solut/reunion-tecnica-geosom`). Copia ambas.
7. Pásame los 2 links para insertarlos en `03_Flujo_Conversacional/guion-calificacion-prospectos.md` (sección 4, reemplazando `[Link agenda virtual]`).

## Pendiente

- [ ] Crear cuenta Calendly y conectar Google Calendar
- [ ] Decidir si se activa plan Standard ahora o se parte solo con 1 tipo de evento (gratis) y se agrega el segundo después
- [ ] Crear los 2 tipos de evento y devolver los links
