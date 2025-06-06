---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Agregar un correo electrónico de Outlook como tarea a su lista de trabajos
description: Puede convertir [!DNL Outlook] correos electrónicos en [!DNL Adobe Workfront] tareas. Después de convertir un correo electrónico, la tarea está disponible en la Lista de trabajos en el área de Inicio.
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 22%

---

# Agregar un correo electrónico [!DNL Outlook] como tarea a su lista de trabajos

>[!IMPORTANT]
>
>[Microsoft está deshabilitando la compatibilidad con los tokens en línea heredados de Exchange](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que el complemento Outlook de Workfront usa actualmente para la autenticación. Este cambio de Microsoft ya ha comenzado a afectar a los clientes y seguirá implementándose por fases hasta octubre de 2025.
>
>* **Después de que Microsoft deshabilite completamente estos tokens, la integración de Workfront para Microsoft Outlook dejará de funcionar.**
>
>Como parte de este cambio, Microsoft ha tomado la decisión de cambiar la forma en que se vuelven a habilitar los tokens. Después del **30 de junio de 2025**, los administradores ya no podrán volver a habilitar los tokens, solo el soporte de Microsoft puede conceder excepciones. **El 1 de octubre de 2025, los tokens heredados se desactivarán para todos los inquilinos. No se concederán excepciones.**


Puede convertir [!DNL Outlook] correos electrónicos en [!DNL Adobe Workfront] tareas. Después de convertir un correo electrónico, la tarea estará disponible en su lista de [!UICONTROL Trabajar] en el área de [!UICONTROL Inicio].

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

## Agregar un correo electrónico [!DNL Outlook] como tarea a su lista de trabajos

1. Seleccione el correo electrónico de [!DNL Outlook] que desea convertir en una tarea.
1. Haga clic en el icono **[!DNL Workfront]** en la esquina superior derecha del mensaje de correo electrónico para mostrar el complemento [!DNL Workfront].\
   Es posible que deba hacer clic en la flecha hacia abajo situada en la parte superior derecha del correo electrónico para acceder al icono [!DNL Workfront].

1. Haga clic en el icono **[!UICONTROL Menú]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) para mostrar la lista de las opciones de [!DNL Workfront] disponibles.\


1. Haga clic en **[!UICONTROL Agregar al trabajo]**.\

1. Anule la selección del campo **[!UICONTROL Agregar al proyecto]**.
1. (Opcional) Puede actualizar la siguiente información del correo electrónico antes de guardarlo como una tarea:

   * **[!UICONTROL Nombre de tarea]:** De forma predeterminada, el nombre de tarea es el mismo que el Asunto del correo electrónico. Puede modificar el nombre de la tarea como desee.
   * **[!UICONTROL Descripción]:** De forma predeterminada, la descripción es la misma que el cuerpo del correo electrónico. Puede modificar la descripción como desee.
   * **[!UICONTROL Archivos adjuntos]:** Los archivos adjuntos de los mensajes de correo electrónico se guardarán en el área de [!UICONTROL Documentos] de la tarea. Puede eliminar los archivos adjuntos antes de guardar el correo electrónico como una tarea.

1. Haga clic en **[!UICONTROL Add]**.\
   La tarea se agrega a la [!UICONTROL Lista de trabajos] en su área de Inicio sin fecha de confirmación.

1. (Opcional) Haga clic en **[!UICONTROL Ver en Workfront]** para mostrar la tarea dentro de la aplicación [!DNL Workfront] en una nueva pestaña.

1. (Opcional) Vuelva a [!DNL Outlook] y seleccione el correo electrónico original.\
   En la parte superior del panel del complemento [!DNL Workfront], observe la confirmación con un vínculo de que el correo electrónico se agregó a Workfront como una tarea. El vínculo incluye la fecha en la que se convirtió.\
