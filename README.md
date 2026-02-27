# IMAR Costa Norte - Arquitectura Web con Astro & Tailwind (CONCEPT)

Este repositorio contiene el rediseño integral de la plataforma institucional de **IMAR Costa Norte**. El proyecto destaca por una arquitectura modular que separa la lógica de marca corporativa de la identidad visual de proyectos específicos (como Cuencas Vivas). 

**Demo:** [https://Imarc-prototipo.concept](https://clever-starship-947434.netlify.app/)

**Screnshots:** [Imagenes-Referenciales](./public/screenshots/2026-02-27-122514_hyprshot.png)

## Especificaciones Técnicas del Código

El proyecto ha sido descompuesto en componentes reutilizables y layouts inteligentes para optimizar el mantenimiento y el rendimiento.

### 1. Sistema de Layouts (Estructura Maestra)
- **`MainLayout.astro`**: Centraliza la identidad institucional. Incluye una navegación con efecto `backdrop-blur` (cristal esmerilado) y un footer complejo con grid responsivo. Gestiona el menú móvil mediante un script inyectado directamente en el componente.
- **`CuencasLayout.astro`**: Un layout especializado para el proyecto "Cuencas Vivas". Cambia el esquema de navegación a uno minimalista y carga estilos CSS exclusivos para esta submarca, demostrando versatilidad en el manejo de múltiples identidades visuales.

### 2. Componentes de Configuración
- **`BaseHead.astro`**: El cerebro del SEO. Centraliza los metadatos, la configuración del viewport y la precarga de tipografías (**Inter** y **Outfit**). Al usar este componente en todos los layouts, se garantiza que el SEO sea consistente en todo el sitio.

### 3. Desarrollo de Páginas (Rutas)
Cada archivo `.astro` en la carpeta `pages/` utiliza un sistema de composición:
- **`index.astro`**: Página de aterrizaje con secciones de héroe dinámicas y grid de aliados estratégicos con efectos de escala y filtros de escala de grises.
- **Áreas Temáticas (`gestion-agua.astro`, `gestion-ambiental.astro`, etc.)**: Utilizan estructuras de `MainLayout` y presentan una barra lateral de navegación interna para mejorar la retención del usuario.
- **`cuencas-vivas.astro`**: Implementa el `CuencasLayout`, utilizando secciones de impacto visual con gradientes lineales sobre imágenes para garantizar la legibilidad del texto.
- **`contacto.astro`**: Integra formularios de captura de datos y un mapa embebido de Google Maps optimizado para contenedores con bordes redondeados (`rounded-2xl`).

### 4. Ingeniería de Estilos (CSS & UI)
- **`global.css`**: Configuración base de Tailwind CSS.
- **`imar-modern.css`**: Define el sistema de diseño corporativo (Azul Profundo #0056b3 y Teal #07d5c0) mediante variables CSS nativas. Incluye efectos de elevación en tarjetas (`hover:-translate-y-1`).
- **`cuencas-vivas-theme.css`**: Paleta cromática inspirada en la naturaleza (Verde Bosque #2d6a4f y Tierra #d4a373) para el proyecto ecológico.

## Funcionalidades Clave Implementadas

* **Atomic Design:** Separación clara entre el "esqueleto" (Layouts) y el "contenido" (Pages).
* **Diseño Responsivo Avanzado:** Uso extensivo de clases de Tailwind como `md:grid-cols-3` y `sm:flex-row` para adaptabilidad total.
* **Optimización de Rendimiento:** Gracias a Astro, el sitio tiene un tiempo de carga mínimo al eliminar JavaScript innecesario del lado del cliente.
* **Micro-interacciones:** Transiciones suaves de color y escala en botones y enlaces de navegación (`transition-all duration-500`).

## Jerarquía de Archivos

```text
/src
  ├── components/
  │   └── BaseHead.astro       # Configuración global de metadatos
  ├── layouts/
  │   ├── MainLayout.astro     # Layout corporativo principal
  │   └── CuencasLayout.astro   # Layout para proyectos ecológicos
  ├── pages/
  │   ├── index.astro          # Landing principal
  │   ├── contacto.astro       # Página de contacto y ubicación
  │   └── areas-tematicas/     # Repositorios técnicos de gestión
  └── styles/
      ├── global.css           # Tailwind base
      ├── imar-modern.css      # Estilos corporativos
      └── cuencas-vivas-theme.css # Estilos de proyecto
```
⚠️ **Nota importante:** Este proyecto **no es la página oficial** ni tiene vínculo laboral vigente con la institución. Es un concepto desarrollado con **fines educativos y de aprendizaje propio**. Lo hice para pulir mis habilidades en el stack moderno.