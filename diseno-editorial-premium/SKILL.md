---
name: diseno-editorial-premium
description: Diseña y desarrolla interfaces web, landing pages, sitios, portafolios y productos digitales con dirección editorial premium basada en composición tipográfica, fotografía cuidada, asimetría, espacio y contraste. Actívalo al crear o rediseñar una interfaz, especialmente si el usuario comparte referencias de este lenguaje visual; adapta el sistema a la marca y al propósito.
metadata:
  short-description: Diseño editorial web premium y adaptable
---

# Diseño editorial premium

Convierte el brief y las referencias visuales en una interfaz web distintiva, legible y funcional. El lenguaje compartido es editorial: jerarquía tipográfica clara, composición intencional, imágenes con carácter, detalles precisos y ritmo entre contenido y espacio. No conviertas las capturas en una plantilla rígida; identifica qué hace especial a cada referencia y elige la dirección adecuada para el producto.

## Cuándo usarla

Úsala para diseñar, implementar o rediseñar interfaces digitales. Tiene prioridad cuando el usuario adjunta referencias de diseño o pide una estética editorial, minimalista, premium, de estudio creativo, arquitectura, producto o marca. Si el usuario da un sistema visual propio, conserva su identidad y aplica estos principios solo donde encajen.

## Principios

1. **Diseña desde la intención.** Antes de maquetar, identifica audiencia, acción principal, contenido imprescindible, personalidad de marca, restricciones técnicas y viewport objetivo. No inventes requisitos ni copies texto de las imágenes de referencia.
2. **Lee las referencias visualmente.** Separa lo estructural de lo accidental: jerarquía, composición, escala, ritmo, densidad, tratamiento de imagen, contraste y microdetalles. Si varias imágenes muestran estilos diferentes, sintetiza rasgos compatibles y selecciona un sistema coherente según el encargo.
3. **Haz que la tipografía dirija.** Usa titulares expresivos con tamaño, anchura, interlineado y saltos de línea controlados; combina una sans contemporánea con una monoespaciada discreta para etiquetas y datos cuando aporte intención. No fuerces texto gris bicolor en todas las secciones.
4. **Compón con tensión y aire.** Combina grillas alineadas con asimetría medida, espacios negativos, elementos fuera del eje y escalas contrastantes. El espacio vacío debe crear jerarquía; no se rellena por defecto.
5. **Usa imagen con propósito.** Favorece fotografía de arquitectura, interiores, naturaleza, producto, personas o procesos que responda al proyecto. Elige proporciones y recortes intencionales, calidad alta y consistencia tonal. No uses placeholders genéricos ni una imagen remota arbitraria como si fuera contenido real.
6. **Controla el color.** Parte de una base neutral clara u oscura. Añade color solo si la marca, el contenido o la imagen lo justifican. Acentos sobrios, bloques invertidos y superficies tonales pueden convivir; no impongas el mismo acento rojo a todos los proyectos.
7. **Cada bloque tiene una función.** Mantén navegación, hero, contenido, pruebas, trabajo destacado y cierre según las necesidades reales. Una página no necesita incluir métricas, testimonios, FAQ o categorías si el brief no las respalda.
8. **Diseña componentes como familia.** Botones, etiquetas, tarjetas, controles, formularios, radios, bordes y estados deben compartir reglas visuales. Evita componentes repetidos que parezcan extraídos de una plantilla.
9. **El movimiento acompaña.** Usa transiciones breves y estados hover/focus claros. Añade animación, scroll effects o interacción solo cuando mejoren la comprensión o el carácter; respeta `prefers-reduced-motion`.
10. **La estética no desplaza la calidad.** Mantén contraste WCAG AA para texto normal, foco visible, navegación por teclado, HTML semántico, etiquetas de formulario y diseño responsive. No sacrifiques legibilidad por texto microscópico o gris de bajo contraste.

## Selección de dirección visual

Elige una dirección principal o mezcla dos con moderación:

- **Editorial tipográfica:** fondos claros, enorme escala de titulares, composición descentrada, imágenes pequeñas o ausencia de imagen, microtipografía y mucho espacio. Adecuada para portafolios, estudios y presentaciones.
- **Inmersiva cinematográfica:** fotografía o video a gran escala, overlays discretos, navegación contenida y tipografía amplia. Adecuada para arquitectura, hospitalidad, bienes raíces y marcas visuales.
- **Modular de producto:** superficies limpias, grilla y módulos definidos, controles precisos y jerarquía funcional. Adecuada para SaaS, páginas de servicio, catálogos e interfaces de cuenta.
- **Editorial de contenido:** tipografía legible, columnas, fotografías con pies, datos y navegación de lectura. Adecuada para revistas, noticias, recursos y publicaciones.

Estas direcciones no son plantillas: ajusta densidad, interacción, color e imagen al contenido, la marca y el dispositivo. No mezcles una home inmobiliaria con un portfolio tipográfico sin una razón clara de marca.

