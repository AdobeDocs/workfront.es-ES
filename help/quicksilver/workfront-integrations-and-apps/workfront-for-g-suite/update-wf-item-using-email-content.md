---
product-area: workfront-integrations;projects
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Actualizar un elemento de  [!DNL Adobe Workfront]  y Google Workspace mediante contenido de correos electrónicos
description: Es posible actualizar un proyecto, tarea o problema existente con información de correos electrónicos que no sean de Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 77%

---

# Actualización de elementos de [!DNL Adobe Workfront] de [!DNL Google Workspace] mediante contenido de correos electrónicos

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

Es posible actualizar un proyecto, tarea o problema existente con información de un mensaje de correo electrónico que no sea de [!DNL Adobe Workfront].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p><p>Trabajo o superior</p>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de actualizar un elemento de [!DNL Workfront] mediante el contenido de un correo electrónico de [!DNL Google Workspace], es necesario

* Instalar [!DNL Workfront for Google Workspace]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Actualizar un elemento de [!DNL Workfront] mediante el contenido de correos electrónicos de [!DNL Google Workspace]

1. Si no se muestra el panel [!UICONTROL Workfront for Google Workspace], haga clic en el icono de Workfront ![Workfront icon](assets/wf-lion-icon.png) en la barra lateral de complementos de [!DNL Google Workspace], en el extremo derecho de la página.
1. Con el mensaje de correo electrónico abierto en [!DNL Google Workspace], haga clic en **[!UICONTROL Publicar como nueva actualización]** en el panel [!DNL Google Workspace].
1. En **[!UICONTROL Tipo]**, haga clic en la flecha desplegable y, a continuación, haga clic en el tipo de objeto en el que quiera añadir la actualización.
1. Haga clic en la opción **[!UICONTROL Buscar]**, empiece a escribir el nombre del objeto en el que quiera añadir la actualización y, a continuación, seleccione el elemento cuando aparezca en la lista siguiente.

   Esta opción variará según lo seleccionado en el paso 3. Podría ser **[!UICONTROL Buscar un proyecto]**, **[!UICONTROL Buscar una tarea]** o **[!UICONTROL Buscar un problema]**.

   >[!NOTE]
   >
   >Al escribir el nombre de una tarea, las tareas personales ad hoc se excluirán de la lista de nombres que aparece a continuación.

1. Realice cualquiera de estos cambios opcionales:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Edite cualquier parte de este texto, que se toma de la línea de asunto y del texto del cuerpo del correo electrónico.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td><p>(Solo está disponible si el correo electrónico contiene al menos un archivo adjunto). Haga clic en esta opción para guardar los archivos adjuntos en la ficha [!UICONTROL Documents] de la tarea o el problema. </p><p>Si no desea guardar un archivo adjunto, haga clic en la X situada a la derecha de su nombre. </p><p>Si el correo electrónico contiene vínculos a documentos en [!DNL Google Drive], los vínculos se guardarán en la pestaña [!UICONTROL Overview] de la tarea o problema que esté creando. </p><p>Importante: <span style="color: #ff1493;"><span style="color: #000000;">Para que esto funcione, el administrador de </span></span>[!DNL Workfront]<span style="color: #ff1493;"><span style="color: #000000;"> deberá autorizar a [!DNL Google Drive] para que trabaje con [!DNL Workfront]</span></span></p>
      <p>Si activa esta opción, permanecerá habilitada para otros correos electrónicos que convierta a tareas, problemas y actualizaciones.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notificar</td> 
      <td>Haga clic en <strong>[!UICONTROL Notify]</strong> y en la opción <strong>[!UICONTROL Search for a user or team]</strong> que aparecerá y, a continuación, empiece a escribir el nombre de la persona o equipo y haga clic en él cuando aparezca en la lista siguiente. Repita esto para cada persona y equipo que quiera añadir y, a continuación, haga clic en <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Actualizar]**.

   Al actualizar el explorador, un mensaje con un vínculo en la parte inferior del panel de [!DNL Workfront for Google Workspace] confirmará que convirtió el correo electrónico en una actualización:

   Haga clic en el vínculo para ir a la pestaña [!UICONTROL Actualizaciones] de [!DNL Workfront] para el objeto especificado en el paso 4.

   Repita estos pasos para convertir el mismo correo electrónico en actualizaciones, tareas y problemas (consulte [Crear un problema de Adobe Workfront en [!DNL Google Workspace] uso del contenido del correo electrónico](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Al actualizar el explorador o cuando vuelva al correo electrónico en otro momento, todos los vínculos creados para el correo electrónico se mostrarán en la parte inferior del panel [!UICONTROL Workfront para Google Workspace].

1. (Opcional) Continúe trabajando con la actualización en el panel de complementos de [!DNL Workfront] realizando cualquiera de las siguientes acciones:

   * Para añadir otra actualización en la pestaña **[!UICONTROL Actualizaciones]**, haga clic en **[!UICONTROL Iniciar una nueva actualización]** y escriba la información.

   * Para responder a una actualización en la pestaña **[!UICONTROL Actualizaciones]**, haga clic en **[!UICONTROL Responder]** y escriba la respuesta.

     Para ambas opciones, haga clic en **[!UICONTROL Notificar]** para especificar los destinatarios de la respuesta, como en el paso 5. Cuando esté listo, haga clic en **[!UICONTROL Publicar]** para añadir la actualización o la respuesta.

   * Haga clic en la pestaña **[!UICONTROL Detalles]** para ver los detalles del nuevo proyecto, tarea o problema.
