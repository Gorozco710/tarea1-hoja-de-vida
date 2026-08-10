Parte 2, Medicion de imagenes

Original (JFIF): 25.8 KB, Imagen original.
JPG: 46.3 KB, Se ve bien, pero aumentó de peso respecto al original debido a la recodificación.
PNG: 256 KB, Conserva la calidad sin pérdida, pero genera el peso más alto por mucho.
WebP: 35.1 KB, Buena calidad visual, aunque aumentó de peso frente al archivo JFIF base.
AVIF: 24.7 KB,  Excelente calidad visual con el peso de archivo más bajo de todos (superando al original).

5) Use como opcion principal AVIF ya que el es mas liviano y moderno, como segunda opcion Webp por si algun navegador antiguo no pudiera leer avif, es un poco mas pesado pero mas compatible y como ultima opcion use jpg por si el navegador es todavia mas antiguo quesda como ultima opcion.
6) El resultado vario en los distintos formatos ya que la imagen original, de por si ya venia en un formato comprimido pero menos compatible con los navegadores, al cambiarlo a los diferentes formatos aumento considerablemente su peso.

Tarea 3:

1) Contenedores e Ítems:
 Header (Flexbox): El contenedor es `<header>` y sus ítems son `<h1>`, `<picture>` y los `<p>`.
 Main (Grid): El contenedor es `<main>` y sus ítems son las etiquetas `<section>`.
 Formulario (Flexbox): El contenedor es `<form>` y sus ítems son los bloques `.campo-form` y el `<button>`.

2) Justificación Flexbox vs Grid:
 Flexbox: Lo usé en header y formulario porque el diseño es unidimensional.
 Grid: Lo usé en el main porque organiza la estructura principal en dos dimensiones que son filas y columnas adaptables.

3) Adaptación autónoma:
 Usé `grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));` en el `<main>`.
 `auto-fit` calcula las columnas según el espacio disponible y `minmax(280px, 1fr)` colapsa las secciones a una sola columna cuando la pantalla mide menos de 280px, sin depender de un `@media`.

4) Respuestas:
 Eje en Flexbox: Al cambiar la dirección a columna (`flex-direction: column`), la propiedad que centra horizontalmente pasa a ser `align-items`.
 Fracciones vs Porcentajes: Las fracciones (`fr`) reparten el espacio sobrante restando los espacios de `gap`, usar porcentajes ignora el `gap` y provoca desbordamientos en pantalla.
 Etiqueta meta viewport: Define el área visible y escala la página a 1:1 con el tamaño real del pantalla del dispositivo, sin ella, el teléfono renderiza como pantalla de escritorio y todo se ve microscópico.
