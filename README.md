# Proyecto Rutinas

App web para seguir rutinas de gimnasio desde el celular o la compu. Es un único archivo (`index.html`), sin instalación: se abre en el navegador.

## Funciones

- **Pensada para celular**: barra de pestañas abajo, botones grandes y +/− para cargar kilos y repeticiones.
- **Varias personas, una rutina**: cada persona tiene su color, su semana y sus propios pesos, tiempos y descansos. Se cambia de persona con un toque arriba (ideal para entrenar de a dos con un solo celular).
- **Entrada en calor con cardio**: bicicleta, caminadora, elíptico o escaladora, con temporizador de 5 a 15 minutos.
- **Precalentamiento por ejercicio** (opcional, plegado): movilidad y series de aproximación con los kilos calculados. Se puede ocultar en Personas.
- **Marcar como hecho** cada serie y cada ejercicio; al terminar uno se abre el siguiente.
- **Cronómetro por ejercicio** y **descanso automático** por persona (suena y vibra al terminar). Si bloqueás el celular, al volver el descanso sigue ahí y muestra el tiempo extra (+0:42).
- **Notas** por ejercicio y por día, y opción "Hoy no lo hice".
- **Compartir historial** (último entreno, semana o todo): mensaje armado para WhatsApp o para pasarle a una IA, descarga en .txt o JSON.
- **Importar historial** en JSON (el mismo formato que exporta: `usuario`, `sesiones[]` con `fecha`, `dia`, `ejercicios[]`).
- **Registro de pesos**: "última vez" de la semana anterior, sugerencia de subir peso e historial por persona.
- **Cargar rutinas** desde Word (.docx), .txt o texto pegado.
- **Bloque de fuerza** opcional desde la semana 5 (primer básico a 4 × 4-6).
- Mantiene la pantalla encendida mientras entrenás y permite **copias de seguridad** en JSON.

## Uso

Abrí `index.html` en el navegador, o activá GitHub Pages (Settings → Pages → rama `main`) para usarla desde el celular.

Los datos se guardan en el navegador (localStorage). Para pasarlos a otro dispositivo usá "Descargar copia" y "Restaurar copia" en la pestaña Personas.

### Nube (Supabase) y Progreso Gym

En **Personas → Cuenta y nube** podés iniciar sesión con la misma cuenta de
[Progreso Gym](https://github.com/LucasIbanez13/proyecto-llevar-peso). Al estar conectado:

- Todo (personas, semanas, pesos, rutina) se guarda en la nube y se sincroniza entre dispositivos.
- Los pesos de la persona elegida en **"Mis pesos son los de"** se copian al historial de Progreso Gym
  (tabla `workout_sets`), donde se calculan 1RM, progresión y proyección semanal.
- **Enviar rutina a Progreso Gym** reemplaza los días y ejercicios de esa app por los de esta.

Requiere haber ejecutado `supabase/schema.sql` y `supabase/02_conexion_proyecto_rutinas.sql`
del repositorio de Progreso Gym. La URL y la clave *publishable* de Supabase están al principio del `<script>`.

### Formato de texto aceptado

```
DÍA 1 – TORSO A (Empuje)
Press de banca | Básico | 3 × 6-8 | 3 min
Press militar | Accesorio | 3 × 8-10 | 90 seg
DÍA 2 – PIERNA
Sentadilla 4x5 3 min
Plancha 3x30-45 seg 60 seg
```
