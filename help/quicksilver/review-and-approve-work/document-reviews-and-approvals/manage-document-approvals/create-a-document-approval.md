---
product-area: documents
navigation-topic: approvals
title: Crear un flujo de trabajo de aprobación de documentos
description: Puede solicitar la aprobación de otros usuarios para un documento en Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OoGv4oNg6GkKeo-zoVi5lSxtPK3UE64-EYW21Mz7GRA
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
source-wordcount: 1473
ht-degree: 10%

---

# Crear un flujo de trabajo de aprobación de documentos

{{highlighted-preview}}

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
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de Workfront para administrar aprobaciones mediante el almacenamiento heredado de Workfront.</p>
<p>Cualquier paquete de flujo de trabajo para administrar aprobaciones mediante el almacenamiento en la nube de Adobe</p> </td> 
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

## Cree un flujo de trabajo de aprobación desde el panel de resumen en el área de documentos heredados de Producción

Si su organización está en el almacenamiento de Workfront, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento de Workfront, consulte [Diferencias entre el almacenamiento en la nube de Adobe y el almacenamiento de Workfront heredado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Para crear un flujo de trabajo de aprobación:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento que necesita y se abrirá el panel Resumen del documento para ese documento.

1. Seleccione la versión del documento para la que desea crear una aprobación en el menú desplegable de versión. La última versión está seleccionada de forma predeterminada.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** y haga clic en **Crear flujo de trabajo**.


1. Complete los siguientes detalles:

   <table>
   <tr>
   <td><strong>Nombre de la fase</strong></td>
   <td>Añada un nombre de fase. Puede cambiar el nombre por otro más descriptivo, como <em>Revisión inicial</em> o <em>Aprobación final</em>.</td>
   </tr>
   <tr>
   <td><strong>Añadir nombres o correos electrónicos</strong></td>
   <td>Empiece a escribir el nombre de un usuario o equipo que desee agregar como aprobador o revisor. Si solo tiene revisores, se les notificará y tendrán la opción de completar la revisión, pero no se requerirá ni se adoptará ninguna decisión.</td>
   </tr>
   <tr>
   <td><strong>Se requiere una decisión (opcional)</strong></td>
   <td>La primera persona que toma una decisión completa la etapa.</td>
   </tr>
   <tr>
   <td><strong>Fecha de vencimiento (opcional)</strong></td>
   <td>Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas y, a continuación, 24 horas antes de la fecha de vencimiento especificada.</td>
   </tr>
   </table>

1. (Opcional) Repita el paso anterior para agregar etapas adicionales según sea necesario.

   >[!NOTE]
   >
   >Si agrega varias fases, el flujo de trabajo de aprobación se ejecuta en el orden en que se enumeran las fases. Cuando se toman todas las decisiones necesarias, comienza la siguiente etapa y se bloquea la anterior.

   ![Detalles del documento](assets/new-stage.png)


<div class="preview">

## Cree un flujo de trabajo de aprobación desde el Panel de resumen en el área de documentos heredados en Vista previa

Si su organización está en el almacenamiento de Workfront, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento de Workfront, consulte [Diferencias entre el almacenamiento en la nube de Adobe y el almacenamiento de Workfront heredado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Para crear un flujo de trabajo de aprobación:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento que necesita y se abrirá el panel Resumen del documento para ese documento.

1. Seleccione la versión del documento para la que desea crear una aprobación en el menú desplegable de versión. La última versión está seleccionada de forma predeterminada.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** y haga clic en **Crear flujo de trabajo**.

1. Complete los siguientes detalles:

   <table>
   <tr>
   <td><strong>Nombre de la fase</strong></td>
   <td>Añada un nombre de fase. Puede cambiar el nombre por otro más descriptivo, como <em>Revisión inicial</em> o <em>Aprobación final</em>.</td>
   </tr>
   <tr>
   <td><strong>Añadir nombres o correos electrónicos</strong></td>
   <td>Empiece a escribir el nombre de un usuario o equipo que desee agregar como aprobador o revisor. Si solo tiene revisores, se les notificará y tendrán la opción de completar la revisión, pero no se requerirá ni se adoptará ninguna decisión.</td>
   </tr>
   <tr>
   <td><strong>Solo se requiere una decisión (opcional)</strong></td>
   <td>La primera persona que toma una decisión completa la etapa.</td>
   </tr>
   <tr>
   <td><strong>Vence el (opcional)</strong></td>
   <td>Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas y, a continuación, 24 horas antes de la fecha de vencimiento especificada.</td>
   </tr>
   <tr>
   <td><strong>Añadir mensaje personalizado (opcional)</strong></td>
   <td>Escriba un mensaje en el cuadro de texto <strong>Agregar mensaje personalizado</strong>. El mensaje aparece en la notificación de correo electrónico de aprobación y en la pestaña Aprobaciones de Workfront.
   <p>Al agregar una segunda etapa, <strong>Mostrar este mensaje en todas las etapas</strong> está seleccionado de manera predeterminada. Deje seleccionado para utilizar el mismo mensaje en cada fase. Para usar un mensaje diferente para cada fase, desactive <strong>Mostrar este mensaje en todas las fases</strong> y, a continuación, escriba el mensaje específico de cada fase en el cuadro de texto <strong>Agregar mensaje personalizado</strong> de cada fase según sea necesario.</p></td>
   </tr>
   </table>

1. (Opcional) Repita el paso anterior para agregar etapas adicionales según sea necesario.

   >[!NOTE]
   >
   >* Si agrega varias fases, el flujo de trabajo de aprobación se ejecuta en el orden en que se enumeran las fases. Cuando se toman todas las decisiones necesarias, comienza la siguiente etapa y se bloquea la anterior.
   >* Si edita un mensaje personalizado después de crear el flujo de trabajo de aprobación, se envía una notificación por correo electrónico actualizada a todos los participantes existentes. Si agrega un participante más adelante, el mensaje personalizado se incluye en su notificación por correo electrónico.

   ![Agregar mensaje personalizado a una fase](assets/add-custom-message.jpeg)

</div>


## Cree un flujo de trabajo de aprobación desde el panel Resumen en el nuevo área Documentos de Producción

Si su organización utiliza el almacenamiento en la nube de Adobe, verá la nueva área Documentos al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para crear un flujo de trabajo de aprobación:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento y luego en el icono **Aprobaciones** que encontrará a la derecha de la página.

   ![Agregar aprobadores en el resumen del documento](assets/approvals-icon-new.png)

1. Haga clic en **Crear flujo de trabajo** y rellene los siguientes detalles:

   <table>
   <tr>
   <td><strong>Nombre de la fase</strong></td>
   <td>Añada un nombre de fase. Puede cambiar el nombre por otro más descriptivo, como <em>Revisión inicial</em> o <em>Aprobación final</em>.</td>
   </tr>
   <tr>
   <td><strong>Añadir nombres o correos electrónicos</strong></td>
   <td>Empiece a escribir el nombre de un usuario o equipo que desee agregar como aprobador o revisor. Si solo tiene revisores, se les notificará y tendrán la opción de completar la revisión, pero no se requerirá ni se adoptará ninguna decisión.</td>
   </tr>
   <tr>
   <td><strong>Se requiere una decisión (opcional)</strong></td>
   <td>La primera persona que toma una decisión completa la etapa.</td>
   </tr>
   <tr>
   <td><strong>Fecha de vencimiento (opcional)</strong></td>
   <td>Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas y, a continuación, 24 horas antes de la fecha de vencimiento especificada.</td>
   </tr>
   </table>

1. (Opcional) Repita el paso anterior para agregar etapas adicionales según sea necesario.

   >[!NOTE]
   >
   >Si agrega varias fases, el flujo de trabajo de aprobación se ejecuta en el orden en que se enumeran las fases. Cuando se toman todas las decisiones necesarias, comienza la siguiente etapa y se bloquea la anterior.

   ![Detalles del documento](assets/new-stage.png)


<div class="preview">

## Cree un flujo de trabajo de aprobación desde el panel Resumen en el nuevo área Documentos de la vista previa

Si su organización utiliza el almacenamiento en la nube de Adobe, verá la nueva área Documentos al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para crear un flujo de trabajo de aprobación:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento y luego en el icono **Aprobaciones** que encontrará a la derecha de la página.

   ![Agregar aprobadores en el resumen del documento](assets/approvals-icon-new.png)

1. Haga clic en **Crear flujo de trabajo** y rellene los siguientes detalles:

   <table>
   <tr>
   <td><strong>Nombre de la fase</strong></td>
   <td>Añada un nombre de fase. Puede cambiar el nombre por otro más descriptivo, como <em>Revisión inicial</em> o <em>Aprobación final</em>.</td>
   </tr>
   <tr>
   <td><strong>Añadir nombres o correos electrónicos</strong></td>
   <td>Empiece a escribir el nombre de un usuario o equipo que desee agregar como aprobador o revisor. Si solo tiene revisores, se les notificará y tendrán la opción de completar la revisión, pero no se requerirá ni se adoptará ninguna decisión.</td>
   </tr>
   <tr>
   <td><strong>Solo se requiere una decisión (opcional)</strong></td>
   <td>La primera persona que toma una decisión completa la etapa.</td>
   </tr>
   <tr>
   <td><strong>Vence el (opcional)</strong></td>
   <td>Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas y, a continuación, 24 horas antes de la fecha de vencimiento especificada.</td>
   </tr>
   <tr>
   <td><strong>Añadir mensaje personalizado (opcional)</strong></td>
   <td>Escriba un mensaje en el cuadro de texto <strong>Agregar mensaje personalizado</strong>. El mensaje aparece en la notificación de correo electrónico de aprobación y en la pestaña Aprobaciones de Workfront.
   <p>Al agregar una segunda etapa, <strong>Mostrar este mensaje en todas las etapas</strong> está seleccionado de manera predeterminada. Deje seleccionado para utilizar el mismo mensaje en cada fase. Para usar un mensaje diferente para cada fase, desactive <strong>Mostrar este mensaje en todas las fases</strong> y, a continuación, escriba el mensaje específico de la fase en el cuadro de texto <strong>Agregar mensaje personalizado</strong> de cada fase.</p></td>
   </tr>
   </table>

1. (Opcional) Repita el paso anterior para agregar etapas adicionales según sea necesario.

   >[!NOTE]
   >
   >* Si agrega varias fases, el flujo de trabajo de aprobación se ejecuta en el orden en que se enumeran las fases. Cuando se toman todas las decisiones necesarias, comienza la siguiente etapa y se bloquea la anterior.
   >* Si edita un mensaje personalizado después de crear el flujo de trabajo de aprobación, se envía una notificación por correo electrónico actualizada a todos los participantes existentes. Si agrega un participante más adelante, el mensaje personalizado se incluye en su notificación por correo electrónico.

   ![Agregar mensaje personalizado a una fase](assets/add-custom-message.jpeg)

</div>



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
