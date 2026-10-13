# HW-Frontend-Seccion2

# Ejercicio Guiado — Estructura HTML, Flexbox y Grid

## Curso: ICINF1107 · Desarrollo de Frontend · Sesión 5

---

## Contexto

Vamos a construir una página web **sencilla desde cero**, aplicando la estructura HTML que ya conocen y dos herramientas de CSS: **Flexbox** y **Grid**. El ejercicio es corto a propósito: estructura simple, estilos simples y resultado visible en pocos minutos.

## Objetivo de aprendizaje

Construir una página HTML con estructura básica y aplicarle estilos con CSS (color de fuente, color de fondo, alineación, padding y margen), usando **Flexbox** para ordenar tres tarjetas y **Grid** para una grilla de 3×3.

---

## Requerimientos del HTML (estructura)

Tu archivo `index.html` debe contener:

1. **Un título principal** (`<h1>`) con el nombre de tu página. Elige un tema: mascotas, videojuegos, comida, lo que prefieras.
2. **Dos títulos secundarios** (`<h2>`): uno para la sección de tarjetas y otro para la sección de la grilla.
3. **Dos títulos de tercer nivel** (`<h3>`): uno dentro de cada sección (un subtítulo por bloque).
4. **Una lista** (`<ul>` con al menos 3 `<li>`): por ejemplo, una lista de características o de pasos.
5. **Una sección con 3 tarjetas**: tres `<div class="tarjeta">` dentro de un contenedor `<div class="tarjetas">`.
6. **Una grilla de 3×3**: nueve celdas `<div class="celda">` dentro de un contenedor `<div class="grilla">`.

## Requerimientos de estilos (CSS)

En tu archivo `style.css` (separado del HTML) debes aplicar:

1. **Color de fuente** (`color`): un color para el texto del cuerpo y otro para los títulos.
2. **Color de fondo** (`background-color`): un color para la página y un color distinto para las tarjetas.
3. **Alineación**: títulos centrados (`text-align: center`).
4. **Padding** dentro de las tarjetas y de las celdas.
5. **Margen** entre las secciones.
6. **Flexbox** en el contenedor de tarjetas: `display: flex`, `justify-content: center` y `gap`.
7. **Grid** en el contenedor de la grilla: `display: grid`, `grid-template-columns: repeat(3, 1fr)` y `gap`.
8. *(Opcional, para destacar)* `border-radius` en las tarjetas y un efecto `:hover` en las celdas.

---

## Estructura esperada

```
<body>
├── <h1> Título de la página
├── <ul> Lista (3 ítems)
├── <h2> Sección 1: Tarjetas (Flexbox)
│   ├── <h3> Subtítulo de la sección
│   └── <div class="tarjetas">
│       ├── <div class="tarjeta"> 1
│       ├── <div class="tarjeta"> 2
│       └── <div class="tarjeta"> 3
└── <h2> Sección 2: Grilla (Grid)
    ├── <h3> Subtítulo de la sección
    └── <div class="grilla">
        └── 9 × <div class="celda">
```

---

## Criterios de aceptación (checklist)

- [ ] La página abre con doble clic y se ve ordenada.
- [ ] Existe exactamente **1** `<h1>`, **2** `<h2>` y **2** `<h3>`.
- [ ] La lista se muestra con viñetas.
- [ ] Las 3 tarjetas están en fila y centradas (Flexbox funcionando).
- [ ] La grilla muestra 3 columnas × 3 filas (9 celdas visibles).
- [ ] Se aplicaron: color de fuente, color de fondo, alineación centrada, padding y margen.
- [ ] El HTML y el CSS están en archivos separados (`index.html` y `style.css`) y conectados con `<link>`.

---

## Pistas (sin resolver el ejercicio)

- El CSS se conecta al HTML con `<link rel="stylesheet" href="style.css">` dentro de `<head>`.
- Para la grilla: `grid-template-columns: repeat(3, 1fr)` crea 3 columnas iguales; las 9 celdas se acomodan solas en 3 filas.
- Para las tarjetas: `display: flex` + `gap` las separa; `justify-content: center` las centra.

