---
name: visual-design
description: Diseña y desarrolla interfaces digitales —páginas web, landing pages, dashboards, aplicaciones, portafolios y presentaciones— con dirección visual premium: jerarquía tipográfica, composición intencional, color y contraste, imagen cuidada y detalle. Actívalo al crear, rediseñar o revisar cualquier interfaz o sistema visual; adapta el sistema al brief, la marca, el contenido y el dispositivo.
metadata:
  short-description: Dirección visual premium para cualquier interfaz
---

# Diseño visual

Convierte el brief y las referencias visuales en una interfaz distintiva, legible y funcional. El lenguaje es universal: jerarquía clara, composición intencional, imágenes con carácter, detalles precisos y ritmo entre contenido y espacio. No conviertas las capturas en una plantilla rígida; identifica qué hace especial a cada referencia y elige la dirección adecuada para el proyecto.

## Cuándo usarla

Úsala para diseñar, implementar, rediseñar o revisar interfaces y sistemas visuales, con independencia del tipo de producto:

- **Web y marketing:** landing pages, sitios corporativos, portafolios, páginas de producto.
- **Producto y datos:** dashboards, paneles de administración, interfaces de cuenta, herramientas.
- **Móvil:** apps iOS, Android o multiplataforma.
- **Contenido y presentación:** publicaciones, revisiones, diapositivas, material editorial.

Tiene prioridad cuando el usuario adjunta referencias de diseño o pide una estética concreta (editorial, minimalista, premium, de estudio creativo, técnica, brutalista, cinematográfica…). Si el usuario da un sistema visual propio, conserva su identidad y aplica estos principios solo donde encajen.

## Sistema visual por defecto

Este es el estándar de la skill y se aplica **siempre**, salvo que el usuario pida explícitamente lo contrario o exista un sistema de marca que lo sustituya.

- **Color:** solo **blanco, gris y negro**, en neutros puros y sin tinte. Sin colores de acento y sin tonos crema, beige o cálidos.
- **Todo plano:** sin sombras, sin bordes y sin líneas (ni separadores, ni rejillas dibujadas, ni subrayados decorativos). Las secciones y bloques se distinguen **solo por el tono** del fondo: blanco, gris o negro.
- **Jerarquía por peso y tono:** usa una sola familia sans. Para titulares y textos grandes sube el **peso** a **bold o heavy** (700–900) con tracking negativo. La diferencia entre un titular y su continuación se logra con **peso y tono de gris**, no con otra familia ni con color.
- **Tipografía:** familias **sans normales y minimalistas** (Inter, system-ui, Helvetica, Arial). Sin serif, sin cursivas y sin display decorativos.
- **Marca:** si no existe un logotipo, **no inventes uno**; deja el espacio sin logo y usa el nombre en texto si hace falta identidad.
- **Imagen:** si no hay imágenes reales, no uses placeholders genéricos ni imágenes remotas arbitrarias; trabaja con tipografía, espacio y datos.

Solo si el usuario pide color, serif o una estética concreta aplicas esa dirección (ver *Direcciones visuales*); fuera de ese caso, mantén siempre este sistema neutro y minimalista.

## Principios

1. **Diseña desde la intención.** Antes de maquetar, identifica audiencia, acción principal, contenido imprescindible, personalidad de marca, restricciones técnicas y dispositivo objetivo. No inventes requisitos ni copies texto de las imágenes de referencia.
2. **Lee las referencias visualmente.** Separa lo estructural de lo accidental: jerarquía, composición, escala, ritmo, densidad, tratamiento de imagen, contraste y microdetalles. Si varias imágenes muestran estilos diferentes, sintetiza rasgos compatibles y selecciona un sistema coherente según el encargo.
3. **Haz que la tipografía dirija.** Usa titulares expresivos con tamaño, **peso** (bold/heavy) y saltos de línea controlados. Escala y peso antes que familias: por defecto una sola sans neutra, y reserva segundas familias o serif para cuando la marca lo pida.
4. **Compón con tensión y aire.** Combina grillas alineadas con asimetría medida, espacios negativos, elementos fuera del eje y escalas contrastantes. El espacio vacío debe crear jerarquía; no se rellena por defecto.
5. **Usa imagen con propósito.** Favorece fotografía, ilustración o gráficos que respondan al proyecto. Elige proporciones y recortes intencionales, calidad alta y consistencia tonal. No uses placeholders genéricos ni una imagen remota arbitraria como si fuera contenido real.
6. **Controla el color.** Por defecto, **solo blanco, gris y negro** (ver *Sistema visual por defecto*). Añade color únicamente si el usuario lo pide o una marca lo exige, y entonces define un sistema (superficie, texto, acento, estados); no impongas el mismo acento a todos los proyectos.
7. **Cada bloque tiene una función.** Incluye navegación, hero, contenido, prueba y cierre según las necesidades reales. Una vista no necesita métricas, testimonios, FAQ o categorías si el brief no las respalda.
8. **Diseña componentes como familia.** Botones, etiquetas, tarjetas, tablas, controles, formularios, radios, bordes y estados deben compartir reglas visuales. Evita componentes que parezcan extraídos de una plantilla.
9. **El movimiento acompaña.** Usa transiciones breves y estados hover/focus claros. Añade animación, scroll effects o interacción solo cuando mejoren la comprensión o el carácter; respeta `prefers-reduced-motion`.
10. **La estética no desplaza la calidad.** Mantén contraste WCAG AA para texto normal, foco visible, navegación por teclado, HTML/estructura semántica, etiquetas de formulario y diseño responsive. No sacrifiques legibilidad por texto microscópico o gris de bajo contraste.

