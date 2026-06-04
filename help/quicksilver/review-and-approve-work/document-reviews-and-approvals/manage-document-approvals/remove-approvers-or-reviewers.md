---
product-area: documents
navigation-topic: approvals
title: Quitar aprobadores o revisores de un flujo de trabajo de aprobación de documentos
description: Puede quitar aprobadores o revisores individuales de un documento.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/zSKSGDHN8vNwozS4R-GYqsxP52Iob6SqcY0G32-3FyQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 544
ht-degree: 36%

---

# Quitar aprobadores o revisores de un flujo de trabajo de aprobación de documentos

Puede quitar aprobadores o revisores individuales de un recurso o documento después de haberlos asignado.

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
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de Workfront para administrar aprobaciones mediante el almacenamiento heredado de Workfront.</p>
<p>Cualquier paquete de flujo de trabajo para administrar aprobaciones mediante el almacenamiento en la nube de Adobe</p>  </td> 
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
   <td> <p>Acceso de administración al objeto asociado con el acceso de solicitud o la aprobación </p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Eliminar aprobadores o revisores de un flujo de trabajo de aprobación en el área de documentos heredados

Si su organización está en el almacenamiento de Workfront, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento de Workfront, consulte [Diferencias entre el almacenamiento en la nube de Adobe y el almacenamiento de Workfront heredado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Para eliminar aprobadores o revisores de un flujo de trabajo de aprobación:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento que necesita y se abrirá el panel Resumen del documento para ese documento.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del panel Resumen del documento.

1. Haga clic en **Editar flujo de trabajo**.

1. Busque el participante que desea eliminar y haga clic en el icono **Eliminar** que aparece junto a su nombre.

   La solicitud de aprobación o revisión se elimina y el aprobador recibe una notificación que le informa de que ya no necesita su aprobación. También se elimina su acceso compartido relacionado con la aprobación.

   ![editar flujo de trabajo de aprobación](assets/edit-approval-in-legacy.png)

1. (Opcional) Para cambiar la función de un aprobador a un revisor o viceversa, haga clic en el menú desplegable situado junto al nombre de usuario y seleccione la nueva función.

1. Repita el paso anterior para eliminar los aprobadores o revisores adicionales.

</div>


## Eliminar aprobadores o revisores a un flujo de trabajo de aprobación en el área de nuevos documentos

Si su organización utiliza el almacenamiento en la nube de Adobe, verá la nueva área Documentos al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para crear un flujo de trabajo de aprobación:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento y luego en el icono **Aprobaciones** que encontrará a la derecha de la página.

   ![Agregar aprobadores en el resumen del documento](assets/approvals-icon-new.png)


1. Haga clic en **Editar flujo de trabajo**.

1. Busque el participante que desea eliminar y haga clic en el icono **Eliminar** que aparece junto a su nombre.

   La solicitud de aprobación o revisión se elimina y el aprobador recibe una notificación que le informa de que ya no necesita su aprobación.

1. (Opcional) Para cambiar la función de un aprobador a un revisor o viceversa, haga clic en el menú desplegable situado junto al nombre de usuario y seleccione la nueva función.

1. Repita el paso anterior para eliminar los aprobadores o revisores adicionales.

   ![quitar participantes de una fase](assets/add-or-remove-participants.png)

1. Haga clic en **Guardar**.