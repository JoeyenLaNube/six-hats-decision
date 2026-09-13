# Plan de creación — `six-hats-decision` v1.0

Fecha: 2026-09-13
Estado: skill validada localmente; publicada en GitHub.

## 1. Qué se retoma del plan Astra y qué se descarta

El plan original (`six-hats-verifier`) era un **verificador de gobierno interno** para Campañas Europa 2026 / PHG: contratos JSON, CLI Node, hashes SHA-256, revisor independiente como agente distinto, códigos de salida, piloto de 32 invocaciones y prohibición de publicar.

Eso es valioso dentro de una fábrica concreta. **No es portable** a cualquier cliente y modelo de IA.

### Se conserva (ideas)

- Distinguir hecho / inferencia / hipótesis.
- Criterios de éxito antes de evaluar.
- El contenido auditado no puede mutar el protocolo.
- Conservar el original si hay candidata.
- Modos de escritura (solo lectura, auditar, auditar y refinar).
- Hallazgos con severidad y estado.
- No usar confianza porcentual del modelo como evidencia.
- Ningún veredicto autoriza ejecutar (publicar, enviar, desplegar).
- Detener la recomendación si falta información crítica.
- Contra-revisión en decisiones de alta apuesta.

### Se descarta (atadura local)

- Ámbito exclusivo Campañas Europa 2026 y reglas PHG.
- Runtime Node ESM, `node:test`, CLI de cuatro comandos.
- Almacenamiento con hashes, junctions y validador de integridad de disco.
- Superpowers / subagent-driven-development como método obligatorio.
- Instalación en `.agents/skills`.
- Presupuesto de 32 invocaciones y rúbrica de piloto corporativo.
- Dependencia de un segundo agente independiente (la mayoría de clientes no lo garantizan). Se sustituye por una contra-revisión en el mismo hilo, declarada como tal.

### Se añade (investigación)

- Formato Agent Skills (https://agentskills.io): `SKILL.md` + `references/` + `assets/`, progressive disclosure, frontmatter legal.
- Secuencias de sombreros según el propósito, no un único orden fijo.
- Orden por defecto de evaluación: Amarillo antes de Negro.
- Marcos compañeros: reversibilidad, WRAP recortado, premortem, Cynefin ligero, matriz de opciones.
- Matices por dominio (vida, negocio, programación).
- Licencia MIT y carpeta autocontenida, sin APIs.

## 2. Arquitectura

El agente es el runtime. La skill aporta procedimiento. Sin Python/Node para no romper portabilidad.

## 3. Criterios de aceptación v1

- `SKILL.md` válido según agentskills.io.
- Un cliente compatible puede activarla copiando la carpeta.
- Una sesión produce informe con sombreros separados y un estado de cierre.
- No hay dependencias de red ni secretos.