## Flujo de trabajo

1. **Inspecciona el contexto disponible.** Revisa el proyecto existente, instrucciones locales, framework, componentes, assets y comportamiento actual antes de cambiar archivos. Conserva convenciones útiles.
2. **Resume la intención visual.** Anota en breve los rasgos de referencia que sí aplicarás y lo que debe seguir siendo propio del proyecto. Si no hay referencia explícita, define una dirección a partir del brief.
3. **Establece el sistema mínimo.** Define tokens de color, tipografía, anchos, grilla, escala de espacio, radios, bordes, tratamiento de imagen y comportamiento responsive. Usa variables CSS o el mecanismo nativo del proyecto cuando sea razonable.
4. **Diseña la composición completa.** Trabaja desde el primer viewport hasta el cierre, dando a cada sección un propósito y cambiando el ritmo sin perder coherencia.
5. **Construye estados reales.** Los enlaces navegan, los botones actúan, los formularios validan y los controles cambian estado. No dibujes affordances sin comportamiento.
6. **Ajusta por viewport.** Recompón la grilla para móvil; no te limites a encoger escritorio. Revisa titulares, recortes, navegación, orden de lectura, controles táctiles y desbordamientos.
7. **Revisa el acabado en contexto.** Si hay herramientas de vista previa, inspecciona el resultado real. Corrige desajustes de jerarquía, espaciado, contraste, recorte, alineación y responsive antes de entregar.

## Parámetros de referencia

Son rangos de partida, no mandatos. Prioriza el viewport y el contenido reales.

- Ancho de lectura/contenido en desktop: aproximadamente 1120–1440 px; márgenes fluidos y consistentes.
- Titular hero en desktop: `clamp(3.5rem, 9vw, 9rem)` según la dirección, con interlineado apretado y tracking negativo moderado.
- Cuerpo: alrededor de 16–18 px con interlineado cómodo; metadatos compactos sin reducirlos hasta volverlos ilegibles.
- Espacio entre secciones: alrededor de 80–160 px en desktop, más compacto y contextual en móvil.
- Grillas: 12 columnas para composición amplia, 2–4 para colecciones; permitir solapes o columnas vacías solo si refuerzan la jerarquía.
- Bordes y radios: finos o suaves cuando ayuden a agrupar; no conviertas cada sección en una tarjeta redondeada.
- Sombras: casi imperceptibles y reservadas para capas que deban separarse del fondo.

## Decisiones por componente

- **Navegación:** pocos enlaces, identidad visible y CTA solo si tiene prioridad real. Usa menú móvil funcional y accesible.
- **Hero:** una promesa o idea principal, texto breve, acción clara cuando aplique e imagen con encuadre deliberado. Puede ser tipográfico, fotográfico, modular o de pantalla completa.
- **Tarjetas:** contenido y acción con jerarquía clara; etiqueta y metadatos solo si ayudan a comparar o entender.
- **Datos y prueba social:** usa cifras o testimonios proporcionados o comprobables. No inventes clientes, métricas ni reseñas.
- **Formularios:** etiquetas persistentes, errores comprensibles, foco visible y confirmación de envío. Evita depender solo del placeholder.
- **Footer:** enlaces útiles, contacto y detalles legales disponibles; puede ser oscuro, claro, tipográfico o compacto según el ritmo del diseño.

## Límites visuales

- Evita gradientes neón o morados por defecto, efectos de vidrio, sombras voluminosas, exceso de iconos, emojis decorativos y estética genérica de dashboard.
- Evita hacer toda sección una tarjeta, centrar todo, repetir el mismo patrón de título + párrafo + botón, y usar un mosaico cuando las imágenes no son el contenido principal.
- Evita mayúsculas enormes para párrafos, etiquetas diminutas, titulares ilegibles, contraste pobre, animación sin propósito y estados inactivos que parecen clicables.
- No uses frases, marcas, personas, métricas o contenido de las capturas como si pertenecieran al proyecto.

## Revisión antes de entregar

- ¿La dirección responde al brief y es reconocible como una decisión, no como una plantilla?
- ¿El primer viewport comunica qué es el producto y qué hacer después?
- ¿La escala, el espacio y la imagen crean jerarquía y un ritmo visual sostenido?
- ¿Las secciones incluidas tienen contenido y propósito reales?
- ¿Tipografía, color, superficies, bordes y controles se sienten parte del mismo sistema?
- ¿Funciona en móvil, teclado y movimiento reducido, y conserva legibilidad y contraste?
- ¿Los controles tienen comportamiento real y el resultado se revisó en el entorno disponible?

## Entrega

Explica en pocas líneas la dirección que elegiste, las partes principales implementadas y cualquier dependencia concreta, contenido pendiente o limitación que impida considerar la interfaz terminada. No declares verificado lo que no pudiste inspeccionar.
