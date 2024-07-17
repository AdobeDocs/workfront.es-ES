---
product-area: requests
navigation-topic: create-requests
title: Crear solicitudes a partir de borradores
description: Además de utilizar los borradores disponibles que Workfront le sugiere al introducir una nueva solicitud, también puede acceder a una solicitud de borrador desde la sección Borradores y terminar de enviarla desde allí.
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 0f30ff23ef828d32c406cc2d9733c23b095014c9
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# Crear solicitudes a partir de borradores

Además de utilizar los borradores disponibles que Workfront le sugiere al introducir una nueva solicitud, también puede acceder a una solicitud de borrador desde la sección Borradores y terminar de enviarla desde allí.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos para crear solicitudes desde borradores

Debe hacer lo siguiente para poder crear una solicitud a partir de un borrador: 

* Comience a crear una solicitud. Esto guarda la solicitud como borrador automáticamente en la sección Borradores.

  Para obtener información sobre cómo crear solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Crear solicitudes a partir de borradores

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront.
1. Haga clic en **Solicitudes** > **Borradores**.

   En esta lista se muestra un borrador para cada tema de cola de cada cola de solicitudes.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. (Opcional) Haga clic en un encabezado de columna para ordenar la lista por esa columna.

1. Revise la información sobre cada borrador en las siguientes columnas de la lista Borradores:

   | Asunto | Este es el nombre que le dio a su solicitud cuando empezó a crearla. |
   |---|---|
   | Ruta | El nombre de la cola de solicitudes, los grupos de temas y los temas de colas donde originalmente planeó enviar la solicitud. |
   | Fecha de entrada | La fecha en la que inició la creación de la solicitud. |
   | Fecha de última actualización | La última de su última actualización. Si no lo ha actualizado desde que inició la solicitud por primera vez, la fecha de entrada y la fecha de última actualización deben ser las mismas. |

   {style="table-layout:auto"}

1. (Opcional) Con el filtro rápido de la esquina superior derecha de la lista Borradores, empiece a escribir el nombre de una solicitud de borrador, cola de solicitudes, tema de cola o grupo de temas y, a continuación, haga clic en el nombre de un borrador para abrirlo.

   >[!TIP]
   >
   >No puede aplicar filtros permanentes en la sección Borradores del área Solicitudes. Además, no hay opciones para modificar o cambiar la vista de la lista de borradores.

1. Actualice la información de la solicitud tal como se describe en [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Opcional y condicional) En cualquier momento mientras escribe la solicitud, haga clic en **Descartar** borrador si desea eliminarlo. Esto elimina el borrador que no se puede recuperar. Para obtener más información sobre cómo eliminar borradores, consulte [Eliminar un borrador de solicitud](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Opcional) Haga clic en **Cancelar** en la esquina inferior izquierda de la página si desea revertir la acción y conservar el borrador.

1. Después de completar la información de la solicitud, realice una de las siguientes acciones:

   * Haga clic en **Enviar** si está listo para enviar la solicitud. La solicitud se guarda en la sección Enviada. En función de la regla de enrutamiento de la cola de solicitudes, esta solicitud puede redirigirse a un proyecto diferente al designado como cola de solicitudes. Para obtener información acerca de las reglas de enrutamiento, vea [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     O

     Haz clic en **Cerrar** si no estás listo para enviarlo y es posible que vuelvas y lo termines más tarde. La solicitud se guardará en la sección Borradores y estará disponible la próxima vez que envíe una solicitud para esta cola de solicitudes.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     Al enviar la solicitud, el borrador se eliminará y no se podrá restaurar.
