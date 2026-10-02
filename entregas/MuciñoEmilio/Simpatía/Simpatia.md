# Modelo del Dominio: Simpatía

## 1. Contexto del Modelo del Dominio

El **Modelo del Dominio de Simpatía** evalúa la conducta social y la disposición de una persona generan sensaciones de calidez, apertura y afinidad en su entorno. En lugar de tratar la simpatía como un rasgo estático o innato, este modelo la aborda como un estado dinámico que resulta de la percepción acumulada de sus interacciones.

### Flujo del Dominio

1. Una **Persona** realiza una **Interacción Social** (conversar, escuchar, sonreír o dar apoyo).

2. La interacción produce una **Percepción Empática** en el interlocutor o grupo.

3. Un **Evaluador de Empatía** recibe estas percepciones y las contrasta contra sus propios criterios sociales o culturales.

4. Si las experiencias positivas superan el umbral esperado, la persona se considera "simpática" dentro de ese grupo o contexto.

## 2. Glosario de Términos
| **Término** | **Definición** |
|---|---|
| **Simpatía** | Cualidad percibida que refleja la capacidad de un sujeto para transmitir calidez, trato agradable y cercanía. |
| **Interacción Social** | Acto comunicativo o gesto observable que ocurre entre una persona y su entorno. |
| **Percepción Empática** | Impresión afectiva o nivel de agrado que deja una interacción en el receptor. |
| **Evaluador de Empatía** | Entidad o sujeto que procesa las impresiones recibidas y determina el umbral de afinidad. |

## 3. Suposiciones del Modelo

1. **Estado Dinámico:** La simpatía no se posee de forma fija; se construye o se pierde según la calidad de las interacciones recientes.

2. **Dependencia del Contexto:** Un mismo comportamiento puede generar percepciones distintas dependiendo de la cultura o el estado de ánimo del evaluador.

3. **Requerimiento Recíproco:** Mantener la simpatía exige equilibrio entre expresividad (atención, humor) y escucha activa.

## 4. Decisiones de Modelado

### Decisión 1: Condición Derivada

- **Decisión:** La simpatía es un resultado calculado a partir de las `PercepcionEmpatica` recibidas, no un valor estático asignado manualmente.

- **Justificación:** Mantiene la fidelidad con la interacción humana real, donde la reputación de alguien cambia de forma fluida según su conducta.

### Decisión 2: Separación del Criterio de Evaluación

- **Decisión:** Mover la lógica del umbral de aprobación a la entidad `EvaluadorEmpatia`.

- **Justificación:** Permite que diferentes sujetos califiquen a la misma persona de forma independiente según sus propias expectativas personales.




