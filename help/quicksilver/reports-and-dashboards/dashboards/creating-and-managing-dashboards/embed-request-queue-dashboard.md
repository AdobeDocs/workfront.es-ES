---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incrustar una cola de solicitudes en un panel
description: Puede incrustar una nueva cola de solicitudes en un tablero para proporcionar acceso directo a la cola de solicitudes a los usuarios, sin tener que ir al área Solicitudes .
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 2894161b61a00dab04c17ef642ace4a45179eb17
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 1%

---

# Incrustar una cola de solicitudes en un panel

Puede incrustar una nueva cola de solicitudes en un tablero para proporcionar acceso directo a la cola de solicitudes a los usuarios, sin tener que ir al área Solicitudes . 

Por ejemplo, si tiene una cola de solicitud abierta a toda la organización, como una cola de asistencia técnica o una cola de solicitud de pago a la que todos deben acceder con regularidad, puede que sea conveniente insertar la cola de solicitudes directamente en uno de sus paneles para acceder fácil y rápidamente a ella. El proceso de configuración es similar al de creación de una página externa en un tablero.

En primer lugar, debe obtener una URL a la cola de solicitudes. En segundo lugar, puede incrustar la dirección URL en un panel agregando una página externa.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administrar permisos en el tablero</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Para poder incrustar una cola de solicitudes en un tablero, se deben crear las dos opciones siguientes:

* **El tablero**: Para obtener información sobre la creación de tableros, consulte [Crear un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).
* **La cola de solicitudes**: Para obtener información sobre la creación de colas de solicitud, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## Obtener la dirección URL de la cola de solicitudes {#obtain-the-url-of-the-request-queue}

Puede obtener la dirección URL de una cola de solicitudes de varias formas, dependiendo de la parte de la cola de solicitudes que desee exponer a los usuarios cuando accedan a ella desde un panel.

