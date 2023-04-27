---
product-area: projects
navigation-topic: convert-issues
title: Convertir un problema en un proyecto en Adobe Workfront
description: Convertir un problema en un proyecto en Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: 61a107e1ee8a415fd94e73fc65fa5f59f7de02d1
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 0%

---

# Convertir un problema en un proyecto en Adobe Workfront

Si es necesario trabajar más para completar un problema después de que se envíe el problema, puede convertir el problema en un proyecto.

Puede convertir un problema en un nuevo proyecto o convertirlo en un proyecto mediante una plantilla. Este artículo describe ambos modos de convertir problemas a proyectos.

Para obtener información general sobre la conversión de problemas, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Al crear un proyecto a partir de un problema, algunos de los campos del proyecto se rellenan con otros objetos. Para obtener más información, consulte la sección &quot;Nueva configuración predeterminada del proyecto&quot; en el artículo [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas, Tareas y Proyectos</p> <p>Editar el acceso a los datos financieros para actualizar la información financiera para una conversión proyectada a partir de la emisión</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para el problema</p> <p>Obtenga permisos de administración para el proyecto después de convertir el problema</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Convertir un problema en un proyecto

Puede convertir un problema en un proyecto en blanco o convertir un problema en un proyecto mediante una plantilla.

1. Vaya a un proyecto y haga clic en **[!UICONTROL Problemas]** en el panel izquierdo.
1. En la lista de problemas que se muestra, realice una de las siguientes acciones:

   * Para convertir un problema en un proyecto en blanco, haga clic en el nombre del problema y haga clic en el botón **[!UICONTROL Más]** menú ![](assets/more-icon.png) a la derecha del nombre del problema y haga clic en **[!UICONTROL Convertir en un proyecto en blanco]**.


      O

      Seleccione el problema en la lista de problemas y haga clic en el botón **[!UICONTROL Más]** menú ![](assets/more-icon.png) en la parte superior de la lista, haga clic en **[!UICONTROL Convertir en un proyecto en blanco]**.

      >[!IMPORTANT]
      >
      >La opción Convertir en un proyecto en blanco solo se muestra cuando el administrador del sistema o del grupo habilitó el [!UICONTROL Permitir que los usuarios creen proyectos sin usar una plantilla] en la variable [!UICONTROL Configuración] . Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


      Debe añadir manualmente tareas al proyecto o adjuntar una plantilla al proyecto después de convertir el problema.

      Continúe con el paso 3e siguiente.

      <!--
     Is this accurate?
     -->

      >[!TIP]
      >   
      >* Si el problema se creó con una cola de solicitudes, el nuevo proyecto hereda el grupo de la cola de solicitudes.
      >* Si el problema se creó añadiéndolo a la sección Problemas del proyecto, el nuevo proyecto hereda el proyecto del Grupo del problema.


   * Para convertir un problema en un proyecto mediante una plantilla, realice una de las siguientes acciones:

      * Haga clic en el nombre de un problema y, a continuación, haga clic en el [!UICONTROL **Más**] menú ![](assets/more-icon.png) a la derecha del nombre de la emisión

         ![](assets/issue-more-menu-expanded-with-convert-to-project-options-nwe-350x213.png)

         O

      * Seleccione el problema en la lista de problemas, en un informe o panel, haga clic en el botón **Más** menú ![](assets/more-icon.png) en la parte superior de la lista, haga clic en **Convertir en proyecto desde plantilla** y empiece a escribir el nombre de una plantilla en la **Plantilla de búsqueda** y, a continuación, haga clic en el nombre de la plantilla cuando aparezca en la lista. Continúe con el paso 3.

         <!--      
        (is this accurate?)      
        -->
      >[!TIP]
      >
      >Si ha agregado plantillas a la lista Favoritos, puede pasar el ratón sobre la [!UICONTROL **Plantillas favoritas**] y haga clic en la plantilla que desee utilizar.

      Se muestra el cuadro Nuevo proyecto de plantilla .

      ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

      >[!TIP]
      >
      >Si el problema está asociado a un proceso de aprobación o ya está asociado a un objeto de resolución, Workfront muestra una advertencia en la parte superior del cuadro Convertir a proyecto para notificarle que la aprobación se eliminará o que el objeto de resolución se sobrescribirá durante la conversión. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).


