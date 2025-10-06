---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Actualizar un objeto existente desde un correo electrónico de Outlook
description: Puede actualizar un proyecto, tarea o problema existente con información proveniente de un correo electrónico de Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 90%

---

# Actualizar un objeto existente de un correo electrónico de [!DNL Outlook]

>[!IMPORTANT]
>
>[Microsoft ha deshabilitado la compatibilidad con los tokens en línea heredados de Exchange](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que el complemento de Workfront Outlook utilizaba para la autenticación. Este cambio de Microsoft se implementó por fases y se completó el 1 de octubre de 2025.
>
>**Debido a que Microsoft ha deshabilitado estos tokens, la integración de Workfront para Microsoft Outlook ya no funciona.**

Puede actualizar un proyecto, tarea o problema existente con la información de un correo electrónico de [!DNL Outlook].

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

El administrador de [!DNL Workfront] debe habilitar [!DNL Outlook for Office] con [!DNL Workfront] antes de poder usar esta integración.

## Actualizar un objeto existente desde un correo electrónico de [!DNL Outlook]

1. En [!DNL Outlook], seleccione el correo electrónico que contiene la información que desea incluir en una [!DNL Adobe Workfront update].
1. Haga clic en el icono **[!DNL Workfront]** en la esquina superior derecha del mensaje de correo electrónico para mostrar el complemento de Workfront.\
   Es posible que deba hacer clic en la flecha hacia abajo situada en la parte superior derecha del correo electrónico para acceder al icono de [!DNL Workfront].

1. Haga clic en el icono **[!UICONTROL Menú]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) para mostrar la lista de opciones de [!DNL Workfront] disponibles.\


1. Haga clic en **[!UICONTROL Actualizar] en Workfront**.\
   Puede actualizar la siguiente información del correo electrónico antes de guardarlo como una tarea:

   * **[!UICONTROL Tipo]**: seleccione el tipo de objeto que está actualizando. Puede seleccionar **[!UICONTROL Proyecto]**, **[!UICONTROL Tarea]** o **[!UICONTROL Problema]**. El objeto que seleccione determina los resultados que se muestran en el campo **[!UICONTROL Nombre]** siguiente. Si no está seguro del tipo de objeto, seleccione **[!UICONTROL Todo]** para buscar proyectos, tareas y problemas simultáneamente.

   * **[!UICONTROL Nombre]**: empiece a escribir el nombre del proyecto, tarea o problema que desea actualizar. Haga clic sobre el nombre cuando aparezca en la lista.
   * **[!UICONTROL Actualización]**: de forma predeterminada, la actualización es la misma que el cuerpo del correo electrónico. Puede modificar la actualización como desee.\

     Esta [!UICONTROL actualización] se muestra como el estado de actualización en Workfront.

   * **[!UICONTROL Archivos adjuntos]**: todos los archivos adjuntos de los correos electrónicos se guardan en el área de [!UICONTROL Documentos] de la tarea. Puede eliminar los archivos adjuntos antes de enviar la actualización.

1. (Opcional) Haga clic en **[!UICONTROL Incluir otros]**, empiece a escribir el nombre de los usuarios que desea incluir en la actualización y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.\
   Repita este proceso para incluir usuarios adicionales y, a continuación, haga clic en **[!UICONTROL Listo]**.\
   De forma predeterminada, el usuario al que responde recibe una notificación independientemente de si los incluye o no.\

1. (Opcional) Haga clic en el icono **[!UICONTROL Bloqueado]** para restringir esta actualización a los usuarios de su compañía. Cuando la actualización está bloqueada, los usuarios que no pertenezcan a su compañía no podrán verla.

   * **[!UICONTROL Desbloqueado]:** cualquier usuario con acceso al proyecto, tarea o problema en el que reside la actualización puede verla.\

     De forma predeterminada, la actualización está desbloqueada.\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL Bloqueado]:** solo los usuarios de su compañía pueden ver la actualización.\

     ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. Haga clic en **[!UICONTROL Actualizar]**.
1. (Opcional) Haga clic en **[!UICONTROL Ver en Workfront]** para ver el elemento actualizado con la integración de [!DNL Workfront] en [!UICONTROL Outlook].
