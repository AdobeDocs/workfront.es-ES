---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Revisar proyectos solicitados
description: Las solicitudes de proyecto se muestran como proyectos con un estado de [!UICONTROL Solicitado] en Adobe Workfront. Este artículo describe cómo revisar las solicitudes de proyectos.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 98%

---

# Revisar proyectos solicitados

Cuando se presentan varias solicitudes de proyectos para su revisión, la oficina de administración de proyectos o el comité de portafolio pueden reunirse para examinar las solicitudes enviadas y determinar las aprobaciones de solicitudes de proyectos. Las solicitudes de proyecto se muestran como proyectos con un estado de [!UICONTROL Solicitado] en [!DNL Adobe Workfront].

Puede enviar una solicitud de revisión de proyecto siguiendo uno de estos procedimientos:

* Cambie el estado del proyecto a **[!UICONTROL Solicitado]**.
* Complete el [!UICONTROL caso empresarial] del proyecto y envíelo para su aprobación.\
   Para obtener más información sobre cómo completar un caso comercial para un proyecto, consulte [Crear un caso comercial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Puede revisar los proyectos solicitados en las siguientes áreas de [!DNL Adobe Workfront]:

* En un informe de proyecto
* En un portafolio

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td><p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso [!UICONTROL View] o superior a portafolios</p> <p>Acceso [!UICONTROL Edit] a proyectos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de [!UICONTROL View] o superiores en el portafolio</p> <p>Permisos de [!UICONTROL Manage] en los proyectos para actualizar su estado</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Revisar los proyectos solicitados en un informe de proyecto

Puede generar un informe de proyectos para ver qué proyectos tienen un estado de [!UICONTROL Solicitado].

Para obtener más información sobre cómo aprobar solicitudes de proyecto mediante la generación de un informe de proyecto, consulte la sección [[!UICONTROL Aprobación del caso comercial mediante la creación de un informe de proyecto]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) en [Aprobar un caso comercial](../../../manage-work/projects/define-a-business-case/approve-business-case.md). 

## Revisar los proyectos solicitados dentro de un portafolio

1. Vaya al portafolio cuyos proyectos solicitados desee revisar.
1. Haga clic en **[!UICONTROL Proyectos]** en el panel izquierdo
1. En el menú desplegable **[!UICONTROL Filtro]**, seleccione **[!UICONTROL Solicitado]**.

   En la lista solo se muestran los proyectos con el estado **[!UICONTROL Solicitado]**.

   >[!TIP]
   >
   > Además de tener un estado de **[!UICONTROL Solicitado]**, los proyectos deben estar asociados al portafolio seleccionado para que se muestren en esta lista.

1. Haga clic en el nombre de un proyecto de la lista para abrirlo.
1. Haga clic en **[!UICONTROL Detalles del proyecto]** en el panel izquierdo.
1. Realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Caso comercial]** y, a continuación, haga clic en **[!UICONTROL Aprobar]** o **[!UICONTROL Rechazar]** en el área de [!UICONTROL Resumen de caso comercial] para aprobar o rechazar el caso comercial.

     ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

     El estado del proyecto cambia a **[!UICONTROL Aprobado]** si se aprueba el caso comercial.

     El estado del proyecto se cambia a **[!UICONTROL Rechazado]** si se rechaza el caso empresarial.

     >[!NOTE]
     >
     >No hay notificaciones que avisen al usuario que envió la aprobación del caso empresarial sobre si su solicitud de proyecto se aprobó o rechazó. 

     O

   * Cambie el estado del proyecto a cualquier otro estado en el menú desplegable **[!UICONTROL Estado]**.

     ![Cambiar el estado del proyecto del menú desplegable](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)
 

 
