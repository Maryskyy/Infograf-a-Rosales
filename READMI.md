```markdown
# Neurodiversidad y Aprendizaje Universal — Infografía Interactiva

Infografía vertical interactiva tipo lista que presenta cinco hallazgos clave sobre la relación entre neurodiversidad y el Diseño Universal de Aprendizaje (UDL) en contextos de ingeniería, basada en el artículo de investigación de Frontiers in Education (2025).

![Tema](https://img.shields.io/badge/Tema-Neurodiversidad%20y%20UDL-1F3A5F?style=for-the-badge)
![Formato](https://img.shields.io/badge/Formato-Infografía%20Interactiva-4CAF50?style=for-the-badge)
![Estado](https://img.shields.io/badge/Estado-Completo-brightgreen?style=for-the-badge)

---

## Vista previa

La infografía presenta un diseño limpio, vertical y orientado a lectura en pantalla, con tarjetas interactivas que se expanden al hacer clic para mostrar información adicional.

**Estructura visual:**
- Encabezado con título, subtítulo y badge temático
- 5 tarjetas numeradas con iconos, títulos y descripciones
- Separadores decorativos entre tarjetas
- Footer con referencia bibliográfica y crédito de autoría

---

## Contenido

| # | Hallazgo | Icono |
|---|----------|-------|
| 01 | UDL como enfoque inclusivo | Libro |
| 02 | Neurodiversidad como variación | Cerebro |
| 03 | ADHD reduce la autoeficacia | Señal de peligro |
| 04 | Depresión mejora resultados en UDL | Estadística ascendente |
| 05 | Necesidad de apoyo diferenciado | Pieza de rompecabezas |

---

## Características técnicas

### Diseño
- **Paleta:** `#1F3A5F` (principal), `#4CAF50` (secundario), `#F5F7FA` (fondo)
- **Tipografías:** DM Serif Display (títulos) + DM Sans (cuerpo) via Google Fonts
- **Iconos:** Font Awesome 6.5
- **Estilo:** Minimalista, académico, con buen espaciado y jerarquía visual clara

### Interactividad
- **Entrada escalonada:** Las tarjetas aparecen con animación progresiva al hacer scroll (IntersectionObserver)
- **Expansión de contenido:** Cada tarjeta se expande al hacer clic para mostrar un detalle adicional
- **Efecto de brillo:** Un resplandor sutil sigue al cursor sobre cada tarjeta (CSS custom properties + mousemove)
- **Barra de progreso:** Indicador fijo en la parte superior que muestra el avance de lectura
- **Tooltip de scroll:** Indicador flotante que desaparece al comenzar a desplazarse

### Accesibilidad
- Roles ARIA (`article`, `button`, `aria-expanded`, `progressbar`)
- Navegación completa por teclado (Tab + Enter/Espacio para expandir)
- Etiquetas semánticas HTML5 (`<header>`, `<main>`, `<section>`, `<article>`, `<footer>`)
- Respeto a `prefers-reduced-motion` (desactiva animaciones y transiciones)
- Textos legibles con contraste adecuado

### Rendimiento
- Sin dependencias de frameworks (vanilla JS + CSS puro)
- Sin llamadas a APIs externas
- Animaciones optimizadas con `requestAnimationFrame`
- Scroll listener pasivo (`{ passive: true }`)
- Todo contenido en un solo archivo HTML

---

## Uso

No requiere instalación ni build. Simplemente abre el archivo `index.html` en cualquier navegador moderno.

```bash
# Opción 1: Abrir directamente
open index.html

# Opción 2: Servidor local (recomendado para desarrollo)
npx serve .
# o
python3 -m http.server 8000
```

---

## Estructura del archivo

```
infografia-neurodiversidad-udl/
├── index.html      # Archivo único con HTML, CSS y JS embebidos
└── README.md       # Este archivo
```

El archivo `index.html` contiene todo en uno:
- `<style>` — Variables CSS, reset, layout, componentes, animaciones, responsive
- `<body>` — Estructura semántica de la infografía
- `<script>` — Lógica de interactividad (observador, expansión, progreso, brillo)

---

## Paleta de colores

| Color | Hex | Uso |
|-------|-----|-----|
| Azul oscuro | `#1F3A5F` | Color principal, textos, iconos |
| Verde | `#4CAF50` | Color secundario, acentos, badges |
| Gris claro | `#F5F7FA` | Fondo general |
| Blanco | `#FFFFFF` | Fondo de tarjetas |
| Gris texto | `#5A6B80` | Texto secundario/descripciones |

---

## Compatibilidad

| Navegador | Versión mínima |
|-----------|---------------|
| Chrome | 88+ |
| Firefox | 85+ |
| Safari | 14+ |
| Edge | 88+ |

Requiere soporte para: IntersectionObserver, CSS Custom Properties, `scroll-behavior: smooth`.

---

## Fuente de la investigación

> **Examining neurodiversity and student resources in an engineering universal design learning context**
> Frontiers in Education, 2025
> DOI: [10.3389/feduc.2025.1654115](https://doi.org/10.3389/feduc.2025.1654115)

---

## Autoría del diseño

**Marycielo Rosales**

---

## Licencia

Este recurso visual fue creado con fines educativos y de divulgación científica. El contenido pertenece a sus respectivos autores de investigación. El código fuente es de uso libre.
```