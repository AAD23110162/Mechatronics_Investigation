# Mechatronics Investigation

### Autor: Alejandro Aguire Díaz

### Demo en línea: https://aad23110162.github.io/Mechatronics_Investigation/

## Descripcion
Mechatronics Investigation es un juego web estática que simula una experiencia interactiva de investigación en una planta industrial. El usuario asume el rol de inspector y, mediante la navegación por un mapa de planta, recopilación de pistas y manejo de expedientes, intenta identificar la causa y el responsable de una falla.


## Características principales
- Interfaz interactiva con mapa de planta y localizaciones clicables.
- Sistema de pistas y expediente que habilita una acusación final.
- Casos/historias precargadas gestionadas desde `data.json`/`data.js`.
- Recursos multimedia: imágenes en `Images/` y sonidos en `Sound/`.
- Compatible con GitHub Pages (incluye `404.html` para redirecciones SPA).

## Tecnologías
- HTML5, CSS3 (variables y layout responsivo).
- JavaScript moderno (módulos ES): `main.js`, `ui.js`, `state.js`, `map.js`, `helpers.js`, `flowchart.js`.
- JSON para contenido narrativo (`data.json`).

## Requisitos
- Navegador moderno con soporte ES Modules.
- Servidor HTTP para servir archivos estáticos (no funciona correctamente abriendo `index.html` por `file://`).

## Ejecutar localmente
1. Clona el repositorio en tu máquina.
2. Desde la raíz del proyecto, ejecuta un servidor HTTP simple. Ejemplo con Python:

```bash
python3 -m http.server 8000
# abrir http://localhost:8000
```

O con Node (si prefieres):

```bash
npm install -g http-server
http-server -c-1 . 8000
# abrir http://localhost:8000
```

## Estructura del repositorio (resumen)
Se incluyen los archivos y carpetas principales que conforman la aplicación. La carpeta `PROTOTIPO_V2.0/` existe en el repositorio pero no se documenta en detalle aquí.

- [index.html](index.html): página principal y contenedores de UI.
- [styles.css](styles.css): estilos globales del proyecto.
- [data.json](data.json): contenido narrativo (historias, personajes, locaciones, causas).
- [data.js](data.js): respaldo/alternativa para carga de datos.
- [main.js](main.js): inicialización y orquestación de módulos.
- [ui.js](ui.js): gestión de componentes y eventos de la interfaz.
- [state.js](state.js): gestión del estado del juego y progreso del usuario.
- [map.js](map.js): lógica de interacción y render del mapa de planta.
- [flowchart.js](flowchart.js): utilidades y flujo de la narrativa.
- [helpers.js](helpers.js): funciones auxiliares reutilizables.
- [Images/](Images/): recursos gráficos (personajes, íconos, fondos).
- [Sound/](Sound/): archivos de audio y efectos.
- [Capturas/](Capturas/): capturas de pantalla y material visual.




