# Landing Page – Estructura Semántica, Accesibilidad y Diseño Responsive

## Descripción

Esta landing page está desarrollada con HTML5 semántico, y un diseño adaptable a cualquier dispositivo. El objetivo es ofrecer una estructura clara, fácil de navegar y comprensible tanto para todos los usuarios.

---

## Estructura Semántica

- **`<header>`**  
  Contiene la barra de navegación principal, que permite acceder rápidamente a las secciones clave de la página.  
  Se utiliza `aria-label="Navegación principal"` para mejorar la accesibilidad.

- **`<nav>`**  
  Incluye enlaces ancla que llevan a las secciones "Inicio", "Producto", "Preguntas frecuentes", etc.

- **`<main>`**  
  Agrupa el contenido principal de la página, dividido en secciones:

  - **`<section id="hero">`**  
    Presenta el producto con una imagen destacada, un título y una frase de valor.

  - **`<section id="caracteristicas">`**  
    Muestra una grilla de tarjetas de características, cada una con un ícono, título y descripción.  
    Se utiliza Flexbox para el diseño de las tarjetas.

  - **`<section id="preguntas-frecuentes">`**  
    Incluye una sección de preguntas frecuentes usando la estructura `<dl>`, `<dt>`, `<dd>`, y puede contener imágenes explicativas.  
    Se usa Flexbox para alinear el contenido de cada respuesta.

  - **`<section id="galeria">`**  
    Galería de imágenes, cada una con una pequeña descripción textual debajo.  
    Las imágenes y sus descripciones se agrupan en `.galeria-item` y se distribuyen en columnas usando Flexbox y media queries.

  - **`<section id="testimonios">`**  
    Sección de testimonios, donde cada opinión aparece en una tarjeta vertical.  
    Las tarjetas se distribuyen con Flexbox y se adaptan a diferentes tamaños de pantalla.

- **`<footer>`**  
  Proporciona información de contacto, derechos de autor y una sección de términos y condiciones.  
  Se utiliza `aria-label="Pie de página"` para describir su función a lectores de pantalla.

---

## Cambios y Mejoras Recientes

- **Sección de Características:**  
  Ahora es una grilla de tarjetas verticales con ícono, título y descripción, usando Flexbox.

- **Sección de Galería:**  
  Cada imagen y su descripción están agrupadas en `.galeria-item` para mantenerlas juntas en todas las resoluciones.  
  El número de columnas se ajusta automáticamente con media queries.

- **Sección de Testimonios:**  
  Añadida una grilla de tarjetas de testimonios, usando Flexbox para la disposición y adaptabilidad.

- **Navegación Mejorada:**  
  El nav usa Flexbox y se adapta a pantallas pequeñas apilando los enlaces verticalmente.

- **Accesibilidad:**  
  Uso de atributos ARIA, textos alternativos en imágenes y jerarquía de encabezados.

---

## Breakpoints y Media Queries

La página utiliza media queries para asegurar un diseño responsive:

- **Navegación (`header nav`):**
  - En pantallas menores a 600px, los enlaces se apilan verticalmente (`flex-direction: column;`).

- **Galería de imágenes (`.galeria-item`):**
  - **Pantallas grandes (≥900px):** 3 columnas (`width: 300px` por item).
  - **Pantallas medianas (600px–899px):** 2 columnas (`width: 250px` por item).
  - **Pantallas pequeñas (≤590px):** 1 columna (`width: 100%` por item).

---

## Accesibilidad

- Uso de etiquetas semánticas (`header`, `nav`, `main`, `section`, `footer`).
- Imágenes descriptivas con `alt`.
- Navegación clara y jerárquica.
- Uso de atributos ARIA donde es relevante.

---

## Personalización

Puedes modificar los textos, imágenes y estilos en los archivos correspondientes para adaptar la landing page a tu producto o servicio.
