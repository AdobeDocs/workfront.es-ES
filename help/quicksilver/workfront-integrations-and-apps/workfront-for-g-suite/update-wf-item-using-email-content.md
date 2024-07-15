---
product-area: workfront-integrations;projects
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Actualizar un [!DNL Adobe Workfront] elemento de Google Workspace mediante contenido de correo electrónico
description: Puede actualizar un proyecto, tarea o problema existente con información de un correo electrónico que no sea de Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# Actualizar un elemento [!DNL Adobe Workfront] de [!DNL Google Workspace] mediante contenido de correo electrónico

>[!NOTE]
>
>La versión más reciente del complemento de Adobe Workfront para Google se publicó el 26 de junio de 2023.

Puede actualizar un proyecto, tarea o problema existente con información de un mensaje de correo electrónico que no sea [!DNL Adobe Workfront].

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

Antes de poder actualizar un elemento de [!DNL Workfront] mediante el contenido de correo electrónico de [!DNL Google Workspace], debe

* Instalar [!DNL Workfront for Google Workspace]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Actualizar un elemento de [!DNL Workfront] mediante el contenido de correo electrónico de [!DNL Google Workspace]

1. Si no se muestra el panel [!UICONTROL Workfront for Google Workspace], haga clic en el icono de Workfront ![](assets/wf-lion-icon.png) en la barra lateral de complementos de [!DNL Google Workspace], en el extremo derecho de la página.
1. Con el mensaje de correo electrónico abierto en [!DNL Google Workspace], haga clic en **[!UICONTROL Post como una nueva actualización]** en el panel [!DNL Google Workspace].
1. En **[!UICONTROL Tipo]**, haga clic en la flecha desplegable y, a continuación, haga clic en el tipo de objeto donde desea agregar la actualización.
1. Haga clic en la opción **[!UICONTROL Buscar]**, empiece a escribir el nombre del objeto donde desea agregar la actualización y, a continuación, seleccione el elemento cuando aparezca en la lista siguiente.

   Esta opción varía según lo que haya seleccionado en el paso 3. Podría ser **[!UICONTROL Buscar un proyecto]**, **[!UICONTROL Buscar una tarea]** o **[!UICONTROL Buscar un problema]**.

   >[!NOTE]
   >
   >Al escribir el nombre de una tarea, las tareas personales ad hoc se excluyen de la lista de nombres que aparece a continuación.

1. Realice cualquiera de estos cambios opcionales:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Actualización]</td> 
      <td>Edite cualquier parte de este texto, que se toma de la línea de asunto y del texto del cuerpo del correo electrónico.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir datos adjuntos de correo electrónico]</td> 
      <td><p>(Solo está disponible si el correo electrónico contiene al menos un archivo adjunto). Haga clic en esta opción para guardar los archivos adjuntos en la ficha [!UICONTROL Documents] de la tarea o el problema. </p><p>Si no desea guardar un archivo adjunto, haga clic en la X a la derecha de su nombre. </p><p>Si el correo electrónico contiene vínculos a documentos en [!DNL Google Drive], los vínculos se guardan en la ficha [!UICONTROL Overview] de la tarea o problema que está creando. </p><p>Importante: <span style="color: #ff1493;"><span style="color: #000000;">Para que esto funcione, el administrador de </span></span>[!DNL Workfront]<span style="color: #ff1493;"><span style="color: #000000;"> debe autorizar a [!DNL Google Drive] para que trabaje con [!DNL Workfront]</span></span></p>
      <p>Si activa esta opción, permanecerá habilitada para otros correos electrónicos que convierta a tareas, problemas y actualizaciones.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notificar</td> 
      <td>Haga clic en <strong>[!UICONTROL Notificar]</strong>, haga clic en la opción <strong>[!UICONTROL Buscar un usuario o equipo]</strong> que aparece y, a continuación, empiece a escribir el nombre de la persona o equipo y haga clic en él cuando aparezca en la lista siguiente. Repita esto para cada persona y equipo que desee agregar y, a continuación, haga clic en <strong>[!UICONTROL Guardar]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Actualizar]**.

   Al actualizar el explorador, un mensaje con un vínculo en la parte inferior del panel [!DNL Workfront for Google Workspace] confirma que ha convertido el correo electrónico en una actualización:

   Puede hacer clic en el vínculo para ir a la ficha [!UICONTROL Actualizaciones] en [!DNL Workfront] para el objeto especificado en el paso 4.

   Puede repetir estos pasos para convertir el mismo correo electrónico en actualizaciones, tareas y problemas (consulte [Crear un problema de Adobe Workfront en [!DNL Google Workspace] usando el contenido del correo electrónico](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Cuando actualice el explorador o vuelva al correo electrónico en otro momento, todos los vínculos que haya creado para el correo electrónico se mostrarán en la parte inferior del panel [!UICONTROL Workfront for Google Workspace].

1. (Opcional) Continúe trabajando con la actualización en el panel de complementos de [!DNL Workfront] realizando cualquiera de las siguientes acciones:

   * Para agregar otra actualización en la ficha **[!UICONTROL Actualizaciones]**, haga clic en **[!UICONTROL Iniciar una nueva actualización]** y escriba la información.

   * Para responder a una actualización en la ficha **[!UICONTROL Actualizaciones]**, haga clic en **[!UICONTROL Responder]** y escriba la respuesta.

     Para ambas opciones, puede hacer clic en **[!UICONTROL Notificar]** para especificar los destinatarios de la respuesta, como en el paso 5. Cuando esté listo, haga clic en **[!UICONTROL Post]** para agregar la actualización o la respuesta.

   * Haga clic en la ficha **[!UICONTROL Detalles]** para ver los detalles del nuevo proyecto, tarea o problema.
