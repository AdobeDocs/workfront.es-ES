---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Información general sobre el progreso y el estado de la revisión
description: En el área Documentos puede consultar información sobre el progreso de una revisión en el proceso de revisión y ver un resumen general del estado de decisión de la revisión.
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 97%

---

# Información general sobre el progreso y el estado de la revisión

En el área Documentos puede consultar información sobre el progreso de una revisión en el proceso de revisión y ver un resumen general del estado de decisión de la revisión.

## Información general sobre el progreso de la revisión

El progreso de la revisión indica el trabajo realizado en una revisión desde el momento en que se envía a los destinatarios hasta que estos toman una decisión sobre ella. Los iconos de progreso, S, O, C y D, aparecen junto al nombre de la revisión y proporcionan información sobre su progreso.

![Modificar progreso existente](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Icono de progreso</strong> </p> </td> 
   <td> <p><strong>Descripción</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>Enviada</strong> </p> </td> 
   <td> <p>La revisión se ha enviado a los destinatarios asignados.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Se abrió</strong> </p> </td> 
   <td> <p>Todos los destinatarios asignados abren la revisión o la página de detalles de la revisión.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Comentarios realizados</strong> </p> </td> 
   <td> <p>Todos los destinatarios asignados realizan al menos un comentario sobre la revisión.</p> <p>Si no hay revisores asignados a la revisión, el icono <strong>C</strong> no aparece en la barra de progreso.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>Se tomó una decisión</strong> </p> </td> 
   <td> <p>Todos los aprobadores asignados toman una decisión sobre la revisión. Todos los aprobadores asignados toman una decisión sobre la revisión, a menos que el creador de la revisión especifique que solo se necesita una decisión.</p> <p>Si no hay aprobadores (responsables de la toma de decisiones) designados para la revisión, el icono <strong>D</strong> no aparece en la barra de progreso. </p> </td> 
  </tr> 
 </tbody> 
</table>

Los iconos de progreso pueden aparecer en los siguientes colores para indicar cierta información sobre el progreso de la revisión:

* **Verde**: completa.
* **Blanco**: incompleta.
* **Naranja**: incompleta y la fecha de entrega es en menos de 24 horas.
* **Rojo**: incompleta y fuera de plazo.

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## Información general sobre el estado de la revisión

El estado de la revisión muestra el estado de las decisiones que se requieren para la revisión. El estado de la prueba lo determina el participante “en el peor de los casos”. Por ejemplo, supongamos que hay tres decisiones sobre la revisión: dos tienen el estado **Aceptado** y una tiene el estado **Rechazado**. La decisión “en el peor de los casos” de **Rechazada** prevalece sobre las demás decisiones y el estado general de la revisión se muestra como **Rechazada**. 

![Progreso existente de edición de revisión](assets/proof-edit-existing-progress-350x62.png)

Las opciones de estado estándar son las siguientes:

* Pendiente
* Aprobado
* Aprobado con cambios
* Es necesario hacer cambios
* No es relevante

Si las decisiones personalizadas se configuran en la cuenta, las opciones de estado reflejarán la configuración de decisiones personalizada.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->