## Flujo de trabajo

1. **Inspecciona el contexto disponible.** Revisa el proyecto existente, instrucciones locales, framework, componentes, assets y comportamiento actual antes de cambiar archivos. Conserva convenciones útiles.
2. **Elige la dirección visual.** Selecciona una dirección principal (o mezcla dos con moderación) según el producto y el brief. Consulta `references/direcciones-visuales.md` para los arquetipos y cuándo aplicarlos.
3. **Resume la intención visual.** Anota en breve los rasgos de referencia que sí aplicarás y lo que debe seguir siendo propio del proyecto. Si no hay referencia explícita, define una dirección a partir del brief.
4. **Establece el sistema mínimo.** Define tokens de color, tipografía, anchos, grilla, escala de espacio, radios, bordes, tratamiento de imagen y comportamiento responsive. Usa variables CSS o el mecanismo nativo del proyecto cuando sea razonable.
5. **Diseña la composición completa.** Trabaja desde el primer viewport o pantalla hasta el cierre, dando a cada sección un propósito y cambiando el ritmo sin perder coherencia.
6. **Construye estados reales.** Los enlaces navegan, los botones actúan, los formularios validan y los controles cambian estado. No dibujes affordances sin comportamiento. Incluye estados vacíos, de carga y de error en producto y datos.
7. **Ajusta por viewport.** Recompón la grilla para móvil y, si aplica, para tablet y escritorio; no te limites a encoger una versión. Revisa titulares, recortes, navegación, orden de lectura, controles táctiles y desbordamientos.
8. **Revisa el acabado en contexto.** Si hay herramientas de vista previa, inspecciona el resultado real. Corrige desajustes de jerarquía, espaciado, contraste, recorte, alineación y responsive antes de entregar.

## Direcciones visuales

Elige una dirección principal o mezcla dos con moderación:

- **Editorial tipográfica:** fondos claros, enorme escala de titulares, composición descentrada, imágenes pequeñas o ausencia de imagen, microtipografía y mucho espacio. Portafolios, estudios, presentaciones.
- **Inmersiva cinematográfica:** fotografía o video a gran escala, overlays discretos, navegación contenida y tipografía amplia. Arquitectura, hospitalidad, bienes raíces, marcas visuales.
- **Modular de producto:** superficies limpias, grilla y módulos definidos, controles precisos y jerarquía funcional. SaaS, páginas de servicio, catálogos, interfaces de cuenta.
- **Editorial de contenido:** tipografía legible, columnas, fotografías con pies, datos y navegación de lectura. Revistas, noticias, recursos, publicaciones.
- **Técnica / utilitaria:** densidad alta, datos precisos, tablas y estados claros, tipografía monoespaciada para valores. Dashboards, herramientas, paneles de administración.
- **Expresiva / brutalista:** contraste extremo, tipografía a gran escala, color plano, bordes duros o retícula visible. Declaraciones de marca, campañas, sitios de autor.

Estas direcciones no son plantillas: ajusta densidad, interacción, color e imagen al contenido, la marca y el dispositivo. Detalle y criterios de elección en `references/direcciones-visuales.md`. Salvo que el usuario pida una dirección concreta, mantén el **Sistema visual por defecto** (blanco, gris y negro; sans minimalista; sin logo inventado). No mezcles una home inmobiliaria con un portfolio tipográfico sin una razón clara de marca.

