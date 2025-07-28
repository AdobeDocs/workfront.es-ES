---
product-area: workfront-integrations
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Acceso al contenido de inicio de  [!DNL Adobe Workfront]  desde Google Workspace
description: Puede acceder al contenido de Inicio de  [!DNL Adobe Workfront] , incluidas todas las tareas, problemas, aprobaciones y solicitudes de acceso que se le hayan asignado, sin salir de Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: da2ecaf1-5cfb-470e-90a1-fbb386db8670
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 52%

---

# Acceso al contenido de Inicio de [!DNL Adobe Workfront] desde [!DNL Google Workspace]

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

Puede acceder al contenido de [!DNL Adobe Workfront] [!UICONTROL Inicio], incluidas todas las tareas, problemas, aprobaciones y solicitudes de acceso que se le hayan asignado, sin salir de Google Workspace.

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

Para poder obtener acceso al contenido de [!UICONTROL Inicio] desde [!DNL Google Workspace], debe

* Instalar [!DNL Workfront for Google Workspace]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Acceso a [!DNL Workfront] [!UICONTROL Inicio] desde [!DNL Google Workspace]

1. Asegúrese de haber iniciado sesión en [!DNL Workfront].
1. Si no se muestra el panel [!UICONTROL Workfront for Google Workspace], haga clic en el icono [!DNL Workfront] ![Workfront icon](assets/wf-lion-icon.png) en la barra lateral de complementos de [!DNL Google Workspace], en el extremo derecho de la página.
1. Si ve una flecha izquierda en la parte superior de [!DNL Workfront] para [!DNL Google Workspace], haga clic en la flecha para ir al área de [!UICONTROL Inicio].

1. En el área **[!UICONTROL Ordenar por]**, haga clic en la flecha de expansión ![Expandir flecha](assets/dropdown-arrow.png) y, a continuación, haga clic en una opción para especificar cómo desea agrupar los elementos de trabajo de modo que pueda encontrar el que desee.

   Al ordenar por **[!UICONTROL fecha de confirmación]** o **[!UICONTROL fecha planificada de finalización]**, los elementos de trabajo más antiguos se encuentran en la parte superior.

   Al ordenar por **[!UICONTROL Proyecto]**, los elementos de trabajo aparecen en el orden de sus proyectos principales, enumerados alfabéticamente de la A a la Z. Los elementos de trabajo sin proyecto principal se muestran en **[!UICONTROL Sin proyecto]**.

1. Haga clic en la flecha de expansión ![Expandir flecha](assets/dropdown-arrow.png) para la agrupación que desee ver.

   El número de elementos contenidos en cada grupo se muestra entre paréntesis. Al hacer clic en la flecha [!UICONTROL expand], se muestran todos los elementos de trabajo del grupo.

   Los elementos de trabajo aparecen de la siguiente manera:

   * ![Icono de tarea](assets/task-icon.png) **Las tareas** muestran el nombre del proyecto principal, el nombre de la tarea y la fecha planificada de finalización.

   * ![Icono de problema](assets/issue-icon.png) **Problemas** muestra el nombre del proyecto principal, el nombre del problema y la fecha planificada de finalización.

   * ![Icono del documento](assets/document-icon.png) **Aprobaciones** muestra el nombre del solicitante, el nombre del documento y la fecha de envío.
   * Las **solicitudes de acceso** muestran el nombre, el nombre de objeto y la fecha de envío del solicitante. El icono del tipo de objeto se muestra a la izquierda.

1. Haga clic en cualquier lugar de un elemento de trabajo para ver sus detalles, actualizaciones y documentos.
