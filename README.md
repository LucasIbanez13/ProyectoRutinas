# Proyecto Rutinas

App web para seguir rutinas de gimnasio desde el celular o la compu. Es un único archivo (`index.html`), sin instalación: se abre en el navegador.

## Funciones

- **Pensada para celular**: barra de pestañas abajo, botones grandes y +/− para cargar kilos y repeticiones.
- **Varias personas, una rutina**: cada persona tiene su color, su semana y sus propios pesos, tiempos y descansos. Se cambia de persona con un toque arriba (ideal para entrenar de a dos con un solo celular).
- **Entrada en calor con cardio**: bicicleta, caminadora, elíptico o escaladora, con temporizador de 5 a 15 minutos.
- **Precalentamiento por ejercicio**: movilidad específica y series de aproximación con los kilos calculados.
- **Marcar como hecho** cada serie y cada ejercicio; al terminar uno se abre el siguiente.
- **Cronómetro por ejercicio** y **descanso automático** por persona (suena y vibra al terminar).
- **Registro de pesos**: "última vez" de la semana anterior, sugerencia de subir peso e historial por persona.
- **Cargar rutinas** desde Word (.docx), .txt o texto pegado.
- **Bloque de fuerza** opcional desde la semana 5 (primer básico a 4 × 4-6).
- Mantiene la pantalla encendida mientras entrenás y permite **copias de seguridad** en JSON.

## Uso

Abrí `index.html` en el navegador, o activá GitHub Pages (Settings → Pages → rama `main`) para usarla desde el celular.

Los datos se guardan en el navegador (localStorage). Para pasarlos a otro dispositivo usá "Descargar copia" y "Restaurar copia" en la pestaña Rutina.

### Formato de texto aceptado

```
DÍA 1 – TORSO A (Empuje)
Press de banca | Básico | 3 × 6-8 | 3 min
Press militar | Accesorio | 3 × 8-10 | 90 seg
DÍA 2 – PIERNA
Sentadilla 4x5 3 min
Plancha 3x30-45 seg 60 seg
```
