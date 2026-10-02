# Modelo del Dominio: Farmear Aura

## 1. Contexto del Modelo del Dominio
El **Modelo de Farmear Aura** captura la dinámica social con la que un individuo ejecuta acciones para acumular, multiplicar o arriesgar su prestigio y respeto social (*Aura*) ante un grupo de observadores.
### Flujo del Dom
inio
1. Una **Persona** realiza una **Acción** pública dentro de un contexto dado.
2. Un **Observador** (o sistema validador) presenciará el acto y evaluará su nivel de estilo, riesgo o torpeza.
3. El **Criterio de Aura** aplica multiplicadores según la dificultad y la autenticidad de la acción.
4. Se genera un **Impacto de Aura** (+Aura o -Aura) que actualiza el balance acumulado del individuo.

---

## 2. Glosario de Términos

| Término | Definición |
| :--- | :--- |
| **Aura** | Métrica abstracta de prestigio, presencia y respeto social que posee un individuo. |
| **Farmear Aura** | Ejecución recurrente de acciones calculadas para maximizar la ganancia de aura. |
| **Acción Realizada** | Conducta o evento observable ejecutado por una persona en un momento específico. |
| **Impacto de Aura** | Ajuste numérico (+ / -) asignado a una acción tras su evaluación social. |
| **Observador** | Entidad o testigo que presencia la acción y valida su impacto. |
| **Criterio de Aura** | Reglas y multiplicadores basados en el riesgo, elegancia o ridículo de la acción. |

---

## 3. Suposiciones del Modelo

1. **Dependencia de Testigos:** Una acción no observada ni validada no genera ni resta aura.
2. **Volatilidad Bidireccional:** El aura se gana gradualmente, pero se puede perder de golpe tras una acción fallida o ridícula.
3. **Escalamiento por Riesgo:** A mayor riesgo o presión social en la acción, mayor es el multiplicador sobre el resultado.

---

## 4. Decisiones de Modelado

### Decisión 1: Desacoplamiento entre Acción e Impacto
* **Decisión:** El `ImpactoAura` se calcula en una entidad independiente a la `AccionRealizada`.
* **Justificación:** Una misma acción puede provocar reacciones opuestas según la percepción y expectativas del observador.

### Decisión 2: Balance Signado Único
* **Decisión:** Se utiliza un valor entero con signo (+/-) para consolidar las variaciones en lugar de registrar entidades separadas para pérdidas y ganancias.
* **Justificación:** Simplifica las operaciones aritméticas directas sobre el balance total del sujeto.
