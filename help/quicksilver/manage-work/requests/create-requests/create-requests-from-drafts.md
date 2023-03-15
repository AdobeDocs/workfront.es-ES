---
product-area: requests
navigation-topic: create-requests
title: Crear solicitudes a partir de borradores
description: Además de utilizar los borradores disponibles que Workfront le sugiere cuando introduce una nueva solicitud, también puede acceder a una solicitud de borrador de la sección Borradores y terminar de enviarla desde allí.
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 1%

---

# Crear solicitudes a partir de borradores

Además de utilizar los borradores disponibles que Workfront le sugiere cuando introduce una nueva solicitud, también puede acceder a una solicitud de borrador de la sección Borradores y terminar de enviarla desde allí.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos para crear solicitudes a partir de borradores

Debe hacer lo siguiente antes de crear una solicitud a partir de un borrador: 

* Comience a crear una solicitud. Esto guarda la solicitud como un borrador automáticamente en la sección Borradores .

   Para obtener información sobre la creación de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Crear solicitudes a partir de borradores

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront.
1. Haga clic en **Solicitudes** > **Borradores**.

   En esta lista se muestra un borrador para cada tema de cola de cada cola de solicitud.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. Revise la información sobre cada borrador en las siguientes columnas de la lista Borradores:

   | Asunto | Este es el nombre que dio a la solicitud cuando la empezó a crear. |
   |---|---|
   | Ruta | El nombre de la cola de solicitudes, los grupos de temas y los temas de cola donde originalmente se pretendía enviar la solicitud. |
   | Fecha de entrada | La fecha en la que se inició la creación de la solicitud. |
   | Fecha de última actualización | La última actualización. Si no lo ha actualizado desde que inició la solicitud, la fecha de entrada y la fecha de última actualización deberían ser las mismas. |

   {style="table-layout:auto"}

1. (Opcional) Haga clic en **Filtrar por tipo de solicitud** en la esquina superior derecha de la lista de borradores, seleccione la cola de solicitudes que contiene los borradores que desea mostrar.
1. Haga clic en el nombre de un borrador para abrirlo.
1. Actualice la información de la solicitud tal como se describe en [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Opcional y condicional) En cualquier momento durante la introducción de la solicitud, haga clic en **Descartar** borrador si desea eliminar el borrador. Esto elimina el borrador que no se puede recuperar. Para obtener más información sobre la eliminación de borradores, consulte [Eliminar un borrador de solicitud](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Opcional) Haga clic en **Cancelar** en la esquina inferior izquierda de la página si desea revertir la acción y mantener el borrador.

1. Después de completar la información de la solicitud, realice una de las siguientes acciones:

   * Haga clic en **Submit** si está listo para enviar la solicitud. La solicitud se guarda en la sección Enviado . En función de la regla de enrutamiento de la cola de solicitud, esta solicitud puede enrutarse a un proyecto diferente al designado como cola de solicitud. Para obtener información sobre las reglas de enrutamiento, consulte [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      O

      Haga clic en **Cerrar** si no estás listo para enviarlo y puedes volver y terminarlo más tarde. La solicitud se guarda en la sección Borradores y estará disponible la próxima vez que envíe una solicitud para esta cola de solicitudes.

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

      Cuando envía la solicitud, el borrador se elimina y no se puede restaurar.
