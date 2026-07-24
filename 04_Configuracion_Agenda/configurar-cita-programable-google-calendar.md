# Configurar "Cita programable" en Google Calendar

Requiere cuenta de **Google Workspace** (ej. `@solut.cl`) — la "Programación de citas" no está disponible en cuentas Gmail gratuitas.

## Pasos

1. Entra a [calendar.google.com](https://calendar.google.com) con la cuenta que administrará las reuniones (ej. `fmatamala@solut.cl` o una cuenta compartida tipo `agenda@geosom.cl` si prefieren separarlo).
2. (Opcional pero recomendado) Crea un calendario nuevo llamado **"GEOSOM - Reuniones"** para no mezclar con tu calendario personal: *Otros calendarios* → **+** → *Crear calendario nuevo*.
3. Click en **Crear** (botón azul, esquina superior izquierda) → **Programación de citas** (Appointment schedule).
4. Vas a crear **dos programaciones distintas** (según el guion en `03_Flujo_Conversacional/`):

### A. "Reunión técnica y evaluación económica" (prospectos calificados)
- Duración sugerida: 45–60 min
- Calendario asociado: GEOSOM - Reuniones
- Disponibilidad: bloques donde el equipo técnico realmente pueda atender (dejar buffer de 15 min entre reuniones)
- Formulario de reserva — pedir:
  - Nombre y apellido
  - Empresa / organización
  - Email corporativo
  - Teléfono
  - Tipo de proyecto (campo libre — o pre-llenado si viene del asistente con los datos de calificación)
- Notificaciones: activar confirmación y recordatorio por email (24h y 1h antes)

### B. "Llamada corta" (proyectos pequeños / personas naturales — ver sección 3 del guion)
- Duración sugerida: 15–20 min
- Mismo calendario o uno separado
- Formulario más simple: nombre, teléfono, email

5. Al guardar cada una, Google genera una **URL pública de reserva** (tipo `calendar.google.com/calendar/appointments/schedules/...`). Cópiala.
6. Pégame esos dos links aquí (o los agrego yo directo al repo) para:
   - Insertarlos en `03_Flujo_Conversacional/guion-calificacion-prospectos.md` (sección 4, reemplazando `[Link agenda virtual]`)
   - Dejarlos disponibles para quien construya el bot (WhatsApp/web)

## Pendiente

- [ ] Confirmar que la cuenta usada tiene Google Workspace activo
- [ ] Decidir si se usa una cuenta personal (`fmatamala@solut.cl`) o una cuenta/calendario compartido del equipo
- [ ] Crear las 2 programaciones y devolver los links
