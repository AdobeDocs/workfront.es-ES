---
title: Envío de solicitudes de Adobe Workfront Planning
description: Una vez que alguien comparta un vínculo a un formulario de solicitud con usted desde una página de tipo de registro en Adobe Workfront Planning, puede añadir una solicitud para crear registros para el tipo de registro asociado al formulario de solicitud.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1875'
ht-degree: 5%

---

# Envío de solicitudes de Adobe Workfront Planning para crear registros

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Después de que un administrador de espacio de trabajo cree un formulario de solicitud para un tipo de registro en Adobe Workfront Planning, puede utilizar el formulario para enviar solicitudes que crearán registros para el tipo de registro asociado al formulario.

Puede enviar una solicitud de Workfront Planning desde las siguientes áreas:

* Desde el área Solicitudes de Workfront.
* Desde un vínculo directo al formulario de solicitud compartido.
* Desde la página de tipo de registro, al agregar o solicitar un registro nuevo. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).

En este artículo se describe cómo puede enviar una solicitud para agregar nuevos registros a un tipo de registro desde el área Solicitudes de Workfront o desde un vínculo compartido.


Los usuarios de Workfront y los usuarios externos pueden enviar solicitudes a los tipos de registros de Planning y crear registros. <!--double check on the external users-->

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

   * Si no tiene una cuenta de Workfront, se ha compartido un vínculo al formulario con personas externas.

     Los usuarios de Workfront también pueden acceder a un vínculo compartido con personas externas.

* El vínculo al formulario no debe haber caducado.

## Consideraciones sobre el envío de solicitudes a Workfront Planning

* Una solicitud no se puede editar en Workfront una vez que se ha enviado.
* Cada solicitud enviada crea un registro para el tipo de registro asociado al formulario que utiliza, si el formulario no está asociado a una aprobación o si la aprobación ha sido concedida por todos los aprobadores.
* Los registros creados al enviar formularios de solicitud no se pueden diferenciar de los registros agregados mediante ningún otro método en Workfront Planning.

  Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
* Las solicitudes enviadas se muestran en el área Solicitudes de Workfront.
* Las solicitudes de Planning enviadas solo son visibles en la nueva experiencia de solicitud. No puede ver solicitudes de Planning en la experiencia de solicitudes heredadas.
* Existen limitaciones en la forma en que se muestran ciertos tipos de campo en un formulario de solicitud o en la página de detalles de la solicitud después de enviar un formulario.

  Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Envíe una solicitud a Workfront Planning en el área de solicitudes de Workfront

{{step1-to-requests}}

1. Habilite **Cambiar a una nueva configuración de experiencia**, en la esquina superior derecha de la pantalla.
Si habilita esta configuración, los formularios de solicitud de Workfront Planning estarán disponibles en el área **Solicitudes** de Workfront.

   >[!TIP]
   >
   >Esta configuración solo está disponible cuando se aplican las siguientes opciones:
   >
   >* Su compañía ha adquirido un paquete de Workfront Planning.
   >* La instancia de Workfront está integrada en la experiencia unificada de Adobe.
   >* Tiene acceso para ver al menos un espacio de trabajo.
   >

1. Haga clic en la barra **Qué solicitud desea enviar** para abrir una lista de formularios de solicitud.
1. Seleccione un formulario de solicitud de la lista o empiece a escribir su nombre y, a continuación, selecciónelo cuando aparezca en la lista.

   Se abrirá una ventana con el nombre del formulario de solicitud en la parte superior.
