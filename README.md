<div align="center">

# 🚀 Portfolio 3D — José Luis Díaz Alonso

### Desarrollador Web Full Stack &amp; Desarrollador Android

*"Transformo ideas en aplicaciones Web y Android funcionales, rápidas y listas para producción."*

<br>

![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white&style=for-the-badge)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite&logoColor=white&style=for-the-badge)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3-06B6D4?logo=tailwindcss&logoColor=white&style=for-the-badge)
![Three.js](https://img.shields.io/badge/Three.js-R3F-8B5CF6?logo=three.js&logoColor=white&style=for-the-badge)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-EC4899?logo=framer&logoColor=white&style=for-the-badge)
![License](https://img.shields.io/badge/Licencia-MIT-22D3EE?style=for-the-badge)

<br>

[![Estado](https://img.shields.io/badge/Estado-En%20desarrollo-f59e0b?style=flat-square)](#-roadmap)
[![Último commit](https://img.shields.io/github/last-commit/TU-USUARIO/TU-REPOSITORIO?style=flat-square&color=22d3ee)](../../commits/main)
[![Issues abiertos](https://img.shields.io/github/issues/TU-USUARIO/TU-REPOSITORIO?style=flat-square&color=8b5cf6)](../../issues)

**[🌐 Ver demo en producción](https://joseluisdiazdeveloper.es)** · **[🐛 Reportar un problema](../../issues/new)**

</div>

## 📖 Índice

- [Sobre el proyecto](#-sobre-el-proyecto)
- [Vista previa](#-vista-previa)
- [Características](#-características)
- [Stack tecnológico](#-stack-tecnológico)
- [Estructura del proyecto](#-estructura-del-proyecto)
- [Puesta en marcha](#-puesta-en-marcha)
- [Scripts disponibles](#-scripts-disponibles)
- [Internacionalización](#-internacionalización)
- [Rendimiento](#-rendimiento)
- [Roadmap](#-roadmap)
- [Licencia](#-licencia)
- [Contacto](#-contacto)

---

## 💡 Sobre el proyecto

Portfolio personal en formato **web 3D**, pensado para presentar de forma visual y profesional
mi trabajo como desarrollador Web Full Stack y desarrollador Android freelance. El objetivo no
es solo mostrar proyectos: es que el propio sitio funcione como una demostración de nivel técnico,
combinando una estética "oscuro futurista", animaciones cuidadas y una arquitectura pensada para
cargar rápido y funcionar bien en la mayoría de dispositivos, no solo en los más potentes.

El proyecto sigue un enfoque **híbrido de 3D**: una escena interactiva con Three.js reservada
para la sección principal (donde más impacto visual aporta), y micro-interacciones ligeras con
CSS 3D + Framer Motion en el resto del sitio, para mantener el rendimiento bajo control.

---

## ✨ Características

- 🎬 **Hero 3D interactivo** — objeto wireframe construido con React Three Fiber, con parallax
  según la posición del ratón, carga diferida (`lazy`) y *fallback* estático para dispositivos
  de gama baja o con `prefers-reduced-motion` activado.
- 🧩 **Tilt 3D con CSS** en el resto de secciones (tarjetas de proyectos, etc.) — sin coste de
  WebGL fuera del Hero.
- 🛠️ **Sección Herramientas** con barras de progreso animadas al entrar en el viewport.
- 💼 **Sección Proyectos** con enlaces condicionales: solo se muestra el acceso a la Web y/o a
  Google Play cuando el proyecto realmente lo tiene.
- 🎓 **Timeline de Formación** responsive (zig-zag en desktop, lineal en mobile).
- 📬 **Contacto directo** vía LinkedIn, GitHub, Email y WhatsApp.
- 📰 **Blog** con artículos (origen LinkedIn), listado + vista de detalle por artículo.
- 🌍 **Selector de idioma ES / EN** persistente.
- ⬆️ **Botón "volver arriba"** flotante tras cierto scroll.
- 📱 **100% responsive** — mobile, tablet y desktop.
- ⚡ **Enfocado en rendimiento**: code-splitting del bundle 3D, imágenes optimizadas y carga
  diferida fuera del viewport inicial.

---

## 🧱 Stack tecnológico

| Categoría | Tecnología |
|---|---|
| Framework | [React](https://react.dev/) + [Vite](https://vitejs.dev/) |
| Estilos | [TailwindCSS](https://tailwindcss.com/) |
| 3D | [Three.js](https://threejs.org/) vía [React Three Fiber](https://docs.pmnd.rs/react-three-fiber) + [drei](https://github.com/pmndrs/drei) |
| Animación | [Framer Motion](https://www.framer.com/motion/) |
| Internacionalización | [react-i18next](https://react.i18next.com/) |
| Enrutado | [React Router](https://reactrouter.com/) (vista de detalle del blog) |
| Despliegue | [Vercel](https://vercel.com/) |

---

## 📂 Estructura del proyecto

```
├── public/
│   └── cv.pdf                  # CV descargable desde la sección "Sobre Mí"
├── src/
│   ├── assets/                 # Imágenes, iconos, modelos 3D
│   ├── components/             # Componentes reutilizables (Navbar, BackToTop, Card, etc.)
│   ├── sections/                # Hero, Herramientas, Proyectos, Formación, Contacto, Blog, Footer
│   ├── data/                    # tools.json · projects.json · education.json · blog.json
│   ├── i18n/
│   │   ├── es.json
│   │   └── en.json
│   ├── App.jsx
│   └── main.jsx
├── docs/
│   ├── mockup/                  # PDF de diseño / referencia visual
│   └── screenshots/             # Capturas reales para este README
├── tailwind.config.js
├── vite.config.js
└── package.json
```

---

## 🚀 Puesta en marcha

### Requisitos previos

- [Node.js](https://nodejs.org/) 18 o superior
- npm (o pnpm/yarn, ajustando los comandos)

### Instalación

```bash
# 1. Clona el repositorio
git clone https://github.com/TU-USUARIO/TU-REPOSITORIO.git
cd TU-REPOSITORIO

# 2. Instala las dependencias
npm install

# 3. Levanta el entorno de desarrollo
npm run dev
```

El proyecto quedará disponible en `http://localhost:5173` (puerto por defecto de Vite).

---

## 📜 Scripts disponibles

| Comando | Descripción |
|---|---|
| `npm run dev` | Levanta el servidor de desarrollo con recarga en caliente |
| `npm run build` | Genera la build de producción en `/dist` |
| `npm run preview` | Sirve localmente la build de producción para revisarla |
| `npm run lint` | Ejecuta ESLint sobre todo el proyecto |

---

## 🌍 Internacionalización

El contenido textual del sitio vive en `src/i18n/es.json` y `src/i18n/en.json`. Para añadir un
nuevo idioma:

1. Duplica uno de los ficheros JSON y tradúcelo.
2. Regístralo en la configuración de `react-i18next`.
3. Añade la opción correspondiente en el selector de idioma del `Navbar`.

---

## ⚡ Rendimiento

Este proyecto prioriza que el sitio cargue rápido y vaya fluido en la mayoría de dispositivos,
no solo en los de gama alta. Puntos clave a mantener en cada cambio:

- El bundle de **Three.js/React Three Fiber no debe formar parte del chunk principal** —
  siempre cargado vía `React.lazy`.
- Objetivo de referencia en Lighthouse (mobile): **Performance ≥ 90**, **Accesibilidad ≥ 95**.
- Imágenes en formato moderno (WebP/AVIF) y con `loading="lazy"` fuera del viewport inicial.
- Respetar siempre `prefers-reduced-motion` para desactivar animaciones no esenciales.

---

## 🗺️ Roadmap

- [x] Setup inicial del proyecto (Vite + React + Tailwind)
- [x] Sistema de diseño (tokens Tailwind)
- [x] Internacionalización ES/EN
- [ ] Navbar (desktop + mobile) y botón "volver arriba"
- [ ] Sección Hero — contenido y maquetación
- [ ] Sección Hero — integración de la escena 3D
- [ ] Sección Herramientas
- [ ] Sección Proyectos
- [ ] Sección Formación
- [ ] Sección Contacto
- [ ] Blog (listado + detalle)
- [ ] Footer
- [ ] QA responsive multi-dispositivo
- [ ] Auditoría de rendimiento (Lighthouse)
- [ ] Despliegue y CI

> El backlog completo, con historias de usuario, criterios de aceptación y estimaciones para
> cada punto, está en las *Issues* de este repositorio.

---

## 📄 Licencia

Este proyecto se distribuye bajo la licencia **MIT**. Consulta el archivo [`LICENSE`](LICENSE)
para más detalles.

---

## 📬 Contacto

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/TU-USUARIO-LINKEDIN)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/TU-USUARIO)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tu-email@ejemplo.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/TUNUMERO)

**José Luis Díaz Alonso** — Madrid, España

</div>

<br>

<div align="center">
<sub>Diseñado y desarrollado por José Luis Díaz Alonso · © 2026</sub>
</div>
