<div align="center">

# 🔍 ReqLens

### **Análisis de Requerimientos por Inspección Visual**

*Una herramienta educativa y profesional que transforma interfaces de software existentes en especificaciones de requerimientos formales mediante Inteligencia Artificial.*

![ReqLens Banner](assets/reqlens-banner.png)

[![MIT License](https://img.shields.io/badge/License-MIT-3b82f6.svg?style=for-the-badge&logo=mit&logoColor=white)](LICENSE)
[![Engine](https://img.shields.io/badge/AI_Engine-Claude_3.5_Sonnet-d97706.svg?style=for-the-badge&logo=anthropic&logoColor=white)](https://www.anthropic.com/)
[![HTML5](https://img.shields.io/badge/Frontend-HTML5_/_CSS3-e34f26.svg?style=for-the-badge&logo=html5&logoColor=white)](https://html.spec.whatwg.org/)
[![UI Style](https://img.shields.io/badge/UI_Style-Premium_Dark-6366f1.svg?style=for-the-badge&logo=csswizardry&logoColor=white)](#diseño-visual-impecable)

---

[✨ Características](#-características-principales) · [🚦 Modos de Trabajo](#-modos-de-trabajo-onboarding-ramificado) · [📂 Estructura](#-estructura-del-proyecto) · [🚀 Cómo Usar](#-cómo-usar) · [🔒 Seguridad](#-api-key-y-seguridad)

</div>

---

## 📖 ¿Qué es ReqLens?

**ReqLens** toma lo que cualquier persona puede observar de un sistema de software (sus pantallas, flujos de navegación y comportamiento visual) y, mediante el poder del motor de **Claude (Anthropic)**, infiere y construye el levantamiento de requerimientos formal que se necesitaría para reproducirlo desde cero.

Con un enfoque de **inspección técnica**, la herramienta está diseñada con una estética minimalista premium (estilo *taste* / Emil Kowalski) sobre un entorno ultra-oscuro, fluido e interactivo.

---

## ✨ Características Principales

*   **📄 Especificación IEEE 830 Completa:** Genera de forma automatizada un documento de requerimientos funcionales y no funcionales estructurado y listo para descargar en texto plano.
*   **📊 Diagrama de Módulos Interactivo:** Renderiza un mapa arquitectónico de bloques que representa la estructura, responsabilidades y relaciones de dependencia del sistema.
*   **📐 Modelo Conceptual de Entidades:** Identifica las entidades principales, atributos inferidos (con su respectiva fuente de origen) y relaciones de cardinalidad.
*   **🛡️ Niveles de Confianza (Trazabilidad):** Cada requerimiento es clasificado dinámicamente con una etiqueta visible:
    *   `[CONFIRMADO]` — Observado directamente en las capturas o descripción provistas.
    *   `[INFERIDO]` — Sugerido de manera lógica por ser estándar para el dominio del negocio.
    *   `[NO ACCESIBLE]` — Identificado como necesario pero oculto tras pantallas de login o permisos especiales.
*   **🌐 100% en Español:** Traduce e interpreta interfaces construidas en cualquier idioma al español técnico estándar de ingeniería de software.

---

## 🚦 Modos de Trabajo (Onboarding Ramificado)

La herramienta ajusta el nivel de asistencia en la UI en función del perfil y las necesidades del usuario:

| Modo | 🎯 Enfoque | 📋 Requisitos | 💡 Experiencia de UI |
| :--- | :--- | :--- | :--- |
| **Aprendizaje** | **Educativo** (Ideal para estudiantes) | Capturas de pantalla obligatorias con validación previa. | Guía paso a paso explicando conceptos de ingeniería de software en cada paso. |
| **Guiado** | **Asistencia Moderada** | Capturas o texto opcionales. | Avisos puntuales solo en zonas críticas del análisis sin tutoriales intrusivos. |
| **Profesional** | **Máxima Velocidad** (Para profesionales) | Entrada libre (capturas, texto o ambas) con mayor límite de caracteres. | Interfaz directa enfocada a la agilidad de análisis. |

---

## 🎨 Diseño Visual Impecable

ReqLens ha sido pulido con una estética moderna y funcional que prioriza la experiencia interactiva:

*   **Estilo 'Taste' / Emil Kowalski:** Fondos negros profundos (`#060709`), bordes ultra-finos semi-transparentes y un uso estratégico del color azul lente (`#3b82f6`) y cian escaneo (`#06b6d4`).
*   **Desenfoques de Vidrio (Glassmorphism):** La cabecera, los modales y el overlay de carga incorporan `backdrop-filter: blur(12px)` para una sensación táctil y premium.
*   **Microanimaciones de Entrada:** Las pantallas del onboarding y las tarjetas se deslizan con transiciones `fadeInUp` orgánicas y de ritmo ágil (`cubic-bezier(0.16, 1, 0.3, 1)`).
*   **Carga Estilo Retícula:** El cargador de análisis simula un objetivo o lente óptico de alta precisión con anillos que giran de forma concéntrica a diferentes velocidades.

---

## 📂 Estructura del Proyecto

El código está estructurado para facilitar la escalabilidad y la edición independiente:

```
reqlens/
├── assets/
│   └── reqlens-banner.png — Imagen de banner que representa el sistema
├── index.html             — Estructura HTML y lógica JS (API, canvas y modales)
├── style.css              — Tokens de diseño, animaciones y responsive layout
└── README.md              — Documentación del proyecto (este archivo)
```

### Tecnologías Utilizadas

-   **Lucide Icons:** Sistema de iconografía limpio de alta resolución.
-   **Google Fonts:** Fuentes *Outfit* (títulos), *Inter* (cuerpo de texto) y *JetBrains Mono* (código e identificadores).
-   **Anthropic API:** Claude 3.5 Sonnet como motor inteligente de inferencia y traducción.

---

## 🚀 Cómo Usar

### Opción A: Uso Local Rápido (Sin Servidor)
1. Descarga el repositorio o los archivos [index.html](index.html) y [style.css](style.css) en una misma carpeta.
2. Haz doble clic en `index.html` para abrirlo directamente en cualquier navegador (Chrome, Edge, Firefox, Safari).
3. Ingresa tu API Key de Anthropic, selecciona tu modo, sube tus capturas y haz clic en **Iniciar Análisis**.

### Opción B: Clonar el Repositorio
```bash
git clone https://github.com/tu-usuario/reqlens.git
cd reqlens
# Abre index.html en tu navegador
```

### Opción C: Despliegue en la Nube
Puedes subir este proyecto a plataformas como **Vercel** o **Netlify** de forma directa. Al ser una aplicación puramente frontend, no requiere configuración de compilación ni servidores backend.

---

## 🔒 API Key y Seguridad

ReqLens realiza las peticiones a la API de Anthropic **directamente desde tu navegador (cliente-servidor)** mediante el encabezado `anthropic-dangerous-direct-browser-access`.

> [!NOTE]
> **Privacidad:** Tu API Key se almacena únicamente en el `localStorage` de tu navegador de manera codificada. Ningún servidor intermedio o tercero tiene acceso a ella.

> [!IMPORTANT]
> **Costos:** El costo aproximado por análisis completo (validaciones, diagramas, IEEE 830) es de **$0.04 USD**. Anthropic suele otorgar $5 USD en créditos gratuitos al crear tu cuenta en [console.anthropic.com](https://console.anthropic.com).

---

## 🤝 Relación con StakeFlow

ReqLens y [StakeFlow](https://github.com/tu-usuario/stakeflow) son soluciones hermanas diseñadas para abordar los dos flujos principales de la ingeniería de requerimientos:

| Solución | 🎯 Enfoque Principal | 🏁 Punto de Partida |
| :--- | :--- | :--- |
| **StakeFlow** | Elicitación conversacional mediante entrevistas simuladas con stakeholders ficticios. | Un proyecto nuevo en fase de idea (sin código ni pantallas). |
| **ReqLens** | Ingeniería inversa de requerimientos funcionales a través de la inspección de interfaces. | Un sistema ya construido (de la competencia o de apoyo) que se quiere analizar. |

---

## ⚠️ Uso Responsable

ReqLens es un proyecto con fines educativos y de aprendizaje.
*   **No extrae código fuente**, contenido protegido por propiedad intelectual ni activos visuales protegidos.
*   Infiere de manera conceptual cómo opera un modelo de negocio a nivel genérico (ej. especifica "un carro de compras" en lugar de simular la marca analizada).
*   No debe utilizarse con fines comerciales que infrinjan los términos de servicio de los sistemas analizados.

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Siéntete libre de adaptarlo, modificarlo y compartirlo con atribución.

<div align="center">
Construido con el motor inteligente de Anthropic Claude · ReqLens v1.0
</div>
