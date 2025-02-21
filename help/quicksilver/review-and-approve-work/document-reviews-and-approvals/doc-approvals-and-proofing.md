---
product-area: documents
navigation-topic: approvals
title: Usar aprobaciones y revisiones de documentos nuevas conjuntamente
description: Puede utilizar nuevas aprobaciones de documentos con revisión.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
source-git-commit: 8270a107ba2501eddbb27f52c843c337aa1f8a99
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 7%

---

# Usar aprobaciones y revisiones de documentos nuevas conjuntamente

Las nuevas aprobaciones de documentos en Workfront presentan un nuevo conjunto de funciones para ayudarle a revisar y aprobar documentos. Puede utilizar el nuevo flujo de trabajo de aprobaciones de documentos con el visor de revisiones existente para agregar comentarios y marcas a los documentos que se están revisando.

Existen algunas diferencias clave en el flujo de trabajo al utilizar juntas nuevas aprobaciones de documentos y revisiones:

* Los botones de decisión no aparecen en el visor de pruebas

* Los participantes se muestran en el documento Resumen, no en el flujo de trabajo de revisión

* Los detalles enviados, abiertos, comentarios y decisiones (SOCD) de la lista de documentos están relacionados con la revisión y no reflejan el estado de decisión del documento.

## Cargar un documento y crear una prueba

1. Vaya al proyecto, tarea o problema en el que desee agregar un documento nuevo.
1. Haga clic en la ficha **Documentos** y, a continuación, haga clic en el menú desplegable **Agregar nuevo**.
O
Arrastre y suelte el documento en la lista de documentos.

   >[!NOTE]
   >
   >Si tiene la opción **Generar pruebas automáticamente al cargar documentos** habilitada en su perfil de usuario, el sistema crea automáticamente una prueba simple.

1. Pase el ratón sobre el documento, luego haga clic en el vínculo **Crear revisión** que aparece debajo del nombre del documento y seleccione **Revisión simple**. Debe crear una prueba sencilla, ya que no utilizará el flujo de trabajo de prueba para las aprobaciones.

Los usuarios asignados como participantes pueden utilizar el visor de revisión para agregar comentarios y marcas en el documento. Continúe con la siguiente sección para aprender a agregar participantes de la revisión.

## Abra el documento Resumen y asigne participantes

Tiene la opción de asignar revisores, aprobadores o una combinación de ambos:

* **Los revisores** pueden agregar comentarios y marcar los recursos. Una vez finalizada, puede marcar su revisión como completada. No es necesario marcar la revisión como completada para que el documento avance en el proceso de aprobación.
* **Los aprobadores** pueden agregar comentarios y marcar los recursos. Deben tomar la decisión de adelantar el proceso de aprobación.

Para asignar participantes:

1. Seleccione el documento que ha cargado y abra el documento Resumen.
   ![Abrir resumen del documento](assets/open-doc-summary.png)

1. Desplácese hacia abajo hasta la sección Aprobaciones y haga clic en **Agregar**.

1. (Opcional) Elija una plantilla de aprobación existente. Los usuarios con una licencia Standard pueden crear plantillas de aprobación reutilizables desde el área de Configuración. Para obtener más información, consulte [Crear una plantilla de aprobación para recursos y documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Opcional) Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas antes y 24 horas antes del plazo especificado.

1. Para agregar un aprobador, haga clic en el botón Aprobador y y empiece a escribir el nombre de un usuario o equipo.

1. Para agregar un revisor, haga clic en el botón Revisor y empiece a escribir el nombre de un usuario o equipo.

   ![Agregar aprobadores](assets/add-approvers.png)

1. Una vez que haya agregado todos los revisores y aprobadores, haga clic en **Enviar solicitud**. Los participantes reciben notificaciones por correo electrónico.

## Cree una nueva versión según sea necesario

Si necesita otra ronda de revisión y aprobación, puede crear una nueva versión de prueba.  <!-- and add the previous participants, new participants, or a mix of both. --> Puede ver información sobre versiones anteriores y participantes en el documento Resumen.

Para agregar una nueva versión:

1. Arrastre y suelte el nuevo archivo sobre el documento anterior en Workfront. Esto crea automáticamente una nueva versión.

1. Una vez que termine la carga del documento, selecciónelo y haga clic en **Crear revisión** > **Revisión simple**.

1. Vuelva a seleccionar el documento y abra el documento Resumen.
   ![Abrir resumen del documento](assets/open-doc-summary.png)

1. Desplácese hacia abajo hasta la sección Aprobaciones y haga clic en **Agregar**.

1. (Opcional) Elija una plantilla de aprobación existente. Los usuarios con una licencia Standard pueden crear plantillas de aprobación reutilizables desde el área de Configuración. Para obtener más información, consulte [Crear una plantilla de aprobación para recursos y documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Opcional) Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas antes y 24 horas antes del plazo especificado.

1. Para agregar un aprobador, haga clic en el botón Aprobador y empiece a escribir el nombre de usuario o equipo <span class="preview">, o bien elija un aprobador de la versión anterior.</span>

1. Para agregar un revisor, haga clic en el botón Revisor y empiece a escribir el nombre de un usuario o equipo <span class="preview">, o bien elija un revisor de la versión anterior. </span>

   ![Agregar aprobadores](assets/add-approvers.png)

1. Una vez que haya agregado todos los revisores y aprobadores, haga clic en **Enviar solicitud**. Los participantes reciben notificaciones por correo electrónico.

<!-- add info about reusing previous participants once released -->


## Revise la prueba y tome una decisión

El documento no pasa a un estado aprobado hasta que todos los aprobadores asignados eligen &quot;aprobado&quot;.

Si algún aprobador elige &quot;necesita trabajo&quot;, el estado del documento cambia inmediatamente a Necesita trabajo. El documento deberá revisarse y cargarse como una nueva versión con un nuevo flujo de trabajo de aprobación.

>[!IMPORTANT]
>
>Los botones de decisión del documento no aparecen en el visor de pruebas. Debe volver a la página Resumen del documento o Detalles del documento para tomar una decisión o marcar como completada la revisión.

Para revisar y aprobar un documento:

1. Vaya a la notificación de correo electrónico de revisión y haga clic en **Ir a revisión**.

1. Una vez que estés en Workfront, haz clic en **Ir a la revisión**.

1. Revise el contenido y agregue cualquier comentario o marca. Para obtener más información acerca de cómo usar el visor de revisión, vea [Revisar pruebas en Adobe Workfront: índice de artículos](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Cuando termine con la revisión, cierre el visor de pruebas.

1. Si se encuentra en la página Detalles del documento, los botones de decisión se encuentran en la esquina superior derecha de la pantalla.

1. Elija una de las siguientes decisiones:

   * **Aprobar**: el documento no necesita cambios y está listo para usarse.
   * **Aprobar con cambios**: el documento necesita cambios y está listo para usarse una vez que se hayan realizado. No se requiere una aprobación adicional.
   * **Necesita trabajo**: el documento necesita cambios y no está listo para usarse. Una vez realizados los cambios especificados, el documento debe cargarse como una nueva versión y pasar por otra ronda de aprobaciones. Para obtener más información sobre cómo cargar una nueva versión, consulte [Crear una nueva versión según sea necesario](#create-a-new-version-as-needed) en este artículo.

Una vez que tome una decisión, se notifica al propietario del documento por correo electrónico.