## Pregunta de reflexión (para el cierre)

¿Qué pasa si cambias `justify-content: center` por `space-between` en las tarjetas? ¿Y si cambias `repeat(3, 1fr)` por `repeat(2, 1fr)`?

---

## Entrega


# Portafolio Profesional — Evaluación P2 (ICINF1107)

Portafolio web individual desarrollado como mockup de interfaz y primera pieza de presentación profesional, abarcando los contenidos del bloque RA1 de la asignatura Desarrollo de Frontend (ICINF1107).

---

## 📋 Ficha Técnica del Proyecto
* **Asignatura:** ICINF1107 — Desarrollo de Frontend
* **Carrera:** Ingeniería Civil en Informática (Sección 3)
* **Institución:** Universidad Católica de Temuco
* **Docente:** Cristian Iglesias Vera
* **Modalidad:** Presentación Oral Individual (P2)
* **Semestre / Año:** 2° Semestre, 2026

---

## 🚀 Descripción del Proyecto y Audiencia
Este sitio web es un portafolio profesional interactivo y responsivo diseñado bajo un enfoque centrado en el usuario. Su propósito principal es servir como carta de presentación ante docentes, reclutadores técnicos o clientes, mostrando de forma clara y accesible el perfil técnico y los proyectos académicos desarrollados durante el periodo lectivo.

---

## 🛠️ Tecnologías Utilizadas
* **HTML5 Semántico:** Estructurado mediante etiquetas semánticas (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`) para garantizar una jerarquía limpia, accesible y navegable.
* **CSS3 Explicito (Externo):** Estilos aplicados mediante una hoja externa (`style.css`), organizados mediante variables globales (`:root`) para consistencia en la paleta cromática y diseño fluido.
* **Render & GitHub:** Control de versiones con Git y despliegue continuo en la nube para acceso multiplataforma en tiempo real.

---

## 📱 Diseño Responsivo (3 Breakpoints)
La interfaz fue maquetada pensando en la adaptabilidad multiplataforma, implementando 3 puntos de quiebre (*breakpoints*) bien definidos mediante `@media`:

1. **Móvil (`< 600px`):** Ajuste de la navegación a un menú táctil de botones compactos, tipografía fluida y distribución de contenido en una sola columna (`1fr`).
2. **Tablet (`600px - 1023px`):** Reorganización de la retícula de proyectos a 2 columnas para una lectura cómoda en pantallas medianas.
3. **Escritorio (`≥ 1024px`):** Apertura completa del layout en cuadrícula adaptativa optimizada para pantallas de alta resolución.

---

## ♿ Accesibilidad y Buenas Prácticas (WCAG / WAI-ARIA)
* **WAI-ARIA:** Implementación de roles semánticos (`role="banner"`, `role="navigation"`, `role="main"`, `role="contentinfo"`) y atributos para tecnologías de asistencia (`aria-label`, `aria-labelledby`, `aria-required`, `aria-hidden`).
* **Navegación por Teclado:** Foco visual evidente (`:focus`, `outline`) en todos los elementos interactivos (enlaces, botones e insumos de formulario).
* **Contraste de Color:** Paleta de contraste elevado (cumpliendo pautas WCAG) para asegurar la legibilidad de textos sobre fondos oscuros.
* **Formulario Accesible:** Uso de etiquetas `<label>` vinculadas directamente a sus correspondientes `<input>` mediante el atributo `for`.

---

## 📂 Estructura de Archivos del Proyecto
```text
portafolio-evaluacion/
│
├── index.html        # Estructura principal en HTML5 semántico con atributos WAI-ARIA
├── style.css         # Hoja de estilos CSS externa con los 3 breakpoints responsivos
└── README.md         # Documentación técnica y fundamentación del proyecto


Una carpeta con `index.html` y `style.css`. Nada más: estructura simple y estilos básicos.

---
Elaborado por: Cristian Iglesias Vera — Escuela Ingeniería Civil en Informática — UC Temuco

