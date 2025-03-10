3. Ejemplo Real: Layout de Blog
Vamos a ver cómo usar CSS Grid para crear un diseño típico de blog con un encabezado, contenido principal, barra lateral y
pie de página.

/* Layout de blog */
.grid-contenedor {
display: grid;
grid-template-areas:
"header header" /* Fila 1: El encabezado ocupa todo el ancho */
"main sidebar" /* Fila 2: Contenido principal y barra lateral */
"footer footer"; /* Fila 3: El pie de página ocupa todo el ancho */
grid-template-columns: 3fr 1fr; /* Tres columnas principales y una mas pequena */

.header { grid-area: header; } /* Coloca el encabezado en la zona "header" */
/* Coloca el contenido principal en la zona "main" */
.main { grid-area: main; }
. sidebar{ grid-area: sidebar; }/* Coloca la barra lateral en la zona "sidebar" */
. footer { grid-area: footer; } /* Coloca el pie de pagina en la zona "footer" */
