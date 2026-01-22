# III EYE COLLECTIVE // DIGITAL INTERFACE v1.0

> **STATUS:** STABLE  
> **TYPE:** ARCHIVAL EXHIBITION SYSTEM  
> **FRAMEWORK:** SINGLE-FILE ARCHITECTURE (HTML/JS/TAILWIND)

---

## 👁️ Descripción del Sistema

Este repositorio aloja el código fuente de la interfaz digital de **III EYE COLLECTIVE**. Diseñada bajo el concepto de un "Consorcio Técnico de Bienestar", la plataforma funciona como una exhibición informativa y educativa, no transaccional.

La estética combina el **Lujo Minimalista** con una dirección de arte **Cyberpunk/Archivística**, utilizando una paleta de colores estricta (Cocoa, Crema, Oro) y tipografías de alto contraste (Bodoni Moda & JetBrains Mono).

## ⚡ Especificaciones Técnicas

* **Arquitectura Monolítica:** Todo el sistema (Estructura, Estilo y Lógica) reside en un único archivo `index.html` para máxima portabilidad y facilidad de despliegue.
* **Styling Engine:** Tailwind CSS implementado vía CDN (JIT mode) con configuración personalizada de temas en tiempo de ejecución.
* **Zero-Build Requirement:** No requiere Node.js, NPM, ni compiladores. Funciona directamente en cualquier navegador moderno.
* **Responsive Design:** Adaptabilidad fluida desde dispositivos móviles hasta pantallas de alta resolución (4K).
* **Motion UI:** Sistema de micro-interacciones y "Scroll Reveals" nativos (Vanilla JS).

## 🚀 Protocolo de Despliegue (Quick Start)

### Opción A: Ejecución Local
1.  Descarga el archivo `index.html`.
2.  Ábrelo directamente en tu navegador preferido (Chrome, Firefox, Safari).
3.  *No se requiere servidor local.*

### Opción B: Publicación en Web (Netlify/Vercel/GitHub Pages)
1.  Sube el archivo `index.html` a la raíz de tu repositorio.
2.  Configura tu proveedor de hosting estático para servir la carpeta raíz.
3.  El sistema detectará automáticamente la configuración de producción.

## 🛠️ Configuración y Personalización

El sistema está diseñado para ser modular. Todas las configuraciones críticas se encuentran dentro del bloque `<script>` de Tailwind en el `index.html`.

### 1. Paleta de Colores
Para modificar los colores de marca, edita la sección `tailwind.config` en el `<head>`:

```javascript
colors: {
    cocoa: '#1a0f0d',       // Fondo Principal
    cream: '#f3e5ab',       // Texto Principal
    gold: '#C5A059',        // Acentos y Bordes
    'gold-dim': 'rgba...',  // Estados Hover
}
