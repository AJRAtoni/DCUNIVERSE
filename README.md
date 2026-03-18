# DC Universe Timeline 🦸

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-green?logo=github)](https://dc.ajra.es)
[![Airtable](https://img.shields.io/badge/Airtable-API-21D891?logo=airtable)](https://airtable.com)
[![Status](https://img.shields.io/badge/Status-Active-lightgrey)](https://dc.ajra.es)
[![License](https://img.shields.io/badge/License-All+Rights+Reserved-red.svg)]()

**Sitio estático con timeline de películas y series de DC Comics**

> 🌐 **Live demo:** https://dc.ajra.es
> 📅 **Activo desde:** 2020-presente
> 🔧 **Tecnología:** HTML5 + CSS3 + Vanilla JS + Airtable API
> 📱 **Responsive:** Sí (mobile-first)

---

## 📋 Descripción

**DC Universe Timeline** es un sitio web estático que muestra un listado cronológico de películas y series de DC Comics programadas para estrenarse en los próximos años. El contenido se carga dinámicamente desde una base de datos de **Airtable**, permitiendo actualizaciones sin necesidad de desplegar nuevo código.

### Características principales

- ✅ **Actualización dinámica** — Los datos vienen de Airtable API
- ✅ **Diseño responsive** — Se adapta a móviles, tablets y desktop
- ✅ **Lazy animations** — Animaciones al hacer scroll (IntersectionObserver)
- ✅ **Orden inteligente** — Alternancia de imágenes izquierda/derecha
- ✅ **Formato de fechas en español** — Localización completa
- ✅ **Google Analytics integrado** — Tracking de visitas
- ✅ **Sin build tools** — Sin dependencias, solo HTML/CSS/JS plano
- ✅ **Hosting gratuito** — GitHub Pages con dominio personalizado

---

## 🏗️ Arquitectura

```
DCUNIVERSE/
├── index.html              # Página principal (single-page)
├── assets/
│   ├── app.js              # Lógica de fetch Airtable + renderizado
│   ├── main.js             # Carrd framework JS (no modificar)
│   ├── main.css            # Carrd framework CSS + estilos base
│   ├── noscript.css        # Estilos para usuarios sin JS
│   ├── icons.svg           # Sprite SVG de iconos sociales
│   └── images/             # Imágenes de logotipos y banners
├── CLAUDE.md               # Guía para Claude Code (desarrollo)
├── CNAME                   # Configuración de dominio personalizado
└── README.md               # Este archivo
```

---

## 🎨 Diseño y UX

- **Tipografía:** Inter + Poppins (Google Fonts)
- **Layout:** Container con ancho máximo, centrado
- **Cards:** Layout alternado izquierda/derecha
  - Índices pares: imagen-izq / texto-der
  - Índices impares: texto-izq / imagen-der
  - En móvil (≤736px): imagen siempre arriba
- **Animaciones:** Fade-in con `IntersectionObserver`
- **Fechas:** Formato "15 JUNIO 2026" en español, con corrección de timezone
- **Títulos:** Transformados a uppercase vía CSS

---

## 🚀 Despliegue

### GitHub Pages (automático)

1. Push a la rama `main` → GitHub Pages despliega automáticamente
2. Dominio configurado via archivo `CNAME` → `dc.ajra.es`
3. CDN global de GitHub (rápido, gratis)

### Actualizar datos

Solo necesitas modificar la tabla `eventos` en Airtable:
1. Agrega/edita registros con los campos correctos
2. El sitio se actualiza automáticamente en tiempo real (cada que un usuario recarga)
3. No requiere deploy, no requiere Git

---

## 🛠️ Stack tecnológico

| Componente | Tecnología | Uso |
|-----------|-----------|-----|
| HTML | HTML5 semántico | Estructura |
| CSS | SCSS compilado a CSS | Estilos + Carrd framework |
| JavaScript | ES6+ | Lógica de negocio |
| API | Airtable REST API | Backend como servicio |
| Hosting | GitHub Pages | CDN estático |
| Analytics | Google Analytics 4 | Tracking |
| Linters | — | No configurados |
| Build tools | — | No requiere |

---

## 📞 Contacto

Desarrollado con 🧠 & 💛 por [AJRA](https://ajra.es)
Email: [info@ajra.es](mailto:info@ajra.es)
Sígueme en [Threads](https://threads.net/@ajra_toni) | [Instagram](https://instagram.com/ajra_toni) | [Facebook](https://facebook.com/AJRA.ES/)

---

**¡Que disfrutes explorando el universo DC!** 🚀🎬