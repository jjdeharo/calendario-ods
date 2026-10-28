# Calendario ODS

Calendario de los días internacionales relacionados con los Objetivos de Desarrollo Sostenible (ODS), con propuestas de actividades para el aula y la opción de abrir un chatbot de IA con una petición ya preparada para crear una actividad. En castellano y catalán.

Versión en uso: <https://bilateria.org/app/ods/>

## Cómo funciona

Es una página estática, sin servidor ni cuentas: `index.html` carga los datos de dos archivos JSON.

- `ods-data.json`: los 17 ODS, con su color, título, descripción y metas.
- `events-data.json`: los días internacionales, con los ODS con que se relacionan y las actividades propuestas.

Para probarla en local hace falta servirla, porque el navegador no deja cargar los JSON desde `file://`:

```bash
python3 -m http.server 8000
```

## Autoría y licencia

Aplicación de Juan José de Haro ([@jjdeharo](https://bilateria.org)), creada en cocreación con IA ([MIAE, nivel 4](https://jjdeharo.github.io/miae/?nivel=4)).

- Código: [AGPL v3](LICENSE).
- Contenidos (textos, datos de los ODS y de los días internacionales, actividades propuestas): [CC BY-SA 4.0](LICENSES/CC-BY-SA-4.0.txt).
