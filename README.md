# Alcalnik.github.io
# Documentación de decisiones de diseño - index.html

Este documento resume las decisiones tomadas en la creación de la página **Pamplona Music Festival**.

---

## Estructura general

- Se utilizó HTML5 con una estructura semántica clara, dividiendo el contenido en secciones (`<section>`) para:
  - Home / Hero
  - Artistas invitados
  - Entradas
  - Horario
  - Preguntas frecuentes (FAQ)
  - Consejos para el festival
  - Footer

- Se implementó **Bootstrap 5** para garantizar un diseño responsive y consistente.

---

## Navbar

- Barra de navegación adaptativa usando clases de Bootstrap (`navbar-expand-lg`, `collapse`, `navbar-toggler`).
- Los enlaces del menú permiten navegación interna hacia secciones específicas usando `href="#id"`.
- Se añadieron botones de acción (Iniciar sesión / Usuario) con clases de Bootstrap.

---

## Hero / Carousel

- Se decidió usar un **carrusel** para destacar imágenes principales del festival.
- Uso de `carousel-indicators` y controles prev/next para mejorar la navegación visual.
- Las imágenes se optimizaron con `img-fluid` y `w-90` para escalado responsivo.
- Se mantuvo la compatibilidad con lectores de pantalla usando `aria-label` y `aria-current`.

---

## Sección de Artistas

- Se muestran los artistas en un **grid responsive**:
  - `row row-cols-1 row-cols-md-2 row-cols-lg-4 g-4` para adaptarse a diferentes tamaños de pantalla.
- Cada artista tiene un **modal** con información y foto ampliada.
- Se agregó un **margen exterior** (`p-2` en las cards) para separación visual.

---

## Entradas

- Presentadas en cards con imagen, título, descripción y botón de compra.
- Se usaron offsets (`offset-md-2`) para centrar visualmente en pantallas medianas.
- Diferenciación entre entrada normal y premium usando imágenes y texto descriptivo.

---

## Horario

- Tabla responsive con horarios y artistas.
- Se utilizó `table-responsive` para asegurar scroll horizontal en pantallas pequeñas.
- Diferenciación visual con `table-secondary` para encabezados y `bg-secondary bg-opacity-10` en el contenedor.

---

## FAQ y Consejos

- Preguntas frecuentes estructuradas en bloques `<div>` con títulos `<h5>` y párrafos `<p>`.
- Se incluyó un **video con modal** para consejos del festival:
  - Imagen de portada con superposición de icono y texto.
  - Modal centrado con `modal-lg` para mayor visibilidad.
  - Uso de subtítulos `.vtt` y `.srt` para accesibilidad.

---

## Footer

- Diseñado con tres columnas usando grid de Bootstrap:
  - Info legal
  - Redes sociales y nombre del festival
  - Contacto
- Orden de columnas adaptable con `order-*` según tamaño de pantalla.
- Inclusión de licencias Creative Commons de forma clara y visual.

---

## Elecciones de diseño y estilo

- Clases de Bootstrap combinadas con estilos personalizados (`custom-min.css`).
- Consistencia de colores usando `text-primary`, `text-secondary` y `bg-dark`.
- Iconos de FontAwesome para redes sociales y controles de video.
- Tarjetas con sombra y bordes redondeados para un look moderno.

---

## Decisiones importantes

- Se optó por **modales** para información ampliada (artistas, video) evitando recargar la página.
- Uso de **videos locales** para consejos del festival, con poster y subtítulos.
- Diseño **mobile-first** y responsive, probando distintos breakpoints (`md`, `lg`, `xl`).
- Se priorizó la **accesibilidad** y la **usabilidad**, manteniendo una estética clara y coherente.

---

> Esta documentación resume la lógica y decisiones detrás del `index.html`, enfocándose en responsividad, accesibilidad y experiencia de usuario.
