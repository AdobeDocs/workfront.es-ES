---
product-area: projects
navigation-topic: convert-issues
title: Conversión de un problema en un proyecto en Adobe Workfront
description: Conversión de un problema en un proyecto en Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1980'
ht-degree: 1%

---

# Conversión de un problema en un proyecto en Adobe Workfront

<!--Audited: 01/2024-->

Si es necesario trabajar más para completar un problema después de enviarlo, puede convertir el problema en un proyecto.

Puede convertir un problema en un proyecto nuevo o convertirlo en un proyecto mediante una plantilla. Este artículo describe las dos maneras de convertir problemas en proyectos.

>[!IMPORTANT]
>
>Para obtener información general acerca de la conversión de problemas, le recomendamos que lea también el artículo [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Al crear un proyecto a partir de un problema, algunos de los campos del proyecto se rellenan desde otros objetos. Para obtener más información, consulte la sección &quot;Nueva configuración predeterminada de proyecto&quot; en el artículo [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar </p> 
    <p>Actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas, Tareas y Proyectos</p> <p>Editar el acceso a los datos financieros para actualizar la información financiera de una emisión convertida proyectada</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para el problema</p> <p>Puede obtener permisos de administración en el proyecto después de convertir el problema</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Convertir un problema en un proyecto

Puede convertir un problema en un proyecto en blanco.

1. Vaya a un proyecto y haga clic en **[!UICONTROL Problemas]** en el panel izquierdo.
1. En la lista de problemas que se muestra, realice una de las siguientes acciones:

   * Para convertir un problema en un proyecto en blanco, haga clic en el nombre del problema, haga clic en el menú **[!UICONTROL Más]** ![](assets/more-icon.png) a la derecha del nombre del problema y, a continuación, haga clic en **[!UICONTROL Convertir en proyecto en blanco]**.


     O

     Seleccione el problema en la lista de problemas, haga clic en el menú **[!UICONTROL Más]** ![](assets/more-icon.png) en la parte superior de la lista y, a continuación, haga clic en **[!UICONTROL Convertir en proyecto en blanco]**.

     >[!IMPORTANT]
     >
     >La opción Convertir en un proyecto en blanco solo se muestra cuando el administrador del sistema o del grupo habilitó la preferencia [!UICONTROL Permitir que los usuarios creen proyectos sin usar una plantilla] en el área [!UICONTROL Configuración]. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     Debe agregar manualmente tareas al proyecto o adjuntar una plantilla al proyecto después de convertir el problema.

     >[!TIP]
     >   
     >* Si el problema se creó mediante una cola de solicitudes, el nuevo proyecto heredará el grupo de la cola de solicitudes.
     >* Si el problema se creó agregándolo a la sección Problemas del proyecto, el nuevo proyecto heredará el grupo del proyecto del problema.

     >[!TIP]
     >
     >Si el problema está asociado a un proceso de aprobación o ya está asociado a un objeto de resolución, Workfront muestra una advertencia en la parte superior del cuadro Convertir en proyecto para notificarle que la aprobación se eliminará o que el objeto de resolución se sobrescribirá durante la conversión. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Opcional y condicional) Haga clic en [!UICONTROL **Opciones**] en el panel izquierdo y, a continuación, seleccione una de las opciones disponibles:

   * [!UICONTROL **Mantener el problema original y enlazar su solución al proyecto**]

     Si no se selecciona, se elimina el problema original.

     >[!NOTE]
     >
     >Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo vayan convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:
     >
     >* [Conceder acceso a problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Compartir un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Permitir que (Nombre de usuario) tenga acceso a este proyecto**]

     Si no se selecciona, el [!UICONTROL contacto principal] del problema no tendrá acceso a la nueva tarea.

     >[!NOTE]
     >
     >Las opciones disponibles aquí dependen de cómo las haya configurado el administrador de Workfront para todos los miembros del sistema o para su grupo. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >O bien, si los grupos de nivel superior de su organización los configuraron por separado, las opciones disponibles aquí dependen del grupo seleccionado para el nuevo proyecto en el paso 6. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. Haga clic en [!UICONTROL **Forms personalizado**] y realice una de las acciones siguientes:

   * Revise los formularios personalizados adjuntos al problema. Se transferirán al nuevo proyecto si también son formularios personalizados de proyecto.
   * Agregar más formularios personalizados
   * Asegúrese de que todos los campos obligatorios tengan información válida.
   * Reorganice los formularios personalizados arrastrándolos ![](assets/drag-object-icon.png) a donde desee.
   * Haga clic en el icono **x** a la derecha de cualquier formulario que no desee transferir al proyecto. Esto quita el formulario del proyecto.
   * Si es necesario, transfiera la información del formulario personalizado del problema al proyecto.

     >[!TIP]
     >
     >* Si un formulario personalizado de varios objetos adjunto al problema está configurado para usarse tanto con problemas como con proyectos, toda la información guardada en el formulario se conservará cuando realice la conversión si los campos existen tanto en el problema como en los formularios personalizados del proyecto.
     >* Si se adjunta un formulario personalizado de varios objetos con un campo calculado al problema y al proyecto, el problema y el proyecto deben ser compatibles con todos los campos a los que se hace referencia en los campos personalizados calculados del formulario. Si se produce una incompatibilidad, un mensaje le advierte de que realice los ajustes necesarios. Para obtener más información, consulte la sección &quot;Campos personalizados calculados en formularios personalizados de varios objetos&quot; en [Agregar datos calculados a un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

1. Haga clic en [!UICONTROL **Convertir en proyecto**].

   >[!TIP]
   >
   >Si ha decidido eliminar el problema original, este pasará a ser un proyecto.
   >   
   >O
   >  
   >Si ha decidido conservar el problema original, ahora el problema está vinculado al nuevo proyecto y se completará cuando se complete el proyecto.
   >
   >La información de algunos campos de problema se transfiere al proyecto si no se ha modificado durante la conversión.

1. (Opcional) Defina cualquier detalle adicional del proyecto (propietario del proyecto, fechas del proyecto) y las tareas según sea necesario.
1. Haga clic en [!UICONTROL **Convertir en proyecto**].

   El problema ahora se convierte en un proyecto. Se muestra la página del proyecto.

## Conversión de un problema en un proyecto mediante una plantilla

Puede convertir un problema en un proyecto mediante una plantilla.

1. Vaya a un proyecto y haga clic en **[!UICONTROL Problemas]** en el panel izquierdo.
1. En la lista de problemas que se muestra, haga clic en el nombre del problema, haga clic en el menú **[!UICONTROL Más]** ![](assets/more-icon.png) a la derecha del nombre del problema, luego haga clic en **Convertir en proyecto a partir de plantilla** y empiece a escribir el nombre de una plantilla en el cuadro **Buscar plantilla**; a continuación, haga clic en el nombre de la plantilla cuando se muestre en la lista. Continúe con el paso 3.

   >[!TIP]
   >
   >Si agregaste plantillas a tu lista Favoritos, puedes pasar el ratón sobre el menú [!UICONTROL **Plantillas favoritas**] y hacer clic en la plantilla que quieras usar.

   Se muestra el cuadro Nuevo proyecto a partir de plantilla.

   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* Si el problema está asociado a un proceso de aprobación o ya está asociado a un objeto de resolución, Workfront muestra una advertencia en la parte superior del cuadro Convertir en proyecto para notificarle que la aprobación se eliminará o que el objeto de resolución se sobrescribirá durante la conversión. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).
   >   
   >* Si el problema se creó mediante una cola de solicitudes, el nuevo proyecto heredará el grupo de la cola de solicitudes.
   >* Si el problema se creó agregándolo a la sección Problemas del proyecto, el nuevo proyecto heredará el grupo del proyecto del problema.

1. Revise los detalles de la plantilla a la derecha.

   Los detalles de la plantilla incluyen lo siguiente:

   * Duración de plantilla
   * Propietario de plantilla
   * Número de tareas de nivel superior que incluye los nombres de las tres tareas principales
   * Número de todas las tareas de la plantilla
   * Nombres de los formularios personalizados de plantilla

1. (Opcional) Pase el cursor sobre el nombre de una plantilla y haga clic en el icono **Favoritos** ![](assets/favorites-icon-small.png) para marcarla como favorita para uso futuro.

   >[!TIP]
   >
   >Puede tener hasta 40 elementos de Workfront marcados como favoritos. Esto incluye plantillas y otros elementos.

1. Haga clic en [!UICONTROL **Usar plantilla**] para seleccionar una plantilla.

   Se abre el cuadro [!UICONTROL Convertir en proyecto].

   ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. Si un campo ya se ha rellenado en la plantilla, ya se ha rellenado previamente en el cuadro [!UICONTROL Convertir en proyecto]. Puede editar los valores rellenados previamente para que coincidan mejor con su proyecto. Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!TIP]
   >
   >* El administrador del sistema o del grupo puede agregar o quitar campos en el [!UICONTROL cuadro Convertir en proyecto] al actualizar la información de detalles del proyecto en su [!UICONTROL plantilla de diseño].
   >
   >* Para actualizar los campos de la sección [!UICONTROL Finanzas] en el cuadro [!UICONTROL Convertir en proyecto], debe tener acceso de [!UICONTROL Editar] a [!UICONTROL Datos financieros] en su nivel de acceso. Si tiene acceso de [!UICONTROL Ver] a [!UICONTROL Datos financieros] en su nivel de acceso, toda la información financiera de la plantilla se transfiere al nuevo proyecto y no puede editarla mientras convierte el problema. Para obtener más información, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) y [Compartir una plantilla](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Opcional y condicional) Haga clic en [!UICONTROL **Opciones**] en el panel izquierdo y, a continuación, seleccione una de las opciones disponibles:

   * [!UICONTROL **Mantener el problema original y enlazar su solución al proyecto**]

     Si no se selecciona, se elimina el problema original.

     >[!NOTE]
     >
     >Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo vayan convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:
     >
     >* [Conceder acceso a problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Compartir un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Permitir que (Nombre de usuario) tenga acceso a este proyecto**]

     Si no se selecciona, el [!UICONTROL contacto principal] del problema no tendrá acceso a la nueva tarea.

     >[!NOTE]
     >
     >Las opciones disponibles aquí dependen de cómo las haya configurado el administrador de Workfront para todos los miembros del sistema o para su grupo. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >O bien, si los grupos de nivel superior de su organización los configuraron por separado, las opciones disponibles aquí dependen del grupo seleccionado para el nuevo proyecto en el paso 6. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Haga clic en [!UICONTROL **Forms personalizado**] y realice una de las acciones siguientes:

      * Revise los formularios personalizados adjuntos a la plantilla. Se transferirán al nuevo proyecto.
      * Revise los formularios personalizados adjuntos al problema. Se transferirán al proyecto si también son formularios de proyecto.
      * Asegúrese de que todos los campos obligatorios tengan información válida.
      * Reorganice los formularios personalizados arrastrándolos ![](assets/drag-object-icon.png) a donde desee.
      * Haga clic en el icono **x** a la derecha de cualquier formulario que no desee transferir al proyecto.
      * Si es necesario, transfiera la información del formulario personalizado del problema al proyecto.

        >[!TIP]
        >
        >* Si un formulario personalizado de varios objetos adjunto al problema está configurado para usarse tanto con problemas como con proyectos, toda la información guardada en el formulario se conservará cuando realice la conversión si los campos existen tanto en el problema como en los formularios personalizados del proyecto.
        >* Si se adjunta un formulario personalizado de varios objetos con un campo calculado al problema y al proyecto, el problema y el proyecto deben ser compatibles con todos los campos a los que se hace referencia en los campos personalizados calculados del formulario. Si se produce una incompatibilidad, un mensaje le advierte de que realice los ajustes necesarios. Para obtener más información, consulte la sección &quot;Campos personalizados calculados en formularios personalizados de varios objetos&quot; en [Agregar datos calculados a un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
        >* Si un formulario personalizado adjunto a la plantilla contiene un campo personalizado que también se encuentra en un formulario personalizado adjunto al problema, el valor de campo del problema se utiliza para el nuevo proyecto. Sin embargo, si el campo personalizado está en blanco sobre el problema, se utiliza el valor de la plantilla.

1. (Opcional) Defina cualquier detalle adicional del proyecto (propietario del proyecto, fechas del proyecto) y las tareas según sea necesario.

   1. Haga clic en [!UICONTROL **Convertir en proyecto**].

      >[!TIP]
      >
      >Si ha decidido eliminar el problema original, este pasará a ser un proyecto.
      >   
      >O
      >  
      >Si ha decidido conservar el problema original, ahora el problema está vinculado al nuevo proyecto y se completará cuando se complete el proyecto.
      >
      >Algunos campos de problema se transfieren al proyecto. La mayoría de los campos definidos en la plantilla se transfieren automáticamente al proyecto recién creado si no los ha cambiado en los pasos anteriores. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   El problema ahora se convierte en un proyecto. Se muestra la página del proyecto.