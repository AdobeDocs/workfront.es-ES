---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Actualizar un objeto existente desde un correo electrónico de Outlook
description: Puede actualizar un proyecto, tarea o problema existente con información de un correo electrónico de Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: 16acba0f1981b75ca141a36d096fb6f5d37c40d1
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# Actualizar un objeto existente de un correo electrónico de [!DNL Outlook]

Puede actualizar un proyecto, tarea o problema existente con información de un correo electrónico de [!DNL Outlook].

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

El administrador de [!DNL Workfront] debe habilitar [!DNL Outlook for Office] con [!DNL Workfront] para poder usar esta integración.

## Actualizar un objeto existente de un correo electrónico de [!DNL Outlook]

1. En [!DNL Outlook], seleccione el correo electrónico que contiene la información que desea incluir en un [!DNL Adobe Workfront update].
1. Haga clic en el icono **[!DNL Workfront]** en la esquina superior derecha del mensaje de correo electrónico para mostrar el complemento de Workfront.\
   Es posible que deba hacer clic en la flecha hacia abajo situada en la parte superior derecha del correo electrónico para acceder al icono [!DNL Workfront].

1. Haga clic en el icono **[!UICONTROL Menú]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) para mostrar la lista de opciones de [!DNL Workfront] disponibles.\


1. Haga clic en **[!UICONTROL Actualizar] en Workfront**.\
   Puede actualizar la siguiente información del correo electrónico antes de guardarlo como una tarea:

   * **[!UICONTROL Tipo]**: seleccione el tipo de objeto que está actualizando. Puede seleccionar **[!UICONTROL Proyecto]**, **[!UICONTROL Tarea]** o **[!UICONTROL Problema]**. El objeto que seleccione determina los resultados que se muestran en el campo **[!UICONTROL Nombre]** siguiente. Si no está seguro del tipo de objeto, seleccione **[!UICONTROL Todos]** para buscar proyectos, tareas y problemas simultáneamente.

   * **[!UICONTROL Nombre]**: empiece a escribir el nombre del proyecto, tarea o problema que desea actualizar. Haga clic en el nombre cuando aparezca en la lista desplegable.
   * **[!UICONTROL Actualización]**: de forma predeterminada, la actualización es la misma que el Cuerpo del correo electrónico. Puede modificar la actualización como desee.\

     Esta [!UICONTROL actualización] se muestra como el estado de actualización en Workfront.

   * **[!UICONTROL Archivos adjuntos]**: todos los archivos adjuntos de los correos electrónicos se guardan en el área de [!UICONTROL Documentos] de la tarea. Puede eliminar los archivos adjuntos antes de enviar la actualización.

1. (Opcional) Haga clic en **[!UICONTROL Incluir otros]**, empiece a escribir el nombre de los usuarios que desea incluir en la actualización y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.\
   Repita este proceso para incluir usuarios adicionales y luego haga clic en **[!UICONTROL Listo]**.\
   De forma predeterminada, el usuario al que responde recibe una notificación independientemente de si los incluye o no.\

1. (Opcional) Haga clic en el icono **[!UICONTROL Bloquear]** para restringir esta actualización a los usuarios de su compañía. Cuando la actualización está bloqueada, los usuarios que no pertenezcan a su empresa no podrán ver la actualización.

   * **[!UICONTROL Desbloqueado]:** Cualquier usuario con acceso al proyecto, tarea o problema en el que reside la actualización puede ver la actualización.\

     De forma predeterminada, la actualización está desbloqueada.\
      ![o365_addin_desbloquear.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL Bloqueado]:** Solo los usuarios de su compañía pueden ver la actualización.\

     ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. Haga clic en **[!UICONTROL Actualizar]**.
1. (Opcional) Haga clic en **[!UICONTROL Ver en Workfront]** para ver el elemento actualizado con la integración de [!DNL Workfront] en [!UICONTROL Outlook].
