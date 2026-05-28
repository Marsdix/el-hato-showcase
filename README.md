<div align="center">

# 🍷 El Hato y el Garabato

**Bodega familiar · Arribes del Duero · Zamora**

*Sitio web oficial diseñado y desarrollado como proyecto fin de ciclo de DAW*

<br/>

![Astro](https://img.shields.io/badge/Astro-6_SSG-FF5D01?style=for-the-badge&logo=astro&logoColor=white&labelColor=1a1a2e)
![React](https://img.shields.io/badge/React-18.3_Islands-61DAFB?style=for-the-badge&logo=react&logoColor=white&labelColor=20232a)
![CMS](https://img.shields.io/badge/Sanity-Headless_CMS-F03E2F?style=for-the-badge&logo=sanity&logoColor=white&labelColor=1a1a1a)
![Deploy](https://img.shields.io/badge/GitHub_Pages-Deploy-22272E?style=for-the-badge&logo=github&logoColor=white)
![i18n](https://img.shields.io/badge/i18n-ES%20%2F%20EN-c8a255?style=for-the-badge&logo=googletranslate&logoColor=white&labelColor=3a2a10)

<br/>

> Rediseño completo del sitio WordPress original de la bodega. Construido en Astro 6 con generación estática (SSG), componentes React con Islands Architecture y un diseño editorial propio — rápido, accesible y bilingüe.

</div>

---

## 🌿 El proyecto

**El Hato y el Garabato** es una bodega familiar del municipio de Formariz, en el Parque Natural Arribes del Duero (Zamora). Sus vinos, elaborados con variedades autóctonas como Juan García, Bruñal y Puesta en Cruz, tienen una marcada personalidad de territorio.

Este proyecto migra el sitio WordPress + Astra original a una arquitectura JAMstack moderna: Astro 6 genera HTML estático por ruta, React 18 gestiona la interactividad mediante islas aisladas, y Sanity CMS centraliza el contenido sin requerir conocimientos técnicos.

---

## ✦ Funcionalidades

<table>
  <tr>
    <td align="center" width="160">🍾</td>
    <td><strong>Catálogo de vinos</strong><br/>Ficha completa por botella: notas de cata visual, olfativa y gustativa, datos analíticos y precio. Animación de revelado al hacer scroll.</td>
  </tr>
  <tr>
    <td align="center">🛒</td>
    <td><strong>Tienda con carrito</strong><br/>Selector de cantidad, resumen del pedido, subtotales y formulario de envío a Formspree. Estado compartido entre islas con Nanostores.</td>
  </tr>
  <tr>
    <td align="center">📰</td>
    <td><strong>Blog y prensa</strong><br/>Artículos propios y apariciones en medios, con filtro multi-selección por categoría, <code>AnimatePresence</code> por tarjeta y soporte de vídeo.</td>
  </tr>
  <tr>
    <td align="center">🗺️</td>
    <td><strong>Enoturismo</strong><br/>Página de visitas con formularios de reserva independientes para cada experiencia (visita bodega / visita viña + bodega) y mapa embebido.</td>
  </tr>
  <tr>
    <td align="center">🌐</td>
    <td><strong>Bilingüe ES / EN</strong><br/>Cambio de idioma en tiempo real sin recarga de página. Persistencia en <code>localStorage</code>. Títulos de página actualizados por ruta en ambos idiomas.</td>
  </tr>
  <tr>
    <td align="center">🌙</td>
    <td><strong>Modo oscuro / claro</strong><br/>Tema completo con variables CSS y atributo <code>data-theme</code>. Activable desde la barra de navegación, persistente entre sesiones.</td>
  </tr>
  <tr>
    <td align="center">♿</td>
    <td><strong>Accesibilidad WCAG 2.1 AA</strong><br/>Skip link, <code>focus-visible</code> global, ARIA semántico, labels accesibles, jerarquía de headings correcta y contraste AA verificado en toda la interfaz.</td>
  </tr>
  <tr>
    <td align="center">⚡</td>
    <td><strong>Rendimiento</strong><br/>HTML estático por ruta, JS de React cargado solo donde hace falta. Scroll suave con Lenis, animaciones con Framer Motion 12.</td>
  </tr>
  <tr>
    <td align="center">📱</td>
    <td><strong>Diseño responsivo</strong><br/>Adaptado a móvil, tablet y escritorio. Navegación con menú hamburguesa, tipografía fluida con <code>clamp()</code> y layouts adaptativos.</td>
  </tr>
</table>

---

## 🎨 Diseño

El diseño es completamente personalizado, sin frameworks de estilos, construido sobre variables CSS globales para garantizar coherencia visual en toda la aplicación.

| | |
|---|---|
| **Tipografía editorial** | Cormorant Garamond — serif de alto contraste para títulos y precios |
| **Tipografía de caps** | Cinzel — versalitas para etiquetas y navegación |
| **Tipografía de interfaz** | Jost — sans-serif limpia para cuerpo y UI técnica |
| **Color base** | `#faf8f3` — blanco roto cálido (papel verjurado) |
| **Acento dorado** | `#c8a255` — inspirado en el color del vino añejo |
| **Fondo oscuro** | `#15110e` — marrón casi negro para el modo noche |

Las animaciones acompañan el scroll sin entorpecerlo: parallax en heroes con `useScroll` + `useTransform`, gris-a-color en fotos de bodega y equipo, tilt 3D en tarjetas, CountUp animado en estadísticas y scroll reveals escalonados en listas.

---

## 📦 Gestión de contenido

Los vinos, artículos del blog, apariciones en prensa y textos del sitio se gestionan desde **Sanity CMS** (headless) sin necesidad de tocar código. El sitio incluye datos de respaldo para garantizar que siempre hay contenido visible, incluso sin conexión al CMS.

---

<div align="center">

### 🔒 Repositorio privado

El código fuente completo se encuentra en un repositorio privado.  
Este espacio es únicamente una presentación pública del proyecto.

<br/>

*Proyecto académico — DAW 2025–2026*  
*Todos los derechos del contenido (marca, imágenes y textos) pertenecen a Bodega El Hato y el Garabato*

</div>
