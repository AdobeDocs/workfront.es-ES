---
title: Envío de solicitudes de Adobe Workfront Planning
description: Una vez que alguien comparta un vínculo a un formulario de solicitud con usted desde una página de tipo de registro en Adobe Workfront Planning, puede añadir una solicitud para crear registros para el tipo de registro asociado al formulario de solicitud.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '2026'
ht-degree: 6%

---

# Enviar solicitudes de Adobe Workfront Planning para crear registros

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Después de que un administrador de espacio de trabajo cree un formulario de solicitud para un tipo de registro en Adobe Workfront Planning, puede utilizar el formulario para enviar solicitudes que crearán registros para el tipo de registro asociado al formulario.

Puede enviar una solicitud de Workfront Planning desde las siguientes áreas:

* Desde el área Solicitudes de Workfront o desde el widget Mis solicitudes en Inicio.
* Desde un vínculo directo al formulario de solicitud compartido.
* Desde la página de tipo de registro, cuando se añade un nuevo registro enviando una solicitud. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).

En este artículo se describe cómo puede enviar una solicitud para agregar nuevos registros a un tipo de registro desde el área Solicitudes de Workfront o desde un vínculo compartido.

Los administradores de Workspace pueden crear formularios de solicitud que puede utilizar, como usuario o como persona externa, para enviar solicitudes a los tipos de registro de Planning. Las solicitudes crean registros para el tipo de registro asociado al formulario de solicitud.

