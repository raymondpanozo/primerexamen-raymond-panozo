# primerexamen-raymond-panozo
PRIMER EXAMEN

Yo RAYMOND JESUS PANOZO CRESPO tecnico superior en SISTEMAS INFORMATICOS "Oruro - Bolivia" que actualmente estudia en la
universidad UAB universidad adventista de Bolivia - licenciatura en ingieniria de sistemas
 he sido contratado como desarrollador/a web por la empresa MANACO para crear una landing
page de la empresa.

Accesibilidad (a11y)
•  1 Skip link: Cómo se hizo: Con CSS lo “escondemos” fuera de pantalla y al recibir foco (:focus) aparece.
Esto permite a personas con lectores de pantalla o que navegan con teclado saltar directamente al contenido, evitando pasar siempre por el menú.
Por qué se hizo: Recomendación WCAG 2.1 (2.4.1 Bypass Blocks), Mejora usabilidad para usuarios de teclado. Enlace al inicio para saltar directo al contenido principal.
•  2 Contraste de colores: Cómo se validó: En el CSS usé colores oscuros sobre fondo claro (#111 sobre #fff, contraste de 21:1). El enlace skip-link tiene blanco sobre azul oscuro (#1a3d7c) → contraste de 9.7:1.
Por qué se hizo: Cumplir con WCAG 1.4.3 (Contraste mínimo): nivel AA pide al menos 4.5:1 para texto normal.
•  3 Navegación por teclado: Cómo se hizo: En cualquier navegador puedes usar: Tab → avanza entre enlaces y botones, Shift + Tab → retrocede, Enter → activa enlaces, En el código: Todos los elementos interactivos son nativos de HTML (<a>, <button> implícito, <input> si existiera),
No se usaron div con onclick (mala práctica, rompe accesibilidad) y :focus tiene estilos visibles (outline azul).
Por qué se hizo:Cumple WCAG 2.1.1 (Teclado) y es obligatorio que todo sea accesible sin mouse.
•  4 Texto alternativo en imágenes: Cómo se hizo: Cada <img> tiene un alt descriptivo y contextual.
Por qué se hizo: Cumple WCAG 1.1.1 (Texto alternativo) y permite que lectores de pantalla describan el producto.
•  5 Uso de aria-* solo si es necesario: Cómo se hizo: En <nav> añadí aria-label="Navegación principal", esto da contexto si hay varios menús en la página, no puse role="main", role="footer", etc. porque HTML5 ya es semántico.
Por qué se hizo:Evitar “sobrecargar” con ARIA y Regla: "Usa HTML antes que ARIA" (first rule of ARIA).

