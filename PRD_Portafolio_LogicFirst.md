# Documento de Requerimientos de Producto (PRD)

## Proyecto: Portafolio Personal / Landing Page (Logic-First)

### 1. Visión General
El objetivo es crear una landing page personal alojada en GitHub Pages que funcione como portafolio digital definitivo. Está orientada a mostrar habilidades de desarrollo con un enfoque **logic-first** (centrado en la lógica, algoritmos y resolución de problemas técnicos), prescindiendo de proyectos reales con interfaces de usuario (UI) complejas en esta fase inicial.

### 2. Objetivos del Producto
* **Conversión:** Facilitar que los visitantes entiendan tu capacidad lógica y técnica mediante proyectos abstractos y te contacten de forma directa.
* **Rendimiento:** Carga ultrarrápida al ser un sitio estático (`index.html` autocontenido) optimizado para Lighthouse con +90 de puntuación.
* **Estética:** Interfaz profesional en **Dark Mode nativo** por defecto, evocando un entorno de terminal o desarrollo moderno.

---

### 3. Requerimientos Funcionales (UX/UI)

#### A. Hero Section (Inicio)
* **Título de alto impacto:** *"Transformo ideas complejas en código eficiente y soluciones de arquitectura."*
* **Subtexto:** Descripción orientada al desarrollo técnico, estructuras de datos y lógica pura sin dependencias pesadas.
* **Llamado a la Acción (CTA):** Dos botones principales: `[ Ver Proyectos de Lógica ]` (scroll a proyectos) y `[ Contacto Directo ]` (scroll a contacto).

#### B. Sección de Proyectos (Conceptual / Backend & Lógica)
Un grid de 4 tarjetas (*Cards*) con proyectos conceptuales enfocados netamente en algoritmos, optimización y manejo de datos:

1. **Motor de Emparejamiento de Datos (Data Matching Engine)**
   * **Descripción:** Algoritmo optimizado para comparar y unificar bases de datos masivas en milisegundos, detectando duplicados mediante distancia de Levenshtein de manera asíncrona.
   * **Tags:** `JavaScript` / `Algoritmos` / `Data Structures` / `Git`
   * **Enlaces:** `[ Ver Documentación de la API ]` y `[ Ver Repositorio ]`

2. **Simulador de Físicas en Consola (CLI Physics Sandbox)**
   * **Descripción:** Motor de cálculo bidimensional que procesa vectores de colisión, fuerza de gravedad y coeficientes de restitución elástica, exportando las matrices de estado en formato JSON estructurado.
   * **Tags:** `JavaScript` / `Matemáticas` / `Física` / `JSON`
   * **Enlaces:** `[ Ver Specs Técnicos ]` y `[ Ver Repositorio ]`

3. **Validador de Sintaxis y Autómata (State Machine Parser)**
   * **Descripción:** Extractor y parseador de texto basado en una máquina de estados finitos (FSM) que valida arquitecturas complejas de datos estructurados de manera determinista y sin dependencias externas.
   * **Tags:** `JavaScript` / `Regex` / `Ciencias de la Computación`
   * **Enlaces:** `[ Ver Arquitectura ]` y `[ Ver Repositorio ]`

4. **Middleware de Cache y Optimización de Memoria (In-Memory Cache Manager)**
   * **Descripción:** Sistema de gestión de memoria temporal basado en políticas de expiración estricta LRU (Least Recently Used), diseñado específicamente para optimizar tiempos de respuesta en consultas de alta complejidad.
   * **Tags:** `JavaScript` / `Optimización` / `Arquitectura`
   * **Enlaces:** `[ Ver Benchmark ]` y `[ Ver Repositorio ]`

#### C. Sección de Habilidades (Skills)
* Bloques limpios que listan el dominio técnico core: `HTML5`, `CSS3 / Responsive Design`, `JavaScript (ES6+)`, `Git & GitHub`, `Estructuras de Datos`, `Optimización de Código`, `JSON / RegEx`.

#### D. Sección de Contacto
* Formulario o enlaces directos de acción rápida para captación de clientes o propuestas: Email (`mailto:`), LinkedIn y GitHub.

---

### 4. Requerimientos No Funcionales & Técnicos

* **Arquitectura:** Single Page Application (SPA) estática en un único archivo `index.html` con CSS embebido para máxima velocidad.
* **Diseño:** 100% Responsivo adaptado a Mobile, Tablet y Desktop con semántica limpia.
* **Despliegue:** Alojamiento sin costo en **GitHub Pages** sincronizado a la rama principal (`main`).

---

### 5. Plan de Desarrollo y Lanzamiento

```
[Fase 1: Maquetación Dark Mode] ➔ [Fase 2: Integración de los 4 Proyectos] ➔ [Fase 3: Deploy GitHub Pages]
```

1. **Fase 1:** Configurar la estructura semántica base del HTML y variables de entorno CSS (`:root`) para el esquema de colores oscuros.
2. **Fase 2:** Poblar las tarjetas estáticas con la información de los 4 proyectos lógicos ficticios y configurar los hipervínculos vacíos (`#`).
3. **Fase 3:** Crear el repositorio público en GitHub, subir el archivo `index.html` y activar el servicio desde la pestaña *Settings -> Pages*.
