

# Modelo del Dominio: Óptica de Sombras

## 1. Contexto del Modelo del Dominio

El **Modelo del Dominio de Sombras** describe la relación entre una fuente emisora de luz, un objeto que interrumpe su trayectoria, la sombra resultante de dicha intercepción y la superficie sobre la cual esta se proyecta.

### Flujo del Dominio
1. La **Fuente de Luz** emite radiación luminosa hacia el espacio.
2. El **Objeto** intercepta y ocluye parte de esa luz.
3. La **Sombra** se genera como consecuencia de esta oclusión.
4. La **Sombra** se proyecta sobre una **Superficie** receptora.

---

## 2. Glosario de Términos

| Término | Definición |
| :--- | :--- |
| **Fuente de Luz** | Entidad emisora de flujo luminoso. |
| **Objeto** | Entidad opaca o semiopaca que interrumpe o bloquea la luz emitida. |
| **Sombra** | Región de oscuridad o penumbra resultante de la oclusión de la luz por parte del objeto. |
| **Superficie** | Plano o volumen receptor donde se proyecta la sombra. |

---

## 3. Suposiciones del Modelo

1. **Propagación Rectilínea:** La luz viaja en línea recta en el medio.
2. **Dependencia de Oclusión:** No existe sombra sin la presencia simultánea de una fuente de luz y un objeto oclusor.
3. **Recepción Única por Instante:** Cada sombra se manifiesta o proyecta sobre la geometría de una superficie determinada.

---

## 4. Decisiones de Modelado

### Decisión 1: Sombra como Entidad de Dominio Reificada
* **Decisión:** Tratar a la `Sombra` como una clase explícita dentro del dominio en lugar de una propiedad implícita de la superficie.
* **Justificación:** Permite capturar la relación m:n entre fuentes, objetos y proyecciones, así como modelar atributos propios de la sombra (como intensidad o tipo de borde) de manera independiente.

### Decisión 2: Simplicidad en las Definiciones de Clases
* **Decisión:** Mantener las clases abstractas/minimalistas en esta etapa del modelado inicial.
* **Justificación:** Facilita la extensión futura del modelo (por ejemplo, añadiendo atributos geométricos o fotométricos) sin acoplar la arquitectura a una implementación concreta.
