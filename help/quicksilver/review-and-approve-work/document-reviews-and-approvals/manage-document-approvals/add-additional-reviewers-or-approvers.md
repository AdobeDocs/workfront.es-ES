---
product-area: documents
navigation-topic: approvals
title: Agregar aprobadores o revisores adicionales a un flujo de trabajo de aprobación de documentos
description: Puede añadir aprobadores o revisores adicionales a un documento que ya tenga aprobaciones pendientes.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 24%

---

# Agregar aprobadores o revisores adicionales a un flujo de trabajo de aprobación de documentos

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

Puede agregar aprobadores o revisores adicionales a un flujo de trabajo de aprobación de documentos que ya tenga aprobaciones pendientes.

>[!IMPORTANT]
>
>El contenido de este artículo hace referencia a la funcionalidad actualizada de aprobación de documentos que solo está disponible para cuentas específicas. Para obtener información sobre los procesos de aprobación estándar, consulte los artículos enumerados en [Aprobaciones de trabajo](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
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
   <td> <p>Acceso de visualización o superior a Proyectos, Tareas, Problemas, Plantillas, Portafolios, Programas, Informes, Tableros, Calendarios y Documentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de visualización o superior al objeto asociado al acceso de solicitud o la aprobación </p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Agregue aprobadores o revisores adicionales desde la página Detalles del documento en su entorno de producción

1. Vaya a la página del documento haciendo clic en el nombre del documento y, a continuación, seleccione la versión del documento a la que desea agregar un aprobador o revisor en el menú desplegable de la versión. La última versión está seleccionada de forma predeterminada.

1. Seleccione **Aprobaciones** en el panel izquierdo. Aquí se enumeran todos los aprobadores y revisores existentes.

1. Para agregar un aprobador, asegúrese de que la casilla de verificación **Aprobador** esté marcada y, a continuación, empiece a escribir en el cuadro de texto **Revisores**. Puede añadir usuarios o equipos de Workfront por el nombre. Si desea añadir un revisor en su lugar, simplemente anule la selección de la casilla de verificación **Aprobador** antes de escribir.

1. Repita el paso anterior para añadir más aprobadores o revisores.

## Agregar aprobadores o revisores adicionales del resumen del documento en el entorno de producción

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.

1. Haga clic en el documento que necesita y se abrirá el panel Resumen del documento.

1. Seleccione la versión del documento a la que desea agregar un aprobador o revisor en el menú desplegable Versión. La última versión está seleccionada de forma predeterminada.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del panel Resumen del documento, donde se enumeran todos los aprobadores y revisores existentes. Para agregar un aprobador, asegúrese de que la casilla de verificación **Aprobador** esté marcada y, a continuación, empiece a escribir en el cuadro de texto **Revisores**. Puede añadir usuarios o equipos de Workfront por el nombre. Si desea añadir un revisor en su lugar, simplemente anule la selección de la casilla de verificación **Aprobador** antes de escribir.

1. Repita el paso anterior para añadir más aprobadores o revisores.

<div class="preview">

## Agregue aprobadores o revisores adicionales del Resumen del documento en el entorno de vista previa del área de documentos heredados

Si su organización está en el almacenamiento de Workfront, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento de Workfront, consulte [Almacenamiento de Workfront frente al almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Para agregar aprobadores o revisores adicionales desde el resumen de documento:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento que necesita y se abrirá el panel Resumen del documento para ese documento.

1. Seleccione la versión del documento a la que desea agregar un aprobador o revisor en el menú desplegable Versión. La última versión está seleccionada de forma predeterminada.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** y haga clic en **Editar flujo de trabajo**.

   ![editar flujo de trabajo de aprobación](assets/edit-approval-in-legacy.png)

1. Busque el escenario en el que desea agregar aprobadores o revisores y, a continuación, agregue el nombre del usuario o correo electrónico en el cuadro de texto. También puede agregar todo un equipo si es necesario.

1. Una vez agregado el nombre, seleccione si es un aprobador o revisor.

   ![lista desplegable de aprobadores o revisores](assets/choose-approver-or-reviewer.png)

1. Repita los pasos del 5 al 6 para agregar más aprobadores o revisores.
Una vez guardado, los participantes añadidos reciben una notificación por correo electrónico que indica que se necesita su aprobación o revisión en el documento.

</div>


## Agregar aprobadores o revisores adicionales del Resumen del documento en el área de nuevos documentos

Si su organización utiliza el almacenamiento empresarial, verá el área de nuevos documentos al acceder a ellos en Workfront. Para obtener más información acerca del almacenamiento empresarial, vea [Información general sobre el almacenamiento empresarial](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento y luego en el icono **Aprobaciones** que encontrará a la derecha de la página.

   ![Agregar aprobadores en el resumen del documento](assets/approvals-icon-new.png)


1. Haga clic en **Editar flujo de trabajo**.

1. Busque el escenario en el que desea agregar aprobadores o revisores y, a continuación, agregue el nombre del usuario o correo electrónico en el cuadro de texto. También puede agregar todo un equipo si es necesario.

1. Una vez agregado el nombre, seleccione si es un aprobador o revisor.

   ![lista desplegable de aprobadores o revisores](assets/choose-approver-or-reviewer.png)

1. Repita los pasos del 5 al 6 para agregar más aprobadores o revisores.
Una vez guardado, los participantes añadidos reciben una notificación por correo electrónico que indica que se necesita su aprobación o revisión en el documento.







<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![Home icon](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->
