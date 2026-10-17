# Checklist de entrega

Revisión final antes de dar por terminada una interfaz. Aplica a web, producto, datos, móvil y contenido.

## Jerarquía y composición

- [ ] El primer viewport o pantalla comunica qué es el producto y qué hacer después.
- [ ] La escala, el espacio y la imagen crean jerarquía y un ritmo sostenido.
- [ ] Cada sección o vista tiene un propósito y contenido real.
- [ ] No hay patrones repetidos de forma mecánica (título + párrafo + botón en todo).

## Sistema visual

- [ ] Tipografía, color, superficies, bordes y controles se sienten del mismo sistema.
- [ ] Los tokens (color, espacio, radios, sombras) se usan de forma consistente.
- [ ] Los componentes comparten reglas: radios, bordes, sombras, estados.
- [ ] El color es solo blanco, gris y negro salvo petición expresa; no hay fondos tintados.
- [ ] La tipografía es sans (sin serif ni cursivas) y no hay logotipo inventado si el proyecto no tiene uno.
- [ ] Color de acento solo si el proyecto lo justifica.
- [ ] El color tiene función (jerarquía, estado, marca), no decora sin motivo.

## Comportamiento

- [ ] Los enlaces navegan y los botones actúan; no hay affordances muertas.
- [ ] Los formularios validan y muestran errores comprensibles con etiquetas persistentes.
- [ ] Existen estados vacíos, de carga y de error donde corresponda.
- [ ] El móvil usa menú y controles táctiles funcionales.

## Accesibilidad

- [ ] Contraste WCAG AA para texto normal (≥ 4.5:1) y para texto grande (≥ 3:1).
- [ ] Foco visible y navegación completa por teclado.
- [ ] Estructura y HTML semántico; encabezados jerárquicos.
- [ ] Imágenes con texto alternativo significativo; iconos con etiqueta si comunican solos.
- [ ] `prefers-reduced-motion` respetado cuando hay animación.
- [ ] No se depende solo del color para transmitir información.

## Responsive

- [ ] Recomposición real por viewport, no solo reducción de escala.
- [ ] Titulares, recortes de imagen y navegación revisados en móvil y tablet.
- [ ] Sin desbordamientos horizontales ni elementos cortados.
- [ ] Orden de lectura coherente al apilar columnas.

## Contenido

- [ ] No se copian frases, marcas, personas ni métricas de las referencias.
- [ ] Cifras y testimonios son proporcionados o comprobables; nada inventado.
- [ ] El texto de relleno está identificado como pendiente, no presentado como final.

## Verificación

- [ ] Si hubo herramientas de vista previa, se inspeccionó el resultado real.
- [ ] Se anotan dependencias, contenido pendiente y limitaciones conocidas.
- [ ] No se declara verificado lo que no se pudo inspeccionar.
