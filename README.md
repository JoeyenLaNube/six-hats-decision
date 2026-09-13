# six-hats-decision

Skill portable de [Agent Skills](https://agentskills.io) para tomar o auditar cualquier decisión con los **Seis Sombreros para Pensar** de Edward de Bono.

Sirve para decisiones vitales, de negocio, de producto o de programación. El método no garantiza un buen resultado; reduce puntos ciegos al separar hechos, emociones, valor, riesgos y alternativas.

English summary: a portable Agent Skill that runs a Six Thinking Hats decision session, with optional reversible/irreversible classification, WRAP checks, premortem and option widening. Copy the folder into any client that implements the Agent Skills standard.

## Qué hace

- Diseña una secuencia de sombreros según el tipo de decisión (rápida, estándar, crítica, auditoría o comparación).
- Obliga a etiquetar afirmaciones como hecho, inferencia o hipótesis.
- Incluye premortem en decisiones de alta apuesta.
- Puede auditar una propuesta y, si se pide, producir una candidata separada sin borrar el original.
- Cierra con un estado explícito (`SEGUIR`, `REFINAR`, `NO_SEGUIR`, `NECESITA_INFO`, `NO_EVALUADO`).
- Nunca autoriza publicar, firmar, desplegar ni gastar.

Marcos compañeros (no sustituyen a los sombreros):

- Puertas de un sentido / dos sentidos (Bezos)
- WRAP (Heath) recortado a cuatro preguntas
- Premortem (Klein)
- Cynefin ligero para elegir profundidad
- Matriz de opciones cuando hay tres o más caminos

## Instalación

Copia la carpeta `six-hats-decision/` a la ruta de skills de tu cliente:

| Cliente | Ruta habitual |
| --- | --- |
| Claude Code / Claude Desktop | `~/.claude/skills/six-hats-decision/` o `.claude/skills/six-hats-decision/` en el repo |
| Cursor | `.cursor/skills/six-hats-decision/` |
| Codex u otros agentes compatibles | la carpeta de skills que documente el cliente |
| Grok | skills de usuario persistentes |

No hay dependencias, APIs ni runtime. Solo Markdown.

## Uso

Invoca la skill de forma explícita:

- «Usa six-hats-decision para decidir si acepto esta oferta.»
- «Aplica los seis sombreros a este RFC.»
- «Audita este plan de negocio con sombrero negro y premortem.»
- «Compara estas tres arquitecturas con la skill de sombreros.»

## Contenido

```
six-hats-decision/
├── SKILL.md
├── LICENSE
├── README.md
├── references/
│   ├── hats.md
│   ├── sequences.md
│   ├── companion-frameworks.md
│   ├── domains.md
│   └── report-spec.md
└── assets/
    └── decision-report-template.md
```

## Método

El sombrero azul abre y cierra. El orden por defecto de una sesión estándar es:

Azul → Blanco → Rojo → Amarillo → Negro → Verde → Azul

Amarillo va antes que Negro para no cegar el valor. El azul puede cambiar la secuencia; ver `references/sequences.md`.

Six Thinking Hats es una marca y un método descritos por Edward de Bono. Esta skill es material original de procedimiento para agentes; no reproduce el libro.

## Licencia

MIT. Ver `LICENSE`.
