# Pagina
Bootstrap se está utilizando para proporcionar una estructura y un estilo básico a la página web. 

### 1. **Enlaces a los archivos de Bootstrap**
En la sección `<head>`, tienes un enlace al archivo CSS de tu tema (`css/styles.css`) que incluye el soporte de Bootstrap. Además, también está vinculado un archivo JavaScript de Bootstrap:

```html
<link href="css/styles.css" rel="stylesheet" />
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"></script>
```

El archivo CSS (`styles.css`) probablemente tiene algunas personalizaciones adicionales para adaptar el diseño a tus necesidades, pero se basa en gran parte en las clases de Bootstrap para el estilo y la disposición de los elementos.

### 2. **Clases de Bootstrap en los elementos HTML**
A continuación se muestran algunos ejemplos de cómo se están utilizando las clases de Bootstrap en el HTML:

#### a. **Navbar (barra de navegación)**
La barra de navegación usa varias clases de Bootstrap para su diseño y comportamiento responsivo:

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-primary fixed-top" id="sideNav">
    <!-- Contenido del navbar -->
</nav>
```

- **`navbar`**: Define el contenedor para la barra de navegación.
- **`navbar-expand-lg`**: Hace que la barra de navegación sea expansible en pantallas grandes, pero en pantallas pequeñas se colapsa.
- **`navbar-dark`**: Establece un color de texto claro para los elementos de la barra de navegación.
- **`bg-primary`**: Asigna un color de fondo de la paleta de colores primarios de Bootstrap (por lo general, un azul).
- **`fixed-top`**: Hace que la barra de navegación se quede fija en la parte superior de la página mientras se hace scroll.

#### b. **Contenedores responsivos**
Dentro de tu contenido, estás usando contenedores para asegurarte de que el diseño se ajuste bien a diferentes tamaños de pantalla:

```html
<div class="container-fluid p-0">
    <!-- Secciones del contenido -->
</div>
```

- **`container-fluid`**: Define un contenedor de ancho completo que se adapta al tamaño de la pantalla.
- **`p-0`**: Elimina el padding del contenedor.

#### c. **Cards (tarjetas)**
Las tarjetas son utilizadas para mostrar los proyectos con imágenes y descripciones:

```html
<div class="card">
    <img src="foto 1.jpg" class="card-img-top" alt="Proyecto 1">
    <div class="card-body">
        <h5 class="card-title">Seguridad y Alta Disponibilidad</h5>
        <p class="card-text">Configuración de entornos seguros...</p>
        <a href="https://github.com/adriancns8/SAD" class="btn btn-primary">Ver proyecto</a>
    </div>
</div>
```

- **`card`**: Crea una tarjeta que puede contener texto, imágenes o botones.
- **`card-img-top`**: Coloca la imagen en la parte superior de la tarjeta.
- **`card-body`**: Define el área que contiene el contenido de la tarjeta (como el título, el texto y el botón).
- **`btn btn-primary`**: Aplica el estilo de un botón de Bootstrap con un fondo de color primario.

#### d. **Listas de íconos (por ejemplo, para las habilidades)**
Para mostrar los íconos de habilidades, se usa una lista sin orden, estilizada con clases de Bootstrap:

```html
<ul class="list-inline dev-icons">
    <li class="list-inline-item"><i class="fab fa-html5"></i></li>
    <li class="list-inline-item"><i class="fab fa-css3-alt"></i></li>
    <!-- Más íconos -->
</ul>
```

- **`list-inline`**: Hace que los elementos de lista se muestren en línea, es decir, de forma horizontal.
- **`list-inline-item`**: Aplica estilo a cada ítem de la lista para alinearlos horizontalmente.

#### e. **Formulario de contacto**
El formulario utiliza un estilo básico con etiquetas y campos de entrada:

```html
<form action="mailto:contacto@tucorreo.com" method="post" enctype="text/plain">
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre" required placeholder="Tu nombre completo">
    <!-- Otros campos -->
    <button type="submit">Enviar</button>
</form>
```

Aunque este formulario no está utilizando clases específicas de Bootstrap en su estilo visual, Bootstrap puede proporcionar estilos predeterminados para los formularios si se añaden clases como `form-control` a los elementos de entrada.

### 3. **Responsividad**
Bootstrap ayuda a que el diseño sea responsivo, es decir, que se adapte a diferentes tamaños de pantalla. Por ejemplo:

- **`navbar-expand-lg`** hace que la barra de navegación se expanda en pantallas grandes y se colapse en pantallas pequeñas.
- Las tarjetas dentro de las secciones de "Proyectos" usan clases como **`col-md-4`**, que definen el ancho de las columnas en pantallas medianas (y más grandes), asegurando que las tarjetas se ajusten bien en dispositivos móviles y en pantallas grandes.

### Conclusión
Bootstrap está siendo utilizado en este código principalmente para:

- Crear una **barra de navegación responsiva**.
- Organizar el **contenido en contenedores y columnas** que se adaptan a diferentes tamaños de pantalla.
- Estilizar los **botones, tarjetas e íconos** para darles una apariencia moderna y atractiva.
- Asegurar que el diseño sea **responsivo**, es decir, que se vea bien tanto en dispositivos móviles como en pantallas más grandes.

Al integrar Bootstrap, facilitas la creación de un diseño consistente, flexible y adaptado a dispositivos de diferentes tamaños sin necesidad de escribir CSS personalizado desde cero.
