---
product-area: documents
navigation-topic: approvals
title: Creación de una plantilla de flujo de trabajo de aprobación para documentos
description: Puede crear plantillas de aprobación para optimizar el proceso de aprobación.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
source-git-commit: 6d6ac026bb2aa10ba3e678fb7e0f32dc95d0405f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 45%

---

# Creación de una plantilla de flujo de trabajo de aprobación para documentos

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

En el área Configuración de Workfront, los usuarios con una licencia Estándar pueden crear plantillas de aprobación reutilizables. Una vez creadas, las plantillas de aprobación se pueden aplicar a los recursos del área Documentos de un proyecto, tarea o problema.

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
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Plan</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++




## Crear una plantilla de aprobación en el entorno de producción

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Revisar y aprobar** > **Plantillas de aprobación**.
1. Haga clic en **Nueva plantilla** en el lado derecho de la página.
1. Especifique la siguiente información:

   | Nombre de plantilla | Empiece a escribir un nombre para esta plantilla. |
   |----------------------------|---|
   | **Período de tiempo (opcional)** | Introduzca el período de tiempo en días. La fecha límite de aprobación se calcula a partir de este campo una vez que la plantilla se aplica a un recurso. |
   | **Añadir aprobadores o revisores** | Empiece escribiendo el nombre de los usuarios o equipos y, a continuación, desígnelos como revisores o aprobadores. |

1. Haga clic en **Guardar**.



<div class="preview">

## Creación de una plantilla de aprobación en el entorno de vista previa

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Revisar y aprobar** > **Plantillas de aprobación**.
1. Haga clic en **Nueva plantilla** en el lado derecho de la página.

1. Complete los siguientes detalles:

   <table>
     <tr>
   <td><strong>Nombre de plantilla</strong></td>
   <td>Añada un nombre de plantilla. </td>
   </tr>
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
   <td><strong>Días de trabajo hasta la fecha de vencimiento</strong></td>
   <td>Elija cuántos días laborables hasta que la aprobación venza después de activar una fase.</td>
   </tr>
   </table>

1. (Opcional) Repita el paso anterior para agregar etapas adicionales según sea necesario.

   >[!NOTE]
   >
   >Si agrega varias fases, el flujo de trabajo de aprobación se ejecuta en el orden en que se enumeran las fases. Cuando se toman todas las decisiones necesarias, comienza la siguiente etapa y se bloquea la anterior.

   ![Detalles del documento](assets/new-stage.png)

1. Haga clic en **Guardar**.

Una vez creada la plantilla, se puede aplicar a documentos del área Documentos de un proyecto, tarea o problema para iniciar el proceso formal de revisión y aprobación en Workfront.

</div>


<!-- Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)-->
