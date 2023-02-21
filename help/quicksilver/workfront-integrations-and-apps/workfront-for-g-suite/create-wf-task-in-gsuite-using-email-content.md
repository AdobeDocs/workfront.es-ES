---
product-area: workfront-integrations;projects
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Cree un [!DNL Adobe Workfront] tarea en G Suite con contenido de correo electrónico
description: Puede convertir un correo electrónico externo (no generado por el Adobe) [!DNL Workfront]) a una tarea de Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# Cree un [!DNL Adobe Workfront] tarea en [!DNL G Suite] uso del contenido de correo electrónico

>[!NOTE]
>
>Hay un [problema conocido](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) con la versión actual de [!DNL Workfront for G Suite] no funciona como se esperaba. Estamos trabajando en una nueva versión y esperamos que se publique en el [!DNL Google Marketplace] en un futuro próximo.

Puede convertir un correo electrónico externo (no generado por [!DNL Adobe Workfront]) a [!DNL Workfront] tarea.

También puede convertir un correo electrónico externo en una actualización de una tarea existente. Para obtener más información, consulte [Actualizar un [!DNL Adobe Workfront] Elemento de [!DNL G Suite] con contenido de correo electrónico](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Para obtener información sobre el uso de [!DNL G Suite] para trabajar con correos electrónicos de notificación enviados por [!DNL Workfront], consulte [Administrar [!DNL Adobe Workfront] detalles de notificaciones de [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Antes de crear un [!DNL Workfront] tarea en [!DNL G Suite], debe

* Instalar [!DNL Workfront for G suite]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Cree un [!DNL Adobe Workfront] tarea en [!DNL G Suite] uso del contenido de correo electrónico

1. Si la variable [!UICONTROL Workfront para G Suite] no se muestra el panel, haga clic en el botón [!DNL Workfront] icono ![](assets/wf-lion-icon.png) en el [!DNL G Suite] barra lateral de complementos en el extremo derecho de la página.
1. Con el mensaje de correo electrónico abierto en [!DNL G Suite], haga clic en una opción de [!DNL Workfront for G Suite] para convertir el correo electrónico en un nuevo [!DNL Workfront] tarea.

1. Seleccione un **[!UICONTROL Crear nuevo]** para indicar si la tarea va a formar parte de un proyecto o de una tarea personal independiente de él.
1. Si desea adjuntar la tarea a un proyecto principal, haga clic en **[!UICONTROL Nombre del proyecto]**, empiece a escribir el nombre del proyecto en el que desea la tarea y, a continuación, haga clic en el nombre del proyecto cuando aparezca en la lista siguiente.
1. Realice cualquiera de estos cambios:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Task name]</td> 
      <td>Edite cualquier parte de este texto, que se toma de la línea de asunto del correo electrónico.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td>Edite cualquier parte de este texto, que se toma del cuerpo del correo electrónico.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Asignar a]</td> 
      <td>Haga clic en <strong>[!UICONTROL Asignar a]</strong>, haga clic en <strong>[!UICONTROL Asignar esto a]</strong> que aparece, empiece a escribir el nombre de la persona y haga clic en él cuando aparezca en la lista siguiente. Repita esto para cada persona que desee agregar y luego haga clic en <strong>[!UICONTROL Guardar]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Duración prevista]</td> 
      <td> <p>Haga clic en <strong>[!UICONTROL Duración prevista]</strong>y, a continuación, escriba el número de días que desea que dure la tarea. </p> <p>Nota: Esta opción se puede configurar para su organización de diferentes maneras. Por ejemplo, para su organización, es posible que tenga que escribir un número de horas en lugar de días. Si necesita más información, consulte [!DNL Workfront] administrador. Si desea especificar un período de tiempo distinto al predeterminado configurado, escriba <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong>o <strong>mo</strong> después del número para indicar minutos, horas, días, semanas o meses.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Haga clic en la flecha desplegable y, a continuación, haga clic en la prioridad que desee para la tarea.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir archivos adjuntos de correo electrónico]</td> 
      <td> <p>(Disponible solo si el correo electrónico contiene al menos un archivo adjunto). Haga clic en esta opción para guardar archivos adjuntos en el correo electrónico en el área [!UICONTROL Documents] de la tarea. </p> <p>Si no desea guardar un archivo adjunto, haga clic en la X a la derecha de su nombre. </p> <p>Si el correo electrónico contiene vínculos a documentos en [!DNL Google Drive], se guardan en la pestaña [!UICONTROL Overview] de la tarea que está creando. </p> <p>Importante: Para que esto funcione, su [!DNL Workfront] el administrador debe autorizar [!DNL Google Drive] para trabajar con documentos en [!DNL Workfront], tal como se describe en la sección <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configuración de integraciones para administrar documentos</a> en el artículo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurar integraciones de documentos</a>.</p> <p>Si activa esta opción, permanece habilitada para los demás correos electrónicos que convierta a tareas, problemas y actualizaciones.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir archivo de correo electrónico]</td> 
      <td> <p>Haga clic en esta opción para guardar el correo electrónico original como archivo de correo electrónico (EML) <span>al área [!UICONTROL Documents]</span> de la tarea. Desde allí, puede hacer doble clic en el archivo para abrir el correo electrónico en su aplicación de correo electrónico.</p> <p>Si activa esta opción, permanece habilitada para los demás correos electrónicos que convierta a tareas, problemas y actualizaciones.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear tarea]**.

   La variable **[!UICONTROL Detalles]** para la nueva tarea, aparece en la pestaña [!DNL Workfront for G Suite] panel. Puede hacer clic en **[!UICONTROL Actualizaciones]** y empiece a comunicarse con los colaboradores de inmediato sin dejar su bandeja de entrada.

   En la parte inferior del **[!UICONTROL Detalles]** , también puede hacer clic en **[!UICONTROL Ver en[!DNL Workfront]]** para ir a la nueva tarea en Workfront.

   Al actualizar el explorador, aparece un mensaje con un vínculo en la parte inferior de la variable [!DNL Workfront for G Suite] confirma que ha convertido el correo electrónico en una tarea:

   Puede hacer clic en el vínculo para ir a la vista Detalles, dentro del [!DNL Workfront for G Suite] para la tarea que ha creado.

   Puede repetir estos pasos para convertir el mismo correo electrónico en varias tareas. Cuando actualiza el explorador o vuelve al correo electrónico en otro momento, todos los vínculos que ha creado para el correo electrónico se enumeran en la parte inferior del [!UICONTROL Workfront para G Suite] panel.

1. (Opcional) Continúe trabajando con la tarea en la [!DNL Workfront for G Suite] realizando cualquiera de las siguientes acciones:

   * Para agregar una actualización en el **[!UICONTROL Actualizaciones]** , haga clic en **[!UICONTROL Iniciar una nueva actualización]** y escriba la actualización.

   * Para responder a una actualización en la **[!UICONTROL Actualizaciones]** , haga clic en **[!UICONTROL Responder]** y escriba su respuesta.

      Para ambas acciones anteriores, puede notificar a usuarios concretos su comentario. Haga clic en **[!UICONTROL Notificar]**, empiece a escribir el nombre de un usuario y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable. Repita este proceso para los demás usuarios a los que desee enviar la notificación y, a continuación, haga clic en **[!UICONTROL Publicación]**.

   * Haga clic en el **[!UICONTROL Documentos]** para ver los documentos guardados con la tarea.

Puede repetir estos pasos para convertir el mismo correo electrónico en varias tareas. Cuando actualiza el explorador o vuelve al correo electrónico en otro momento, todos los vínculos que ha creado para el correo electrónico se enumeran en la parte inferior del [!DNL Workfront for G Suite] panel.
