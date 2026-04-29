# Mechatronics_Investigation

Proyecto interactivo "Mechatronics Clue" — listo para desplegar en GitHub Pages.

## Temática

Mechatronics Clue es un juego narrativo de investigación ambientado en una planta industrial. El jugador asume el rol de un inspector de calidad que debe resolver una falla en la Línea 3 observando pistas, revisando expedientes y tomando una acusación final sobre quién, qué y dónde provocó el incidente.

La experiencia mezcla estética industrial con una historia tipo detective: paneles de control, rutas de inspección, archivadores técnicos, mapas de planta y pantallas de veredicto. Todo el juego está construido para funcionar como una investigación guiada, con sonido, imágenes y rutas visuales coherentes con el entorno de fábrica.

## Qué incluye

- 4 personajes jugables/seleccionables con imagen en `Images/`.
- 5 locaciones de investigación dentro de la planta.
- 5 tipos de falla posibles.
- Sistema de pistas, expediente y acusación final.
- 5 historias precargadas con combinaciones consistentes.
- Soporte para GitHub Pages con `404.html` de respaldo.

## Capturas

Vista rápida del juego en sus pantallas principales:

![Pantalla 1](Capturas/Pantalla%201.png)

![Pantalla 2](Capturas/Pantalla%202.png)

![Pantalla 3](Capturas/Pantalla%203.png)

![Pantalla 4](Capturas/Pantalla%204.png)

Instrucciones rápidas de despliegue:

1. Asegúrate de que el repositorio contiene los archivos en la raíz (`index.html`, `data.json`, carpetas `js/`, `Images/`, `Sound/`, `Capturas/`).
2. Empuja los cambios al branch `main` (o a la rama que uses para Pages).
3. En GitHub > Settings > Pages, configura Source: `main` branch / root (`/`).
4. Opcional: si usas la rama `gh-pages`, crea la rama y configura Pages desde ahí.

## Estructura

- `index.html`: interfaz principal y contenedores de pantallas.
- `data.json`: contenido narrativo principal usado por el juego.
- `data.js`: respaldo local cuando no se carga JSON.
- `js/`: módulos del juego, estado, mapa, UI, flujo y utilidades.
- `Images/`: arte e iconografía del juego.
- `Sound/`: música y efectos de ambiente.
- `Capturas/`: imágenes usadas en este README.

## Cómo jugar

1. Abre el juego desde un servidor local o desde GitHub Pages.
2. Revisa el briefing inicial para entender el caso.
3. Investiga al menos 3 locaciones para habilitar la acusación.
4. Compara sospechosos, causa y lugar con las pistas recolectadas.
5. Presenta tu acusación y revisa el veredicto final.

## Detalles útiles

- El juego usa módulos ES y por eso debe abrirse desde HTTP, no desde `file://`.
- Las rutas de imágenes y sonidos son relativas al directorio raíz.
- Si el navegador muestra un `404` de `favicon.ico`, no afecta el funcionamiento.

Probar localmente:

```bash
# desde la raíz del proyecto
python3 -m http.server 8000
# abrir http://localhost:8000
```

Notas:
- Se incluyó `404.html` que redirige a `/` para compatibilidad con GitHub Pages.
- El cargador principal usa módulos ES desde `js/main.js`; abre el sitio desde un servidor (no `file://`).
