---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definir tipos de hora y disponibilidad para hojas de hora
description: Un tipo de hora es una etiqueta que le permite categorizar la entrada horaria. En función de los requisitos de informes de su organización durante horas, esto puede ser una parte esencial del tiempo de registro.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# Definir tipos de hora y disponibilidad para hojas de hora

Un tipo de hora es una etiqueta que le permite categorizar la entrada horaria. En función de los requisitos de informes de su organización durante horas, esto puede ser una parte esencial del tiempo de registro.

Hay dos conjuntos de tipos de hora en Adobe Workfront:

* **Horario general:** Horas que no están asociadas con un proyecto, como el tiempo de enfermedad o la administración. Solo puede registrar las horas generales en el parte de horas.
* **Horas específicas del proyecto:** Horas registradas en proyectos, tareas y problemas. Puede registrar las horas específicas del proyecto desde cualquier ubicación donde pueda registrar la hora.

Al iniciar sesión en Workfront, los tipos de hora específicos del proyecto que están disponibles dependen de las opciones de configuración establecidas en los niveles del sistema, el proyecto y el usuario. (Siempre están disponibles los siguientes tipos predeterminados de hora específicos del proyecto: Hora del proyecto, Hora de la tarea y Hora del problema).

Los tipos de hora que se pueden seleccionar al iniciar la sesión (en proyectos, tareas y problemas) están determinados primero por los tipos de hora que el administrador del sistema pone a disposición en todo el sistema y, a continuación, por los tipos de hora seleccionados en los niveles de proyecto y usuario.

Una vez configurados los tipos de hora adecuados, puede registrar la hora desde varias ubicaciones en Workfront, tal como se describe en [Tiempo de registro](../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso del administrador del sistema para definir tipos de hora de todo el sistema y editar todos los usuarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administrar el acceso en el proyecto para definir los tipos de hora en un proyecto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Definir la disponibilidad a nivel del sistema

El administrador del sistema determina qué tipos de hora específicos del proyecto están disponibles en todo el sistema, tal como se describe en la sección [Administrar tipos de hora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) en  [Administrar tipos de hora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definir la disponibilidad a nivel de proyecto {#define-availability-at-the-project-level}

El propietario del proyecto determina si todos los tipos de hora definidos a nivel del sistema están disponibles en el proyecto (y las tareas y problemas dentro del proyecto) o si solo está disponible un subconjunto de esos tipos de hora. 

1. Vaya al proyecto en el que desea determinar la disponibilidad de los tipos de hora.
1. Haga clic en el **Más** junto al nombre de la tarea y haga clic en **Editar**.

1. Haga clic en **Editar proyecto**.
1. En el **Configuración** , ubique la sección **Filtrar tipos de hora** .

1. Select **No** para que todos los tipos de hora específicos del proyecto estén disponibles en el proyecto.

   O

   Select **Sí** para que solo un subconjunto de los tipos de hora específicos del proyecto esté disponible en el proyecto, seleccione los tipos de hora que desee poner a disposición. (Mantenga pulsada la tecla Mayús para seleccionar varios tipos de hora).

   Si selecciona esta opción, solo los tipos de hora que seleccione estarán disponibles para seleccionarlos al iniciar sesión en el proyecto (o en las tareas y problemas dentro del proyecto). Si selecciona esta opción y no selecciona ningún tipo de hora, el proyecto muestra solo los tipos generales de hora.

   Se deben realizar las mismas selecciones a nivel de usuario individual para que el usuario vea estas opciones de tipo de hora en el proyecto.

1. Haga clic en **Guardar cambios**.

## Definir la disponibilidad a nivel de usuario

Puede registrar horas para un tipo de hora determinado en proyectos, tareas y problemas solo si ese tipo de hora está disponible en el sistema, en el nivel de proyecto y en el nivel de usuario.

Si pone un tipo de hora a disposición del usuario como se describe en esta sección, pero no ve ese tipo de hora al iniciar sesión en un proyecto, tarea o problema, ese tipo de hora no se ha puesto a disposición del proyecto (como se describe en [Definir la disponibilidad a nivel de proyecto](#define-availability-at-the-project-level)).

Para definir los tipos de hora disponibles para un usuario:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en el avatar del usuario en la esquina superior izquierda.
1. Haga clic en el **Más** junto al nombre de usuario y haga clic en **Editar**.

1. Solo los administradores del sistema pueden editar otros usuarios. Si tiene una licencia de Plan, puede editar los tipos de horas en su propio perfil.
1. En el **Planificación de recursos** en la sección **Tipos de hora disponibles** menú desplegable, realice una de las acciones siguientes en función de los tipos de hora que desee que estén disponibles al iniciar sesión en un proyecto, tarea o problema:

   * **Para que todos los tipos de horas estén disponibles para el usuario:** Seleccione todos los tipos de hora.\
      Si deja todos los tipos de hora sin seleccionar, técnicamente es lo mismo que seleccionar todos los tipos de hora. Sin embargo, en este caso, todo el tipo de hora solo está disponible para el usuario en proyectos, tareas y problemas en los que **No** se selecciona en la variable **Filtrar tipos de hora** al editar el proyecto, tal como se describe en [Definir la disponibilidad a nivel de proyecto](#define-availability-at-the-project-level).
   * **Para que solo un subconjunto de los tipos de hora esté disponible para el usuario:** Seleccione solo los tipos de hora que desea poner a disposición.

      Para que los tipos de hora que seleccione a nivel de usuario estén disponibles en proyectos, tareas y problemas, estos mismos tipos de hora también deben seleccionarse en la variable **Filtrar tipos de hora** al editar el proyecto, tal como se describe en [Definir la disponibilidad a nivel de proyecto](#define-availability-at-the-project-level).

1. Haga clic en **Guardar cambios**.

   Ahora, cuando inicia sesión en un proyecto, tarea o problema, los tipos de hora que selecciona están disponibles si esos mismos tipos de hora están disponibles a nivel de proyecto.
