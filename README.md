# Diseño Editorial Premium

Skill para agentes de IA que diseñan e implementan páginas web e interfaces con una dirección editorial premium: tipografía con carácter, composición intencional, fotografía cuidada, espacio, contraste y detalles precisos.

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

## Instalación mediante un prompt

Descarga o clona este repositorio y envía el siguiente prompt al agente que tenga acceso a esos archivos:

```text
Instala y configura en este entorno la skill `diseno-editorial-premium` desde la carpeta `diseno-editorial-premium` de este repositorio. Lee sus instrucciones, copia la carpeta completa de la skill al directorio persistente de skills de este agente (para Codex: `$CODEX_HOME/skills`, o `~/.codex/skills` si CODEX_HOME no está definido). Comprueba que contiene SKILL.md y agents/openai.yaml. Para que se use automáticamente en trabajos futuros de diseño, añade a las instrucciones persistentes apropiadas de este entorno una regla breve que indique: “Para diseñar o implementar interfaces, consulta y aplica la skill diseno-editorial-premium antes de decidir la dirección visual; adapta sus principios al brief, a la marca y a las referencias del proyecto”. Si el entorno usa AGENTS.md, coloca la regla en el AGENTS.md global del usuario cuando exista y sea editable; si no, usa el archivo global de instrucciones que realmente lea ese agente. No reemplaces instrucciones existentes: añade la regla sin borrar contenido, verifica la ruta y explica qué archivo controla la activación futura. No afirmes que la regla aplica a otros agentes, cuentas o dispositivos fuera de este entorno.
```

El prompt pide instalar la skill y añadir una instrucción persistente a la configuración que el agente realmente carga. La ruta exacta varía entre herramientas. La instalación de la carpeta hace disponible la skill; la instrucción persistente hace que el agente la considere automáticamente en tareas relevantes cuando su plataforma admite esa configuración.

## Instalación manual en Codex

1. Copia la carpeta `diseno-editorial-premium/` en `~/.codex/skills/` (o en `$CODEX_HOME/skills/` si esa variable está configurada).
2. Para activar su consideración automática, añade la regla breve del prompt de instalación a `~/.codex/AGENTS.md`, conservando las instrucciones existentes. Si tu entorno documenta otro archivo global persistente, usa el que aplique a tu instalación.
3. Inicia una tarea de diseño o menciona `$diseno-editorial-premium` para invocarla directamente.

Las instrucciones persistentes ayudan al agente a recordar la skill en ese entorno. Ninguna skill o prompt puede garantizar que todos los agentes, proveedores o futuras sesiones la obedezcan universalmente.

## Estructura

```text
diseno-editorial-premium/
├── SKILL.md
└── agents/
    └── openai.yaml
```

## Licencia

Este repositorio se publica bajo la licencia MIT. Consulta [LICENSE](LICENSE).
