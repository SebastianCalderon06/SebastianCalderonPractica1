# Informe de Auditoría Recibido

**Proyecto Auditado:** Club Deportivo Calderón  
**Fecha de Recepción:** 25 de Octubre de 2026  

---

## Tabla de Hallazgos Recibidos

| N° | Requisito | Ubicación | Hallazgo | Norma que incumple | Evidencia | Severidad |
| :-: | :--- | :--- | :--- | :-: | :-: | :-: |
| **1** | Base 5: contraste | `estilos.css`, línea 77, color `#e7c270` | El contraste entre el fondo y el texto del `nav` no cumple con la relación 4.5:1 en modo oscuro. | WCAG 2.2 (1.4.3) | `evidencia/evi_1.png` | Alta |
| **2** | Base 5: contraste | `estilos.css`, líneas 201 y 202 | El contraste entre el fondo del botón y el texto no cumple con la relación 4.5:1 en modo oscuro. | WCAG 2.2 (1.4.3) | `evidencia/evi_2.png` | Alta |
| **3** | Base 5: colores en `var()` | `estilos.css`, línea 55 | Se definen colores directamente en código hexadecimal sin hacer uso de variables `var()`. | W3C | `evidencia/evi_3.png` | Baja |