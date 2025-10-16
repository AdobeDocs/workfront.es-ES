---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incrustar una cola de solicitudes en un panel de control
description: Puede incrustar una nueva cola de solicitudes en un panel de control para proporcionar a los usuarios acceso directo a la cola de solicitudes sin tener que ir al área de solicitudes.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 97%

---

# Incrustar una cola de solicitudes en un panel de control

<!-- Audited: 1/2025 -->

Puede incrustar una nueva cola de solicitudes en un panel de control para proporcionar a los usuarios acceso directo a la cola de solicitudes sin tener que ir al área de solicitudes.

Por ejemplo, si tiene una cola de solicitudes abierta a toda la organización, como una cola del servicio de asistencia o una cola de solicitudes de PTO a la que todos deben tener acceso de forma regular, puede que sea conveniente insertar la cola de solicitudes directamente en uno de sus paneles de control para tener un acceso rápido y sencillo. El proceso de configuración es similar a la creación de una página externa en un panel de control.

En primer lugar, debe obtener una dirección URL para la cola de solicitudes. En segundo lugar, puede incrustar la dirección URL en un panel de control añadiendo una página externa.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
      <p>Estándar</p>
      <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en el panel de control</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Requisitos previos

Para poder incrustar una cola de solicitudes en un panel de control, se deben crear los dos elementos siguientes:

