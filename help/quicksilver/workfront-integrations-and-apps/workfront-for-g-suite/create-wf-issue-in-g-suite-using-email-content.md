---
product-area: workfront-integrations;projects
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Crear  [!DNL Adobe Workfront] problema en Google Workspace mediante contenido de correo electrónico
description: Puede convertir un correo electrónico externo (no generado por  [!DNL Adobe Workfront)] ) en un  [!DNL Workfront] problema.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# Crear un problema de [!DNL Adobe Workfront] en [!DNL Google Workspace] mediante contenido de correo electrónico

>[!NOTE]
>
>La versión más reciente del complemento de Adobe Workfront para Google se publicó el 26 de junio de 2023.

Puede convertir un correo electrónico externo (no generado por [!DNL Adobe Workfront]) en un problema de [!DNL Workfront].

También puede convertir un correo electrónico externo en una actualización de un problema existente. Para obtener más información, consulta [Actualizar un [!DNL Adobe Workfront] elemento de [!DNL Google Workspace] usando contenido de correo electrónico](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Para obtener información sobre cómo usar [!DNL Google Workspace] para trabajar con los correos electrónicos de notificación enviados por [!DNL Workfront], consulte [Administrar [!DNL Adobe Workfront] detalles de notificación de [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

Para poder crear un problema a partir de [!DNL Google Workspace], debe

* Instalar [!DNL Workfront for Google Workspace]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Crear un problema de [!DNL Adobe Workfront] en [!DNL Google Workspace] mediante contenido de correo electrónico

1. Si no se muestra el panel [!UICONTROL Workfront for Google Workspace], haga clic en el icono [!DNL Workfront] ![](assets/wf-lion-icon.png) en la barra lateral de complementos de [!DNL Google Workspace], en el extremo derecho de la página.
1. Con el mensaje de correo electrónico abierto en [!DNL Google Workspace], haga clic en una opción de [!DNL Workfront for Google Workspace] para convertir el correo electrónico en un nuevo problema de [!DNL Workfront].

   ![](assets/convert-email-task-issue-update.png)

1. Si desea adjuntar el problema a un proyecto principal, haga clic en **[!UICONTROL Nombre del proyecto]**, empiece a escribir el nombre del proyecto donde desea el problema y, a continuación, haga clic en el nombre del proyecto cuando aparezca en la lista siguiente.
1. Realice cualquiera de estos cambios:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de problema]</td> 
      <td>Edite cualquier parte de este texto, que se toma de la línea de asunto del correo electrónico.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td>Edite cualquier parte de este texto, que se toma del cuerpo del correo electrónico.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Asignar a]</td> 
      <td>Haga clic en <strong>[!UICONTROL Asignar a]</strong>, haga clic en la opción <strong>[!UICONTROL Asignar esto a]</strong> que aparece y, a continuación, empiece a escribir el nombre de la persona y haga clic en él cuando aparezca en la lista siguiente. Repita esto para cada persona que desee agregar y, a continuación, haga clic en <strong>[!UICONTROL Guardar]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Prioridad]</td> 
      <td>Haga clic en la flecha desplegable y, a continuación, haga clic en la prioridad que desee para el problema.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir datos adjuntos de correo electrónico]</td> 
      <td> <p>(Solo está disponible si el correo electrónico contiene al menos un archivo adjunto). Haga clic en esta opción para guardar los archivos adjuntos en el correo electrónico en el área [!UICONTROL Documents] del problema. </p> <p>Si no desea guardar un archivo adjunto, haga clic en la X a la derecha de su nombre. </p> <p>Si el correo electrónico contiene vínculos a documentos en [!DNL Google Drive], se guardan en la ficha [!UICONTROL Overview] del problema que está creando. </p> <p>Importante: Para que esto funcione, el administrador de [!DNL Workfront] debe autorizar a [!DNL Google Drive] para que trabaje con documentos en [!DNL Workfront], tal como se describe en la sección <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurar integraciones para administrar documentos</a> en el artículo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurar integraciones de documentos</a>.</p> <p>Si activa esta opción, permanecerá habilitada para otros correos electrónicos que convierta a tareas, problemas y actualizaciones.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Incluir archivo de correo electrónico</td> 
      <td> <p>Haga clic en esta opción para guardar el correo electrónico original como un archivo de correo electrónico (EML) (correo electrónico) <span> en el área </span> de [!UICONTROL Documents] del problema. Desde allí, puede hacer doble clic en el archivo para abrir el correo electrónico en su aplicación de correo electrónico.</p> <p>Si activa esta opción, permanecerá habilitada para otros correos electrónicos que convierta a tareas, problemas y actualizaciones.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear problema]**.

   La ficha **[!UICONTROL Detalles]** del nuevo problema se muestra en el panel [!DNL Workfront for Google Workspace]. Puede hacer clic en **[!UICONTROL Actualizaciones]** y comenzar a comunicarse con los colaboradores de inmediato sin salir de su bandeja de entrada.

   En la parte inferior de la ficha **[!UICONTROL Detalles]**, también puedes hacer clic en **[!UICONTROL Ver en Workfront]** para ir al nuevo problema en Workfront.

   Al actualizar el explorador, un mensaje con un vínculo en la parte inferior del panel [!UICONTROL Workfront for Google Workspace] confirma que ha convertido el correo electrónico en un problema:

   Puede hacer clic en el vínculo para ir a la vista Detalles, en el panel [!DNL Workfront for Google Workspace], del problema que ha creado.

   Puede repetir estos pasos para convertir el mismo correo electrónico en varios problemas. Cuando actualice el explorador o vuelva al correo electrónico en otro momento, todos los vínculos que haya creado para el correo electrónico se mostrarán en la parte inferior del panel [!UICONTROL Workfront for Google Workspace].

1. (Opcional) Continúe trabajando con el problema en el panel [!DNL Workfront for Google Workspace] haciendo cualquiera de las siguientes acciones:

   * Para agregar una actualización en la ficha **[!UICONTROL Actualizaciones]**, haga clic en **[!UICONTROL Iniciar una nueva actualización]** y escriba la actualización.

   * Para responder a una actualización en la ficha **[!UICONTROL Actualizaciones]**, haga clic en **[!UICONTROL Responder]** y escriba la respuesta.

     Para ambas acciones, puede notificar a usuarios concretos su comentario. Haga clic en **[!UICONTROL Notificar]**, empiece a escribir el nombre de un usuario y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable. Repita este proceso para los demás usuarios a los que desee notificar y luego haga clic en **[!UICONTROL Post]**.

   * Haga clic en la ficha **[!UICONTROL Documentos]** para ver los documentos guardados con el problema.
