# Portafolio Minimalista con JSON CV

[![Astro](https://img.shields.io/badge/Astro-5.1.1-FF5D01?style=flat-square&logo=astro&logoColor=white)](https://astro.build/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.5.4-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Licencia MIT](https://img.shields.io/badge/Licencia-MIT-green.svg)](LICENSE.txt)

Un portafolio minimalista y elegante basado en un archivo JSON que sigue el esquema de [jsonresume.org](https://jsonresume.org/schema/). Este proyecto te permite crear un CV profesional y una página web de portafolio personal utilizando un único archivo JSON como fuente de datos.

## 📋 Características

- **Diseño Minimalista**: Interfaz limpia y profesional inspirada en el diseño de [Bartosz Jarocki](https://github.com/BartoszJarocki/cv)
- **Basado en JSON**: Utiliza el estándar JSON Resume para almacenar toda tu información profesional
- **Fácil de Personalizar**: Modifica un solo archivo JSON para actualizar todo tu portafolio
- **Responsive**: Se adapta perfectamente a dispositivos móviles, tablets y escritorio
- **Exportación a PDF**: Funcionalidad para exportar tu CV como documento PDF
- **Optimizado para SEO**: Estructura optimizada para motores de búsqueda
- **Rápido y Ligero**: Construido con Astro para un rendimiento óptimo

## 🚀 Demo

Puedes ver una demostración del proyecto en [este enlace](https://gcruces.netlify.app/)

## 🛠️ Tecnologías Utilizadas

- [Astro](https://astro.build/) - Framework web moderno para sitios estáticos
- [TypeScript](https://www.typescriptlang.org/) - Superset tipado de JavaScript
- [HTML2Canvas](https://html2canvas.hertzen.com/) - Para capturas de pantalla del CV
- [jsPDF](https://parall.ax/products/jspdf) - Para generar documentos PDF
- [Hotkeypad](https://github.com/hotkeypad) - Para atajos de teclado

## 📁 Estructura del Proyecto

```
/
├── public/              # Activos estáticos
│   └── favicon.svg
├── src/
│   ├── components/      # Componentes reutilizables
│   │   ├── sections/    # Secciones del CV
│   │   │   └── Hero.astro
│   │   │   └── About.astro
│   │   │   └── Experience.astro
│   │   │   └── Education.astro
│   │   │   └── Projects.astro
│   │   │   └── Skills.astro
│   │   ├── KeyBoardManager.astro
│   │   └── Section.astro
│   ├── layouts/         # Plantillas de página
│   │   └── Layout.astro
│   ├── pages/           # Páginas de la aplicación
│   │   └── index.astro
│   ├── icons/           # Iconos del proyecto
│   └── cv.json          # Archivo principal con todos tus datos profesionales
└── package.json
```

## 🚀 Cómo Empezar

### Requisitos Previos

- [Node.js](https://nodejs.org/) (versión 16 o superior)
- [npm](https://www.npmjs.com/) (viene con Node.js)

### Instalación

1. **Clona este repositorio**
   ```bash
   git clone https://github.com/gcruces95/minimalist-portfolio-json.git
   cd minimalist-portfolio-json
   ```

2. **Instala las dependencias**
   ```bash
   npm install
   ```

3. **Personaliza tu CV**
   - Edita el archivo `src/cv.json` con tu información personal y profesional
   - El archivo sigue el esquema de [jsonresume.org](https://jsonresume.org/schema/)

4. **Inicia el servidor de desarrollo**
   ```bash
   npm run dev
   ```

5. **Accede a tu portafolio**
   - Abre [http://localhost:4321](http://localhost:4321) en tu navegador

## 📝 Personalización

### Datos del CV

Toda la información del portafolio se gestiona desde el archivo `src/cv.json`. Este archivo sigue la estructura del esquema JSON Resume, que incluye secciones para:

- Información básica y de contacto
- Experiencia laboral
- Educación
- Habilidades
- Proyectos
- Voluntariado
- Idiomas
- Intereses
- Referencias

### Personalización Visual

Si deseas personalizar el aspecto visual:

1. Los componentes de las secciones se encuentran en `src/components/sections/`
2. El layout principal está en `src/layouts/Layout.astro`
3. Los estilos generales pueden modificarse según las convenciones de Astro

## 📦 Despliegue

Para construir tu sitio para producción:

```bash
npm run build
```

Esto generará una versión optimizada de tu sitio en el directorio `dist/`, que puedes desplegar en cualquier servicio de hosting estático como:

- [GitHub Pages](https://pages.github.com/)
- [Netlify](https://www.netlify.com/)
- [Vercel](https://vercel.com/)
- [Cloudflare Pages](https://pages.cloudflare.com/)

## 🧞 Comandos Disponibles

| Comando                   | Acción                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Instala las dependencias                         |
| `npm run dev`             | Inicia el servidor de desarrollo en `localhost:4321` |
| `npm run build`           | Construye el sitio para producción en `./dist/`  |
| `npm run preview`         | Previsualiza tu build localmente antes de desplegar |
| `npm run astro ...`       | Ejecuta comandos CLI como `astro add`, `astro check` |
| `npm run astro -- --help` | Obtiene ayuda sobre el CLI de Astro              |

## 🤝 Contribuir

Las contribuciones son bienvenidas y apreciadas. Si deseas contribuir:

1. Haz un fork del repositorio
2. Crea una rama para tu característica (`git checkout -b feature/amazing-feature`)
3. Realiza tus cambios
4. Haz commit de tus cambios (`git commit -m 'Añade una característica increíble'`)
5. Haz push a la rama (`git push origin feature/amazing-feature`)
6. Abre un Pull Request

## 📄 Licencia

Este proyecto está licenciado bajo la Licencia MIT - vea el archivo [LICENSE.txt](LICENSE.txt) para más detalles.

## 👏 Agradecimientos

- [Bartosz Jarocki](https://github.com/BartoszJarocki/cv) por la inspiración del diseño
- [JSON Resume](https://jsonresume.org/) por el esquema estándar de CV
- [Astro](https://astro.build/) por el increíble framework

---

Desarrollado con ❤️ por [Gabriel Cruces Gallardo](https://github.com/gcruces95)