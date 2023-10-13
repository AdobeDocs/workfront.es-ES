---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definir tipos de horas y disponibilidad para hojas de horas
description: Un tipo de hora es una etiqueta que le permite categorizar la entrada de tiempo. Según los requisitos de informes de su organización en cuanto a horas, esto puede ser una parte esencial del tiempo de registro.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# Definir tipos de horas y disponibilidad para hojas de horas

Un tipo de hora es una etiqueta que le permite categorizar la entrada de tiempo. Según los requisitos de informes de su organización en cuanto a horas, esto puede ser una parte esencial del tiempo de registro.

Hay dos conjuntos de tipos de horas en Adobe Workfront:

* **Horario general:** Horas que no están asociadas a un proyecto, como tiempo de enfermedad o administración. Solo puede registrar horas generales en la hoja de horas.
* **Horas específicas del proyecto:** Horas registradas en proyectos, tareas y problemas. Puede registrar horas específicas del proyecto desde cualquier ubicación en la que pueda registrar horas.

Al registrar el tiempo en Workfront, los tipos de horas específicos del proyecto que están disponibles dependen de las opciones de configuración establecidas en los niveles del sistema, del proyecto y del usuario. (Siempre están disponibles los siguientes tipos de horas predeterminados específicos del proyecto: Hora del proyecto, Hora de la tarea y Hora del problema).

Los tipos de horas disponibles para seleccionar al registrar el tiempo (en proyectos, tareas y problemas) están determinados primero por los tipos de horas disponibles en todo el sistema por el administrador del sistema y, a continuación, por los tipos de horas seleccionados en los niveles de proyecto y usuario.

