---
product-area: documents
navigation-topic: approvals
title: Usar las aprobaciones unificadas y la revisión de forma conjunta
description: Puede utilizar las aprobaciones unificadas con la revisión.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
source-git-commit: 6d6ac026bb2aa10ba3e678fb7e0f32dc95d0405f
workflow-type: tm+mt
source-wordcount: '1723'
ht-degree: 7%

---

# Usar las aprobaciones unificadas y la revisión de forma conjunta

Aprobaciones unificadas en Workfront presenta un nuevo conjunto de funciones para ayudarle a revisar y aprobar documentos. Puede utilizar un flujo de trabajo de aprobaciones unificadas con el visor de revisiones existente para agregar comentarios y marcas a los documentos que se están revisando.

Existen algunas diferencias clave en el flujo de trabajo al utilizar aprobaciones unificadas y revisiones juntas:

* Los participantes se muestran en el documento Resumen, no en el flujo de trabajo de revisión.

* Los detalles enviados, abiertos, comentarios y decisiones (SOCD) de la lista de documentos están relacionados con la revisión y no reflejan el estado de decisión del documento.

## Utilice aprobaciones unificadas y pruebas juntas en su entorno de producción

### Cargar un documento y crear una prueba

1. Vaya al proyecto, tarea o problema en el que desee agregar un documento nuevo.
1. Haga clic en la ficha **Documentos** y, a continuación, haga clic en el menú desplegable **Agregar nuevo**.
O
Arrastre y suelte el documento en la lista de documentos.

   >[!NOTE]
   >
   >Si tiene la opción **Generar pruebas automáticamente al cargar documentos** habilitada en su perfil de usuario, el sistema crea automáticamente una prueba simple.

1. Pase el ratón sobre el documento, luego haga clic en el vínculo **Crear revisión** que aparece debajo del nombre del documento y seleccione **Revisión simple**. Debe crear una prueba sencilla, ya que no utilizará el flujo de trabajo de prueba para las aprobaciones.

Los usuarios asignados como participantes pueden utilizar el visor de revisión para agregar comentarios y marcas en el documento. Continúe con la siguiente sección para aprender a agregar participantes de la revisión.

### Abra el documento Resumen y asigne participantes

Tiene la opción de asignar revisores, aprobadores o una combinación de ambos:

* **Los revisores** pueden agregar comentarios y marcar los recursos. Una vez finalizada, puede marcar su revisión como completada. No es necesario marcar la revisión como completada para que el documento avance en el proceso de aprobación.
* **Los aprobadores** pueden agregar comentarios y marcar los recursos. Deben tomar la decisión de adelantar el proceso de aprobación.

Para asignar participantes:

1. Seleccione el documento que ha cargado y abra el documento Resumen.
   ![Abrir resumen del documento](assets/open-doc-summary.png)

1. Desplácese hacia abajo hasta la sección Aprobaciones y haga clic en **Agregar**.

1. (Opcional) Elija una plantilla de aprobación existente. Los usuarios con una licencia Standard pueden crear plantillas de aprobación reutilizables desde el área de configuración. Para obtener más información, consulte [Crear una plantilla de flujo de trabajo de aprobación para los documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Opcional) Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas antes y 24 horas antes del plazo especificado.

1. Para agregar un aprobador, haga clic en el botón Aprobador y empiece a escribir el nombre de un usuario o equipo.

1. Para agregar un revisor, haga clic en el botón Revisor y empiece a escribir el nombre de un usuario o equipo.

   ![Agregar aprobadores](assets/add-approvers.png)

1. Una vez que haya agregado todos los revisores y aprobadores, haga clic en **Enviar solicitud**. Los participantes reciben notificaciones por correo electrónico.

### Cree una nueva versión según sea necesario

Si necesita otra ronda de revisión y aprobación, puede crear una nueva versión de prueba y agregar los participantes anteriores, los participantes nuevos o una combinación de ambos. Puede ver información sobre versiones anteriores y participantes en el documento Resumen.

Para agregar una nueva versión:

1. Arrastre y suelte el nuevo archivo sobre el documento anterior en Workfront. Esto crea automáticamente una nueva versión.

1. Una vez que termine la carga del documento, selecciónelo y haga clic en **Crear revisión** > **Revisión simple**.

1. Vuelva a seleccionar el documento y abra el documento Resumen.
   ![Abrir resumen del documento](assets/open-doc-summary.png)

1. Desplácese hacia abajo hasta la sección Aprobaciones y haga clic en **Agregar**.

1. (Opcional) Elija una plantilla de aprobación existente. Los usuarios con una licencia Standard pueden crear plantillas de aprobación reutilizables desde el área de configuración. Para obtener más información, consulte [Crear una plantilla de flujo de trabajo de aprobación para los documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Opcional) Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas antes y 24 horas antes del plazo especificado.

1. Para agregar un aprobador, haga clic en el botón Aprobador y empiece a escribir el nombre de un usuario o equipo, o elija un aprobador de la versión anterior.

1. Para agregar un revisor, haga clic en el botón Revisor y empiece a escribir el nombre de un usuario o equipo y elija un revisor de la versión anterior.

   ![Agregar aprobadores](assets/add-approvers.png)

1. Una vez que haya agregado todos los revisores y aprobadores, haga clic en **Enviar solicitud**. Los participantes reciben notificaciones por correo electrónico.

<!-- add info about reusing previous participants once released -->


