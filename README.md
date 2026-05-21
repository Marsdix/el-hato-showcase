# 🍷 El Hato y el Garabato

**Sitio web oficial de la bodega El Hato y el Garabato** — Arribes del Duero, Salamanca.  
SPA desarrollada como proyecto fin de ciclo de DAW, reemplazando el WordPress original con una aplicación React moderna, rápida y mantenible.

---

## ✨ Lo que hace el proyecto

| Área | Descripción |
|------|-------------|
| **Catálogo de vinos** | Fichas completas con notas de cata, datos analíticos y galería |
| **Tienda con carrito** | Añadir al carrito con selector de cantidad, resumen de pedido y envío por email |
| **Blog / Prensa** | Artículos con filtro por categoría, portadas y soporte de vídeo embebido |
| **Enoturismo** | Página de visitas y experiencias con mapa interactivo (Leaflet) |
| **i18n ES / EN** | Cambio de idioma en tiempo real sin recarga |
| **Dark mode** | Tema oscuro con filtro CSS sobre mapa y variables globales |
| **CMS sin backend** | Contenido gestionado desde Sanity Studio con fallback estático |

---

## 🛠 Stack técnico

```
React 18 + Vite 5        →  SPA con lazy loading por ruta
React Router 6           →  Routing client-side
Framer Motion            →  Animaciones (PageHero parallax, ScrollReveal, StaggerList)
Sanity v3                →  CMS headless — vinos, blog posts, prensa
Leaflet + React-Leaflet  →  Mapa interactivo de la bodega
Formspree                →  Formulario de pedido sin backend propio
CSS custom (sin Tailwind) →  Variables globales, dark mode nativo
Vercel                   →  Deploy continuo
```

---

## 🏗 Arquitectura

```
src/
├── App.jsx                  # Rutas lazy + Suspense
├── components/
│   ├── layout/              # Navbar, Footer, PageHero, Layout
│   ├── sections/            # Secciones reutilizables por página
│   └── ui/                  # Button, ScrollReveal, AnimatedDivider…
├── context/
│   ├── CartContext.jsx      # Estado global del carrito
│   └── LanguageContext.jsx  # i18n + tema
├── data/                    # Fallback estático (vinos, blog, traducciones…)
├── hooks/                   # useSanityFetch, useScrollReveal, useCursor
├── lib/
│   └── queries.js           # GROQ queries para Sanity
└── pages/                   # Una página por ruta (lazy-loaded)
```

**Patrón `useSanityFetch`** — carga los datos estáticos de `src/data/` de forma inmediata (sin flash de carga) y los reemplaza silenciosamente con los datos de Sanity cuando llegan. Esto garantiza que la página siempre tenga contenido aunque el CMS tarde o falle.

---

## 🎨 Diseño

- Tipografía: **Cormorant Garamond** (serif elegante) · **Cinzel** (caps) · **Jost** (sans)
- Paleta cálida: beige `#faf8f3`, dorado `#c8a255`, oscuro `#140d08`
- Sin frameworks CSS — todo custom con variables CSS
- Cursor personalizado con trailing suave
- Animaciones de entrada escalonadas (`StaggerList`) y parallax en heroes

---

## 🔒 Nota

El código fuente completo está en un repositorio privado.  
Este repositorio es una presentación pública del proyecto.

---

## 📄 Licencia

Proyecto académico — DAW, curso 2024-2025.  
Todos los derechos del contenido (marca, imágenes, textos) pertenecen a Bodega El Hato y el Garabato.
