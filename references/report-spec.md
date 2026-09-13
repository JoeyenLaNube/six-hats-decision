# Especificación del informe

## Estados

| Estado | Significado |
| --- | --- |
| `SEGUIR` | Avanzar con la opción indicada, sin bloqueos abiertos |
| `REFINAR` | Hay que cambiar el plan antes de comprometerse |
| `NO_SEGUIR` | La opción evaluada no se sostiene |
| `NECESITA_INFO` | Falta un dato que cambiaría el sentido |
| `NO_EVALUADO` | No se completó el protocolo |

Un `aviso` no impide `SEGUIR`. Un `bloqueo` sí.

Si el texto de cierre dice adelante pero hay un bloqueo abierto, el estado no puede ser `SEGUIR`.

## Límites de una pasada

- Una candidata nueva.
- Una contra-revisión en `critico`.
- No ejecutar la decisión.
