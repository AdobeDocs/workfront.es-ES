---
product-area: workfront-integrations;projects
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Actualizar un [!DNL Adobe Workfront] Elemento de G Suite con contenido de correo electrónico
description: Puede actualizar un proyecto, tarea o problema existente con información de un correo electrónico que no sea de Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Actualizar un [!DNL Adobe Workfront] elemento de [!DNL G Suite] uso del contenido del correo electrónico

>[!NOTE]
>
>La versión más reciente del complemento de Adobe Workfront para Google se publicó el 26 de junio de 2023.

Puede actualizar un proyecto, tarea o problema existente con información de un[!DNL Adobe Workfront] correo electrónico.

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

Antes de actualizar un [!DNL Workfront] elemento con contenido de correo electrónico de [!DNL G Suite], debe

* Instalar [!DNL Workfront for G suite]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Actualizar un [!DNL Workfront] elemento con contenido de correo electrónico de [!DNL G Suite]

1. Si la variable [!UICONTROL Workfront para G Suite] no se muestra, haga clic en el icono Workfront ![](assets/wf-lion-icon.png) en el [!DNL G Suite] barra lateral de complementos, en el extremo derecho de la página.
1. Con el mensaje de correo electrónico abierto en [!DNL G Suite], haga clic en **[!UICONTROL Publicar como nueva actualización]** en el [!DNL G Suite] panel.
1. En **[!UICONTROL Tipo]**, haga clic en la flecha desplegable y, a continuación, haga clic en el tipo de objeto donde desea agregar la actualización.
1. Haga clic en **[!UICONTROL Buscar por]** , empiece a escribir el nombre del objeto donde desea agregar la actualización y, a continuación, seleccione el elemento cuando aparezca en la lista siguiente.

   Esta opción varía según lo que haya seleccionado en el paso 3. Podría ser... **[!UICONTROL Buscar un proyecto]**, **[!UICONTROL Buscar una tarea]**, o **[!UICONTROL Buscar un problema]**.

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
      <td><p>(Solo está disponible si el correo electrónico contiene al menos un archivo adjunto). Haga clic en esta opción para guardar los archivos adjuntos en la ficha [!UICONTROL Documents] de la tarea o el problema. </p><p>Si no desea guardar un archivo adjunto, haga clic en la X a la derecha de su nombre. </p><p>Si el correo electrónico contiene vínculos a documentos en [!DNL Google Drive]Sin embargo, los vínculos se guardan en la ficha [!UICONTROL Overview] de la tarea o el problema que está creando. </p><p>Importante: <span style="color: #ff1493;"><span style="color: #000000;">Para que esto funcione, su</span></span>[!DNL Workfront] administrador<span style="color: #ff1493;"><span style="color: #000000;"> debe autorizar [!DNL Google Drive] para trabajar con [!DNL Workfront]</span></span></p>
      <p>Si activa esta opción, permanecerá habilitada para otros correos electrónicos que convierta a tareas, problemas y actualizaciones.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notificar</td> 
      <td>Clic <strong>[!UICONTROL Notificar]</strong>, haga clic en <strong>[!UICONTROL Buscar un usuario o equipo]</strong> que aparece y, a continuación, empiece a escribir el nombre de la persona o equipo y haga clic en él cuando aparezca en la lista siguiente. Repita este proceso para cada persona y equipo que desee agregar y haga clic en <strong>[!UICONTROL Guardar]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Actualizar]**.

   Al actualizar el explorador, aparece un mensaje con un vínculo en la parte inferior de la etiqueta [!DNL Workfront for G Suite] el panel confirma que ha convertido el correo electrónico en una actualización:

   Puede hacer clic en el vínculo para ir a [!UICONTROL Actualizaciones] pestaña en [!DNL Workfront] para el objeto especificado en el paso 4.

   Puede repetir estos pasos para convertir el mismo correo electrónico en actualizaciones, tareas y problemas (consulte [Crear un problema de Adobe Workfront en [!DNL G Suite] mediante contenido de correo electrónico](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Cuando actualice el explorador o vuelva al correo electrónico en otro momento, todos los vínculos que haya creado para el correo electrónico se enumeran en la parte inferior de la [!UICONTROL Workfront para G Suite] panel.

1. (Opcional) Continúe trabajando con la actualización en el [!DNL Workfront] panel de complementos mediante cualquiera de las siguientes acciones:

   * Para agregar otra actualización en **[!UICONTROL Actualizaciones]** pestaña, haga clic en **[!UICONTROL Iniciar una nueva actualización]** y escriba la información.

   * Para responder a una actualización en **[!UICONTROL Actualizaciones]** pestaña, haga clic en **[!UICONTROL Responder]** y escriba su respuesta.

     Para ambas opciones anteriores, puede hacer clic en **[!UICONTROL Notificar]** para especificar destinatarios para la respuesta como en el paso 5. Cuando esté listo, haga clic en **[!UICONTROL Publicar]** para añadir la actualización o la respuesta.

   * Haga clic en **[!UICONTROL Detalles]** para ver los detalles del nuevo proyecto, tarea o problema.
