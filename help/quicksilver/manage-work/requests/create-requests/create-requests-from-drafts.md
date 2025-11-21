---
product-area: requests
navigation-topic: create-requests
title: Crear solicitudes a partir de borradores
description: Además de utilizar los borradores disponibles que Workfront le sugiere al introducir una nueva solicitud, también puede acceder a una solicitud de borrador desde la sección Borradores y terminar de enviarla desde allí.
author: Becky
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 38843e2c093d5af9d74d8b4442fd28e194996e8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 17%

---

# Crear solicitudes a partir de borradores

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

Además de utilizar los borradores disponibles que Workfront le sugiere al introducir una nueva solicitud, también puede acceder a una solicitud de borrador desde la sección Borradores y terminar de enviarla desde allí.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Producto</td> 
   <td> <ul><li>Adobe Workfront</li><li>Debe tener Adobe Workfront Planning para ver solicitudes de Planning o formularios de solicitud</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos para crear solicitudes desde borradores

Debe hacer lo siguiente para poder crear una solicitud a partir de un borrador:

* Comience a crear una solicitud. Esto guarda la solicitud como borrador automáticamente en la sección Borradores.

  Para obtener información sobre cómo crear solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Crear solicitudes a partir de borradores

El procedimiento para crear solicitudes a partir de borradores difiere entre la nueva experiencia solicitante y la experiencia heredada.

* <span class="preview">[Crear solicitudes a partir de borradores en la nueva experiencia de solicitud](#create-requests-from-drafts-in-the-new-requesting-experience)</span>
* [Crear solicitudes a partir de borradores en la experiencia de solicitud heredada](#create-requests-from-drafts-in-the-legacy-requesting-experience)

<div class="preview">

### Crear solicitudes a partir de borradores en la nueva experiencia solicitante



<!--
   
1. Open the draft.

   Drafts can be found in the following locations:

   * In the requests list in the Requests area
   * In the requests list in the My Requests widget in Home
   * In the New request dialog (includes only drafts of requests created with the selected form)
   
-->
1. Abra el borrador.

   Los borradores se pueden encontrar en el cuadro de diálogo Nueva solicitud (incluye solo borradores de solicitudes creadas con el formulario seleccionado).
1. Actualice la información de la solicitud tal como se describe en [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Opcional y condicional) En cualquier momento mientras escribe la solicitud, haga clic en **Descartar** borrador si desea eliminarlo. Esto elimina el borrador.

   Si has descartado el borrador por error, puedes hacer clic inmediatamente en **Deshacer** en el mensaje en la parte inferior de la pantalla. Esta opción solo está disponible durante unos segundos.

   Para obtener más información sobre cómo eliminar borradores, consulte [Eliminar un borrador de solicitud o solicitud enviado](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Opcional) Para guardar los cambios en el borrador sin enviarlo, salga de la página Nueva solicitud. Los cambios se guardan automáticamente.

1. Después de completar la información de la solicitud, haz clic en **Enviar**.

   Al enviar la solicitud, el borrador se eliminará y no se podrá restaurar.

</div>

### Crear solicitudes a partir de borradores en la experiencia de solicitud heredada

{{step1-to-requests}}

1. Seleccione **Borradores** en el panel izquierdo.

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

   * Haga clic en **Enviar** si está listo para enviar la solicitud. La solicitud se guarda en la sección Enviada. En función de la regla de enrutamiento de la cola de solicitudes, esta solicitud puede redirigirse a un proyecto diferente al designado como cola de solicitudes. Para obtener información acerca de las reglas de enrutamiento, consulte [Crear reglas de enrutamiento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     O

     Haga clic en **Cerrar** si no estás listo para enviarlo y puede volver y terminarlo más adelante. La solicitud se guardará en la sección Borradores y estará disponible la próxima vez que envíe una solicitud para esta cola de solicitudes.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     Al enviar la solicitud, el borrador se eliminará y no se podrá restaurar.

   >[!NOTE]
   >
   >En la nueva experiencia solicitante, los borradores están en la misma lista que las solicitudes enviadas.
   >Para obtener más información sobre cómo crear solicitudes en la nueva experiencia, consulte [Crear solicitudes y generar borradores en la aplicación web de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md#create-requests-and-generate-drafts-in-the-workfront-web-app) en el artículo Crear y enviar solicitudes.

