# Proyecto Rutinas

App web para seguir rutinas de gimnasio desde el celular o la compu. Es un único archivo (`index.html`), sin instalación: se abre en el navegador.

## Funciones

- **Rutina con el formato del Word**: días con encabezado, tabla Ejercicio / Series × Reps / Descanso y ejercicios básicos resaltados.
- **Cargar rutinas**: subí un Word (.docx) o un .txt, o pegá el texto; la app detecta días y ejercicios.
- **Marcar como hecho** cada serie y cada ejercicio, con el avance del día.
- **Cronómetro por ejercicio** y **temporizador de descanso** automático (suena y vibra al terminar).
- **Registro de pesos**: kg y repeticiones por serie, "última vez" de la semana anterior y sugerencia de subir peso.
- **Precalentamiento por ejercicio**: movilidad específica y series de aproximación con los kilos calculados.
- **Bloque de fuerza** opcional desde la semana 5 (primer básico a 4 × 4-6).
- **Planilla semanal** que se completa sola y **copia de seguridad** en JSON.

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
