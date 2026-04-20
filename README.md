# 🌊 IMAR Costa Norte - Concept Design 

![Astro](https://img.shields.io/badge/Astro-BC52EE?style=for-the-badge\&logo=astro\&logoColor=white) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge\&logo=tailwind-css\&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge\&logo=typescript\&logoColor=white) 

## 📌 Descripción

Este proyecto consiste en un **rediseño conceptual integral** de la plataforma institucional de **IMAR Costa Norte**.

El enfoque principal fue construir una arquitectura web moderna, modular y altamente eficiente, separando claramente la identidad corporativa de los proyectos específicos.

🔗 **Demo en vivo:**
👉 [https://clever-starship-947434.netlify.app/](https://clever-starship-947434.netlify.app/)

---

## 🧠 Enfoque Técnico

El desarrollo prioriza:

* **Escalabilidad**
* **Performance**
* **Modularidad**
* **Separación de responsabilidades**

Todo bajo el stack **Astro + Tailwind CSS + TypeScript**.

---

## 🛠️ Stack Tecnológico

| Tecnología   | Uso                                                         |
| ------------ | ----------------------------------------------------------- |
| Astro        | Renderizado optimizado y arquitectura basada en componentes |
| Tailwind CSS | Sistema de diseño y estilos utilitarios                     |
| TypeScript   | Tipado estático y robustez del código                       |

---

## 🧩 Arquitectura del Proyecto

### 1. Layouts Inteligentes

Se implementa una arquitectura basada en layouts anidados:

* **`MainLayout.astro`**

  * Identidad institucional
  * Navegación con `backdrop-blur`
  * Sistema de menús reactivos

* **`CuencasLayout.astro`**

  * Layout independiente
  * Tematización específica para proyectos ecológicos
  * Demuestra desacoplamiento visual

---

### 2. Optimización y SEO

* **`BaseHead.astro`**

  * Gestión centralizada de metadatos
  * Configuración SEO On-page
  * Integración de fuentes (Inter / Outfit)

* **Astro Islands**

  * JavaScript solo cuando es necesario
  * Mejora directa en:

    * LCP
    * TTI
    * CLS

---

### 3. Ingeniería de Estilos

* **Tematización dinámica**

  * Variables CSS + Tailwind
  * Modos:

    * Corporativo (Azul / Teal)
    * Ecológico (Bosque / Tierra)

* **UI/UX**

  * Micro-interacciones
  * Efectos tipo glassmorphism
  * Layouts responsivos avanzados

---

## 📂 Estructura del Proyecto

```bash
/src
  ├── components/      # Componentes reutilizables (Atomic Design)
  ├── layouts/         # Layouts principales
  ├── pages/           # Rutas del sitio
  └── styles/          # Tailwind + CSS personalizado
```

---

## 🚀 Logros Técnicos

* **Atomic Design**

  * Separación clara entre UI, lógica y estructura

* **Responsive Design Avanzado**

  * Adaptabilidad completa en múltiples dispositivos

* **Performance Optimizada**

  * Enfoque *Zero-JS por defecto*
  * Alta puntuación en Lighthouse

---

## ⚠️ Nota

Este proyecto es un **concepto técnico independiente** desarrollado con fines educativos y de crecimiento profesional.
No representa un producto oficial, sino un ejercicio de arquitectura web moderna.

Creado por **rembodev**
