---
product-area: documents
navigation-topic: approvals
title: Cargar una nueva versión del documento y solicitar una aprobación
description: Puede cargar una nueva versión del documento y solicitar la aprobación de otros usuarios en Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 42fbb40cb8a0f3c70e22fd04bd3d0ce625f58fec
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 22%

---

# Cargar una nueva versión del documento y solicitar una aprobación

Si un documento está marcado necesita trabajar en una revisión anterior, puede cargar una nueva versión en el documento original e iniciar otra ronda de aprobaciones. Una vez cargada una nueva versión del documento, las versiones anteriores se bloquean.

Si el nombre de archivo de la nueva versión es diferente del nombre de archivo de la versión anterior, Workfront muestra el documento con el nombre de archivo más reciente.

Cuando se añade una nueva versión a un documento con aprobaciones pendientes, la aprobación de la versión anterior se muestra como Retirada. El proceso de aprobación previo se cierra, incluso si algunos participantes aún no han tomado una decisión.

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
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p>
   <p>Colaborador o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Editar acceso al objeto asociado con el documento</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utilice arrastrar y soltar para agregar una nueva versión

>[!NOTE]
>
>Arrastrar y soltar no funciona con Internet Explorer.


Si necesita otra ronda de revisión y aprobación de un documento, puede crear una nueva versión del documento en Workfront.

Puede agregar los participantes anteriores, nuevos participantes o una combinación de ambos. Puede ver información sobre versiones anteriores y participantes en la página Detalles del documento.

Para agregar una nueva versión:

1. Navegue hasta el documento en Workfront.
1. Arrastre y suelte el nuevo archivo sobre el documento anterior. Esto crea automáticamente una nueva versión.

1. Una vez que termine la carga del documento, selecciónelo y haga clic en **Detalles del documento**.
   ![Abrir la página de detalles del documento](assets/open-doc-details.png)


1. En el panel izquierdo, haga clic en **Aprobaciones** y luego haga clic en **Agregar**.

1. Para agregar todos los participantes anteriores, haga clic en **Agregar todos**. También puede agregar nuevos participantes o quitar participantes anteriores según sea necesario.


1. Para añadir una plantilla de aprobación existente, haga clic en el botón Template y empiece a escribir el nombre de una plantilla.

   >[!TIP]
   >
   >   Los usuarios con una licencia Standard pueden crear plantillas de aprobación reutilizables desde el área de Configuración. Para obtener más información, consulte [Crear una plantilla de aprobación para recursos y documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


1. (Opcional) Establezca una fecha límite para la aprobación. Los usuarios y equipos reciben una notificación por correo electrónico 72 horas antes y 24 horas antes del plazo especificado.

1. Una vez que haya agregado todos los revisores y aprobadores, haga clic en **Enviar solicitud**. Los participantes reciben notificaciones por correo electrónico.

   ![enviar nueva versión para su aprobación](assets/add-previous-participants.png)