* [Obtener un vínculo a un tema de cola específico con la capacidad de cambiar el tipo de solicitud](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)
* [Obtener un vínculo a una cola de solicitud y la capacidad de cambiar el tipo de solicitud](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)
* [Obtener un vínculo a una cola de solicitud sin capacidad para cambiar el tipo de solicitud](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### Obtener un vínculo a un tema de cola específico con la capacidad de cambiar el tipo de solicitud {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

Cuando comparte un vínculo a un tema de cola específico con otros usuarios, el formulario de solicitud se abre con el tema de cola exacto que necesitan utilizar para enviar la solicitud. Esto es útil cuando los usuarios podrían no estar seguros de qué tema de cola elegir al registrar solicitudes para una cola de solicitudes específica.

Los usuarios pueden cambiar el tipo de solicitud o elegir otro tema si lo necesitan. También se muestra la navegación del área Solicitudes .

1. Haga clic en el **Menú principal** > **Solicitudes** > **Nueva solicitud**.
1. Siga seleccionando grupos de temas y temas de cola hasta que llegue a la cola que desee compartir en el tablero, si desea compartir una cola específica. Para obtener información sobre el envío de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >La selección de grupos de temas y de temas de cola es opcional.

1. Haga clic en **Compartir ruta** en la esquina superior derecha del área Nueva solicitud .

   Esto copia el vínculo a la cola de solicitudes o el tema de la cola mientras lo muestra en la pantalla. Los usuarios pueden actualizar el tipo de solicitud o cualquiera de los grupos de temas y los temas de cola disponibles.

   ![](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### Obtener un vínculo a una cola de solicitud y la capacidad de cambiar el tipo de solicitud {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

Cuando comparte un vínculo a un tipo de solicitud, se selecciona el tipo de solicitud para el usuario. Esto es útil cuando los usuarios necesitan elegir entre varios grupos de temas o temas de cola para el mismo tipo de solicitud. Los usuarios pueden cambiar el tipo de solicitud y elegir otra. También se muestra la navegación del área Solicitudes .

1. Vaya a un proyecto designado como cola de solicitud.

   Para obtener información sobre la creación de una cola de solicitudes desde un proyecto, vaya a [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Vaya a **Detalles de cola**.
1. Copie el código que encuentra en la **Dirección URL de acceso directo** campo .

   El código debe tener un aspecto similar al siguiente:

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   Este es el vínculo a la cola de solicitudes asociada al proyecto seleccionado. El tipo de solicitud está preseleccionado.

   Los usuarios pueden seleccionar cualquier grupo de temas o tema de cola que necesiten, o pueden elegir otro tipo de solicitud.

   ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### Obtener un vínculo a una cola de solicitud sin capacidad para cambiar el tipo de solicitud {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

Cuando comparte un vínculo a un tipo de solicitud preseleccionado, el tipo de solicitud se selecciona para el usuario y no se puede cambiar (está atenuado). Los usuarios pueden elegir los grupos de temas o los temas de cola que necesiten. Esto es útil cuando no desea que los usuarios vean y seleccionen otros tipos de solicitud. La navegación del área Solicitudes no se muestra.

1. Vaya a un proyecto designado como cola de solicitud.

   Para obtener información sobre la creación de una cola de solicitudes desde un proyecto, vaya a [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Vaya a **Detalles de cola**.
1. Copie el código que encuentra en la **Código incrustado** campo .

   El código debe tener un aspecto similar al siguiente:

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. Edite el código para conservar solo la información siguiente:

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >Puede añadir un `<samp>iframe </samp>` al incrustar el código en una aplicación que no sea Workfront.

   Este es el vínculo a la cola de solicitudes asociada al proyecto seleccionado. El tipo de solicitud está preseleccionado y no se puede cambiar.

   Los usuarios pueden seleccionar cualquier grupo de temas o tema de cola que necesiten para el tipo de solicitud seleccionado. Los usuarios no pueden seleccionar otro tipo de solicitud.

   ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## Incrustar una cola de solicitudes en un panel

Puede incrustar un vínculo a la cola de solicitudes o a un tema de cola anidado en una cola de solicitudes en un tablero para que los usuarios tengan acceso directo a la introducción de solicitudes.

1. Obtenga una URL de cola de solicitud mediante uno de los métodos descritos en la sección [Obtener la dirección URL de la cola de solicitudes](#obtain-the-url-of-the-request-queue) de este artículo.
1. Haga clic en el **Menú principal** > **Tableros** > **Nuevo tablero**.
1. Tipo a **Nombre** para el tablero. Este campo es obligatorio.
1. Haga clic en **Agregar página externa**.

   ![](assets/add-external-page-highlighted---nwe-350x214.png)

1. En el **Agregar página externa** , edite los campos siguientes:

   * **Nombre**: introduzca el nombre de la cola de solicitudes tal como desea que aparezca en el panel. Este campo es obligatorio.

   * **Descripción**: introduzca una descripción sobre la visualización de esta página externa. Este campo no es obligatorio y solo es importante para la generación de informes. No se muestra en el tablero.
   * **URL**: pegue la dirección URL que obtuvo mediante uno de los métodos descritos en el paso 1.

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <MadCap:conditionalText data-mc-conditions="">   
     (NOTE: ensure this stays accurate)   
     </MadCap:conditionalText>   
     </MadCap:conditionalText>   
     -->

   * **Altura**: introduzca la altura de la página externa. Esto define cuánto espacio ocupa la página externa que contiene la cola de solicitudes en el panel. Se trata de un campo obligatorio y el valor predeterminado es 500.

1. Haga clic en **Guardar**.
1. Haga clic en **Guardar + Cerrar**. 

   La cola de solicitudes se muestra en el panel como un componente de panel independiente.

   ![](assets/new-dashboard-with-embedded-request-queue-nwe-350x260.png)

1. (Opcional) Haga clic en **Acciones del panel**, luego **Editar** para agregar informes, calendarios o páginas externas adicionales al mismo tablero.\
   Para obtener información sobre cómo agregar componentes a un tablero, consulte [Crear un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

 

 

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - old information)</p>
-->

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