1. (Condicional) Si seleccionó convertir el problema en un proyecto mediante una plantilla, siga con los siguientes pasos:

   1. Revise los detalles de la plantilla a la derecha.

      Los detalles de la plantilla incluyen lo siguiente:

      * Duración de la plantilla
      * Propietario de la plantilla
      * El número de tareas de nivel superior que incluye los nombres de las tres tareas principales
      * El número de todas las tareas de la plantilla
      * Los nombres de los formularios personalizados de plantilla
   1. (Opcional) Pase el cursor sobre el nombre de una plantilla y haga clic en el icono Favoritos . ![](assets/favorites-icon-small.png) para marcarla como favorita para uso futuro.

      >[!TIP]
      >
      >Puede tener hasta 40 elementos de Workfront marcados como favoritos. Esto incluye plantillas y otros elementos.

   1. Haga clic en [!UICONTROL **Usar plantilla**] para seleccionar una plantilla.

      La variable [!UICONTROL Convertir en proyecto] se abre.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. Si un campo ya está rellenado en la plantilla, el campo se rellena previamente en la variable [!UICONTROL Convertir en proyecto] en la ventana Puede editar los valores rellenados previamente para que coincidan mejor con el proyecto. Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* El administrador del sistema o del grupo puede agregar o quitar campos en la variable [!UICONTROL Cuadro Convertir en proyecto] actualizando la información de Detalles del proyecto en su [!UICONTROL Plantilla de diseño].
      >
      >* Para actualizar campos en la variable [!UICONTROL Finanzas] en la sección [!UICONTROL Convertir en proyecto] que debe tener [!UICONTROL Editar] acceso a [!UICONTROL Datos financieros] en su nivel de acceso. Si tiene [!UICONTROL Ver] acceso a [!UICONTROL Datos financieros] en el nivel de acceso, toda la información financiera de la plantilla se transfiere al nuevo proyecto y no puede editarse mientras convierte el problema. Para obtener más información, consulte [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) y [Compartir una plantilla](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).


   1. (Opcional y condicional) Haga clic en [!UICONTROL **Opciones**] en el panel izquierdo, seleccione entre las opciones disponibles:

      * [!UICONTROL **Mantener el problema original y enlazar su resolución con este proyecto**]

         Cuando se anula la selección, se elimina el problema original.

         >[!NOTE]
         >
         >Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo estén convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:
         >
         >* [Concesión de acceso a problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
         > 
         >* [Compartir un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


      * [!UICONTROL **Permitir (nombre de usuario) tener acceso a este proyecto**]

         Si no se selecciona, el problema es [!UICONTROL Contacto principal] no tiene acceso a la nueva tarea.

         >[!NOTE]
         >
         >Las opciones disponibles dependen de cómo las haya configurado el administrador de Workfront para todos los miembros del sistema o para su grupo. Para obtener más información, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
         >
         >
         >O bien, si los grupos de nivel superior de su organización los configuran por separado, las opciones disponibles aquí dependen del grupo que haya seleccionado para el nuevo proyecto en el paso 6. Para obtener más información, consulte [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).
   1. Haga clic en [!UICONTROL **Forms personalizado**] y realice cualquiera de las siguientes acciones:

      * Revise los formularios personalizados adjuntos a la plantilla. Se transferirán al nuevo proyecto.
      * Asegúrese de que todos los campos obligatorios tengan información válida.
      * Reorganizar los formularios personalizados arrastrándolos ![](assets/drag-object-icon.png) donde los quieres.
      * Haga clic en el **x** a la derecha de cualquier formulario que no desee transferir al proyecto.
      * Si es necesario, transfiera información de formulario personalizada del problema al proyecto.

         >[!TIP]
         >
         >* Si un formulario personalizado de varios objetos adjunto al problema está configurado para su uso con problemas y proyectos, toda la información guardada en el formulario se conserva cuando realiza la conversión si los campos existen tanto en el problema como en los formularios personalizados del proyecto.
         >* Si se adjunta un formulario personalizado de varios objetos con un campo calculado al problema, así como al proyecto, el problema y el proyecto deben ser compatibles con todos los campos a los que se hace referencia en los campos personalizados calculados del formulario. Si hay una incompatibilidad, un mensaje le alerta para que realice ajustes. Para obtener más información, consulte la sección &quot;Campos personalizados calculados en formularios personalizados de varios objetos&quot; en la sección [Agregar datos calculados a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
         >* Si utiliza una plantilla para la conversión y un formulario personalizado adjunto a la plantilla contiene un campo personalizado que también se encuentra en un formulario personalizado adjunto al problema, el valor del campo del problema se utiliza para el nuevo proyecto. Sin embargo, si el campo personalizado está vacío en el problema, se utiliza el valor de la plantilla.

   1. Haga clic en [!UICONTROL **Convertir en proyecto**].

      >[!TIP]
      >
      >Si ha decidido eliminar el problema original, el problema ahora es un proyecto.
      >   
      >O
      >  
      >Si ha decidido mantener el problema original, el problema ahora está vinculado al nuevo proyecto y se completará cuando el proyecto finalice.
      >
      >Algunos campos de problema se transfieren al proyecto. La mayoría de los campos definidos en la plantilla se transfieren automáticamente al proyecto recién creado si no los ha cambiado en pasos anteriores. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).




1. (Opcional) Configure cualquier otro detalle del proyecto &#x200B; (propietario del proyecto, fechas del proyecto) y tareas según sea necesario.
1. Haga clic en [!UICONTROL **Convertir en proyecto**].

   El problema se ha convertido en un proyecto.

1. Haga clic en [!UICONTROL **Ir al proyecto**] dentro del [!UICONTROL Correcto] en la esquina superior derecha de la página. Se abre la página del proyecto.
