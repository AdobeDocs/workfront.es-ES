---
product-area: workfront-integrations;projects
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Crear un [!DNL Adobe Workfront] tarea en G Suite mediante contenido de correo electrónico
description: Puede convertir un correo electrónico externo (no generado por el Adobe) [!DNL Workfront]) a una tarea de Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 0%

---

# Crear un [!DNL Adobe Workfront] tarea en [!DNL G Suite] uso del contenido del correo electrónico

>[!NOTE]
>
>La versión más reciente del complemento de Adobe Workfront para Google se publicó el 26 de junio de 2023.

Puede convertir un correo electrónico externo (no generado por [!DNL Adobe Workfront]) a un [!DNL Workfront] tarea.

También puede convertir un correo electrónico externo en una actualización de una tarea existente. Para obtener más información, consulte [Actualizar un [!DNL Adobe Workfront] elemento de [!DNL G Suite] mediante contenido de correo electrónico](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Para obtener información sobre el uso de [!DNL G Suite] para trabajar con correos electrónicos de notificación enviados por [!DNL Workfront], consulte [Administrar [!DNL Adobe Workfront] detalles de notificación de [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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
   <td> <p>[!UICONTROL Trabajo], [!UICONTROL Plan]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Antes de crear un [!DNL Workfront] tarea en [!DNL G Suite], debe

* Instalar [!DNL Workfront for G suite]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Crear un [!DNL Adobe Workfront] tarea en [!DNL G Suite] uso del contenido del correo electrónico

1. Si la variable [!UICONTROL Workfront para G Suite] no se muestra, haga clic en el [!DNL Workfront] icono ![](assets/wf-lion-icon.png) en el [!DNL G Suite] barra lateral de complementos, en el extremo derecho de la página.
1. Con el mensaje de correo electrónico abierto en [!DNL G Suite], haga clic en una opción de [!DNL Workfront for G Suite] para convertir el correo electrónico en un nuevo [!DNL Workfront] tarea.

1. Seleccione una **[!UICONTROL Crear nuevo]** para indicar si la tarea va a formar parte de un proyecto o si va a ser una tarea personal que sea independiente de un proyecto.
1. Si desea adjuntar la tarea a un proyecto principal, haga clic en **[!UICONTROL Nombre del proyecto]** A continuación, empiece a escribir el nombre del proyecto donde desea la tarea y, cuando aparezca en la lista siguiente, haga clic en el nombre del proyecto.
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
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td>Edite cualquier parte de este texto, que se toma del cuerpo del correo electrónico.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Asignar a]</td> 
      <td>Clic <strong>[!UICONTROL Asignar a]</strong>, haga clic en <strong>[!UICONTROL Asignar esto a]</strong> que aparece y, a continuación, empiece a escribir el nombre de la persona y haga clic en él cuando aparezca en la lista siguiente. Repita este proceso para cada persona que desee agregar y haga clic en <strong>[!UICONTROL Guardar]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Duración planificada]</td> 
      <td> <p>Clic <strong>[!UICONTROL Duración planificada]</strong>A continuación, escriba el número de días que desea que tarde la tarea. </p> <p>Nota: Esta opción se puede configurar para su organización de diferentes maneras. Por ejemplo, para su organización, es posible que tenga que escribir un número de horas en lugar de días. Si necesita más información, consulte a su [!DNL Workfront] administrador. Si desea especificar un período de tiempo distinto del predeterminado configurado, escriba <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong>, o <strong>mo</strong> después del número, que indica minutos, horas, días, semanas o meses.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Prioridad]</td> 
      <td>Haga clic en la flecha desplegable y luego haga clic en la prioridad que desee para la tarea.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir datos adjuntos de correo electrónico]</td> 
      <td> <p>(Solo está disponible si el correo electrónico contiene al menos un archivo adjunto). Haga clic en esta opción para guardar los archivos adjuntos en el correo electrónico en el área de [!UICONTROL Documents] de la tarea. </p> <p>Si no desea guardar un archivo adjunto, haga clic en la X a la derecha de su nombre. </p> <p>Si el correo electrónico contiene vínculos a documentos en [!DNL Google Drive], se guardan en la ficha [!UICONTROL Overview] de la tarea que está creando. </p> <p>Importante: Para que esto funcione, su [!DNL Workfront] el administrador debe autorizar [!DNL Google Drive] para trabajar con documentos en [!DNL Workfront], tal como se describe en la sección <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurar integraciones para administrar documentos</a> en el artículo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurar integraciones de documentos</a>.</p> <p>Si activa esta opción, permanecerá habilitada para otros correos electrónicos que convierta a tareas, problemas y actualizaciones.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir archivo de correo electrónico]</td> 
      <td> <p>Haga clic en esta opción para guardar el correo electrónico original como archivo de correo electrónico (EML) <span>al área de [!UICONTROL Documents]</span> de la tarea. Desde allí, puede hacer doble clic en el archivo para abrir el correo electrónico en su aplicación de correo electrónico.</p> <p>Si activa esta opción, permanecerá habilitada para otros correos electrónicos que convierta a tareas, problemas y actualizaciones.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Crear tarea]**.

   El **[!UICONTROL Detalles]** La pestaña de la nueva tarea se muestra en [!DNL Workfront for G Suite] panel. Puede hacer clic en **[!UICONTROL Actualizaciones]** y empiece a comunicarse con sus colaboradores de inmediato sin salir de su bandeja de entrada.

   En la parte inferior de la **[!UICONTROL Detalles]** , también puede hacer clic en **[!UICONTROL Ver en[!DNL Workfront]]** para ir a la nueva tarea en Workfront.

   Al actualizar el explorador, aparece un mensaje con un vínculo en la parte inferior de la etiqueta [!DNL Workfront for G Suite] el panel confirma que ha convertido el correo electrónico en una tarea:

   Puede hacer clic en el vínculo para ir a la vista de detalles, dentro de la variable [!DNL Workfront for G Suite] panel, para la tarea que ha creado.

   Puede repetir estos pasos para convertir el mismo correo electrónico en varias tareas. Cuando actualice el explorador o vuelva al correo electrónico en otro momento, todos los vínculos que haya creado para el correo electrónico se enumeran en la parte inferior de la [!UICONTROL Workfront para G Suite] panel.

1. (Opcional) Continúe trabajando con la tarea en [!DNL Workfront for G Suite] Panel mediante cualquiera de las siguientes acciones:

   * Para añadir una actualización en **[!UICONTROL Actualizaciones]** pestaña, haga clic en **[!UICONTROL Iniciar una nueva actualización]** y escriba la actualización.

   * Para responder a una actualización en **[!UICONTROL Actualizaciones]** pestaña, haga clic en **[!UICONTROL Responder]** y escriba su respuesta.

     Para ambas acciones, puede notificar a usuarios concretos su comentario. Clic **[!UICONTROL Notificar]**, empiece a escribir el nombre de un usuario y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable. Repita este proceso para los demás usuarios a los que desee notificar y haga clic en **[!UICONTROL Publicar]**.

   * Haga clic en **[!UICONTROL Documentos]** para ver los documentos guardados con la tarea.

Puede repetir estos pasos para convertir el mismo correo electrónico en varias tareas. Cuando actualice el explorador o vuelva al correo electrónico en otro momento, todos los vínculos que haya creado para el correo electrónico se enumeran en la parte inferior de la [!DNL Workfront for G Suite] panel.
