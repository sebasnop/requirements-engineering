# Template-based elicitation of requirements

**Educción de requisitos basada en plantillas**.

**Alpha:** Requirements.

&nbsp;

## Table of contents

- [Template-based elicitation of requirements](#template-based-elicitation-of-requirements)
  - [Table of contents](#table-of-contents)
  - [Goals](#goals)
  - [Use case explanatory table](#use-case-explanatory-table)
  - [Process diagram explanatory table](#process-diagram-explanatory-table)
  - [Data dictionary](#data-dictionary)

&nbsp;

## Goals

Iguales a los [Objetivos del modelado visual de requisitos](1_Visual_Modeling.md#goals), solo que asociados a productos de trabajo diferentes:

1. Especificar la funcionalidad del sistema de software.
    - [Use case explanatory table](#use-case-explanatory-table)
2. Adaptar el dominio existente a la solución.
    - [Process diagram explanatory table](#process-diagram-explanatory-table)
    - [Data dictionary](#data-dictionary)
3. Verificar la consistencia
    - [Use case explanatory table](#use-case-explanatory-table)
    - [Process diagram explanatory table](#process-diagram-explanatory-table)
    - [Data dictionary](#data-dictionary)

&nbsp;

## Use case explanatory table

**Tabla explicativa de los casos de uso**.

Define los casos de uso de manera formal con sus causas y sus efectos.

Se basa en el concepto de **Contract**. Agregar una información de cuál es el efecto del caso de uso en el mundo.

- **Use Case**
  
  Nombre (Con codificación`UC##`).
  
- **Version**
  
  Versionamiento.
  
  Libertad de formato de números.Se puede usar solo números naturales (1, 2, etc) o con puntos según la magnitud del cambio (1.1.2, 2.2.0, etc).

- **Date**
  
  Fecha de realización
  
- **Author**
  
  Autor o autores
  
- **Source**
  
  Recurso de donde se sacó la información.

- **Purpose**
  
  Prosa que explica el propósito.
  
- **Goals**
  
  Objetivos asociados y problemas que permite solucionar.

- **Summary**
  
  Resumen de lo que se hace en el caso de uso.

- **Actors**
  
  Con codificación `A#`.

- **Precondition**
  
  Qué es lo que se requiere para que podamos realizar el caso de uso.

- **Interaction Sequence**
  
  **Secuencia normal** de interacción entre el usuario y el sistema.
  
  > Hay que ser muy detallados, demasiado detallados.

  Los casos de uso representan la primera versión de los casos de prueba del sistema.

  Ser detallados con todos los elementos que me sirvan para manejar la interfaz. Que con todos los elementos de la interfaz se pueda reconstruir lo que describe el caso de usuario.

- **Alternative Sequence**
  
  Otros elementos de la interfaz que están presentes y que de alguna forma se debe detallar para que el caso de uso esté completo.

  Funciones adicionales.

  Se define en cuáles pasos de la secuencia normal se pueden realizar estas funciones adicionales.

- **Duration**

  Óptimo, promedio, máximo.

  En la [tabla explicativa del diagrama de procesos](#process-diagram-explanatory-table) solo aparece el promedio.
  
- **Frequency**
  
  Se puede extraer directamente de la [tabla explicativa del diagrama de procesos](#process-diagram-explanatory-table).

- **Type**
  
  Primario o secundario.
  
  - Primary

    Si el caso de uso genera información para resolver los problemas, de modo que se traduce a un beneficio directo para la organzación.

  - Secondary

    Si el caso de uso es necesario para obtener información que sirve para un caso de uso primario, pero que por sí mismo no se traduce a un beneficio directo. Se dice que es un costo para la organización.

- **Postconditions**

  Responde a qué es lo que se cambia en el mundo al realizarse un caso de uso.
  
  Un caso de uso debe cambiar al menos un valor de alguno de los conceptos hoja asociados con algún concepto clase del sistema.

  También las relaciones dinámicas cambian un concepto hoja.

- **Chart**
  
  Porción correspondiente al diagrama de casos de uso.
  
- **Interface**

  Interfaz gráfica del usuario.
  
  Donde se muestre todo lo especificado en el caso de uso.

Recordar que los casos de uso dependen de procesos que están en el [Diagrama de procesos](1_Visual_Modeling.md#process-diagram)

&nbsp;

## Process diagram explanatory table

**Tabla explicativa del diagrama de procesos**.

Producto ya existente. No se elimina la anterior sino que se añade la actualización.

Se actualiza junto con el diagrama de procesos.

&nbsp;

## Data dictionary

Producto ya existente. No se elimina el anterior sino que se añade la actualización.
