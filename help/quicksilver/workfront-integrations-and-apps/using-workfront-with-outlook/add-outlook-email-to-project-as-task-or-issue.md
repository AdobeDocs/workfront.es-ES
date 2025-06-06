---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Añadir un correo electrónico de Outlook a un proyecto como una tarea o un problema
description: Puede convertir correos electrónicos a tareas o problemas de  [!DNL Adobe Workfront] . Después de convertir un correo electrónico, la tarea o el problema aparecen en el proyecto seleccionado mientras lo está convirtiendo.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 00755c27-9fc9-4357-a39b-4f9772484252
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 82%

---

# Añadir un correo electrónico de [!DNL Outlook] a un proyecto como una tarea o problema

>[!IMPORTANT]
>
>[Microsoft está deshabilitando la compatibilidad con los tokens en línea heredados de Exchange](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que el complemento Outlook de Workfront usa actualmente para la autenticación. Este cambio de Microsoft ya ha comenzado a afectar a los clientes y seguirá implementándose por fases hasta octubre de 2025.
>
>* **Después de que Microsoft deshabilite completamente estos tokens, la integración de Workfront para Microsoft Outlook dejará de funcionar.**
>
>Como parte de este cambio, Microsoft ha tomado la decisión de cambiar la forma en que se vuelven a habilitar los tokens. Después del **30 de junio de 2025**, los administradores ya no podrán volver a habilitar los tokens, solo el soporte de Microsoft puede conceder excepciones. **El 1 de octubre de 2025, los tokens heredados se desactivarán para todos los inquilinos. No se concederán excepciones.**


Puede convertir correos electrónicos en tareas o problemas de [!DNL Adobe Workfront]. Después de convertir un correo electrónico, la tarea o el problema aparecen en el proyecto seleccionado mientras lo está convirtiendo.

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

El administrador de [!DNL Workfront] debe habilitar [!DNL Outlook for Office] con [!DNL Workfront] para poder usar esta integración.

## Añadir un correo electrónico de [!DNL Outlook] a un proyecto como una tarea o problema

1. Seleccione el correo electrónico de [!DNL Outlook] que desea convertir en una tarea o un problema.
1. Haga clic en el icono **[!DNL Workfront]** en la esquina superior derecha del mensaje de correo electrónico para mostrar el complemento de Workfront.

   Es posible que deba hacer clic en la flecha hacia abajo situada en la parte superior derecha del correo electrónico para acceder al icono de [!DNL Workfront].

1. Haga clic en el icono de **[!UICONTROL Menú]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) para mostrar la lista de las opciones de [!DNL Workfront] disponibles.



1. Haga clic en **[!UICONTROL Añadir al trabajo]**.

1. Seleccione el campo **[!UICONTROL Añadir al proyecto]**.
1. Empiece a escribir el nombre de un proyecto en el campo **[!UICONTROL Proyecto]** y, a continuación, selecciónelo cuando aparezca en la lista. 
1. Seleccione el botón de opción **[!UICONTROL Tarea]** si desea añadir una tarea al proyecto seleccionado.

   O

   Seleccione el botón de opción **[!UICONTROL Problema]** si desea añadir un problema al proyecto seleccionado.

1. (Opcional) Especifique a quién se asigna esta tarea o este problema en el campo **[!UICONTROL Asignar esto a]**.

   >[!TIP]
   >
   >Puede asignar la tarea o el problema a un equipo, si desea que varias personas lo sepan. Si los miembros del equipo tienen habilitadas sus notificaciones por correo electrónico, recibirán un correo electrónico sobre la nueva tarea o problema asignado a ellos.


1. (Opcional) Especifique el **[!UICONTROL Vencimiento por fecha]**. Se convierte en la [!UICONTROL fecha planificada de finalización] de la tarea o el problema.
1. (Opcional) Actualice la siguiente información del correo electrónico antes de guardarla como una tarea o un problema (los campos obligatorios van precedidos de un asterisco).

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Task or Issue Name]</td>
        <td>De forma predeterminada, el nombre de la tarea es el mismo que el asunto del correo electrónico. Puede modificar el nombre de la tarea como desee.</td>
        <td></td>
      </tr>
      <tr>
        <td>[!UICONTROL Description]</td>
        <td>De forma predeterminada, la descripción es la misma que el cuerpo del correo electrónico. Puede modificar la descripción como desee.</td>
      </tr>
      <tr>
        <td>[!UICONTROL Attachments]</td>
        <td>Los datos adjuntos de los mensajes de correo electrónico se guardan en el área de [!UICONTROL Documents] de la tarea o el problema. Puede eliminar los archivos adjuntos antes de guardar el correo electrónico como una tarea o un problema.</td>
      </tr>
   </table>

1. Haga clic en **[!UICONTROL Añadir]**

   La tarea o el problema se añaden al proyecto especificado

1. (Opcional) Haga clic en **[!UICONTROL Ver en[!DNL Workfront]]** para mostrar la tarea dentro de la aplicación de [!DNL Workfront] en una nueva pestaña.

1. (Opcional) Vuelva a [!DNL Outlook] y seleccione el correo electrónico convertido.

   En la parte superior del panel de complemento de [!DNL Workfront], tome nota de la confirmación con un vínculo de que el correo electrónico se añadió a [!DNL Workfront] como una tarea o un problema. El vínculo incluye la fecha en la que se convirtió.



