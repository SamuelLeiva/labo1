# Landing Page – Estructura Semántica y Accesibilidad

## Descripción

Esta landing page está desarrollada utilizando HTML5 semántico y buenas prácticas de accesibilidad. El objetivo es ofrecer una estructura clara, fácil de navegar y comprensible tanto para usuarios como para tecnologías asistivas.

---

## Estructura Semántica

- **`<header>`**  
  Contiene la barra de navegación principal, que permite acceder rápidamente a las secciones clave de la página.  
  Se utiliza `aria-label="Navegación principal"` para mejorar la accesibilidad.

- **`<nav>`**  
  Incluye enlaces ancla que llevan a las secciones "Inicio", "Producto" y "Preguntas frecuentes".

- **`<main>`**  
  Agrupa el contenido principal de la página, dividido en secciones:

  - **`<section id="hero">`**  
    Presenta el producto con una imagen destacada, un título y una frase de valor.

  - **`<section>`**  
    Lista las características principales del producto, cada una acompañada de un ícono descriptivo.

  - **`<section>`**  
    Incluye una sección de preguntas frecuentes usando la estructura `<dl>`, `<dt>`, `<dd>`, y puede contener imágenes explicativas.

- **`<footer>`**  
  Proporciona información de contacto y derechos de autor.  
  Se utiliza `aria-label="Pie de página"` para describir su función a lectores de pantalla.

---

## Sugerencias de Mejora Aplicadas (por IA)

1. **Navegación Accesible:**  
   Se añadió `aria-label` al `<nav>` para que los lectores de pantalla identifiquen la navegación principal.

2. **Imágenes con Descripción:**  
   Todas las imágenes usan el atributo `alt` para describir su contenido, facilitando la comprensión a usuarios con discapacidad visual.

3. **Enlaces Ancla:**  
   Los enlaces de navegación usan `href="#seccion"` para llevar al usuario directamente a la sección correspondiente.

4. **Jerarquía de Encabezados:**  
   Se utilizan correctamente los encabezados (`<h1>`, `<h2>`, `<dt>`) para mantener una estructura lógica y accesible.

5. **Footer Accesible:**  
   El `<footer>` incluye `aria-label` para describir su función.

6. **Sugerencias adicionales:**  
   - Se recomienda agregar un formulario de contacto para mejorar la interacción.
   - Se sugiere mejorar el contraste y la legibilidad con CSS.
   - Se aconseja agregar un botón de llamada a la acción (CTA) en la sección hero.
   - Se recomienda asegurar el diseño responsive mediante CSS.

---

## Accesibilidad

- Uso de etiquetas semánticas (`header`, `nav`, `main`, `section`, `footer`).
- Imágenes descriptivas con `alt`.
- Navegación clara y jerárquica.
- Uso de atributos ARIA donde es relevante.

---

## Personalización

Puedes modificar los textos, imágenes y estilos en los archivos correspondientes para adaptar la landing page a tu producto o servicio.
