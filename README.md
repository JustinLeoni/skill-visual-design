# Estudio Editorial

Skill para agentes de IA que diseñan e implementan páginas web e interfaces con una dirección editorial premium: tipografía con carácter, composición intencional, fotografía cuidada, espacio, contraste y detalles precisos.

Es una skill **agnóstica al agente**: no depende de un proveedor, modelo ni herramienta concreta. Funciona en cualquier agente que pueda leer una carpeta de skill (un `SKILL.md` de instrucciones) y mantener instrucciones persistentes.

La skill toma como inspiración un conjunto de referencias de portafolios creativos, arquitectura, inmobiliaria, turismo, producto digital y sitios corporativos. No impone una plantilla única. Enseña al agente a identificar el lenguaje de cada referencia y adaptarlo a la marca, contenido, función y dispositivo del proyecto.

## Qué hace

- Convierte un brief y capturas de referencia en decisiones de composición y un sistema visual coherente.
- Orienta la creación y el rediseño de landing pages, sitios, portafolios, páginas de producto e interfaces.
- Guía tipografía, grillas, color, fotografía, ritmo, componentes, responsive y movimiento.
- Incluye criterios de accesibilidad y comportamiento funcional para que el resultado no se quede en una maqueta.
- Evita copiar contenido de las referencias, inventar cifras o testimonios y repetir patrones que no correspondan al proyecto.

## Cómo funciona

El agente carga `SKILL.md` cuando el trabajo es de diseño o implementación de interfaces, o cuando se invoca directamente. Primero entiende el proyecto y las referencias; luego selecciona una dirección visual, define reglas reutilizables y construye la interfaz adaptada al contenido y a distintos tamaños de pantalla. Finalmente revisa legibilidad, accesibilidad, interacción y acabado en la vista disponible.

La selección de dirección puede ser tipográfica, inmersiva con fotografía, modular de producto o editorial de contenido. Son rutas orientativas: el agente debe conservar una identidad común y elegir según el contexto.

## Estructura

```text
estudio-editorial/
├── SKILL.md            # Instrucciones de la skill (agnósticas al agente)
└── agents/
    └── openai.yaml     # Metadatos opcionales del formato agents/*.yaml
```

El núcleo de la skill es `SKILL.md`. El archivo `agents/openai.yaml` es un metadato opcional para plataformas que lo reconozcan; si el agente no lo usa, puede ignorarse sin afectar la skill.

## Instalación mediante un prompt (recomendado)

Clona o descarga este repositorio y envía el siguiente prompt al agente que tenga acceso a esos archivos. El prompt es genérico: el agente debe descubrir en su propio entorno cuál es el directorio de skills y el archivo de instrucciones persistentes que realmente lee.

```text
Instala y configura en este entorno la skill `estudio-editorial` desde la carpeta `estudio-editorial` de este repositorio.

1. Lee SKILL.md y la estructura de la skill.
2. Copia la carpeta completa de la skill al directorio persistente de skills que este agente carga realmente. Detecta la ruta correcta en lugar de asumirla; comprueba las convenciones documentadas del entorno (por ejemplo, un directorio de skills bajo el home del agente o una variable de entorno que lo defina). Si no puedes determinar la ruta con certeza, pregunta antes de escribir.
3. Verifica que la copia contiene SKILL.md y la carpeta agents/.
4. Para que la skill se considere automáticamente en trabajos futuros de diseño, añade una regla breve al archivo de instrucciones persistentes globales que este agente realmente lea (por ejemplo un AGENTS.md global u otro archivo equivalente de su entorno): "Para diseñar o implementar interfaces, consulta y aplica la skill estudio-editorial antes de decidir la dirección visual; adapta sus principios al brief, a la marca y a las referencias del proyecto."
5. No reemplaces instrucciones existentes: añade la regla sin borrar contenido.
6. Al terminar, indica exactamente qué rutas usaste (carpeta de la skill y archivo de instrucciones) y cómo se activará la skill en futuras sesiones de este entorno.

No afirmes que la regla aplica a otros agentes, cuentas o dispositivos fuera de este entorno.
```

El prompt pide instalar la skill y añadir una instrucción persistente a la configuración que el agente realmente carga. La ruta exacta varía entre herramientas y proveedores. La instalación de la carpeta hace disponible la skill; la instrucción persistente hace que el agente la considere automáticamente en tareas relevantes cuando su plataforma admite esa configuración.

## Instalación manual (cualquier agente)

1. Copia la carpeta `estudio-editorial/` al directorio de skills persistente que use tu agente. No hay una ruta universal: usa la que documente tu herramienta o la que el propio agente detecte en su entorno.
2. Para activar su consideración automática, añade la regla breve (la del prompt de instalación) al archivo de instrucciones persistentes globales que tu agente lea —por ejemplo un `AGENTS.md` global u otro archivo equivalente—, conservando las instrucciones existentes.
3. Inicia una tarea de diseño o invoca la skill directamente con su nombre para que se cargue.

Las instrucciones persistentes ayudan al agente a recordar la skill en ese entorno. Ninguna skill o prompt puede garantizar que todos los agentes, proveedores o futuras sesiones la obedezcan universalmente.

## Compatibilidad

- **Núcleo:** `SKILL.md` con frontmatter (`name`, `description`). Es el formato común de skills para agentes.
- **Metadatos opcionales:** `agents/openai.yaml`, para plataformas que reconozcan ese formato. Opcional.

La skill es texto plano y portable: puede usarse tal cual en cualquier agente que lea instrucciones en Markdown.

## Licencia

Este repositorio se publica bajo la licencia MIT. Consulta [LICENSE](LICENSE).
