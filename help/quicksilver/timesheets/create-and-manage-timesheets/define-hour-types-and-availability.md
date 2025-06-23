---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definir tipos de horas y disponibilidad
description: Un tipo de hora es una etiqueta que le permite categorizar la entrada de una hora. Según los requisitos de informes de su organización en cuanto a horas, esto puede ser una parte esencial de la hora de registro.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 49%

---

# Definición de tipos de horas y disponibilidad

<!--Audited: 6/2025-->

Un tipo de hora es una etiqueta que le permite categorizar la entrada de una hora. Según los requisitos de informes por horas de su organización, esto puede ser una parte esencial del tiempo de registro.

Hay 2 conjuntos de tipos de horas en Adobe Workfront:

* **Horas generales**: Horas que no están asociadas con un proyecto, como tiempo de enfermedad o administración. Solo puede registrar horas generales en la hoja de horas.
* **Horas específicas del proyecto**: Horas registradas en proyectos, tareas y problemas. Puede registrar horas específicas del proyecto desde cualquier ubicación en la que pueda registrar horas.

Al registrar las horas en Workfront, los tipos de horas específicos del proyecto que están disponibles dependen de las opciones de configuración establecidas en los niveles de sistema, de proyecto y de usuario. (Los siguientes tipos de horas predeterminados específicos del proyecto siempre están disponibles: Hora del proyecto, Hora de la tarea y Hora del problema).

Los tipos de horas que hay disponibles para seleccionar al registrar las horas (en proyectos, tareas y problemas) vienen determinados primero por los tipos de horas que el administrador del sistema hubiese puesto disponibles en todo sistema y, a continuación, por los tipos de horas seleccionados en los niveles de proyecto y de usuario.

