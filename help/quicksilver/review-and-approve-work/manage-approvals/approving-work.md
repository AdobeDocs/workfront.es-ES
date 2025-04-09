---
product-area: projects
navigation-topic: approvals
title: Aprobación del trabajo
description: Aprobación del trabajo
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 4038180d69d4a8027f33b5bafd2104c7c6916b82
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 19%

---

# Approving work

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

If you are set as an approver, you should regularly review what work is awaiting your approval.

Para obtener información acerca de cómo crear procesos de aprobación, consulte [Crear un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Para obtener información acerca de cómo asociar aprobaciones con trabajo en Workfront, consulte [Asociar un proceso de aprobación nuevo o existente con trabajo](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Vista o acceso superior a los objetos asociados con las aprobaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Vista o permisos superiores a los objetos asociados a aprobaciones</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Localización de aprobaciones en Adobe Workfront

Puede ver y administrar las aprobaciones en varias áreas de Workfront.

Para obtener más información sobre cómo ver los elementos que esperan aprobaciones o los elementos que usted mismo envió para su aprobación, consulte [Ver aprobaciones](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Aprobar trabajo desde el área de Inicio

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) Click **Customize** to add the **My Approvals** widget.
1. (Condicional) Haga clic en el menú desplegable **Filtro** y, a continuación, seleccione **Todos** para ver las aprobaciones que se le han asignado y delegado.

   >[!NOTE]
   >
   >Las aprobaciones asignadas a roles o grupos de trabajos no se muestran en Inicio. Las aprobaciones asignadas a los equipos se muestran en el widget Mis aprobaciones para cada miembro del equipo.


1. Seleccione el elemento en el que desea tomar una decisión de aprobación.

   ![Widget de mis aprobaciones](assets/my-approvals-widget.png)

1. Haga clic en una de las opciones disponibles al tomar una decisión de aprobación en el panel derecho. Las siguientes opciones se muestran en la esquina superior derecha de la página, según el tipo de elemento que apruebe:

   <table>
   <tr>
      <td>
      <p><strong>Acceso</strong></p>
      </td>
      <td>
      <p><strong>Elementos de trabajo</strong></p>
      </td>
      <td>
      <p><strong>Documentos</strong></p>
      </td>
      <td>
      <p><strong>Pruebas</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>Conceder</li>
      <li>Ignorar</li>
      </ul>
      You can adjust the level of access in the <b>Change access</b> drop-down menu if desired.
      </td>
      <td>
         <ul>
         <li>Aprobar</li>
         <li>Rechazar</li>
         </ul>
      You can leave a comment with your decision by click ing the drop-down menu in the decision button.
      </td>
      <td>
   Assigned as an approver
         <ul>
         <li>Aprobar</li>
         <li>Aprobar con cambios</li>
         <li>Necesita trabajo</li>
         </ul>
   Assigned as a reviewer
         <ul>
         <li>Completar mi revisión</li>
         </ul>
      Las opciones de esta columna se aplican únicamente a las aprobaciones unificadas. Las aprobaciones de documentos heredados aparecen igual que las aprobaciones de elementos de trabajo. 
      </td>
      <td>
         <ul>
         <li>Ir a la revisión</li>
         </ul>
         La decisión se toma en el visualizador de pruebas. Para obtener información acerca de cómo revisar una revisión, vea <a href="../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Revisar pruebas en Adobe Workfront</a>.
      </td>
   </tr>
   </table>

Después de tomar una decisión, la aprobación se elimina del widget Mi aprobación.


## Aprobar el trabajo directamente desde un proyecto, tarea o problema

When a project, task, or issue is pending approval, you can approve or reject the approval directly from the project, task, or issue. You can also view details regarding the approval process.

To approve work directly from a project, task, or issue:

1. Go to the project, task, or issue that requires your approval.

   Approval information regarding the current approval process of a project, task, or issue displays in the item&#39;s header.

   ![Current approval process in project header](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   Está disponible la siguiente información sobre la aprobación:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Estado</td> 
      <td>El estado actual del proyecto, tarea o problema. This is the current status of the item that is pending the approval. El estado se aprueba después de aprobar cada fase del proceso de aprobación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approval stages</td> 
      <td>Las fases del proceso de aprobación. <br>La fase actual que está pendiente de aprobación se muestra como Pendiente Las fases que ya se han aprobado se muestran como Aprobadas ; las fases que aún no se han aprobado se muestran como No iniciadas</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Aprobar** o **Rechazar**, dependiendo de si desea aprobar o rechazar el proceso de aprobación.\
   La fase de aprobación que estaba pendiente de aprobación ahora se aprueba y el proceso de aprobación pasa a la siguiente fase. El estado se aprueba después de que se hayan aprobado todas las etapas.

## Aprobar un documento directamente desde un documento

1. Vaya al área de documentos que contiene el documento que requiere su aprobación.
1. Seleccione el documento y haga clic en **Aprobar**, **Cambios** o **Rechazar**.\
   ![Aprobar documento](assets/approval-approve-document-350x215.png)\
   ![Aprobación de documento](assets/document-approval-350x199.png)

1. (Opcional) Si se ha generado una prueba para el documento, puede aprobarlo en la interfaz de revisión, tal como se describe en [Aprobar un documento a partir de una revisión](#approve-a-document-from-a-proof).

## Aprobar un documento a partir de un correo electrónico de notificación de aprobación

Depending on your notification settings, you may receive emails notifying you about documents for which other users need you to make an approval decision. When you receive an email containing a **Make Approval Decision** button, you can can start the approval process directly from the email:

1. From the email, click **Make Approval Decision** to open the Document Details page for the proof .
1. Do any of the following to review the document:

   * View the metadata about the document.
   * If a proof has been created for reviewing the document with markup and comments, click **Open proof** ![Open proof](assets/open-proof-icon-qs.png) near the upper right corner and review the proof.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Para obtener información acerca de la revisión de pruebas, vea [Revisar pruebas en Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Haga clic en una opción **Decisión** en la esquina superior derecha para aprobar, aprobar con cambios o rechazar el documento.

## Approve a document from a proof {#approve-a-document-from-a-proof}

You can approve a document within the proofing viewer. For more information, see [Make a decision on a proof in the proofing viewer](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) in the article [Make a decision on a proof in the proofing viewer](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
