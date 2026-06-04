---
product-area: documents
navigation-topic: approvals
title: Cargar una nueva versión del documento y solicitar una aprobación
description: Puede cargar una nueva versión del documento y solicitar la aprobación de otros usuarios en Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
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
source-wordcount: 664
ht-degree: 9%

---

# Cargar una nueva versión del documento y solicitar una aprobación

Si un documento está marcado como &quot;Necesita trabajo&quot; en una revisión anterior, puede cargar una nueva versión en el documento original e iniciar otra ronda de aprobaciones. Una vez cargada una nueva versión del documento, las versiones anteriores se bloquean.

Si el nombre de archivo de la nueva versión es diferente del nombre de archivo de la versión anterior, Workfront muestra el documento con el nombre de archivo más reciente.

Cuando se añade una nueva versión a un documento con aprobaciones pendientes, la aprobación de la versión anterior se muestra como &quot;Retirada&quot;. El proceso de aprobación previo se cierra, incluso si algunos participantes aún no han tomado una decisión.

Si se elimina la versión más reciente del documento, las versiones anteriores permanecerán bloqueadas. Si necesita editar una versión anterior, debe desbloquearla manualmente.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de Workfront para administrar aprobaciones mediante el almacenamiento heredado de Workfront.</p>
<p>Cualquier paquete de flujo de trabajo para administrar aprobaciones mediante el almacenamiento en la nube de Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> <p>Solicitud o superior</p>
   <p>Colaborador o superior</p>
   <p>Si utiliza la integración de Frame.io, debe tener una licencia Standard para crear flujos de trabajo de aprobación.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Editar acceso al objeto asociado con el documento</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Utilice arrastrar y soltar para agregar una nueva versión en el área de documentos heredados

Si su organización está en el almacenamiento de Workfront, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento de Workfront, consulte [Diferencias entre el almacenamiento en la nube de Adobe y el almacenamiento de Workfront heredado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Arrastrar y soltar no funciona con Internet Explorer.


Si necesita otra ronda de revisión y aprobación de un documento, puede crear una nueva versión del documento en Workfront.

Puede agregar los participantes anteriores, nuevos participantes o una combinación de ambos. Puede ver información sobre versiones anteriores y participantes en la página Detalles del documento.

Para agregar una nueva versión:

1. Navegue hasta el documento en Workfront.
1. Arrastre y suelte el nuevo archivo sobre el documento anterior. Esto crea automáticamente una nueva versión.

1. Una vez que termine la carga del documento, seleccione el documento para abrir el panel Resumen del documento. Aquí verá el número de versión en la parte superior del panel.
   ![Abrir la página de detalles del documento](assets/open-doc-details.png)


1. Desplácese hacia abajo hasta la sección **Aprobaciones**.

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



1. (Opcional) Para añadir una plantilla de aprobación existente, seleccione una plantilla en la parte izquierda del cuadro de diálogo.

   >[!TIP]
   >
   >   Los usuarios con una licencia Standard pueden crear plantillas de aprobación reutilizables desde el área de configuración. Para obtener más información, consulte [Crear una plantilla de flujo de trabajo de aprobación para los documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Una vez que haya agregado todas las etapas y los participantes que necesita, haga clic en **Solicitar aprobación**.

   El flujo de trabajo de aprobación se inicia y los aprobadores reciben una notificación que les informa de que necesitan su aprobación en la nueva versión del documento. La versión anterior del documento está bloqueada y se retiran las aprobaciones pendientes de la versión anterior.

   ![solicitar aprobación](assets/request-approval.png)
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->