* **El panel de control**: para obtener información sobre cómo crear paneles de control, consulte [Crear un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

* **La cola de solicitudes**: para obtener información sobre cómo crear colas de solicitudes, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## Obtener la dirección URL de la cola de solicitudes {#obtain-the-url-of-the-request-queue}

Puede obtener la dirección URL de una cola de solicitudes de varias formas, en función de qué parte de la cola de solicitudes desee exponer a los usuarios cuando accedan a ella desde un panel de control.

* [Obtener un vínculo a un tema específico de la cola con capacidad para cambiar el tipo de solicitud](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)

* [Obtener un vínculo a una cola de solicitudes y poder cambiar el tipo de solicitud](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)

* [Obtener un vínculo a una cola de solicitudes sin poder cambiar el tipo de solicitud](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### Obtener un vínculo a un tema específico de la cola con capacidad para cambiar el tipo de solicitud {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

Cuando comparte un vínculo a un tema específico de la cola con otros usuarios, el formulario de solicitud se abre en el tema exacto de la cola que necesitan utilizar para enviar la solicitud. Esto resulta útil en el caso que los usuarios no estén seguros de qué tema de la cola elegir al registrar solicitudes para una cola de solicitudes específica.

Los usuarios pueden cambiar el tipo de solicitud o elegir otro tema si lo necesitan. También se muestra la navegación en el área de solicitudes.

1. Haga clic en **Menú principal** > **Solicitudes** > **Nueva solicitud**.
1. Continúe seleccionando grupos de temas y temas de colas hasta que llegue a la cola que desea compartir en el panel de control, si desea compartir una cola específica. Para obtener información sobre cómo enviar solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >La selección de grupos de temas y temas de colas es opcional.

1. Haga clic en **Compartir ruta** en la esquina superior derecha del área Nueva solicitud.

   Esto copia el vínculo a la cola de solicitudes o al tema de la cola a medida que se muestra en la pantalla. Los usuarios pueden actualizar el tipo de solicitud o cualquiera de los grupos de temas y los temas de colas disponibles.

   ![Solicitar cola con ruta compartida](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### Obtener un vínculo a una cola de solicitudes y poder cambiar el tipo de solicitud {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

Cuando comparte un vínculo a un tipo de solicitud, se selecciona el tipo de solicitud para el usuario. Esto resulta útil cuando los usuarios necesitan elegir entre varios grupos de temas o temas en cola para el mismo tipo de solicitud. Los usuarios pueden cambiar el tipo de solicitud y elegir otro. También se muestra la navegación en el área de solicitudes.

1. Vaya a un proyecto designado como cola de solicitudes.

   Para obtener información sobre la creación de una cola de solicitudes a partir de un proyecto, vaya a [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Vaya a **Detalles de cola**.
1. Copie el código que encuentre en el campo **URL de acceso directo**.

   El código debe tener un aspecto similar al siguiente:

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   Este es el vínculo a la cola de solicitudes asociada al proyecto seleccionado. El tipo de solicitud está preseleccionado.

   Los usuarios pueden seleccionar cualquier grupo de temas o tema de cola que necesiten, o bien elegir otro tipo de solicitud.

   ![Solicitar URL de cola](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### Obtener un vínculo a una cola de solicitudes sin poder cambiar el tipo de solicitud {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

Al compartir un vínculo a un tipo de solicitud preseleccionado, el tipo de solicitud se selecciona para el usuario y no se puede cambiar (está atenuado). Los usuarios pueden elegir los grupos de temas o los temas de cola que necesiten. Esto resulta útil cuando no se desea que los usuarios vean y seleccionen otros tipos de solicitud. No se muestra la navegación en el área Solicitudes.

1. Vaya a un proyecto designado como cola de solicitudes.

   Para obtener información sobre la creación de una cola de solicitudes a partir de un proyecto, vaya a [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Vaya a **Detalles de cola**.
1. Copie el código que encuentre en el campo **Código incrustado**.

   El código debe tener un aspecto similar al siguiente:

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. Edite el código para conservar solo la siguiente información:

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >Puede añadir una etiqueta `<samp>iframe </samp>` al incrustar el código en una aplicación que no sea Workfront.

   Este es el vínculo a la cola de solicitudes asociada al proyecto seleccionado. El tipo de solicitud está preseleccionado y no se puede cambiar.

   Los usuarios pueden seleccionar cualquier grupo de temas o tema de cola que necesiten para el tipo de solicitud seleccionado. Los usuarios no pueden seleccionar otro tipo de solicitud.

   ![Solicitar código de cola](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## Incrustar una cola de solicitudes en un panel de control

Puede incrustar en un panel de control un vínculo a la cola de solicitudes o a un tema de la cola anidado en una cola de solicitudes para proporcionar a los usuarios acceso directo a la introducción de solicitudes.

1. Obtenga una URL de cola de solicitudes mediante uno de los métodos descritos en la sección [Obtener la URL de la cola de solicitudes](#obtain-the-url-of-the-request-queue) de este artículo.

1. Haga clic en **Menú principal** > **Paneles de control** > **Nuevo panel de control**.

1. Escriba un **nombre** para el panel de control. Este campo es obligatorio.

1. Haga clic en **Añadir página externa**.

   ![Página externa](assets/add-external-page-highlighted---nwe-350x214.png)

1. En el cuadro **Añadir página externa**, edite los campos siguientes:

   * **Nombre**: introduzca el nombre de la cola de solicitudes tal como desea que aparezca en el panel de control. Este campo es obligatorio.

   * **Descripción**: introduzca una descripción sobre lo que muestra esta página externa. No se trata de un campo obligatorio y solo es importante para fines de creación de informes. No se muestra en el panel de control.

   * **URL**: pegue la URL que ha obtenido mediante uno de los métodos descritos en el paso 1.

   * **Altura**: introduzca la altura de la página externa. Esta opción define la cantidad de espacio que ocupa en el panel de control la página externa que contiene la cola de solicitudes. Este campo es obligatorio y el valor predeterminado es 500.

1. Haga clic en **Guardar**.

1. Haga clic en **Guardar + Cerrar**.

   La cola de solicitudes se muestra en el panel de control como un componente de panel de control independiente.

1. (Opcional) Haga clic en **Acciones de panel de control** y luego en **Editar** para añadir informes, calendarios o páginas externas adicionales al mismo panel de control.

   Para obtener información sobre la inclusión de componentes en un panel de control, consulte [Crear un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
