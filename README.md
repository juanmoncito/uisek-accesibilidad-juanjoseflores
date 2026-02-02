# Refactor de Accesibilidad e Inclusión – Sitio Web UISEK

## 1. Introducción

El presente proyecto tiene como objetivo analizar y refactorizar parcialmente el sitio web oficial de la **Universidad Internacional SEK (UISEK – Ecuador)**, aplicando principios de **Diseño Universal** y las **Pautas de Accesibilidad para el Contenido Web (WCAG)**.  

El análisis se realizó sobre el código HTML generado por el sitio original, identificando oportunidades de mejora relacionadas con la estructura semántica, la navegación, la legibilidad del contenido y la experiencia de usuarios con diferentes tipos de discapacidad.

Dado que el sitio original está desarrollado sobre un gestor de contenidos (WordPress) y utiliza código autogenerado, se desarrolló una **versión refactorizada y simplificada del HTML**, enfocada en demostrar buenas prácticas de accesibilidad web.

---

## 2. Objetivo del Proyecto

### Objetivo general
Mejorar la accesibilidad e inclusión del contenido web mediante la aplicación de estándares WCAG y principios de diseño universal.

### Objetivos específicos
- Aplicar correctamente etiquetas semánticas de HTML5.
- Mejorar la navegación por teclado y la visibilidad del foco.
- Optimizar la jerarquía de títulos y la legibilidad del contenido.
- Incorporar descripciones alternativas en imágenes.
- Garantizar enlaces claros y comprensibles.
- Documentar las mejoras realizadas en materia de accesibilidad.

---

## 3. Análisis del Sitio Original

Durante la revisión del código fuente del sitio web de la UISEK se identificaron los siguientes aspectos mejorables:

- Uso de textos genéricos en enlaces (por ejemplo: “Click AQUÍ”).
- Imágenes con atributos `alt` vacíos o inexistentes, aun cuando transmiten información relevante.
- Presencia de múltiples encabezados `h1` en una misma página, afectando la jerarquía semántica.
- Falta de mecanismos visibles para la navegación por teclado.
- Código HTML extenso y poco legible debido a la generación automática por el CMS.

Estos puntos afectan directamente la experiencia de usuarios que utilizan lectores de pantalla, navegación por teclado o requieren mayor claridad visual.

---

## 4. Mejoras Implementadas

### 4.1 Uso de HTML5 Semántico
Se reorganizó la estructura del documento utilizando etiquetas semánticas adecuadas:
- `header`
- `nav`
- `main`
- `section`
- `footer`

Esto mejora la comprensión del contenido por parte de lectores de pantalla y tecnologías asistivas.

---

### 4.2 Jerarquía Correcta de Encabezados
- Se estableció un único encabezado principal `h1`.
- Las secciones y subsecciones se organizaron con `h2` y `h3` de forma lógica.
- Se evitó el uso de encabezados solo con fines visuales.

---

### 4.3 Enlaces Claros y Descriptivos
Se reemplazaron enlaces con textos ambiguos como “Click AQUÍ” por enlaces descriptivos que comunican su propósito, por ejemplo:

- “Cómo llegar al Campus Miguel de Cervantes (Google Maps)”
- “Postula a la UISEK – Proceso de admisión”

Esto mejora la comprensión del contenido al ser leído fuera de contexto.

---

### 4.4 Imágenes con Texto Alternativo
- Se añadieron atributos `alt` descriptivos a imágenes informativas (logo, campus, banners).
- Las imágenes decorativas se marcaron con `alt=""` para que sean ignoradas por lectores de pantalla.
- Se organizaron las imágenes en una carpeta dedicada (`/images`).

---

### 4.5 Navegación por Teclado y Foco Visible
Se implementaron mejoras para usuarios que navegan sin mouse:
- Enlace “Saltar al contenido principal” (skip link).
- Estilos visibles para el foco mediante `:focus-visible`.
- Navegación completa usando la tecla Tab.

---

### 4.6 Legibilidad y Comprensión del Contenido
- Uso de unidades relativas (`rem`) para permitir el escalado del texto.
- Aumento del `line-height` para mejorar la lectura.
- Subrayado de enlaces para facilitar su identificación.
- Redacción clara y directa del contenido textual.

---

## 5. Mejoras Inclusivas Aplicadas (Diseño Universal)

Las siguientes mejoras fueron implementadas para favorecer la inclusión de usuarios con discapacidades:

1. **Navegación por teclado funcional**, sin bloqueos y con foco visible.
2. **Texto escalable y legible**, compatible con zoom del navegador.
3. **Enlaces descriptivos**, comprensibles sin depender del contexto visual.
4. **Estructura semántica clara**, compatible con lectores de pantalla.
5. **Texto alternativo en imágenes**, mejorando la accesibilidad visual.

---

## 6. Tecnologías y Herramientas Utilizadas

- HTML5
- CSS3
- Bootstrap (tema personalizado generado en https://bootstrap.build/)
- GitHub (control de versiones y entrega)
- Navegadores web con herramientas de desarrollo (DevTools)

---

## 7. Estructura del Proyecto

uisek-accesibilidad/
│
├── index.html
├── styles.css
├── README.md
└── images/
├── logo-uisek.png
├── campus-cervantes.jpg
└── campus-segovia.jpg