Para obtener información sobre cómo un administrador del área de trabajo puede crear un formulario de solicitud y asociarlo a un tipo de registro, vea [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquetes de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete Workfront y cualquier paquete Planning</p>
O
<p>Cualquier paquete de flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Cualquiera</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de visualización o superiores para un espacio de trabajo y tipo de registro, si es un usuario de Workfront</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder enviar una solicitud a un formulario de solicitud de Workfront Planning, debe disponer de los siguientes elementos:

* Debe existir lo siguiente en Workfront Planning:

   * Un espacio de trabajo
   * Un tipo de registro
   * Un formulario de solicitud asociado a un tipo de registro.

     Para obtener más información, consulte [Crear un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* El formulario de solicitud debe compartirse para que pueda acceder a él. Se dan los siguientes escenarios:

   * Internamente, el formulario debe compartirse con los usuarios que tengan permisos de Vista o superiores del espacio de trabajo.

     Los usuarios de Workfront pueden acceder al formulario desde un vínculo o encontrarlo en el área de solicitudes de Workfront.

   * Externamente, compartiendo un vínculo al formulario de registro con personas externas que no tienen cuenta de Workfront.

     Los usuarios de Workfront también pueden acceder al vínculo compartido con personas externas.

* Si se comparte con un vínculo, el vínculo al formulario no debe caducar.

## Consideraciones sobre el envío de solicitudes a Workfront Planning

* Una solicitud no se puede editar en Workfront una vez que se ha enviado.
* Cada solicitud enviada crea un registro para el tipo de registro asociado al formulario que utiliza, si el formulario no está asociado a una aprobación o si la aprobación ha sido concedida por todos los aprobadores.
* Los registros creados al enviar formularios de solicitud son idénticos a los registros agregados mediante cualquier otro método en Workfront Planning.

  Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
* Los registros creados al enviar formularios de solicitud están conectados a la solicitud original. No se puede quitar esta conexión.
* Puede ver los registros creados y las solicitudes utilizadas para crearlos en las siguientes áreas:
   * Área de solicitudes en Workfront.

  <div class="preview">

   * En un campo conectado de una página de tipo registro en Workfront Planning cuando se agrega la solicitud como registro conectado.
   * En un campo conectado del área de Detalles de un registro en Workfront Planning cuando se agrega la solicitud como registro conectado.

  </div>

  >[!TIP]
  >
  ><span class="preview">Puede ver el nombre de la solicitud en el campo Asunto del área Solicitudes de Workfront o en el campo Conexión de la solicitud original de Workfront Planning. </span>

* Las solicitudes de Planning enviadas solo son visibles en la nueva experiencia de solicitud. No puede ver solicitudes de Planning en la experiencia de solicitudes heredadas.

  Para obtener más información, consulte [Crear y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).
* Existen limitaciones en la forma en que se muestran ciertos tipos de campo en un formulario de solicitud o en la página de detalles de la solicitud después de enviar un formulario.

  Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Envíe una solicitud a Workfront Planning en el área de solicitudes de Workfront

{{step1-to-requests}}

1. Activar la configuración **Usar nueva experiencia**, en la esquina superior derecha de la pantalla.
Al activar esta configuración, los formularios de solicitud de Workfront Planning estarán disponibles en el área **Solicitudes** de Workfront.

   >[!TIP]
   >
   >Esta configuración solo está disponible cuando la instancia de Workfront está integrada en la experiencia unificada de Adobe.
   >
   >Para poder ejecutar solicitudes de Workfront Planning en esta área, debe cumplir las siguientes condiciones:
   >
   >* Su compañía ha adquirido una licencia de Workfront Planning.
   >
   >* Tiene acceso para ver al menos un espacio de trabajo.

1. Haga clic en **¿Qué solicitud desea enviar?** para abrir una lista de formularios de solicitud.
1. Seleccione un formulario de solicitud de la lista o empiece a escribir su nombre y, a continuación, selecciónelo cuando aparezca en la lista.

   Se abrirá una ventana con el nombre del formulario de solicitud en la parte superior.

   >[!TIP]
   >
   >Las colas de solicitudes de Workfront contienen el nombre de la cola y el nombre del formulario en la lista de solicitudes. Los formularios de solicitudes de Planning solo muestran el nombre del formulario en la lista de solicitudes.

1. Actualice el campo **Asunto**. Nombre de la solicitud. Este campo es obligatorio.
1. Actualice el campo **Nombre**. Este es el nombre del registro futuro.

   >[!TIP]
   >
   >El campo **Nombre** es único para su organización y podría mostrar una etiqueta diferente en su instancia de Workfront. El campo es el campo principal del registro.

1. Actualice los campos restantes del formulario de solicitud. Los campos con un asterisco rojo son obligatorios.
1. (Condicional) Si su organización permite **Rellenar formulario** con tecnología de IA, puede cargar documentos cuando se le solicite. AI utiliza estos documentos para rellenar el formulario, y puede aceptar o rechazar las sugerencias de AI antes de enviar la solicitud.


   Para obtener instrucciones, consulte [Usar el relleno de formulario con tecnología de IA para rellenar una solicitud mediante avisos o documentos](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).
1. Haga clic en **Enviar**.

   El formulario de solicitud se cerrará y volverá al área **Solicitudes**.

   El formulario se enviará y se producirán los siguientes eventos:

   * Si el formulario de solicitud no estaba asociado a una aprobación, esta se agrega a la lista Solicitudes del área Solicitudes de Workfront y al widget Mis solicitudes de Inicio, y se agrega un nuevo registro al tipo de registro asociado al formulario.

     Los siguientes campos muestran la información de solicitud y registro en el área Solicitudes y en el widget Mis solicitudes de Inicio:

      * **Asunto**: El nombre de la solicitud original tal como se agregó en el área de solicitudes. No puede ocultar ni quitar el campo **Asunto** de la lista de solicitudes.
      * **Objeto creado**: El nombre del registro que se creó a partir de la solicitud tal como se muestra en Planning.
      * **Tipo de objeto**: Nombre del área de trabajo y tipo de registro donde se crearon registros a partir de la solicitud en Planning.
      * **Estado**: El estado del objeto de solicitud.
      * **Formulario de solicitud**: Nombre del formulario de solicitud asociado al tipo de registro en Planning.
     <!--* <span class="preview"**Created object status**: The status of the created record.</span> -->

   * Si el formulario de solicitud estaba asociado a una aprobación, esta se agregará a la lista de solicitudes en el área de solicitudes de Workfront y al widget Mis solicitudes con un estado de **Revisión pendiente**. Un nuevo registro se agrega a la página de tipo de registro sólo después de que los aprobadores lo hayan aprobado.

     Para obtener más información, vea [Agregar una aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * <span class="preview">Puede agregar el campo de conexión **Solicitud original** a un tipo de registro en Planning para mostrar el nombre de la solicitud original que creó un registro. Para obtener más información, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md). </span>
   * La solicitud solo es visible para el propietario, el aprobador y las personas que tienen al menos permisos de visualización en el espacio de trabajo. Los administradores de Workfront pueden ver todas las solicitudes enviadas a cualquier espacio de trabajo del sistema.
   * Recibirá una notificación en la aplicación y por correo electrónico que le avisa de que la solicitud se ha enviado correctamente o que se ha enviado para su revisión.
   * Si el formulario de solicitud estaba asociado a una aprobación, los aprobadores reciben una notificación en la aplicación y por correo electrónico para revisar y aprobar la solicitud.

     >[!NOTE]
     >
     >El correo electrónico y las notificaciones en la aplicación solo son visibles cuando la instancia de Workfront de su organización está integrada en la experiencia unificada de Adobe.
     >
     >Hay un vínculo a la solicitud en la confirmación de correo electrónico o la notificación de aprobación.

1. (Opcional) Haga clic en **Ver su solicitud** en el mensaje de confirmación, para abrir la solicitud, o haga clic en el icono **X** para cerrar la confirmación.
1. (Opcional) Para administrar la forma en que se muestra la información en la lista de solicitudes, actualice los siguientes elementos de vista para la lista:

   * Ver
   * Filtro
   * Columnas

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   Para obtener más información, consulte [Crear y administrar vistas en el área de solicitudes](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md).

   <!--   
   1. (Optional) From the requests list, do any of the following:
      * Click **Filters** and start adding conditions for what requests you want to view in the Requests list. 
         ![Editing filters in the Requests area](assets/filters-editing-box-in-requests-planning-tab.png)
         You can filter by the following fields:  
         * **Workspace**: The workspace the request form is associated with.
         * **Object type**: The record type the request form is associated with.
         * **Entry date**: The date when the request was submitted.
         * **Request form**: The name of the request form used to submit the request.
         * **Status**: The status of the request.
         * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.
        You can have multiple filters joined by either **And** or **Or**.
         The request list is filtered automatically, as you add the filter conditions. 
      * Click **Columns** to open the **Fields visibility and order** box, then hide, show, or rearrange the columns in the request list. 
         >[!TIP]
         >
         >You cannot add any more columns. 
         ![Columns editing box in Requests area](assets/columns-editing-box-in-requests-planning-tab.png)
      * Click the **+** icon in the upper-right corner of the request list to open the **Column manager** and add or remove columns in the requests list. 
   -->

1. Haga clic en el nombre de una solicitud en la lista.

   Se abre la página de detalles de la solicitud.

   ![Solicitar página con comentario](assets/new-request-page-with-comment.png)

1. (Opcional) Escriba un comentario en el área **Comentarios**.
1. (Condicional) Si el formulario de solicitud no está asociado a una aprobación, o si la solicitud se ha aprobado, haga clic en el nombre de la solicitud y, a continuación, haga clic en el nombre del registro en el campo **Objeto creado**.

   La página del registro se abre en Workfront Planning.

   >[!TIP]
   >
   >* Si el campo principal del registro no se actualizó en el formulario de solicitud, el nombre del registro en el campo Registro de la solicitud se mostrará como **Sin título**.
   >
   >* Si el formulario de solicitud está asociado a una aprobación, esta debe concederse antes de que pueda acceder al registro desde la página de solicitud. El registro no se crea hasta que se concede la aprobación.

1. (Opcional) Haga clic en el nombre de **Tipo de registro**.

   La página de tipo de registro se abre en Workfront Planning.

## Envíe una solicitud a Workfront Planning desde un vínculo compartido a un formulario de solicitud

La información de esta sección se aplica solo a las personas que envían una solicitud desde un vínculo compartido y que pueden no tener una cuenta de Workfront.

Las personas externas no pueden acceder a las áreas internas de Workfront, como **Solicitudes** o **Hogar**.

1. Vaya al vínculo compartido con usted desde un tipo de registro de Workfront Planning.

1. Actualice los campos disponibles en el formulario. Los campos con asterisco son obligatorios.

   >[!TIP]
   >
   >   Si el campo **Asunto** está disponible, no será visible en Workfront Planning una vez enviada la solicitud.
   >
   >Se recomienda actualizar tantos campos de la solicitud como sea posible para que el nuevo registro sea identificable cuando se añada al tipo de registro en Workfront Planning.

1. Haga clic en **Enviar**.

   El formulario se enviará y recibirá una confirmación.

   Si el formulario está asociado a una aprobación, debe aprobarse antes de crear un registro.

1. (Opcional) Haga clic en **Enviar otra solicitud** para agregar otra solicitud al mismo vínculo compartido.

<!--
   * If the request form was not associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget in Home, and a new record is added to the record type associated with the form. This is available only when you log in to Workfront.
   
   * If the request form was associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget. A new record is added to the record type page only after all the approvers have approved it. This is available only when you log in to Workfront.
   
      For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

      >[!IMPORTANT]
      >
      >You can view only the requests submitted by you or anyone else to the workspaces that you have at least permissions to View. Workfront administrators can view all requests submitted to any workspace in the system. <!--ensure this is correct; asking team in slack
   
   
   * You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.
   * If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.
      >[!NOTE]
      >
      >The email and in-app notification are visible only when your organization's instance of Workfront is onboarded to the Adobe Unified Experience.
   
   <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>


1. (Optional) Click **View your request** to open the request in Workfront.


Or

Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.

   The request details page opens. 

   ![Request page with comment](assets/new-request-page-with-comment.png)

1. (Optional) Enter a comment in the **Comments** area.
1. (Conditional) If the request form is not associated with an approval, or if the request has been approved, click the name of the request, then click the name of the record in the **Created object** field. 

   The record's page opens in Workfront Planning. 

   >[!TIP]
   >
   >* If the record name was not added to the request form, the name of the record in the Record field of the request displays as **Untitled**. 
   >
   >* If the request form is associated with an approval, the approval must be granted before you can access the record from the request page. 

1. (Optional) Click the name of the **Object type**. 

   The record type page opens in Workfront Planning. 

-->

## Crear una solicitud copiando una solicitud existente

Puede copiar una solicitud en la lista de solicitudes de Workfront, luego editar los detalles y enviarla como una solicitud nueva.

Esto solo está disponible en la nueva experiencia de solicitud.

Copiar una solicitud de Planning existente y enviarla como una nueva es similar a copiar una solicitud de Workfront existente.

Para obtener más información, consulte [Copiar y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Crear borradores y solicitudes a partir de borradores existentes

Puede crear un borrador de una solicitud, luego volver al borrador y enviarlo como solicitud más adelante.

Esto solo está disponible en la nueva experiencia de solicitud. Crear borradores y solicitudes a partir de borradores existentes en Workfront Planning es idéntico a crearlos a partir de Adobe Workfront.

Para obtener más información, consulte [Crear solicitudes a partir de borradores](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).

## Eliminar borradores o solicitudes enviadas

Puede eliminar las solicitudes enviadas o sus borradores al utilizar la experiencia de nuevas solicitudes.

Al eliminar una solicitud de Planning, se producen los siguientes problemas:

* La solicitud no se puede recuperar.
* El registro creado a partir de la solicitud no se elimina.
* Los borradores eliminados no se pueden recuperar. No hay registros asociados a borradores.

Eliminar solicitudes de Planning es similar a eliminar solicitudes de Workfront.

Para obtener más información, consulte [Eliminar una solicitud enviada o un borrador de solicitud](/help/quicksilver/manage-work/requests/create-requests/delete-request-draft.md).







