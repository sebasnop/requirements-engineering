# Visual modeling of requirements

**Modelado visual de requisitos**.

**Alpha:** Requirements.

En el [Organization chart](#organization-chart) y el [Process diagram](#process-diagram) se busca adaptar el dominio ya existente a la solución que se creará. Porque la solución creada impacta en los procesos que se llevan a cabo en la organización.

Con los [Use cases](#use-cases) y los [User interface flow diagram](#user-interface-flow-diagram) se busca especificar la funcionalidad del sistema de software.

&nbsp;

## Table of contents

- [Visual modeling of requirements](#visual-modeling-of-requirements)
  - [Table of contents](#table-of-contents)
  - [Goals](#goals)
  - [Use cases](#use-cases)
    - [Extends](#extends)
    - [Include](#include)
    - [Normas mínimas](#normas-mínimas)
  - [User interface flow diagram](#user-interface-flow-diagram)
  - [Organization chart](#organization-chart)
  - [Process diagram](#process-diagram)

&nbsp;

## Goals

1. Especificar la funcionalidad del sistema de software.
    - [Use cases](#use-cases)
    - [User interface flow diagram](#user-interface-flow-diagram)
2. Adaptar el dominio existente a la solución.
    - [Organization chart](#organization-chart)
    - [Process diagram](#process-diagram)
3. Verificar la consistencia
    - [Use cases](#use-cases)
    - [User interface flow diagram](#user-interface-flow-diagram)
    - [Organization chart](#organization-chart)
    - [Process diagram](#process-diagram)

&nbsp;

## Use cases

**Casos de uso**.

Hace parte de UML. Busca mostrar la parte interactiva y comportamiento del sistema del software.

Representación de aquello que se pudiera hacer con el sistema de software.

Hay relación directa entre las acciones y los actores que las activan.

También aparecen relaciones de generalización o especialización de los casos o actores.

### Extends

Una relación de extensión de la funcionalidad original. Se desprenden acciones específicas de una general que las engloba.

```text
Assigns Tag -- extends -> Edits Album
```

No se necesita que la función extensión (hija) esté ligada al actor porque la función extendida (padre) ya está ligada al actor.

### Include

Una relación de implicación. Una acción solo se puede ejecutar si se ejecutó otra previamente.

```text
Deletes Album -- include -> Creates Album
```

### Normas mínimas

> Se pueden manejar tan general o específico como se prefiera, es de libre uso. Sin embargo, se esperan características mínimas.

Los casos de uso deben estar definidos en el preconceptual. La sintaxis mínima: Tríadas dinámicas en forma de casos de uso.

Si tenemos casos de uso agrupados en responsabilidades, estas responsabilidades deberían estar explicitamente como **entornos del sistema** en el esquema preconceptual, agrupando las relaciones dinámicas correspondientes.

Las implicaciones entre relaciones dinámicas usualmente son relaciones de inclusión ([*include*](#include))

En las relaciones de extención ([*extends*](#extends)) se representan relaciones dinámicas que indirectamente solo se pueden realizar cuando ocurren otras (no como implicaciones dinámicas explícitas).

&nbsp;

## User interface flow diagram

**Diagrama de flujo de interfaces de usuario**.

Nos permite establecer de qué modo vamos a navegar el sistema.

Vínculos entre diferentes interfaces gráficas del usuario.

Se suele usar en el desarrollo web.

Cada rectángulo es una interfaz del sistema.

En las flechas se tienen las maneras en que se va a interactuar con el sistema.

Se puede usar el original o uno más intuitivo con imágenes reales de la interfaz sustituyendo los rectángulos.

> Se puede usar la forma original o la forma más intuitiva, cualquiera de las dos.

&nbsp;

## Organization chart

*Organigrama*.

Producto ya existente. (CREO QUE No se elimina el anterior sino que se añade la actualización).

En el *Organization chart* pueden aparecer o desaparecer cargos o responsabilidades (Como aparecer analista de los datos o manejo de base de datos, etc).

&nbsp;

## Process diagram

**Diagrama de procesos**.

Producto ya existente. (CREO QUE No se elimina el anterior sino que se añade la actualización).

Pueden ocurrir muchos cambios. Como que los procesos cambien, se fundan (unos se incluye en otro), se atomicen (se parta uno en varios) o no se consideren en la solución que se llevará a cabo.

La principal diferencia es la aparición de **bordes gruesos** en los procesos, almacenes y características que van a estar en la solución.

> Yo esperaría que no hayan diferencias fundamentales entre el diagrama de procesos del dominio y el de la solución.
