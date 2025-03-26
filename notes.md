touch shopify.theme.toml
shopify theme pull -e development
shopify theme dev -e development
shopify theme push -e development

sync changes on the CMS locally: shopify theme pull -d

Snippets = components
assets = videos, fotos, css, javascript
layout = diferentes layouts de paginas

templates = aqui se guardan las instancias y los datos que el usuario ha escrito desde el editor del CMS. Titulos, subitulos....
En el index.json se guardan los de la pagina principal.
Pueden ser tanto jsons como liquid files. Los liquid files son cosas hardcodeadas y los jsons son instancias de secciones.
Las que tienen un ID como key son las que se han añadido desde el CMS
Se puede poner una propiedad layout (password.json) para elegir que layout usara. Si no se especifica usara el theme.liquid por defecto

{% schema %} solo se puede usar en sections. Es un JSON que permite controlar como funciona la seccion.
