---
product-area: workfront-integrations;projects
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Crear una  [!DNL Adobe Workfront] tarea en Google Workspace mediante contenido de correo electrónico
description: Puede convertir un correo electrónico externo (no generado por Adobe [!DNL Workfront]) en una tarea de Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 38%

---

# Crear una tarea [!DNL Adobe Workfront] en [!DNL Google Workspace] mediante contenido de correo electrónico

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la siguiente funcionalidad de Workfront para Google Workspace no estará disponible después del **28 de febrero de 2026**:
>
>* Acceso a la funcionalidad de Google Workspace desde Workfront
>
>* Visualización y administración de tareas de Workfront desde Gmail o el panel de sitio Calendario de Google
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Google Workspace.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Google Workspace, consulte [Módulos de Gmail](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) y [Módulos de Google Calendar](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Puede convertir un correo electrónico externo (no generado por [!DNL Adobe Workfront]) en una tarea [!DNL Workfront].

También puede convertir un correo electrónico externo en una actualización de una tarea existente. Para obtener más información, consulte [Actualizar un elemento de  [!DNL Adobe Workfront]  desde  [!DNL Google Workspace]  mediante contenido de correo electrónico](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Para obtener información sobre cómo usar [!DNL Google Workspace] para trabajar con los correos electrónicos de notificación enviados por [!DNL Workfront], consulte [Administrar detalles de notificación de  [!DNL Adobe Workfront]  desde  [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

Para poder crear una tarea de [!DNL Workfront] en [!DNL Google Workspace], debe

* Instalar [!DNL Workfront for Google Workspace]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Crear una tarea [!DNL Adobe Workfront] en [!DNL Google Workspace] mediante contenido de correo electrónico

1. Si no se muestra el panel [!UICONTROL Workfront for Google Workspace], haga clic en el icono [!DNL Workfront] ![Workfront icon](assets/wf-lion-icon.png) en la barra lateral de complementos de [!DNL Google Workspace], en el extremo derecho de la página.
1. Con el mensaje de correo electrónico abierto en [!DNL Google Workspace], haga clic en una opción de [!DNL Workfront for Google Workspace] para convertir el correo electrónico en una nueva tarea de [!DNL Workfront].

1. Seleccione una opción **[!UICONTROL Crear nuevo]** para indicar si la tarea formará parte de un proyecto o de una tarea personal que sea independiente de un proyecto.
1. Si desea adjuntar la tarea a un proyecto principal, haga clic en **[!UICONTROL Nombre del proyecto]**, empiece a escribir el nombre del proyecto donde desea la tarea y, a continuación, haga clic en el nombre del proyecto cuando aparezca en la lista siguiente.
1. Realice cualquiera de estos cambios:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de tarea]</td> 
      <td>Edite cualquier parte de este texto, que se toma de la línea de asunto del correo electrónico.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Edite cualquier parte de este texto, que se toma del cuerpo del correo electrónico.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assign To]</td> 
      <td>Haga clic en <strong>[!UICONTROL Assign To]</strong>, luego en la opción <strong>[!UICONTROL Assign this to]</strong> que aparece y, a continuación, empiece a escribir el nombre de la persona y haga clic en él cuando aparezca en la lista siguiente. Repítalo para cada persona que desee añadir y, a continuación, haga clic en <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Duración planificada]</td> 
      <td> <p>Haga clic en <strong>[!UICONTROL Duración planificada]</strong> y, a continuación, escriba el número de días que desea que tarde la tarea. </p> <p>Nota: Esta opción se puede configurar para su organización de diferentes maneras. Por ejemplo, para su organización, es posible que tenga que escribir un número de horas en lugar de días. Si necesita más información, consulte con su administrador de [!DNL Workfront]. Si desea especificar un período de tiempo distinto del predeterminado configurado, escriba <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong> o <strong>mo</strong> después del número para indicar minutos, horas, días, semanas o meses.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Haga clic en la flecha desplegable y luego haga clic en la prioridad que desee para la tarea.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>(Solo está disponible si el correo electrónico contiene al menos un archivo adjunto). Haga clic en esta opción para guardar los archivos adjuntos en el correo electrónico en el área de [!UICONTROL Documents] de la tarea. </p> <p>Si no desea guardar un archivo adjunto, haga clic en la X situada a la derecha de su nombre. </p> <p>Si el correo electrónico contiene vínculos a documentos en [!DNL Google Drive], se guardan en la ficha [!UICONTROL Overview] de la tarea que está creando. </p> <p>Importante: Para que esto funcione, la persona con la función de administrador de [!DNL Workfront] debe autorizar a [!DNL Google Drive] para que trabaje con documentos de [!DNL Workfront], tal como se describe en la sección <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurar integraciones para administrar documentos</a> del artículo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurar integraciones de documentos</a>.</p> <p>Si activa esta opción, permanecerá habilitada para otros correos electrónicos que convierta a tareas, problemas y actualizaciones.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir archivo de correo electrónico]</td> 
      <td> <p>Haga clic en esta opción para guardar el correo electrónico original como un archivo de correo electrónico (EML) <span> en el área </span> de [!UICONTROL Documents] de la tarea. Desde allí, puede hacer doble clic en el archivo para abrir el correo electrónico en su aplicación de correo electrónico.</p> <p>Si activa esta opción, permanecerá habilitada para otros correos electrónicos que convierta a tareas, problemas y actualizaciones.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear tarea]**.

   La ficha **[!UICONTROL Detalles]** de la nueva tarea se muestra en el panel [!DNL Workfront for Google Workspace]. Puede hacer clic en **[!UICONTROL Actualizaciones]** y comenzar a comunicarse con los colaboradores de inmediato sin salir de su bandeja de entrada.

   En la parte inferior de la ficha **[!UICONTROL Detalles]**, también puede hacer clic en **[!UICONTROL Ver en[!DNL Workfront]]** para ir a la nueva tarea en Workfront.

   Al actualizar el explorador, un mensaje con un vínculo en la parte inferior del panel [!DNL Workfront for Google Workspace] confirma que ha convertido el correo electrónico en una tarea:

   Puede hacer clic en el vínculo para ir a la vista Detalles, en el panel [!DNL Workfront for Google Workspace], de la tarea que ha creado.

   Puede repetir estos pasos para convertir el mismo correo electrónico en varias tareas. Cuando actualice el explorador o vuelva al correo electrónico en otro momento, todos los vínculos que haya creado para el correo electrónico se mostrarán en la parte inferior del panel [!UICONTROL Workfront para Google Workspace].

1. (Opcional) Continúe trabajando con la tarea en el panel [!DNL Workfront for Google Workspace] realizando cualquiera de las siguientes acciones:

   * Para añadir una actualización en la ficha **[!UICONTROL Actualizaciones]**, haga clic en **[!UICONTROL Iniciar una nueva actualización]** y escriba la actualización.

   * Para responder a una actualización en la ficha **[!UICONTROL Actualizaciones]**, haga clic en **[!UICONTROL Responder]** y escriba la respuesta.

     Para ambas acciones, puede notificar a usuarios concretos su comentario. Haga clic en **[!UICONTROL Notificar]**, empiece a escribir el nombre de un usuario y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable. Repita este proceso para los demás usuarios a los que desee notificar y luego haga clic en **[!UICONTROL Publicar]**.

   * Haga clic en la ficha **[!UICONTROL Documentos]** para ver los documentos guardados con la tarea.

Puede repetir estos pasos para convertir el mismo correo electrónico en varias tareas. Cuando actualice el explorador o vuelva al correo electrónico en otro momento, todos los vínculos que haya creado para el correo electrónico se mostrarán en la parte inferior del panel [!DNL Workfront for Google Workspace].
