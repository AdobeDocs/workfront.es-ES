---
product-area: documents
navigation-topic: approvals
title: Crear una solicitud de revisión o aprobación de documento
description: Puede solicitar la aprobación de otros usuarios para un documento en Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 83%

---

# Crear una solicitud de revisión o aprobación de documento

Puede solicitar la aprobación de otros usuarios o equipos para un documento en Adobe Workfront o solicitar que revisen un documento sin necesidad de aprobarlo.

>[!IMPORTANT]
>
>El contenido de este artículo hace referencia a la funcionalidad actualizada de aprobación de documentos que solo está disponible para cuentas específicas. Para obtener información sobre los procesos de aprobación estándar, consulte los artículos enumerados en [Aprobaciones de trabajo](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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
   <td>
   <p>Colaborador o superior</p>
   <p>Revisión o superior</p>
   <p>Si utiliza la integración de Frame.io, debe tener una licencia Standard para crear flujos de trabajo de aprobación.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a Proyectos, Tareas, Problemas, Plantillas, Portafolios, Programas, Informes, Paneles de control y Calendarios, Documentos</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de administración al objeto asociado con el acceso de solicitud o la aprobación </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una solicitud de revisión o aprobación de documento desde la página de documento

1. Pase el puntero por encima del documento y haga clic en Detalles del documento.
   ![Detalles del documento](assets/doc-details.png)

1. Cerca del nombre del documento, seleccione la versión del documento para la que desea crear una aprobación en la lista desplegable de versión. La última versión se selecciona de forma predeterminada.

1. Haga clic en **Aprobaciones** en el panel izquierdo.

1. (Opcional) Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas antes y 24 horas antes del plazo especificado.

1. Para añadir un aprobador, haga clic en **Aprobador** y empiece a escribir el nombre de un usuario o equipo.

1. Para añadir un revisor, haga clic en la casilla de verificación **Revisor** y empiece a escribir el nombre de un usuario o equipo.

   ![Agregar aprobador y fecha límite](assets/add-approver-and-deadline.png)

1. Repita el paso anterior para añadir más aprobadores o revisores.

## Crear una solicitud de revisión o aprobación de documento desde el panel Resumen de documento

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.

1. Haga clic en el documento que necesita, se abre el panel Resumen del documento para ese documento.

1. Seleccione la versión del documento para la que desea crear una aprobación en el menú desplegable de versión. La última versión se selecciona de forma predeterminada.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del panel Resumen del documento y haga clic en **Añadir**.

![Agregar aprobadores en el resumen del documento](assets/doc-summary-add-approvers.png)

1. (Opcional) Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas antes y 24 horas antes del plazo especificado.

1. Para añadir un aprobador, haga clic en **Aprobador** y empiece a escribir el nombre de un usuario o equipo.

1. Para añadir un revisor, haga clic en la casilla de verificación **Revisor** y empiece a escribir el nombre de un usuario o equipo.

   ![Agregar aprobador y fecha límite](assets/add-approver-and-deadline.png)

1. Repita el paso anterior para añadir más aprobadores o revisores.





<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