1. Actualice los campos disponibles en el formulario de solicitud. Los campos con un asterisco rojo son obligatorios.
1. Haga clic en **Enviar**.

   El formulario de solicitud se cerrará y volverá al área **Solicitudes**.

   El formulario se enviará y se producirán los siguientes eventos:

   * Si el formulario de solicitud no estaba asociado a una aprobación, esta se agrega a la lista Solicitudes del área Solicitudes de Workfront y al widget Mis solicitudes, y se agrega un nuevo registro al tipo de registro asociado al formulario.

   * Si el formulario de solicitud estaba asociado a una aprobación, esta se agrega a la lista Solicitudes en el área Solicitudes de Workfront y al widget Mis solicitudes. Un nuevo registro se agrega a la página de tipo de registro sólo después de que los aprobadores lo hayan aprobado.

     Para obtener más información, vea [Agregar una aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * La solicitud solo es visible para el propietario, el aprobador y las personas que tienen al menos permisos de visualización en el espacio de trabajo. Los administradores de Workfront pueden ver todas las solicitudes enviadas a cualquier espacio de trabajo del sistema.

   * Recibirá una notificación en la aplicación y por correo electrónico que le avisa de que la solicitud se ha enviado correctamente o que se ha enviado para su revisión.
   * Si el formulario de solicitud estaba asociado a una aprobación, los aprobadores reciben una notificación en la aplicación y por correo electrónico para revisar y aprobar la solicitud.

     >[!NOTE]
     >
     >Las notificaciones por correo electrónico y en la aplicación solo son visibles cuando la instancia de Workfront de su organización está integrada en la experiencia unificada de Adobe.
     >
     >Hay un vínculo a la solicitud en la confirmación de correo electrónico o la notificación de aprobación.

1. (Opcional) Haga clic en **Ver su solicitud** en el mensaje de confirmación, para abrir la solicitud, o haga clic en el icono **X** para cerrar la confirmación.
1. (Opcional) Realice una de las siguientes acciones:

   * Haga clic en **Filtros** y empiece a agregar condiciones para las solicitudes que desee ver en la lista de solicitudes.

     ![Edición de filtros en la ficha de solicitudes de Planning](assets/filters-editing-box-in-requests-planning-tab.png)

     Puede filtrar por los siguientes campos:

      * **Workspace**: área de trabajo con la que está asociado el formulario de solicitud.
      * **Tipo de registro**: Tipo de registro al que está asociado el formulario de solicitud.
      * **Fecha de entrada**: La fecha en la que se envió la solicitud.
      * **Formulario de solicitud**: Nombre del formulario de solicitud utilizado para enviar la solicitud.
      * **Estado**: El estado de la solicitud.
      * **Ingresado por**: nombre del usuario que agregó la solicitud. Si alguien fuera de Workfront agregó la solicitud, el campo **Ingresado por** muestra `N/A`.

        Puede tener varios filtros unidos por **And** o **Or**.
La lista de solicitudes se filtra automáticamente a medida que se añaden las condiciones de filtro.

   * Haga clic en **Columnas** y oculte, muestre o reorganice las columnas de la lista de solicitudes.

     >[!TIP]
     >
     >No se pueden añadir más columnas.
     >
     >No se puede mostrar el campo **Asunto**.

     ![Cuadro de edición de columnas en el área de solicitudes](assets/columns-editing-box-in-requests-planning-tab.png)


1. Haga clic en el nombre de una solicitud en la lista.

   Se abre la página de detalles de la solicitud.

   ![Solicitar página con comentario](assets/new-request-page-with-comment.png)

1. (Opcional) Introduzca un comentario en el área Comentarios.
1. (Condicional) Si el formulario de solicitud no está asociado a una aprobación, o si la solicitud se ha aprobado, haga clic en el nombre de la solicitud y, a continuación, haga clic en el nombre del registro en el campo **Registro**.

   La página del registro se abre en Workfront Planning.

   >[!TIP]
   >
   >* Si el campo principal del registro no se actualizó en el formulario de solicitud, el nombre del registro en el campo Registro de la solicitud se mostrará como **Sin título**.
   >
   >* Si el formulario de solicitud está asociado a una aprobación, esta debe concederse antes de que pueda acceder al registro desde la página de solicitud.

1. (Opcional) Haga clic en el nombre de **Tipo de registro**.

   La página de tipo de registro se abre en Workfront Planning.

## Envíe una solicitud a Workfront Planning desde un vínculo compartido a un formulario de solicitud

1. Vaya al vínculo compartido con usted desde un tipo de registro de Workfront Planning.

1. Actualice los campos disponibles en el formulario. Los campos con asterisco son obligatorios.

   >[!TIP]
   >
   >   Si el campo **Asunto** está disponible, no será visible en Workfront Planning una vez enviada la solicitud.
   >
   >Se recomienda actualizar tantos campos de la solicitud como sea posible para que el nuevo registro sea identificable cuando se añada al tipo de registro en Workfront Planning.

1. Haga clic en **Enviar**.

   El formulario se enviará y se producirán los siguientes eventos:

   * Si el formulario de solicitud no estaba asociado a una aprobación, esta se agrega a la lista Solicitudes del área Solicitudes de Workfront y al widget Mis solicitudes, y se agrega un nuevo registro al tipo de registro asociado al formulario.

   * Si el formulario de solicitud estaba asociado a una aprobación, la solicitud se agrega a la lista Solicitudes en el área Solicitudes de Workfront y al widget Mis solicitudes. Un nuevo registro se agrega a la página de tipo de registro sólo después de que todos los aprobadores lo hayan aprobado.

     Para obtener más información, vea [Agregar una aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     >[!IMPORTANT]
     >
     >Solo puede ver las solicitudes enviadas por usted o por cualquier otra persona a los espacios de trabajo para los que tiene al menos permisos de Vista. Los administradores de Workfront pueden ver todas las solicitudes enviadas a cualquier espacio de trabajo del sistema. <!--ensure this is correct; asking team in slack-->

   * Recibirá una notificación en la aplicación y por correo electrónico que le avisa de que la solicitud se ha enviado correctamente o que se ha enviado para su revisión.
   * Si el formulario de solicitud estaba asociado a una aprobación, los aprobadores reciben una notificación en la aplicación y por correo electrónico para revisar y aprobar la solicitud.

     >[!NOTE]
     >
     >Las notificaciones por correo electrónico y en la aplicación solo son visibles cuando la instancia de Workfront de su organización está integrada en la experiencia unificada de Adobe.

   <!-- <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>-->

1. (Opcional) Haga clic en **Ver su solicitud** para abrir la solicitud en Workfront.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (Opcional) Haga clic en **Menú principal** > **Solicitudes** para ver su solicitud y, a continuación, haga clic en el nombre de la solicitud.

   Se abre la página de detalles de la solicitud.

   ![Solicitar página con comentario](assets/new-request-page-with-comment.png)

1. (Opcional) Introduzca un comentario en el área Comentarios.
1. (Condicional) Si el formulario de solicitud no está asociado a una aprobación, o si la solicitud se ha aprobado, haga clic en el nombre de la solicitud y, a continuación, haga clic en el nombre del registro en el campo **Objeto creado**.

   La página del registro se abre en Workfront Planning.

   >[!TIP]
   >
   >* Si no se agregó el nombre del registro al formulario de solicitud, el nombre del registro en el campo Registro de la solicitud se mostrará como **Sin título**.
   >
   >* Si el formulario de solicitud está asociado a una aprobación, esta debe concederse antes de que pueda acceder al registro desde la página de solicitud.

1. (Opcional) Haga clic en el nombre de **Tipo de objeto**.

   La página de tipo de registro se abre en Workfront Planning.

<div class="preview">

## Crear una solicitud copiando una solicitud existente

Puede copiar una solicitud en la lista de solicitudes de Workfront, luego editar los detalles y enviarla como una solicitud nueva.

Esto solo está disponible en la nueva experiencia de solicitud.

Para obtener instrucciones, consulte [Copiar y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Crear borradores y solicitudes a partir de borradores existentes

Puede crear un borrador de una solicitud, luego volver al borrador y enviarlo como solicitud más adelante.

Esto solo está disponible en la nueva experiencia de solicitud.

Para obtener instrucciones, consulte [Crear solicitudes a partir de borradores](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).

</div>


