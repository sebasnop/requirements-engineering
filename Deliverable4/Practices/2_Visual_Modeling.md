# Visual modeling of requirements

**Modelado visual de requisitos**.

**Alpha:** Requirements.

Los diagramas de [Clases](#class-diagram), [Comunicación](#communication-diagrams) y [Máquina de estados](#state-machine-diagrams) pertececen al estándar UML.

Para describir completamente un sistema de software se requiere al menos un diagrama por cada una de los siguientes conceptos: Estructura (Clases), Interacción (Comunicación) y Comportamiento (Máquina de estados).

Mendiante las [Especificaciones basadas en el Esquema Preconceptual](#ps-based-specifications) se le dará al Esquema Preconceptual (PS) la sintaxis necesaria para que se pueda tener una sintaxis adecuada, semántica precisa y posibilidad de teoría de prueba. Se detallará cada elemento del PS para que su programación sea unívoca, sin omportar el lenguaje de programación usado.

&nbsp;

## Table of contents

- [Visual modeling of requirements](#visual-modeling-of-requirements)
  - [Table of contents](#table-of-contents)
  - [PS-based specifications](#ps-based-specifications)
    - [Atomic dynamic relationships](#atomic-dynamic-relationships)
    - [Data types \& Constraints](#data-types--constraints)
  - [Class diagram](#class-diagram)
  - [Communication diagrams](#communication-diagrams)
  - [State-machine diagrams](#state-machine-diagrams)

## PS-based specifications

**Especificaciones basadas en el Esquema Preconceptual**.

Se estudiarán elementos que pueden estar en **especifiaciones* (specifications) y **restricciones** (constraints) en el PS.

Lo primero es entender que una relación dinámica, relación de logro o un evento puede tener una información por dentro que se detallará.

### Atomic dynamic relationships

Adentro de las relaciones dinámicas, relaciones de logro y eventos hay un conjunto de **relaciones dinámicas atómicas**:

- Inserts
- Updates
- Deletes
- Lists
- Searches
- Selects

Es decir, todas las relaciones dinámicas son una combinación lineal de relaciones dinámicas atómicas.

Aquellas que cambian los valores de los conceptos hoja son Inserts,  Updates & Deletes. Las otras son opcionales y sirven como apoyo para llevar a cabo al menos una de las que cambian valores.

### Data types & Constraints

Al agregar dos puntos, espacio y unos símbolos se define el tipo de dato de un concepto hoja.

- Text: `Concept`
- Date: `Concept: //`
- Number: `Concept: #`
- Boolean: `Concept: ?`
- Email: `Concept: @`

Mediante la forma de las flechas se definen los *NonNull*.

No se necesita especificar las relaciones dinámicas que no tengan asociadas una relación de logro. Es decir, solo se hará para Requisitos, que además estén en el Diagrama de Objetivos.

No se especifican las relaciones de logro asociadas a relaciones dinámicas. Pero sí las que están relacionadas con conceptos o relaciones estructurales. Deben ser consistentes con el KPI y con el objetivo.

También se debe especificar para encuestas. Proveer la interfaz para dicha encuesta.

## Class diagram

Es una evolución del Modelo de Dominio del entregable 1.

Relaciones de agregación o composición.

## Communication diagrams

Uno por cada caso de uso.

Tiene las clases (objetos) y los mensajes que viajan por los enlaces.

## State-machine diagrams

Una por cada concepto clase.

Los nombres de los estados provienen de los nombres de las relaciones dinámicas (En participio pasado) o de estados (posibles valores fijos) de conceptos hoja que tienen posibles valores asociados.
