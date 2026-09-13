# Protocolo por sombrero

Usar un sombrero cada vez. El sombrero dirige la atención; no etiqueta a personas.

## Azul — proceso

Preguntas:

- ¿Qué estamos decidiendo, y qué no?
- ¿Qué secuencia encaja con el tipo de decisión?
- ¿Qué se considerará un cierre válido?
- ¿Qué queda para el humano?

Errores típicos:

- Empezar a opinar antes de fijar alcance.
- Cerrar con un veredicto que no se sigue de los sombreros anteriores.
- Convertir el Azul en un discurso motivacional.

Salida mínima: alcance, modo, secuencia, criterios, y al final recomendación + condiciones + tripwires.

## Blanco — hechos

Preguntas:

- ¿Qué datos hay, con fuente y fecha?
- ¿Qué falta y es decisivo?
- ¿Qué es hecho, qué es inferencia y qué es supuesto?
- ¿Hay contradicción entre fuentes?

Clasificación obligatoria de cada afirmación material:

| Etiqueta | Significado |
| --- | --- |
| `verificado` | El expediente o una fuente citada lo sostiene. |
| `refutado` | Hay evidencia en contra en el expediente o fuente citada. |
| `no_verificable` | No se puede comprobar aquí y ahora. |
| `supuesto` | Se está tratando como cierto sin prueba. |

Errores típicos:

- Opiniones disfrazadas de dato.
- Rellenar huecos con "es obvio".
- Confundir ausencia de evidencia con evidencia de ausencia.

Si falta un dato sin el cual la recomendación cambia de sentido, márcalo como laguna crítica.

## Rojo — emoción e intuición

Preguntas:

- ¿Qué siente el decisor al imaginar cada opción?
- ¿Qué sentirían afectados evidentes (equipo, pareja, usuarios, clientes)?
- ¿Hay rechazo visceral, alivio, orgullo, miedo al ridículo o apego a lo ya invertido?

Reglas:

- No justificar. Una frase basta.
- Corto. Si se alarga, se está racionalizando y ya no es Rojo.
- Toda predicción de adopción o reputación es hipótesis, no hecho.

Errores típicos:

- Usar el Rojo para vetar sin pasar por Negro.
- Inventar el estado emocional de personas no consultadas y tratarlo como evidencia.

## Amarillo — valor

Preguntas:

- ¿Qué valor concreto crea esta opción si funciona?
- ¿Bajo qué condiciones se materializa?
- ¿Qué merece conservarse aunque se cambie el plan?
- ¿Quién gana qué, y cuándo?

Reglas:

- El beneficio debe ser plausible, no un eslogan.
- Separar valor de cumplimiento obligatorio. Una ventaja no legaliza un incumplimiento.

Errores típicos:

- Lista de deseos sin condiciones.
- Contar el mejor caso como caso base.

## Negro — precaución

Preguntas:

- ¿Cómo falla esto, paso a paso?
- ¿Qué tiene que ser cierto para que funcione, y qué pasa si no lo es?
- ¿Hay incumplimiento ya demostrado de una restricción?
- ¿El daño es reversible?

Reglas:

- Describe mecanismo y condición, no adjetivos.
- `bloqueo` solo si el fallo es material y no está mitigado, o si viola una restricción obligatoria.
- En modo `critico`, corre un premortem: "Estamos 6-12 meses adelante y esto salió mal. Escribe las causas más creíbles."

Errores típicos:

- Alarmismo sin mecanismo.
- Confundir incomodidad con riesgo.
- Usar el Negro para matar alternativas antes de generarlas.

## Verde — alternativas

Preguntas:

- ¿Qué corrección directa elimina un bloqueo sin crear otro peor?
- ¿Qué otras dos opciones serias existen además del default?
- ¿Se puede probar en pequeño antes de un compromiso grande?
- ¿La pregunta está mal planteada (falso dilema)?

Reglas:

- Máximo dos alternativas nuevas más la corrección directa, salvo que el usuario pida un abanico más amplio.
- Cada alternativa lleva: problema que ataca, coste, riesgo nuevo, y qué evidencia la haría ganar.
- "No hay alternativa válida ahora" es un resultado legítimo.
- No uses creatividad para saltarte una restricción obligatoria.

Errores típicos:

- Brainstorm decorativo que no se evalúa.
- Una sola opción disfrazada de tres matices.
