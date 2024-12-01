Documentación del Proyecto: Página Web del Supermercado
1. Descripción del Proyecto
Este proyecto consiste en el desarrollo de una página web para un supermercado. El sitio incluye información relevante sobre el supermercado, promociones, productos destacados y una interfaz de usuario amigable. La página está diseñada de manera responsiva, lo que significa que se adapta a diferentes dispositivos, desde computadoras de escritorio hasta móviles, utilizando Bootstrap como framework principal.

Objetivos:

Crear una página web visualmente atractiva y fácil de navegar para un supermercado.
Implementar funcionalidades interactivas utilizando JavaScript.
Usar Bootstrap para garantizar que la página sea completamente responsiva.
Subir el proyecto a un hosting gratuito para que sea accesible en línea.
2. Herramientas Utilizadas
Lenguajes y Tecnologías:
HTML5: Para la estructura de la página.
CSS3: Para el estilo y diseño visual del sitio.
JavaScript: Para agregar interactividad y dinámica a la página.
Bootstrap: Framework CSS para crear una página web responsiva de manera rápida y eficiente.
Editor de Código:
Visual Studio Code: Utilizado para editar y organizar los archivos HTML, CSS, JavaScript.
Bibliotecas y Frameworks:
Bootstrap 5: Framework para el diseño responsivo y componentes predefinidos como botones, tarjetas y barras de navegación.
Hosting:
GitHub Pages: Utilizado para alojar el proyecto de forma gratuita.


3. Estructura del Proyecto
La estructura de archivos del proyecto es la siguiente:

python
Copiar código
mi-proyecto/
├── index.html             # Página principal del proyecto
├── css/
│   └── bootstrap.min.css  # Archivo CSS de Bootstrap (copiado desde la descarga)
├── js/
│   ├── bootstrap.bundle.min.js  # Archivo JS de Bootstrap (copiado desde la descarga)
│   └── script.js          # Script personalizado con interactividad
├── img/
│   └── supermercado.jpg   # Imagen de ejemplo para el sitio web
Explicación de Archivos y Carpetas:

index.html: Contiene la estructura principal de la página, incluyendo el encabezado, la barra de navegación, las secciones de productos y promociones, y el pie de página.
css/: Contiene los archivos de estilo, incluyendo Bootstrap para facilitar el diseño responsivo.
js/: Incluye los archivos JavaScript necesarios para la funcionalidad dinámica. script.js es donde se encuentra la función para mostrar u ocultar las promociones.
img/: Aquí se guardan las imágenes utilizadas en el proyecto (por ejemplo, supermercado.jpg).
4. Funcionalidades Implementadas
1. Barra de Navegación
La barra de navegación permite al usuario navegar entre diferentes secciones de la página. Se utiliza Bootstrap para crear una barra de navegación fija en la parte superior de la página. Esta barra es responsiva, por lo que se adapta bien a dispositivos móviles.

html
Copiar código
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <a class="navbar-brand" href="#">Supermercado</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item active">
        <a class="nav-link" href="#productos">Productos</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#promociones">Promociones</a>
      </li>
    </ul>
  </div>
</nav>
2. Promociones Interactivas
He implementado un botón de "Mostrar/Ocultar Promociones", que permite al usuario ver u ocultar la sección de promociones cuando lo desee. Esto se logra con la función togglePromociones() en JavaScript.

javascript
Copiar código
function togglePromociones() {
  var promociones = document.getElementById("promociones");
  if (promociones.style.display === "none") {
    promociones.style.display = "block";
  } else {
    promociones.style.display = "none";
  }
}
3. Diseño Responsivo
Usé Bootstrap para asegurarme de que la página fuera responsiva, lo que significa que se adapta a diferentes tamaños de pantalla (por ejemplo, de un escritorio a un móvil). Esto se logra con el uso de las clases de Bootstrap como container, row, col-md-6, etc.

4. Estilos y Diseño
Los estilos y el diseño visual de la página se personalizan utilizando CSS. Además de los estilos predeterminados de Bootstrap, se hicieron ajustes como los colores de los botones, márgenes y fondos para que coincidan con el tema del supermercado.

5. Imágenes y Contenido
Se incluyen imágenes relevantes, como la imagen del supermercado. Las imágenes se gestionan dentro de la carpeta img/, y se cargan en la página mediante la etiqueta <img>.

5. Subida del Proyecto a GitHub Pages
Para hacer accesible el proyecto en línea, se utilizó GitHub Pages como servicio de hosting gratuito. Los pasos realizados fueron:

Se creó un repositorio en GitHub y se subieron los archivos del proyecto.
Se configuró GitHub Pages para que los archivos se sirvieran desde la rama main.
El proyecto se encuentra disponible en la siguiente URL: https://toxzeus111.github.io/Paginaweb/.
