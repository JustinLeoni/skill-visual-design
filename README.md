# Skill: Visual Design

Skill para agentes de IA que diseñan, implementan y revisan interfaces digitales con dirección visual premium: jerarquía tipográfica, composición intencional, color y contraste, imagen cuidada, espacio y detalle.

Es una skill **agnóstica al agente**: no depende de un proveedor, modelo ni herramienta concreta. Funciona en cualquier agente que pueda leer una carpeta de skill (un `SKILL.md` de instrucciones) y mantener instrucciones persistentes. El núcleo es portable y está en español.

**Página web:** https://justinleoni.github.io/skill-visual-design/ (fuente en [`docs/`](docs/)). La versión 1 de la web está archivada en [`docs/v1/`](docs/v1/) → https://justinleoni.github.io/skill-visual-design/v1/

Cubre distintos tipos de diseño, no un estilo único:

- **Web y marketing:** landing pages, sitios corporativos, portafolios, páginas de producto.
- **Producto y datos:** dashboards, paneles de administración, interfaces de cuenta, herramientas.
- **Móvil:** apps iOS, Android o multiplataforma.
- **Contenido y presentación:** publicaciones, revisiones, diapositivas, material editorial.

## Qué hace

- Convierte un brief y capturas de referencia en decisiones de composición y un sistema visual coherente.
- Orienta la creación y el rediseño de cualquier interfaz, del primer viewport a la entrega.
- Guía tipografía, grillas, color, fotografía, ritmo, componentes, responsive y movimiento.
- Ofrece direcciones visuales reutilizables (editorial, inmersiva, modular de producto, contenido, técnica, expresiva).
- Aplica **siempre** un sistema visual neutro: solo blanco, gris y negro; tipografía sans minimalista; sin logotipo inventado.

## Sistema visual por defecto

La skill aplica este sistema por defecto, salvo que el usuario pida otra cosa:

- **Color:** solo **blanco, gris y negro**, en neutros puros y sin tinte. Sin colores de acento ni fondos crema, beige o tintados.
- **Tipografía:** sans **normal y minimalista** (Inter, system-ui, Helvetica, Arial). Sin serif, sin cursivas y sin display decorativos.
- **Marca:** si el proyecto no tiene logotipo, no se inventa uno.
- **Imagen:** sin placeholders genéricos ni imágenes remotas arbitrarias; tipografía, espacio y datos.
- Incluye criterios de accesibilidad y comportamiento funcional para que el resultado no se quede en una maqueta.
- Evita copiar contenido de las referencias, inventar cifras o testimonios y repetir patrones que no correspondan al proyecto.

## Cómo funciona

El agente carga `SKILL.md` cuando el trabajo es de diseño o implementación de interfaces, o cuando se invoca directamente. Primero entiende el proyecto y las referencias; luego elige una dirección visual, define reglas reutilizables y construye la interfaz adaptada al contenido y a distintos tamaños de pantalla. Finalmente revisa legibilidad, accesibilidad, interacción y acabado en la vista disponible.

Material de apoyo en `references/`:

- `references/direcciones-visuales.md` — arquetipos de dirección y cuándo aplicarlos.
- `references/checklist-entrega.md` — revisión de jerarquía, sistema, comportamiento, accesibilidad, responsive y contenido.

## Estructura

```text
visual-design/
├── SKILL.md                              # Instrucciones (agnósticas al agente)
├── metadata.json                         # Versión, resumen y referencias
└── references/
    ├── direcciones-visuales.md           # Direcciones visuales
    └── checklist-entrega.md              # Checklist de entrega
```

El núcleo es `SKILL.md` (frontmatter `name` y `description` + instrucciones). `metadata.json` y `references/` son apoyo: no son obligatorios para que el agente cargue la skill, pero enriquecen su uso.

## Instalación mediante un prompt (recomendado)

Copia el bloque siguiente y envíaselo al agente: el propio prompt indica al agente que acceda al repositorio, lo descargue y lo instale, sin que el usuario tenga que preparar archivos. El agente debe descubrir en su entorno el directorio de skills y el archivo de instrucciones persistentes que realmente lee.