Una vez configurados los tipos de horas adecuados, puede registrar el tiempo desde varias ubicaciones en Workfront. Para obtener más información, consulte [Registrar tiempo](../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar</p> 
   <p>Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de administrador del sistema para definir tipos de horas de todo el sistema y editar todos los usuarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administrar el acceso al proyecto para definir los tipos de horas de un proyecto</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Definir la disponibilidad en el nivel del sistema

El administrador del sistema determina qué tipos de horas específicos de proyecto están disponibles en todo el sistema. Para obtener más información, consulte [Administrar tipos de hora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definir la disponibilidad en el nivel de proyecto {#define-availability-at-the-project-level}

El propietario del proyecto determina si todos los tipos de horas definidos en el sistema están disponibles en el proyecto (y las tareas y problemas dentro del proyecto) o si solo está disponible un subconjunto de esos tipos de horas.

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione el proyecto para el que desea determinar la disponibilidad de los tipos de horas.
1. Haga clic en el icono **Más** ![Más icono](assets/more-icon.png) junto al nombre del proyecto en el encabezado y, a continuación, haga clic en **Editar**. Se abre el panel **Editar proyecto**.

1. En la sección **Configuración del proyecto**, busque la configuración **Filtrar tipos de horas**.

1. Seleccione **No** para que todos los tipos de horas específicas del proyecto estén disponibles en el proyecto.

   O

   Seleccione **Sí** para que solo un subconjunto de los tipos de horas específicas del proyecto esté disponible en el proyecto y, a continuación, seleccione los **tipos de horas** que desee poner a disposición. Puede seleccionar varios tipos de horas.

   >[!NOTE]
   >
   >   Tenga en cuenta lo siguiente:
   >   
   >   * Si selecciona **Sí**, solo estarán disponibles los tipos de horas que seleccione al registrar horas en el proyecto (o en tareas y problemas dentro del proyecto).
   >   
   >   * Si selecciona **Yes** y no selecciona ningún tipo de hora, el proyecto solo mostrará los tipos de horas generales.
   >
   >   * Las mismas selecciones deben realizarse en el nivel de usuario individual para que el usuario pueda ver estas opciones de tipo de hora en el proyecto.
   >
   >   * Cuando coinciden el tipo de hora predeterminado del usuario y un tipo de hora filtrado del proyecto, ese tipo de hora se selecciona de forma predeterminada al registrar el tiempo.

1. Haga clic en **Guardar**.

## Definir disponibilidad en el nivel de usuario

Puede registrar horas para un tipo de hora determinado en proyectos, tareas y problemas solo si ese tipo de hora está disponible en los niveles del sistema, del proyecto y del usuario.

Si hace que un tipo de hora esté disponible en el nivel de usuario como se describe en esta sección, pero no ve ese tipo de hora al registrar la hora en un proyecto, tarea o problema, ese tipo de hora no está disponible en el proyecto. Para obtener más información, vea la siguiente sección de este artículo: [Definir disponibilidad en el nivel de proyecto](#define-availability-at-the-project-level).

Para definir los tipos de horas disponibles para un usuario:

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en el avatar del usuario en la esquina superior izquierda.

   O

   Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/adobe-main-menu.png) en la esquina superior derecha, si está disponible, y luego haga clic en **Perfil de Workfront**.

1. Haga clic en el icono **Más** ![Más icono](assets/more-icon.png) junto al nombre de usuario y, a continuación, haga clic en **Editar**. Se abre el cuadro **Editar persona**.

   >[!IMPORTANT]
   >
   >Solo una persona con la función de administrador del sistema puede editar a otros usuarios. Si tiene una licencia Plan, puede editar los tipos de horas en su propio perfil.


1. En la sección **Planificación de recursos**, en el menú desplegable **Tipos de horas disponibles**, realice una de las acciones siguientes, en función de los tipos de horas que desee poner a disposición al registrar tiempo en un proyecto, tarea o problema:

   * **Para que todos los tipos de horas estén disponibles para el usuario:** seleccione todos los tipos de horas.\
     Si deja todos los tipos de horas sin seleccionar, técnicamente es lo mismo que seleccionarlos todos. Sin embargo, en este caso, todos los tipos de horas están disponibles para el usuario solo en proyectos, tareas y problemas donde se ha seleccionado **No** en la opción **Filtrar tipos de horas** al editar el proyecto, como se describe en [Definir la disponibilidad en el nivel de proyecto](#define-availability-at-the-project-level).
   * **Para que solo un subconjunto de los tipos de horas esté disponible para el usuario:** seleccione solo los tipos de horas que desee poner a disposición.

     Para que los tipos de horas que seleccione en el nivel de usuario estén disponibles en proyectos, tareas y problemas, estos mismos tipos de horas también deben haberse seleccionado en la opción **Filtrar tipos de horas** al editar el proyecto, como se describe en [Definir la disponibilidad en el nivel de proyecto](#define-availability-at-the-project-level).

1. (Opcional) En el menú desplegable **Tipo de hora predeterminado**, seleccione un tipo de hora. Cuando coinciden el tipo de hora predeterminado del usuario y un tipo de hora filtrado del proyecto, ese tipo de hora se selecciona de forma predeterminada al registrar la hora.

1. Haga clic en **Guardar cambios**. Ahora, cuando registra horas en un proyecto, tarea o problema, los tipos de horas que seleccione están disponibles si esos mismos tipos de horas están disponibles en el nivel de proyecto.

## Cómo funcionan juntos los tipos de horas de nivel de usuario y de nivel de proyecto

En la siguiente lista se describen los tipos de horas que se muestran en un objeto después de haber personalizado y filtrado los tipos de horas del nivel de usuario y del nivel de proyecto al registrar tiempo en el objeto:

* Después de personalizar el tipo de hora predeterminado para el usuario y los tipos de horas de proyecto filtrados, el menú desplegable tipo de hora muestra uno de los siguientes tipos de horas:

   * Cuando el usuario tiene un tipo de hora predeterminado en su perfil y el proyecto tiene el mismo tipo de hora filtrado, este tipo de hora se muestra como el valor predeterminado seleccionado al registrar tiempo; el tiempo del proyecto, tarea o problema se muestran como opciones adicionales.

   * Cuando el usuario no tiene un tipo de hora predeterminado y el proyecto tiene tipos de horas filtrados, el tipo de hora predeterminado al registrar el tiempo es el proyecto, la tarea o el tiempo del problema, pero los tipos de horas filtrados del proyecto también se muestran como opciones adicionales.

   * Cuando el usuario no tiene un tipo de hora predeterminado y el proyecto no tiene tipos de horas filtrados, solo los tipos de horas de proyecto, tarea o problema se muestran como predeterminados según el objeto en el que esté registrando el tiempo.

   * Cuando el usuario tiene un tipo de hora predeterminado y el proyecto no tiene tipos de horas filtrados, el proyecto, la tarea o el tiempo del problema se muestran como predeterminados al registrar el tiempo en los objetos y no hay otros tipos de horas disponibles como opciones, incluido el tipo de hora predeterminado del usuario.

* Después de personalizar los tipos de horas y definir los tipos de horas disponibles para el usuario o filtrar los tipos de horas para un proyecto, se dan los siguientes escenarios:

   * Cuando seleccionó todos los tipos de horas para el campo Tipo de hora disponible en el perfil del usuario y los Tipos de horas del proyecto no se filtran, verá todos los tipos de horas disponibles cuando registre las horas.
   * Cuando seleccionó únicamente un subconjunto de tipos de horas para el campo Tipo de hora disponible en el perfil del usuario y los tipos de horas del proyecto no se filtran, solo verá los tipos de horas del usuario cuando registre el tiempo.
   * Cuando seleccionó todos los tipos de horas para el campo Tipo de hora disponible en el perfil del usuario y se filtran los tipos de horas del proyecto, solo verá los tipos de horas del proyecto y los tipos de horas predeterminados como Hora del proyecto, Hora de la tarea y Hora del problema según el objeto.
   * Cuando seleccionó únicamente un subconjunto de tipos de horas para el campo Tipo de hora disponible en el perfil del usuario y se filtran los tipos de horas del proyecto, solo verá los tipos de horas que son comunes al usuario y al proyecto. Si no hay tipos de horas comunes para el usuario y el proyecto, solo se mostrarán los tipos de horas predeterminados (Tiempo del proyecto, Tiempo de la tarea, Tiempo del problema).

>[!TIP]
>
>   Si selecciona un tipo de hora distinto del predeterminado para un objeto, el tipo de hora se vuelve fijo. La próxima vez que registre tiempo en el mismo objeto, el tipo de hora se establecerá de forma predeterminada en el que se haya seleccionado por última vez.

