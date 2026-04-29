# Mechatronics_Investigation

Proyecto interactivo "Mechatronics Clue" — listo para desplegar en GitHub Pages.

Instrucciones rápidas de despliegue:

1. Asegúrate de que el repositorio contiene los archivos en la raíz (`index.html`, `data.json`, carpetas `js/`, `Images/`, `Sound/`).
2. Empuja los cambios al branch `main` (o a la rama que uses para Pages).
3. En GitHub > Settings > Pages, configura Source: `main` branch / root (`/`).
4. Opcional: si usas la rama `gh-pages`, crea la rama y configura Pages desde ahí.

Probar localmente:

```bash
# desde la raíz del proyecto
python3 -m http.server 8000
# abrir http://localhost:8000
```

Notas:
- Se incluyó `404.html` que redirige a `/` para compatibilidad con GitHub Pages.
- El cargador principal usa módulos ES desde `js/main.js`; abre el sitio desde un servidor (no `file://`).
