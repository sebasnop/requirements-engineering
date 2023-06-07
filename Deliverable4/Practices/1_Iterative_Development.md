# Iterative development of the software system

**Desarrollo iterativo del sistema de software**.

**Alpha:** Software system.

&nbsp;

## Table of contents

- [Iterative development of the software system](#iterative-development-of-the-software-system)
  - [Table of contents](#table-of-contents)
  - [Beta prototype](#beta-prototype)
    - [Clicks](#clicks)
    - [Base de datos](#base-de-datos)
  - [Source code examples](#source-code-examples)

&nbsp;

## Beta prototype

**Prototipo beta**.

Es exactamente el [prototipo alfa](..\..\Deliverable3\Practices\5_Relative_Development.md#alpha-prototype) pero con unas funcionalidades adicionales que permitirán especificar todo dentro de la aplicación.

Las funcionalidades adicionales son:

### Clicks

- **Click derecho a relación dinámica:** Especificación detallada.
- **Click derecho a un evento:** Especificación detallada.
- **Doble click a relación de lo logro:** KPI con su fórmula.
- **Click derecho a relación de lo logro:** Especificación detallada de cálculo del KPI.

### Base de datos

Simular la base de datos con el *local storage* del navegador web. Cada elemento clase debe tener su contraparte en la Base de datos.

También se tendrá una estructura en un JSON. Con el JSON se manejará la persistencia. Este tendrá las condiciones iniciales de los datos, se carga al *local storage* al iniciar la aplicación y guardará las modificaciones realizadas en el *local storage* al cerrar la aplicación.

La funcionalidad del doble click a los conceptos clase ya no serán con datos quemados sino con los datos persistentes.

Los KPI se irán actualizando con los valores que se tengan actualmente en la aplicación.

&nbsp;

## Source code examples

**Ejemplos de código fuente**.

Se extraerán ejemplos de:

- **Modelo:** Modelado.
- **Vista:** Interfaz gráfica.
- **Controlador:** Cálculos.

Cada elemento debe mantener la consistencia en la terminología con todo el modelo.
  
Demostrar que cada ejemplo efectivamente representa una parte de la especificación. Por ejemplo mediante: Diagrama de clases, Esquema preconceptual, Tabla explicativa del diagrama de procesos.

Demostrar que esos ejemplos de código fuente son una consecuencia directa de alguno de los productos de trabajo.
