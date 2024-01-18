---
product-area: projects
navigation-topic: convert-issues
title: Conversión de un problema en un proyecto en Adobe Workfront
description: Conversión de un problema en un proyecto en Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 1%

---

# Conversión de un problema en un proyecto en Adobe Workfront

Si es necesario trabajar más para completar un problema después de enviarlo, puede convertir el problema en un proyecto.

Puede convertir un problema en un proyecto nuevo o convertirlo en un proyecto mediante una plantilla. Este artículo describe las dos maneras de convertir problemas en proyectos.

>[!IMPORTANT]
>
>Para obtener información general sobre la conversión de problemas, le recomendamos que lea también el artículo [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Al crear un proyecto a partir de un problema, algunos de los campos del proyecto se rellenan desde otros objetos. Para obtener más información, consulte la sección &quot;Nueva configuración predeterminada del proyecto&quot; en el artículo [Creación de un proyecto](../../../manage-work/projects/create-projects/create-project.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas, Tareas y Proyectos</p> <p>Editar el acceso a los datos financieros para actualizar la información financiera de una emisión convertida proyectada</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para el problema</p> <p>Puede obtener permisos de administración en el proyecto después de convertir el problema</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Convertir un problema en un proyecto

Puede convertir un problema en un proyecto en blanco o convertir un problema en un proyecto mediante una plantilla.

1. Vaya a un proyecto y haga clic en **[!UICONTROL Problemas]** en el panel izquierdo.
1. En la lista de problemas que se muestra, realice una de las siguientes acciones:

   * Para convertir un problema en un proyecto en blanco, haga clic en el nombre del problema y luego en el icono **[!UICONTROL Más]** menú ![](assets/more-icon.png) a la derecha del nombre del problema y haga clic en **[!UICONTROL Convertir en un proyecto en blanco]**.


     O

     Seleccione el problema en la lista de problemas y haga clic en **[!UICONTROL Más]** menú ![](assets/more-icon.png) en la parte superior de la lista, haga clic en **[!UICONTROL Convertir en un proyecto en blanco]**.

     >[!IMPORTANT]
     >
     >La opción Convertir en un proyecto en blanco solo se muestra cuando el administrador del sistema o del grupo ha habilitado la opción [!UICONTROL Permitir a los usuarios crear proyectos sin utilizar una plantilla] preferencia en la [!UICONTROL Configurar] área. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     Debe agregar manualmente tareas al proyecto o adjuntar una plantilla al proyecto después de convertir el problema.

     Continúe con el paso 3e siguiente.

     <!--
     Is this accurate?
     -->

     >[!TIP]
     >   
     >* Si el problema se creó mediante una cola de solicitudes, el nuevo proyecto heredará el grupo de la cola de solicitudes.
     >* Si el problema se creó agregándolo a la sección Problemas del proyecto, el nuevo proyecto heredará el grupo del proyecto del problema.

   * Para convertir un problema en un proyecto mediante una plantilla, realice una de las siguientes acciones:

      * Haga clic en el nombre de un problema y, a continuación, haga clic en [!UICONTROL **Más**] menú ![](assets/more-icon.png) a la derecha del nombre del problema

        O

      * Seleccione el problema en la lista de problemas, en un informe o panel, haga clic en **Más** menú ![](assets/more-icon.png) en la parte superior de la lista, haga clic en **Convertir a proyecto desde plantilla** y empiece a escribir el nombre de una plantilla en la **Plantilla de búsqueda** y, a continuación, haga clic en el nombre de la plantilla cuando se muestre en la lista. Continúe con el paso 3.

        <!--      
        (is this accurate?)      
        -->

     >[!TIP]
     >
     >Si ha agregado plantillas a la lista Favoritos, puede pasar el ratón sobre [!UICONTROL **Plantillas favoritas**] y haga clic en la plantilla que desee utilizar.

     Se muestra el cuadro Nuevo proyecto a partir de plantilla.

     ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

     >[!TIP]
     >
     >Si el problema está asociado a un proceso de aprobación o ya está asociado a un objeto de resolución, Workfront muestra una advertencia en la parte superior del cuadro Convertir en proyecto para notificarle que la aprobación se eliminará o que el objeto de resolución se sobrescribirá durante la conversión. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Condicional) Si ha seleccionado convertir el problema en un proyecto mediante una plantilla, continúe con los siguientes pasos:

   1. Revise los detalles de la plantilla a la derecha.

      Los detalles de la plantilla incluyen lo siguiente:

      * Duración de plantilla
      * Propietario de plantilla
      * Número de tareas de nivel superior que incluye los nombres de las tres tareas principales
      * Número de todas las tareas de la plantilla
      * Nombres de los formularios personalizados de plantilla

   1. (Opcional) Pase el ratón sobre el nombre de una plantilla y haga clic en el icono Favoritos ![](assets/favorites-icon-small.png) para marcarlo como favorito para uso futuro.

      >[!TIP]
      >
      >Puede tener hasta 40 elementos de Workfront marcados como favoritos. Esto incluye plantillas y otros elementos.

   1. Clic [!UICONTROL **Usar plantilla**] para seleccionar una plantilla.

      El [!UICONTROL Convertir a proyecto] se abre el cuadro.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. Si un campo ya se ha rellenado en la plantilla, el campo se rellena previamente en la [!UICONTROL Convertir a proyecto] cuadro. Puede editar los valores rellenados previamente para que coincidan mejor con su proyecto. Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* El administrador del sistema o del grupo puede agregar o quitar campos en la [!UICONTROL Convertir a proyecto, cuadro] al actualizar la información de Detalles del proyecto en su [!UICONTROL Plantilla de diseño].
      >
      >* Para actualizar campos en la [!UICONTROL Finanzas] de la sección [!UICONTROL Convertir a proyecto] caja que debe tener [!UICONTROL Editar] acceso a [!UICONTROL Datos financieros] en su nivel de acceso. Si tiene [!UICONTROL Ver] acceso a [!UICONTROL Datos financieros] en su nivel de acceso, toda la información financiera de la plantilla se transfiere al nuevo proyecto y no puede editarla mientras convierte el problema. Para obtener más información, consulte [Concesión de acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) y [Compartir una plantilla](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   1. (Opcional y condicional) Haga clic en [!UICONTROL **Opciones**] en el panel izquierdo, seleccione una de las opciones disponibles:

      * [!UICONTROL **Mantener el problema original y enlazar su solución al proyecto**]

        Si no se selecciona, se elimina el problema original.

        >[!NOTE]
        >
        >Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo vayan convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:
        >
        >* [Conceder acceso a los problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
        > 
        >* [Compartir un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

      * [!UICONTROL **Permitir que (nombre de usuario) tenga acceso a este proyecto**]

        Si no se selecciona, el problema es [!UICONTROL Contacto principal] no tiene acceso a la nueva tarea.

        >[!NOTE]
        >
        >Las opciones disponibles aquí dependen de cómo las haya configurado el administrador de Workfront para todos los miembros del sistema o para su grupo. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
        >
        >
        >O bien, si los grupos de nivel superior de su organización los configuraron por separado, las opciones disponibles aquí dependen del grupo seleccionado para el nuevo proyecto en el paso 6. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Clic [!UICONTROL **Forms personalizado**] y realice una de las acciones siguientes:

      * Revise los formularios personalizados adjuntos a la plantilla. Se transferirán al nuevo proyecto.
      * Asegúrese de que todos los campos obligatorios tengan información válida.
      * Reorganizar los formularios personalizados arrastrándolos ![](assets/drag-object-icon.png) donde los quieras.
      * Haga clic en **x** a la derecha de cualquier formulario que no desee transferir al proyecto.
      * Si es necesario, transfiera la información del formulario personalizado del problema al proyecto.

        >[!TIP]
        >
        >* Si un formulario personalizado de varios objetos adjunto al problema está configurado para usarse tanto con problemas como con proyectos, toda la información guardada en el formulario se conservará cuando realice la conversión si los campos existen tanto en el problema como en los formularios personalizados del proyecto.
        >* Si se adjunta un formulario personalizado de varios objetos con un campo calculado al problema y al proyecto, el problema y el proyecto deben ser compatibles con todos los campos a los que se hace referencia en los campos personalizados calculados del formulario. Si se produce una incompatibilidad, un mensaje le advierte de que realice los ajustes necesarios. Para obtener más información, consulte la sección &quot;Campos personalizados calculados en formularios personalizados de varios objetos&quot; en la [Agregar datos calculados a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
        >* Si utiliza una plantilla para la conversión y un formulario personalizado adjunto a la plantilla contiene un campo personalizado que también se encuentra en un formulario personalizado adjunto al problema, el valor del campo del problema se utiliza para el nuevo proyecto. Sin embargo, si el campo personalizado está en blanco sobre el problema, se utiliza el valor de la plantilla.

   1. Clic [!UICONTROL **Convertir a proyecto**].

      >[!TIP]
      >
      >Si ha decidido eliminar el problema original, este pasará a ser un proyecto.
      >   
      >O
      >  
      >Si ha decidido conservar el problema original, ahora el problema está vinculado al nuevo proyecto y se completará cuando se complete el proyecto.
      >
      >Algunos campos de problema se transfieren al proyecto. La mayoría de los campos definidos en la plantilla se transfieren automáticamente al proyecto recién creado si no los ha cambiado en los pasos anteriores. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Opcional) Defina cualquier detalle adicional del proyecto (propietario del proyecto, fechas del proyecto) y las tareas según sea necesario.
1. Clic [!UICONTROL **Convertir a proyecto**].

   El problema ahora se convierte en un proyecto.

1. Clic [!UICONTROL **Ir al proyecto**] dentro de [!UICONTROL Correcto] notificación en la esquina superior derecha de la página. Esto abre la página del proyecto.