## Parámetros de referencia

Son rangos de partida, no mandatos. Prioriza el viewport y el contenido reales.

- Ancho de lectura/contenido en escritorio: aproximadamente 1120–1440 px; márgenes fluidos y consistentes.
- Titular hero: `clamp(3.5rem, 9vw, 9rem)` según la dirección, con interlineado apretado y tracking negativo moderado.
- Cuerpo: alrededor de 16–18 px con interlineado cómodo; metadatos compactos sin volverlos ilegibles.
- Espacio entre secciones: alrededor de 80–160 px en escritorio, más compacto y contextual en móvil.
- Grillas: 12 columnas para composición amplia, 2–4 para colecciones; solapes o columnas vacías solo si refuerzan la jerarquía.
- Bordes y radios: finos o suaves cuando ayuden a agrupar; no conviertas cada sección en una tarjeta redondeada.
- Sombras: casi imperceptibles y reservadas para capas que deban separarse del fondo.

## Decisiones por componente

- **Navegación:** pocos enlaces, identidad visible y CTA solo si tiene prioridad real. Menú móvil funcional y accesible.
- **Hero / cabecera:** una promesa o idea principal, texto breve, acción clara cuando aplique e imagen con encuadre deliberado. Puede ser tipográfico, fotográfico, modular o de pantalla completa.
- **Tarjetas:** contenido y acción con jerarquía clara; etiqueta y metadatos solo si ayudan a comparar o entender.
- **Tablas y datos:** alineación numérica consistente, énfasis en lo relevante, densidad legible y estados vacíos/neutros definidos.
- **Datos y prueba social:** usa cifras o testimonios proporcionados o comprobables. No inventes clientes, métricas ni reseñas.
- **Formularios:** etiquetas persistentes, errores comprensibles, foco visible y confirmación de envío. Evita depender solo del placeholder.
- **Footer:** enlaces útiles, contacto y detalles legales disponibles; puede ser oscuro, claro, tipográfico o compacto según el ritmo del diseño.

## Límites visuales

- Evita gradientes neón o morados por defecto, efectos de vidrio, sombras voluminosas, exceso de iconos, emojis decorativos y estética genérica de plantilla.
- Evita hacer de cada sección una tarjeta, centrar todo, repetir el mismo patrón de título + párrafo + botón y usar un mosaico cuando las imágenes no son el contenido principal.
- Evita mayúsculas enormes para párrafos, etiquetas diminutas, titulares ilegibles, contraste pobre, animación sin propósito y estados inactivos que parecen clicables.
- No inventes logotipos, isotipos ni marcas si el proyecto no tiene uno; deja el espacio sin logo.
- No uses fondos ni paletas cálidas o tintadas (crema, beige, arena, marfil): el fondo es blanco o gris neutro.
- No dibujes separadores ni rejillas con líneas finas (bordes de 1px); separa con espacio y, para agrupar, usa una superficie de fondo.
- No uses sombras, bordes ni subrayados decorativos: **todo plano**. El tono del fondo (blanco / gris / negro) es el único separador.
- No uses serif, cursivas, display decorativos ni color de acento cuando el brief no lo pide (ver *Sistema visual por defecto*).
- No uses frases, marcas, personas, métricas o contenido de las capturas como si pertenecieran al proyecto.

## Revisión antes de entregar

- ¿La dirección responde al brief y es reconocible como una decisión, no como una plantilla?
- ¿El primer viewport comunica qué es el producto y qué hacer después?
- ¿La escala, el espacio y la imagen crean jerarquía y un ritmo visual sostenido?
- ¿Las secciones incluidas tienen contenido y propósito reales?
- ¿Tipografía, color, superficies, bordes y controles se sienten parte del mismo sistema?
- ¿Funciona en móvil, teclado y movimiento reducido, y conserva legibilidad y contraste?
- ¿Los controles tienen comportamiento real y el resultado se revisó en el entorno disponible?

Checklist completa de accesibilidad y acabado en `references/checklist-entrega.md`.

## Entrega

Explica en pocas líneas la dirección que elegiste, las partes principales implementadas y cualquier dependencia concreta, contenido pendiente o limitación que impida considerar la interfaz terminada. No declares verificado lo que no pudiste inspeccionar.
