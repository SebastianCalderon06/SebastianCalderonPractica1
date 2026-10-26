# Respuesta a la Auditoría Recibida

**Proyecto:** Club Deportivo Calderón  
**Fecha de Respuesta:** 25 de Octubre de 2026  

---

## Plan de Acción y Correcciones Realizadas

### Hallazgo 1: Contraste en el `nav` (Modo Oscuro)
* **Estado:** Correctivo implementado.
* **Respuesta / Solución:** Se crearon variables CSS `--color-header-bg` y `--color-header-texto` con valores diferenciados para modo claro y modo oscuro (`@media (prefers-color-scheme: dark)`). En modo oscuro, se ajustó el tono del encabezado y texto logrando una relación de contraste superior a **4.5:1** conforme a la norma WCAG 2.2.

---

### Hallazgo 2: Contraste en el Botón de Envío (Modo Oscuro)
* **Estado:** Correctivo implementado.
* **Respuesta / Solución:** Se añadió la variable `--color-texto-boton`. En modo claro el texto se mantiene en `#ffffff` sobre azul oscuro, mientras que en modo oscuro el texto cambia a `#1c1917` (oscuro) sobre el fondo de botón rosa (`#fb7185`), alcanzando una relación de contraste de **7:1** (Cumple norma WCAG 2.2 AAA).

---

### Hallazgo 3: Colores fijos sin usar `var()`
* **Estado:** Correctivo implementado.
* **Respuesta / Solución:** Se eliminaron las definiciones de color en código hexadecimal directo (`#e7c270`, `#e5aa70`, `#ffffff`) de los elementos `header`, `aside` y `button`. En su lugar, se vincularon a sus respectivas variables globales declaradas en `:root` mediante la función `var()`.