### Revise la prueba y tome una decisión

El documento no pasa a un estado aprobado hasta que todos los aprobadores asignados eligen &quot;aprobado&quot;.

Para revisar y aprobar un documento:

1. Vaya a la notificación de correo electrónico de revisión y haga clic en **Ir a revisión**.

1. Una vez que estés en Workfront, haz clic en **Ir a la revisión**.

1. Revise el contenido y agregue cualquier comentario o marca. Para obtener más información acerca de cómo usar el visor de revisión, vea [Revisar pruebas en Adobe Workfront: índice de artículos](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Elija una de las siguientes decisiones:

   * **Aprobar**: el documento no necesita cambios y está listo para usarse.
   * **Aprobar con cambios**: el documento necesita cambios y está listo para usarse una vez que se hayan realizado. No se requiere una aprobación adicional.
   * **Necesita trabajo**: el documento necesita cambios y no está listo para usarse. Una vez realizados los cambios especificados, el documento debe cargarse como una nueva versión y pasar por otra ronda de aprobaciones. Para obtener más información sobre cómo cargar una nueva versión, consulte [Crear una nueva versión según sea necesario](#create-a-new-version-as-needed) en este artículo.

Una vez que tome una decisión, se notifica al propietario del documento por correo electrónico.


<div class="preview">


## Uso conjunto de aprobaciones y pruebas unificadas en el entorno de vista previa

### Cargar un documento y crear una prueba

1. Vaya al proyecto, tarea o problema en el que desee agregar un documento nuevo.
1. Haga clic en la ficha **Documentos** y, a continuación, haga clic en el menú desplegable **Agregar nuevo**.
O
Arrastre y suelte el documento en la lista de documentos.

   >[!NOTE]
   >
   >Si tiene la opción **Generar pruebas automáticamente al cargar documentos** habilitada en su perfil de usuario, el sistema crea automáticamente una prueba simple.

1. Pase el ratón sobre el documento, luego haga clic en el vínculo **Crear revisión** que aparece debajo del nombre del documento y seleccione **Revisión simple**. Debe crear una prueba sencilla, ya que no utilizará el flujo de trabajo de prueba para las aprobaciones.

Los usuarios asignados como participantes pueden utilizar el visor de revisión para agregar comentarios y marcas en el documento. Continúe con la siguiente sección para aprender a agregar participantes de la revisión.

### Abra el documento Resumen y asigne participantes

Tiene la opción de asignar revisores, aprobadores o una combinación de ambos:

* **Los revisores** pueden agregar comentarios y marcar los recursos. Una vez finalizada, puede marcar su revisión como completada. No es necesario marcar la revisión como completada para que el documento avance en el proceso de aprobación.
* **Los aprobadores** pueden agregar comentarios y marcar los recursos. Deben tomar la decisión de adelantar el proceso de aprobación.

Para asignar participantes:

1. Seleccione el documento que ha cargado y abra el documento Resumen.
   ![Abrir resumen del documento](assets/open-doc-summary.png)

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

   ![nueva etapa](assets/new-stage.png)

1. Una vez que haya agregado todos los revisores y aprobadores, haga clic en **Solicitar aprobaciones**. Los participantes reciben notificaciones por correo electrónico.


### Cree una nueva versión según sea necesario

Si necesita otra ronda de revisión y aprobación, puede crear una nueva versión de prueba y agregar los participantes anteriores, los participantes nuevos o una combinación de ambos. Puede ver información sobre versiones anteriores y participantes en el documento Resumen.

Para agregar una nueva versión:

1. Arrastre y suelte el nuevo archivo sobre el documento anterior en Workfront. Esto crea automáticamente una nueva versión.

1. Una vez que termine la carga del documento, selecciónelo y haga clic en **Crear revisión** > **Revisión simple**.

1. Vuelva a seleccionar el documento y abra el documento Resumen.
   ![Abrir resumen del documento](assets/open-doc-summary.png)

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

   ![nueva etapa](assets/new-stage.png)

1. Una vez que haya agregado todos los revisores y aprobadores, haga clic en **Solicitar aprobaciones**. Los participantes reciben notificaciones por correo electrónico.



### Revise la prueba y tome una decisión

El documento no pasa a un estado aprobado hasta que todos los aprobadores asignados eligen &quot;aprobado&quot;.

Para revisar y aprobar un documento:

1. Vaya a la notificación de correo electrónico de revisión y haga clic en **Ir a revisión**.

1. Una vez que estés en Workfront, haz clic en **Ir a la revisión**.

1. Revise el contenido y agregue cualquier comentario o marca. Para obtener más información acerca de cómo usar el visor de revisión, vea [Revisar pruebas en Adobe Workfront: índice de artículos](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Elija una de las siguientes decisiones:

   * **Aprobar**: el documento no necesita cambios y está listo para usarse.
   * **Aprobar con cambios**: el documento necesita cambios y está listo para usarse una vez que se hayan realizado. No se requiere una aprobación adicional.
   * **Necesita trabajo**: el documento necesita cambios y no está listo para usarse. Una vez realizados los cambios especificados, el documento debe cargarse como una nueva versión y pasar por otra ronda de aprobaciones. Para obtener más información sobre cómo cargar una nueva versión, consulte [Crear una nueva versión según sea necesario](#create-a-new-version-as-needed) en este artículo.

Una vez que tome una decisión, se notifica al propietario del documento por correo electrónico.

</div>