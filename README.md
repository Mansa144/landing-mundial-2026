# Landing Page – Campaña Mundial 2026

## Descripción

Este proyecto consiste en la implementación de una **landing page promocional** diseñada en Figma.

El diseño fue realizado por una compañera de UX/UI, y el proyecto ya contaba con una base en HTML y CSS que fue modificada y adaptada según los nuevos requerimientos.

---

## Objetivos

- Implementar fielmente el diseño de Figma en HTML y CSS
- Crear una estructura clara, responsive y escalable
- Optimizar la experiencia de usuario (UX)

---

## Estructura del proyecto

```
/landing-mundial-2026
│
├── index.html
├── styles.css
├── /IMG
│   ├── hero.png
│   ├── wave.svg
│   └── logo.png
└── README.md
```

---

## Secciones implementadas

### 1. Header / Navbar

- Logo de la marca
- Botón de regreso
- Acceso directo a WhatsApp

---

### 2. Hero

- Título principal
- Descripción
- CTA destacado
- Imagen lateral con overlay degradado

**Implementación:**

- CSS Grid
- `object-fit` para imágenes
- Gradiente con `::before`

---

### 3. Countdown

- Contador dinámico
- Mensaje de tiempo limitado

---

### 4. Ofertas Relámpago

- Texto persuasivo
- Formulario de captura:

  - Nombre
  - Email
  - WhatsApp

- Botón CTA
- Texto legal con enlace

**Detalles técnicos:**

- Layout con Grid
- SVG decorativo (`wave`)
- Uso de `z-index` para superposición

---

### 5. Sección Producto

- Imagen del producto
- Lista de beneficios
- Precio anterior (tachado)
- Precio actual destacado
- Financiación
- Botón de compra

**Implementación:**

- Grid de 2 columnas
- Jerarquía visual en precios
- Card con fondo y sombras

---

## Tecnologías utilizadas

- HTML5
- CSS3 (Flexbox + Grid)
- SVG (elementos gráficos)
- Media Queries (responsive)

---

## Responsive Design

La landing está adaptada para dispositivos móviles:

```css
@media (max-width: 768px) {
  .hero,
  .product-card,
  .ofertas-content {
    grid-template-columns: 1fr;
  }
}
```

---

## Decisiones técnicas clave

- Uso de CSS Grid para layouts principales
- Uso de `<img>` en lugar de `background-image` para mayor control
- Separación de estilos por sección
- Reutilización de componentes (botones)
- Uso de pseudo-elementos para efectos visuales

---

## Problemas y soluciones

| Problema                      | Solución                                 |
| ----------------------------- | ---------------------------------------- |
| Imagen no ocupaba espacio     | Uso de `object-fit: cover`               |
| Espacio blanco entre columnas | Eliminación de `gap` innecesario         |
| Gradiente sobre imagen        | Implementación con `::before`            |
| Error HTML                    | Corrección de etiquetas sin cerrar       |
| CSS no aplicado               | Corrección de selectores (`.h2` vs `h2`) |
| Texto legal mal alineado      | Uso de `text-align: center`              |

---

## Funcionalidades

- Formulario de captura de leads
- Botón de contacto por WhatsApp
- Navegación simple
- Diseño orientado a conversión

---

## Autor

**Lucía Pintos**
Frontend Developer

Proyecto desarrollado dentro de una **simulación laboral con cliente**, en colaboración con un equipo de desarrolladores y diseñadores.
Enfocado en la implementación de diseño Figma a código HTML/CSS.
