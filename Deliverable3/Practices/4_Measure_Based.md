# Measure-based assessment of the opportunity

**Evaluación de la oportunidad basada en métricas**.

**Alpha:** Opportunity.

Cuál es el valor y el costo de la solución en términos de la oportunidad.

&nbsp;

## Goals

1. Entender las necesidades del interesado.
   - Estimar el esfuerzo necesario del equipo.
     - [Solution Effort](#solution-effort)
2. Garantizar la satisfacción del interesado.
   - Estimar el valor de la solución.
     - [Solution Value](#solution-value)
   - Estimar los factores críticos de éxito.
     - [CSF matrices](#csf-matrices)
     - [Interpretive structural model](#interpretive-structural-model)
   - Definir KPIs (Key Performance Indicator).
     - [KPI definition table](#kpi-definition-table)
   - Diseñar KPIs.
     - [KPI design](#kpi-design)
   - Verificar consistencia.
     - [Solution Effort](#solution-effort)
     - [Solution Value](#solution-value)
     - [CSF matrices](#csf-matrices)
     - [Interpretive structural model](#interpretive-structural-model)
     - [KPI definition table](#kpi-definition-table)
     - [KPI design](#kpi-design)

&nbsp;

## Solution effort

**Esfuerzo de la solución**.

Para un problema pueden plantearse diferentes soluciones. En la ingenería de software no solo se busca llegar a la mejor sino que también se debe tener en cuenta el presupuesto del cliente.

Anteriormente se usaban los **Puntos de función** para estimar el costo de una solución de Software. Sin embargo, con el uso de la Programación Orientada a Objetos (POO), el mecanismo de Puntos de función perdió vigencia.

Karner en Metrics for Objectory (1993) desarrolló métricas que permitirían la estimación de esfuerzos (y costos) para software planeado con el paradigma de la POO. Su resultado son los **Puntos de casos de uso** . Uno de sus problemas es basarse en los casos de uso y es demasiado informal.

### Use case point

Identifican dos elementos principales que describen la complejidad del sistema de software:

- Actor
- Casos de uso

#### Actors: Use case point

Con base en estos elementos se puede observar cuál es la estructura del sistema y calificar los factores técnicos y ambientales para definir el esfuerzo en la realización del sistema de software.

1. Identificar los actores asociados al sitema de software.
2. Clasificar los actores según el nivel de programación necesario para satisfacer sus necesidades.
  
    Tipos de actores
  
    1. Simples
  
        Aquel que tiene un manejo del sistema que no necesita interfaz gráfica.

        Por ejemplo, un administrador de base de datos.
  
    2. Promedios
  
        Intermedio entre Simples y complejos.

        Requiere interfaces para hacer algunas cosas. Para hacer otras cosas no.

    3. Complejos
  
        Son los usuarios finales del sistema. Todo lo observan a partir de la interfaz gráfica de usuario.
        Hay que programarle todo.

3. Contar número de actores según el tipo: **Number of actors**.

4. Multiplicar el número de actores del tipo por su factor multiplicador: **Multiplier**.
    - Simple: 1
    - Promedio: 2
    - Complejo: 3

#### Use case: Use case point

Se hace algo muy similar con los casos de uso. Se examina cuáles casos están en un nivel o en otro de complejidad.

- Simple:
    Caso de uso secundario.
    Solo obtener información.
- Promedio:
    Entre simple y complejo.
- Complejo:
    Caso de uso primario.

También se mide con transacciones (*commits*).

Multiplicador diferente:

- Simple: 5
- Promedio: 10
- Complejo: 15

#### Environmental Factors

**Factores ambientales**.

Referentes al equipo y usuarios.

#### Technical Factors

**Factores técnicos**.

Referentes a cómo se construye la aplicación.

&nbsp;

> Solo se analizará una solución, pero esta herramienta permite analizar diferentes soluciones

&nbsp;

## Solution value

**Valor de la solución**.

Establecer el enlace entre los diferentes [procesos](1_Visual_Modeling.md#process-diagram) y los casos de uso (procesos originados en las tríadas dinámicas del esquema preconceptual).

Lo ideal es que un proceso esté ligado a un caso de uso, sin embargo, se pueden presentar situaciones en que no sea así:

- Varios procesos agrupados en un caso de uso
  
    En el diagrama de procesos de la solución se tendrá solo ese proceso en el diagrama de procesos de la solución.

- Varios casos de uso asociados a un solo proceso.
  
    Se deben atomizar los procesos con los diferentes casos de uso que se tienen.

Todo el resto de la información estará contenida en la [tabla explicativa de casos de uso](2_Template_Based.md#process-diagram-explanatory-table):

- Goals/Requirements
- Problems
- Use cases

### Cause-Effect Heat Map

Esto se hace para cacular el **valor de la solución**. Se llegará a un diagrama Causa-Efecto, usando un mapa de calor que indica cuánto se está trabajando en cada uno de los problemas.

El porcentaje es el de trabajo sobre las causas.

Se busca definir la importancia de la solución por medio de su valor al atender las causas. Se busca llegar a una solución con la mayor cantidad de porcentaje en la mayor cantidad posible de causas.

Un mapa de color totalmente rojo sería lo ideal. Un valor aceptable es entre verde, amarillo y naranja porque nunca se solucionarán todos los problemas con una sola solución.

Se llega al mapa de calor con el causa efecto ya hecho en el entregable 2.

En la tabla se especifica:

- Caso de uso
- Causa asociada: (De Causa-Efecto)
- $P_{i,j}$: Directamente de la tabla asigación porcentajes del Causa-Efecto
- $Q_{i,j}$: Directamente de la tabla asigación porcentajes del Causa-Efecto
- $C_{i}$: Cobertura.

    Definir qué tanto se tienen cubiertos (Se automatizan) todos los procesos que incluyen las causas que se están manejando en la solución.

    Un segundo aspecto que se podría tratar, pero que no hay que hacer, es definir qué tanto resuelte las causas que abarca. Es algo subjetivo.

- $\%$: Porcentaje igual a $P_{i,j} \times Q_{i,j} \times C_{i}$.

&nbsp;

## CSF matrices

**Matrices de factores críticos de éxito**.

Fue extraído del **modelo interpretativo estructural** que se usa para manejar el tema de factores críticos de éxito en el desarrollo de software.

### Critical Factor Success

**Factores críticos de éxito**.

Medida para saber qué tan existosa es una aplicación.

Los conceptos clase serán fundamentales para encontrar los CSF. ¿De qué forma el sistema de software se consideraría exitoso según los conceptos clase?

Agregarle al concepto clase un verbo nominalizado. Ejemplo: Clase: User, Verbo: Recruitment.

Al menos un factor crítico de éxito por cada clase.

&nbsp;

### Self Interaction Matrix

**Matriz de autointeracción** (**SSIM**).

Se hace la matriz de correlación de factores críticos de éxito.

- **V**: El CSF $i$ ayuda a lograr el CSF $j$.
- **A**: El CSF $j$ ayuda a lograr el CSF $i$.
- **X**: Ambos CSF $i$ y $j$ se ayudan el uno al otro.
- **O**: Los CSF $i$ y $j$ no tienen ninguna relación.

Tener en cuenta que $i$ se refiere al valor de la fila y $j$ al valor de la columna.

&nbsp;

### Reachability matrix

**Matriz de alcanzabilidad**.

A partir de la [Matriz de autointeracción](#self-interaction-matrix)

Diagonal con 1. En el resto, colocar un valor según la [Matriz de autointeracción](#self-interaction-matrix) así:

| SSIM $(i, j)$ | Reachability $(i, j)$ | Reachability $(j, i)$ |
| ------------- | --------------------- | --------------------- |
|       V       |           1           |           0           |
|       A       |           0           |           1           |
|       X       |           1           |           1           |
|       O       |           0           |           0           |

Tener en cuenta que $i$ se refiere al valor de la fila y $j$ al valor de la columna.

En las filas se observa cuáles CSF de las columnas dependen del CSF de la fila. Con su suma se obtiene el **Driving Power**: Poder de dirección.

En las columnas se observa de cuáles CSF de las filas depende el CSF de la columna. Con su suma se obtiene la **Dependence**: Dependencia.

&nbsp;

### CSF Level table

Se definen:

- **Conjunto de alcanzabilidad**: CSF sobre los cuáles influye un CSF.
- **Conjunto de antecedentes**: CSF que requieren algún CSF para funcionar.
- **Conjunto de intersección**: Intersección entre los conjuntos de alcanzabilidad y antecedentes.

A partir de la [Matriz de alcanzabilidad](#reachability-matrix)

Se observa cuál conjunto de alcanzabilidad es igual al de intersección. Esos tendrán un nivel $I$. Esos serán los CSF más importantes para la aplicación.

Se hacen iteraciones borrando los CSF con nivel $I$. Se repite el análisis y se les asigna el siguiente nivel $(II, III, IV, etc)$.

Si en alguna iteración ningún conjunto de alcanzabilidad es igual al de intersección, entonces se buscan a los que solo les falte un elemento para ser igual. Si sigue sin estar ninguno así, se buscan con dos elementos menos. Así sucesivamente.

La idea es encontrar una serie de prioridades sobre los CSF. Estas prioridades serán graficadas en el [Modelo interpretativo estructural](#interpretive-structural-model).

&nbsp;

## Interpretive structural model

**Modelo interpretativo estructural**.

Contiene los CSF categorizados con su nivel de importancia (asignado en la [Tabla de niveles de los CSF](#csf-level-table))

De qué forma los CSF podrían determinar las prioridades. Por ejemplo, en SCRUM se busca establecer prioridades en las historias de usuario.

&nbsp;

## KPI definition table

**Tabla de definición de los indicadores clase de rendimiento**.

Se necesita correlacionar los CSF con objetivos. Es importante que el interesado comprenda cómo se van a satisfacer sus objetivos organizacinales.

Un Key Performance Indicator (KPI) es un número o valor que permite establecer qué tan bien se están cumpliendo los objetivos.

- CSF
- Goal
- KPI
- Formula

&nbsp;

## KPI design

**Diseño de los indicadores de rendimiento clave**.

Se deben diseñar los KPI y sus fórmulas de la [Tabla de definición de los KPI](#kpi-definition-table).

Se realiza un esquema preconceptual con toda la información relacionada con el KPI.

Se define la acción a la que va ligada, el objetivo y la variable KPI que cambia.

Luego se diseña una tabla con colores para definir cuándo el KPI da resultado bueno, regular o malo.