Una vez configurados los tipos de horas adecuados, puede registrar el tiempo desde varias ubicaciones en Workfront, tal como se describe en [Registrar tiempo](../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de administrador del sistema para definir tipos de horas de todo el sistema y editar todos los usuarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administrar el acceso al proyecto para definir los tipos de horas de un proyecto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Definir disponibilidad en el nivel del sistema

El administrador del sistema determina qué tipos de horas específicos de proyecto están disponibles en todo el sistema, tal como se describe en la sección [Administrar tipos de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definir disponibilidad en el nivel de proyecto {#define-availability-at-the-project-level}

El propietario del proyecto determina si todos los tipos de horas definidos en el sistema están disponibles en el proyecto (y las tareas y problemas dentro del proyecto) o si solo está disponible un subconjunto de esos tipos de horas. 

1. Vaya al proyecto en el que desea determinar la disponibilidad de los tipos de horas.
1. Haga clic en **Más** junto al nombre de la tarea y haga clic en **Editar**.

1. Clic **Editar proyecto**.
1. En el **Configuración** , busque la sección **Filtrar tipos de horas** opción.

1. Seleccionar **No** para que todos los tipos de horas específicos del proyecto estén disponibles en el proyecto.

   O

   Seleccionar **Sí** para que solo un subconjunto de los tipos de horas específicos del proyecto esté disponible en el proyecto, seleccione los tipos de horas que desee poner a disposición. (Mantenga pulsada la tecla Mayús para seleccionar varios tipos de horas).

   Si selecciona esta opción, solo estarán disponibles para seleccionarlos los tipos de horas que seleccione al registrar horas en el proyecto (o en tareas y problemas dentro del proyecto). Si selecciona esta opción y no selecciona ningún tipo de hora, el proyecto solo muestra los tipos de hora generales.

   Las mismas selecciones deben realizarse en el nivel de usuario individual para que el usuario pueda ver estas opciones de tipo de hora en el proyecto.

1. Haga clic en **Guardar cambios**.

## Definir disponibilidad en el nivel de usuario

Puede registrar horas para un tipo de hora determinado en proyectos, tareas y problemas solo si ese tipo de hora está disponible en el nivel del sistema, del proyecto y del usuario.

Si hace que un tipo de hora esté disponible en el nivel de usuario como se describe en esta sección, pero no ve ese tipo de hora al registrar la hora en un proyecto, tarea o problema, ese tipo de hora no estará disponible en el proyecto (como se describe en [Definir disponibilidad en el nivel de proyecto](#define-availability-at-the-project-level)).

Para definir los tipos de horas disponibles para un usuario:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en el avatar del usuario en la esquina superior izquierda.
1. Haga clic en **Más** junto al nombre de usuario y haga clic en **Editar**.

1. Solamente un administrador del sistema puede editar a otros usuarios. Si tiene una licencia de planificación, puede editar los tipos de horas en su propio perfil.
1. En el **Planificación de recursos** , en la sección **Tipos de horas disponibles** en el menú desplegable, realice una de las acciones siguientes, en función de los tipos de horas que desee poner a disposición al registrar la hora de un proyecto, tarea o problema:

   * **Para que todos los tipos de horas estén disponibles para el usuario:** Seleccione todos los tipos de horas.\
     Si deja todos los tipos de horas sin seleccionar, técnicamente es lo mismo que seleccionar todos los tipos de horas. Sin embargo, en este caso, todos los tipos de horas están disponibles para el usuario solo en proyectos, tareas y problemas en los que **No** está seleccionado en la **Filtrar tipos de horas** al editar el proyecto, tal como se describe en [Definir disponibilidad en el nivel de proyecto](#define-availability-at-the-project-level).
   * **Para que solo un subconjunto de los tipos de hora esté disponible para el usuario:** Seleccione solo los tipos de horas que desee que estén disponibles.

     Para que los tipos de horas que seleccione en el nivel de usuario estén disponibles en proyectos, tareas y problemas, estos mismos tipos de horas también deben estar seleccionados en la **Filtrar tipos de horas** al editar el proyecto, tal como se describe en [Definir disponibilidad en el nivel de proyecto](#define-availability-at-the-project-level).

1. Haga clic en **Guardar cambios**.

   Ahora, cuando registra horas en un proyecto, tarea o problema, los tipos de horas que seleccione están disponibles si esos mismos tipos de horas están disponibles en el nivel de proyecto.


## Cómo funcionan juntos los tipos de horas de nivel de usuario y de nivel de proyecto

En la siguiente lista se describen los tipos de horas que se muestran en un objeto después de personalizar y filtrar los tipos de horas en el nivel de usuario y en el nivel de proyecto:

* De forma predeterminada, cuando se abre un objeto para registrar el tiempo, en el menú desplegable Tipo de hora se muestran los tipos de hora predeterminados asociados al usuario. Esto sucede cuando no personalizó los tipos de horas.

* Después de personalizar los tipos de horas y definir los tipos de horas disponibles para el usuario o filtrar los tipos de horas para un proyecto, existen los siguientes escenarios:

   * Si seleccionó todos los tipos de horas para el campo Tipo de hora disponible en el perfil del usuario y los tipos de horas del proyecto no están filtrados, verá todos los tipos de horas disponibles cuando registre la hora.
   * Si seleccionó únicamente un subconjunto de tipos de horas para el campo Tipo de hora disponible en el perfil del usuario y los tipos de horas del proyecto no están filtrados, sólo verá los tipos de horas del usuario cuando registre la hora.
   * Si seleccionó todos los tipos de horas para el campo Tipo de hora disponible en el perfil del usuario y se filtran los tipos de horas del proyecto, solo verá los tipos de horas del proyecto y los tipos de horas predeterminados como Hora del proyecto, Hora de la tarea y Hora del problema según el objeto.
   * Si ha seleccionado solo un subconjunto de tipos de horas para el campo Tipo de hora disponible en el perfil del usuario y se filtran los tipos de horas del proyecto, solo verá los tipos de horas que son comunes al usuario y al proyecto. Si no hay tipos de horas comunes para el usuario y el proyecto, solo se muestran los tipos de horas predeterminados (Hora del proyecto, Hora de la tarea, Hora del problema).

>[!TIP]
>
>   Si selecciona un tipo de hora diferente al predeterminado para un objeto, el tipo de hora se vuelve fijo. La próxima vez que registre la hora en el mismo objeto, el Tipo de hora se establecerá de forma predeterminada en el que seleccionó por última vez.