```text
Instala y configura en este entorno la skill `visual-design`, que vive en este repositorio público de GitHub:
https://github.com/JustinLeoni/skill-visual-design

1. Accede al repositorio y descárgalo por tu cuenta: usa `git clone` a un directorio temporal (por ejemplo https://github.com/JustinLeoni/skill-visual-design.git). Si no tienes git o acceso a la red, descarga el zip del release más reciente (https://github.com/JustinLeoni/skill-visual-design/releases/latest) y descomprímelo. Si tampoco puedes acceder a la red, pide al usuario el enlace o los archivos.
2. Dentro de lo descargado, localiza la carpeta `visual-design/` (contiene SKILL.md, metadata.json y references/). Léela entera para entender la skill.
3. Copia esa carpeta completa al directorio persistente de skills que este agente carga realmente. Detecta la ruta correcta en lugar de asumirla; comprueba las convenciones documentadas de tu entorno (por ejemplo, un directorio de skills bajo el home del agente o una variable de entorno que lo defina). Si no puedes determinar la ruta con certeza, pregunta antes de escribir.
4. Verifica que la copia contiene SKILL.md y la carpeta references/.
5. Para que la skill se considere automáticamente en trabajos futuros de diseño, añade una regla breve al archivo de instrucciones persistentes globales que este agente realmente lea (por ejemplo un AGENTS.md global u otro archivo equivalente de su entorno): "Para diseñar, implementar o revisar interfaces, consulta y aplica la skill visual-design antes de decidir la dirección visual; adapta sus principios al brief, a la marca y a las referencias del proyecto."
6. No reemplaces instrucciones existentes: añade la regla sin borrar contenido.
7. Elimina el clon o la descarga temporal cuando termines; no dejes archivos sueltos.
8. Al terminar, indica exactamente qué rutas usaste (carpeta de la skill y archivo de instrucciones) y cómo se activará la skill en futuras sesiones de este entorno.

No afirmes que la regla aplica a otros agentes, cuentas o dispositivos fuera de este entorno.
```

La ruta exacta varía entre herramientas y proveedores. La instalación de la carpeta hace disponible la skill; la instrucción persistente hace que el agente la considere automáticamente en tareas relevantes cuando su plataforma admite esa configuración.

### Prompt corto (alternativa)

Si prefieres una sola línea, este prompt también funciona:

```text
Descarga el repositorio https://github.com/JustinLeoni/skill-visual-design, instala su carpeta `visual-design` en el directorio de skills persistente que cargas realmente (detéctalo; si no lo conoces, pregunta), añade a tus instrucciones persistentes globales la regla "para diseñar, implementar o revisar interfaces, consulta y aplica la skill visual-design antes de decidir la dirección visual", y dime las rutas que usaste.
```

## Instalación manual (cualquier agente)

1. Descarga el repositorio (o el zip del release más reciente) y copia la carpeta `visual-design/` al directorio de skills persistente que use tu agente. No hay una ruta universal: usa la que documente tu herramienta o la que el propio agente detecte en su entorno.
2. Para activar su consideración automática, añade la regla breve (la del prompt de instalación) al archivo de instrucciones persistentes globales que tu agente lea —por ejemplo un `AGENTS.md` global u otro archivo equivalente—, conservando las instrucciones existentes.
3. Inicia una tarea de diseño o invoca la skill directamente con su nombre para que se cargue.

Las instrucciones persistentes ayudan al agente a recordar la skill en ese entorno. Ninguna skill o prompt puede garantizar que todos los agentes, proveedores o futuras sesiones la obedezcan universalmente.

## Releases

Cada release incluye la skill empaquetada y lista para instalar:

- `visual-design-vX.Y.Z.zip` — carpeta completa (`SKILL.md`, `metadata.json`, `references/`) para descomprimir en el directorio de skills del agente.

La versión también consta en `visual-design/metadata.json`.

## Compatibilidad

- **Núcleo:** `SKILL.md` con frontmatter (`name`, `description`). Es el formato común de skills para agentes.
- **Apoyo:** `metadata.json` y `references/`, opcionales pero útiles.
- **Sin dependencias:** la skill es texto plano. No depende de metadatos de ningún proveedor.

## Licencia

Este repositorio se publica bajo la licencia MIT. Consulta [LICENSE](LICENSE).
