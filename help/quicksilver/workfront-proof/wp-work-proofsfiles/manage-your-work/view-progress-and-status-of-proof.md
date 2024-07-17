---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Ver el progreso y el estado de una prueba en  [!DNL Workfront Proof]
description: El progreso de la prueba indica el trabajo realizado en una prueba desde el momento en que se envía la prueba a los revisores hasta el momento en que toman una decisión sobre la prueba.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 8fd85595-1403-490e-9d52-2ba5b01457b7
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Ver el progreso y el estado de una prueba en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

## Comprender el progreso de revisión

El progreso de la prueba indica el trabajo realizado en una prueba desde el momento en que se envía la prueba a los revisores hasta el momento en que toman una decisión sobre la prueba.

* [Iconos de progreso](#progress-icons)
* [Niveles de progreso de prueba](#levels-of-proof-progress)

### Iconos de progreso {#progress-icons}

Los iconos de progreso S, O, C y D aparecen en la barra de progreso para indicar el progreso de la prueba.

![proof_edit_existing_progress.png](assets/proof-edit-existing-progress-350x78.png)

Indican la siguiente información sobre una prueba:

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
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt="proof_progress_sent_icon.png"> </p> </td> 
   <td> <p><strong>Enviado</strong>. La prueba se ha enviado a los revisores.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-opened-icon.png" alt="proof_progress_opened_icon.png"> </p> <p> </p> </td> 
   <td> <p><strong>Abierto</strong>. Un revisor ha abierto la página de detalles de la prueba o la propia prueba en el visor de pruebas.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-comment-icon.png" alt="proof_progress_comment_icon.png"> </p> </td> 
   <td> <p><strong>Comentarios</strong>. Los revisores (usuarios que pueden hacer comentarios) han hecho comentarios sobre la prueba.</p> <p>Si no se designa ningún revisor para la prueba, este icono no se muestra.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt="proof_progress_decision_icon.png"> </p> </td> 
   <td> <p><strong>Decisión</strong>. Un revisor ha tomado una decisión sobre la prueba.</p> <p>Si no se designan aprobadores (responsables de la toma de decisiones) para la prueba, este icono no se muestra. </p> </td> 
  </tr> 
 </tbody> 
</table>

Estos iconos pueden aparecer en los colores siguientes para indicar cierta información sobre el progreso de la prueba:

* **Verde**. Completado.
* **Blanco**. No completo.
* **naranja**. No se ha completado y la fecha de entrega es en menos de 24 horas.
* **Rojo**. No se ha completado y ha pasado el plazo.

### Niveles de progreso de prueba {#levels-of-proof-progress}

Workfront Proof utiliza los iconos de progreso para rastrear el progreso de una prueba en cada uno de los siguientes niveles:

* Para cada revisor, en función de la actividad de esa persona en la prueba.
* Para cada fase, en función del progreso del revisor en el escenario que esté más retrasado en el proceso de revisión. Para obtener más información, consulte [Resumen de las fases del flujo de trabajo automatizado](../../../review-and-approve-work/proofing/proofing-overview/stages.md).
* Para la prueba, en función del progreso de la etapa (grupo de revisores), que es el que más se retrasa en el proceso de prueba.

Para ver un ejemplo de cómo determina [!DNL Workfront Proof] el progreso con el revisor o la fase que está más atrasada, supongamos que tres revisores de una prueba necesitan tomar una decisión. Si dos de ellos han tomado su decisión pero el tercero no, la barra de progreso de la prueba no muestra el D en verde debido a la decisión pendiente.

Si la configuración [!UICONTROL Responsable principal de la toma de decisiones] se selecciona en una prueba y el responsable principal de la toma de decisiones envía una decisión, el ID de la barra de progreso de la prueba se vuelve verde para todos los revisores porque no se requieren otras decisiones.

Del mismo modo, si se selecciona la configuración [!UICONTROL Solamente se requiere una decisión] en una prueba y cualquier revisor envía una decisión, el ID de la barra de progreso de la prueba se vuelve verde para todos los revisores porque no se requieren otras decisiones.

## Explicación del estado de prueba

El estado de la prueba muestra el estado de las decisiones que se requieren para la prueba.

![proof_edit_existing_status.png](assets/proof-edit-existing-status-350x78.png)\
Las opciones de estado estándar son:

* Pendiente
* Aprobado
* Aprobado con cambios
* Cambios necesarios
* No relevante

Si las decisiones personalizadas se configuran en la cuenta, las opciones de estado reflejarán la configuración de decisiones personalizada.

El estado de la prueba lo determina el participante &quot;en el peor de los casos&quot;. Por ejemplo, supongamos que hay tres decisiones sobre la prueba: dos tienen el estado **Aceptado** y una tiene el estado **Rechazado**. La decisión &quot;en el peor de los casos&quot; de Rechazado sobrepasa las reglas de las demás decisiones y el estado general de la prueba se muestra como **Rechazado**.

## Visualización del progreso y el estado {#viewing-progress-and-status}

Puede ver el progreso y el estado de las pruebas, las fases y los revisores de cada fase.

* [Resumen de revisión](#proof-summary)
* [Menú Acciones de fase](#stage-actions-menu)
* [En la sección [!UICONTROL Resumen], también puede acceder a los menús de acciones del revisor, siempre que tenga derechos de edición sobre la prueba. Para obtener más información, consulte Perfiles de permisos de pruebas en Workfront Proof y Administrar funciones de prueba en Workfront Proof. El menú [!UICONTROL Acciones del revisor] (1) aparece cuando pasa el ratón por encima de los detalles del revisor y le permite:](#in-the-summary-section-you-can-also-access-the-reviewer-actions-menus-provided-you-have-edit-rights-on-the-proof-for-more-information-see-proof-permissions-profiles-in-workfront-proof-and-manage-proof-roles-in-workfront-proof-the-reviewer-actions-menu-1-appears-when-you-hover-over-the-reviewer-s-details-and-allows-you-to)
* [Menú Acciones de revisión](#proof-actions-menu)

### Resumen de revisión {#proof-summary}

Cada prueba de la carpeta tiene un resumen ampliable que le permite ver y editar rápidamente los detalles de la prueba.

Para expandir o contraer el resumen:

1. Haga clic en la flecha a la izquierda de la prueba en el panel o en cualquier vista de lista.

![Summary_expandable.png](assets/summary-expandable-350x68.png)

El resumen incluye lo siguiente:

* Flujos de trabajo (2)
* Versión (3)
* Carpeta (4)
* Estado (5)\
   ![summary_2.png](assets/summary-2-350x160.png)

En resumen, puede ver y editar los siguientes detalles de la prueba:

* Progreso de la prueba (1)
* Progreso de cada etapa (2)
* Plazo establecido para la fase (3)
* Detalles del revisor:

   * Número de comentarios y respuestas de cada revisor (4)
   * Progreso de cada revisor (5)
   * Decisión (si una decisión ha incluido firmas electrónicas, se mostrará un icono junto a la decisión que lo indique). (6)
   * Función en la prueba (7)
   * Configuración de alertas de correo electrónico (8)

>[!NOTE]
>
>La capacidad para editar los detalles de la revisión depende de los derechos que tenga sobre la revisión (consulte [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) y [Administrar roles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![summary_details_3.png](assets/summary-details-3-350x160.png)

### Menú [!UICONTROL Acciones de ensayo]  {#stage-actions-menu}

Cada fase del flujo de trabajo tiene un menú independiente, que le permite realizar acciones masivas relacionadas con los revisores de esa fase.

El menú [!UICONTROL Acciones de ensayo] aparece cuando pasa el ratón por encima de la sección Fase (1) y le permite

* [!UICONTROL Mensaje completo] (2)
* [!UICONTROL Compartir] (3)
* [!UICONTROL Eliminar fase] (4)

>[!NOTE]
>
>La disponibilidad de estas opciones depende de los derechos que tenga sobre la revisión (consulte [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) y [Administrar roles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![menú_acciones_fase.png](assets/stage-actions-menu-350x161.png)

En la sección Resumen, también puede acceder a los menús de acciones del revisor, siempre que tenga derechos de edición sobre la prueba. Para obtener más información, consulte [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) y [Administrar roles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md). El menú de acciones del Revisor (1) aparece cuando pasa el ratón por encima de los detalles del Revisor y le permite:

* Enviar un mensaje al revisor (2)
* Editar detalles del revisor (3): permite editar el nombre para mostrar, la función de prueba y las alertas de correo electrónico de ese revisor
* Conviértalos en propietarios de la prueba (4)
* Conviértalos en el principal responsable de la toma de decisiones (5)
* Quitar de la prueba (6)

>[!NOTE]
>
>La visibilidad de estas opciones depende de los derechos que tenga sobre la revisión (consulte [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) y [Administrar roles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Menú_acciones_del_revisor.png](assets/reviewer-actions-menu-350x135.png)

### Menú Acciones de revisión {#proof-actions-menu}

Cada revisión también tiene un menú (1) que le permite realizar las siguientes acciones:

* Puede acceder a la página de detalles de la revisión (2)
* Compartir la prueba con otras personas (3)
* Enviar un mensaje a los revisores (4)
* Crear una nueva versión de la revisión (5)
* Copiar la prueba (6)
* Descargar el archivo original (7)
* Compartir enlaces de revisión (8)
* Imprimir comentarios (9)
* Solicitar un resumen de Excel de la prueba (10)
* Bloquear la revisión (11)
* Eliminar la revisión (12)

![Proof_actions_menu__1_.png](assets/proof-actions-menu--1--350x158.png)

>[!NOTE]
>
>La disponibilidad de estas opciones depende de los derechos que tenga sobre la revisión (consulte [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) y [Administrar roles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

Para obtener información sobre cómo ver el progreso y el estado de la revisión en [!DNL Workfront], consulte [Ver progreso y estado](#viewing-progress-and-status).

Para obtener información sobre el progreso y el estado de visualización en el Visor de corrección de escritorio, consulte [Revisar un flujo de trabajo en el visor de revisión](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-workflow.md).
