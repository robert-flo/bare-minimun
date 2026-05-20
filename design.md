# Guía de Diseño del README — BARE-MINIMUN

Este documento establece las directrices visuales, técnicas y de formato para el mantenimiento y evolución del archivo `README.md` de **BARE-MINIMUN**. Cualquier IA o desarrollador que edite el README debe seguir estrictamente estas reglas para garantizar la coherencia y uniformidad del diseño.

---

## 🎨 Paleta de Colores (Catppuccin Macchiato)

El diseño visual se basa rigurosamente en la paleta de colores **Catppuccin Macchiato** para mantener un aspecto moderno, suave y de temática oscura (*dark mode*).

### Colores de Acento (Shields.io & SVGs)

* **Mauve (Púrpura Principal):** `#cba6f7` (Utilizado para títulos y acentos principales).
* **Lavender (Lavanda):** `#b7bdf8` (Utilizado para subtítulos, enlaces e información secundaria).
* **Red (Rojo):** `#f38ba8` o `#e06c75` (Utilizado para etiquetas de actualización o alertas críticas).
* **Peach (Melocotón):** `#f5a97f` (Colaboradores / Gente).
* **Yellow (Amarillo):** `#eed49f` (Estrellas / Destacados).
* **Green (Verde):** `#a6e3a1` (Forks / Éxito).
* **Sky (Celeste):** `#89dceb` (Watchers / Observadores).
* **Base/Base Gray (Fondo de Badges):** `#363a4f` (Utilizado como el parámetro `colorA` en las insignias de Shields.io).

---

## 🅰️ Tipografías

* **Títulos de Cabecera (Title/Subtitle):** *Outfit* (Limpia, moderna, excelente legibilidad en pantalla).
* **Secciones Principales (Separadores SVG):** *Lexend Giga* (Estilo geométrico y futurista).

---

## 📐 Estructura y Reglas del README

### 1. Cabecera Dinámica (Typing SVGs)

* **Separación del Título y Subtítulo:** El título (`bare-minimun`) y el subtítulo (`Minimalist template repository. ✨🛠`) deben ir en líneas e imágenes independientes, separadas por un `<br/>`. Esto evita problemas de superposición y permite que ambas animaciones se ejecuten simultáneamente.
* **Configuración del Título:** `font=Outfit&size=40&color=cba6f7&center=true&vCenter=true&width=600&height=55`
* **Configuración del Subtítulo:** `font=Outfit&size=20&color=b7bdf8&center=true&vCenter=true&width=600&height=35`

### 2. Formato de Badges y Enlaces (Regla del "Sin Espacio")

> [!IMPORTANT]
> **Evitar Subrayados Azules (Rayas Celestes):** GitHub renderiza saltos de línea o espacios en blanco dentro de las etiquetas de anclaje `<a>` como texto subrayado con el color de enlace del sistema.

* **Solución Obligatoria:** Todas las etiquetas `<a>` que envuelvan una imagen `<img>` deben escribirse en una **sola línea contigua, sin espacios internos ni saltos de línea**:
  * *Correcto:* `<a href="..."><img src="..." /></a>`
  * *Incorrecto:*

    ```html
    <a href="...">
      <img src="..." />
    </a>
    ```

* **Agrupamiento:** Los grupos de badges (en la cabecera) y los iconos de contacto (en el pie de página) deben declararse todos en la misma línea de código o usando espaciadores externos `&nbsp;`.

### 3. Barra de Navegación Centrada

* Usa elementos `<kbd>` para dar un aspecto de botón/teclado físico con bordes limpios.
* Añade etiquetas `<br>` dentro del texto de los enlaces de navegación para darles un efecto de botón alto y moderno con suficiente margen vertical.
* *Ejemplo:* `<a href="#features"><kbd> <br> ✨ Features <br> </kbd></a>`

### 4. Separadores de Sección SVG

* Cada sección principal del documento debe comenzar con un encabezado generado dinámicamente mediante `readme-typing-svg`.
* *Formato del SVG:* `https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=24&pause=1000&color=cba6f7&vCenter=true&width=450&height=30&lines=NOMBRE+DE+SECCIÓN`

### 5. Bloques de Alerta (Callouts)

* Usa los bloques nativos de GitHub Flavored Markdown (`> [!IMPORTANT]`, `> [!TIP]`, `> [!WARNING]`).
* **Regla de Parseo:** Para que mantengan sus colores distintivos y no se rendericen como texto plano gris, **siempre deben contener texto inmediatamente en el bloque de cita**.
* **Scoping (Alineación Limpia):** Para evitar desalineaciones estéticas en listas de dependencias, mantén la caja de alerta enfocada únicamente en el título/etiqueta y coloca el texto descriptivo o las listas con viñetas fuera del bloque (sin el símbolo `>`).

### 6. Pie de Página y Contacto

* **Llamado a la Acción (CTA):** Mantener siempre la frase de invitación centrada: `<sub>📬 **Get in touch!** Feel free to reach out...</sub>`.
* **Iconos e Imágenes:** Dado que GitHub sanitiza e inhabilita las etiquetas `<svg>` en línea, los iconos personalizados (como el del correo) deben cargarse desde archivos locales `.svg` usando una etiqueta `<img>` normal (`src="docs/images/mail.svg"`).
