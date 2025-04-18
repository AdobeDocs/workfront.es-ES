---
title: Envío de solicitudes de Adobe Workfront Planning
description: Una vez que alguien comparta un vínculo a un formulario de solicitud con usted desde una página de tipo de registro en Adobe Workfront Planning, puede añadir una solicitud para crear registros para el tipo de registro asociado al formulario de solicitud.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 4bdd4510a5ff7faf8f497299eac0a10f4fe7fbc2
workflow-type: tm+mt
source-wordcount: '1875'
ht-degree: 8%

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

  En este artículo se describe cómo puede enviar una solicitud para agregar nuevos registros a un tipo de registro desde el área Solicitudes de Workfront o desde un vínculo compartido.
* Desde la página de tipo de registro, al agregar o solicitar un registro nuevo. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).

Los usuarios de Workfront y los usuarios externos pueden enviar solicitudes a los tipos de registros de Planning y crear registros. <!--double check on the external users-->

Para obtener información sobre cómo un administrador del área de trabajo puede crear un formulario de solicitud y asociarlo a un tipo de registro, vea [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Productos</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planificación de Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera de los siguientes planes de Workfront:</p>
<ul><li>Seleccionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning no está disponible para planes Workfront heredados</p>
   </td>
<tr>
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera </p>  
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </td>
<tr>
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td>
   <td>
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p>
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Licencia externa, colaboradora, básica o estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td>
   <p>Ver o permisos superiores a un espacio de trabajo <span class="preview">y tipo de registro</span>, si es un usuario de Workfront</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>Para acceder al área de planificación en Workfront, se le debe asignar una plantilla de diseño que incluya el área de planificación en el menú principal. </p>
   <p> Sin embargo, no es necesario acceder al área de Planning para enviar solicitudes a Workfront Planning. </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder enviar una solicitud a un formulario de solicitud de Workfront Planning, debe disponer de los siguientes elementos:

* Debe existir lo siguiente en Workfront Planning:

   * Un espacio de trabajo
   * Un tipo de registro.
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
* Las solicitudes enviadas se muestran en la pestaña Planificación de la sección Enviadas del área Solicitudes de Workfront.
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

1. Haga clic en **Nueva solicitud**.

   ![Nuevo cuadro de solicitud con tarjetas Workfront y Planning unificadas](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   El cuadro **Nueva solicitud** se abre con la siguiente información:

   * Las 6 colas de solicitud de Workfront a las que se ha accedido más recientemente y los formularios de solicitud de Planning se muestran en la sección Reciente.
   * 50 colas de solicitudes de Workfront adicionales y formularios de solicitudes de Planning se muestran en orden alfabético en la sección **Todos los formularios de solicitudes**. Puede buscar una cola de solicitudes que no se muestre de forma predeterminada.

1. Realice una de las siguientes acciones:

   * Haga clic en la tarjeta de uno de los formularios de solicitud de Planning en las secciones Formularios de solicitud recientes o Todos
   * Comience a escribir el nombre de un formulario de solicitud de Planning en el cuadro de búsqueda y, a continuación, haga clic en la tarjeta cuando se muestre en la lista.

   Se abrirá el formulario de solicitud.

1. Actualice los campos disponibles en el formulario de solicitud. Los campos con un asterisco rojo son obligatorios.
1. Haga clic en **Enviar**.

   El formulario de solicitud se cerrará y volverá al área **Solicitudes**.

   El formulario se enviará y se producirán los siguientes eventos:

   * Si el formulario de solicitud no estaba asociado a una aprobación, la solicitud se agrega a la pestaña Planificación de la sección Enviado del área Solicitudes de Workfront y se agrega un nuevo registro al tipo de registro asociado al formulario.

   * Si el formulario de solicitud estaba asociado a una aprobación, la solicitud se agrega a la pestaña Planificación de la sección Enviado del área Solicitudes de Workfront. Un nuevo registro se agrega a la página de tipo de registro sólo después de que todos los aprobadores lo hayan aprobado.

     Para obtener más información, vea [Agregar una aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Área de solicitudes con la opción de pestaña de planificación de flujo de trabajo unificado](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >Todos los usuarios que tengan acceso al menos a un espacio de trabajo pueden ver la pestaña Planificación en el área Solicitudes. Solo puede ver las solicitudes enviadas por usted o por cualquier otra persona a los espacios de trabajo para los que tiene al menos permisos de Vista. Los administradores de Workfront pueden ver todas las solicitudes enviadas a cualquier espacio de trabajo del sistema.

   * La solicitud solo es visible para el propietario, el aprobador y las personas que tienen al menos permisos de visualización en el espacio de trabajo.

   * Recibirá una notificación en la aplicación y por correo electrónico que le avisa de que la solicitud se ha enviado correctamente o que se ha enviado para su revisión.
   * Si el formulario de solicitud estaba asociado a una aprobación, los aprobadores reciben una notificación en la aplicación y por correo electrónico para revisar y aprobar la solicitud.

     >[!NOTE]
     >
     >Las notificaciones por correo electrónico y en la aplicación solo son visibles cuando la instancia de Workfront de su organización está integrada en la experiencia unificada de Adobe.
     >
     >Hay un vínculo a la solicitud en la confirmación de correo electrónico o la notificación de aprobación.

   1. (Opcional) Haga clic en **Ver su solicitud** en el mensaje de confirmación, para abrir la solicitud, o haga clic en el icono **X** para cerrar la confirmación.

1. (Opcional) Haga clic en la ficha **Planificación** del área Solicitudes para ver la solicitud y, a continuación, haga clic en el nombre de la solicitud.

   Se abre la página de detalles de la solicitud.

   ![Página de detalles de solicitud](assets/request-details-page.png)

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

   * Si el formulario de solicitud no estaba asociado a una aprobación, la solicitud se agrega a la pestaña Planificación de la sección Enviado del área Solicitudes de Workfront y se agrega un nuevo registro al tipo de registro asociado al formulario.

   * Si el formulario de solicitud estaba asociado a una aprobación, la solicitud se agrega a la pestaña Planificación de la sección Enviado del área Solicitudes de Workfront. Un nuevo registro se agrega a la página de tipo de registro sólo después de que todos los aprobadores lo hayan aprobado.

     Para obtener más información, vea [Agregar una aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Pestaña Planificación en las solicitudes](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >Todos los usuarios que tengan acceso al menos a un espacio de trabajo pueden ver la pestaña Planificación en el área Solicitudes. Solo puede ver las solicitudes enviadas por usted o por cualquier otra persona a los espacios de trabajo para los que tiene al menos permisos de Vista. Los administradores de Workfront pueden ver todas las solicitudes enviadas a cualquier espacio de trabajo del sistema. <!--ensure this is correct; asking team in slack-->

   * Recibirá una notificación en la aplicación y por correo electrónico que le avisa de que la solicitud se ha enviado correctamente o que se ha enviado para su revisión.
   * Si el formulario de solicitud estaba asociado a una aprobación, los aprobadores reciben una notificación en la aplicación y por correo electrónico para revisar y aprobar la solicitud.

     >[!NOTE]
     >
     >Las notificaciones por correo electrónico y en la aplicación solo son visibles cuando la instancia de Workfront de su organización está integrada en la experiencia unificada de Adobe.

1. (Opcional) Haga clic en **Ver su solicitud** para abrir la solicitud en Workfront.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (Opcional) Haga clic en **Menú principal** > **Solicitudes** > la pestaña **Planificación** para ver su solicitud y, a continuación, haga clic en el nombre de la solicitud.

   Se abre la página de detalles de la solicitud.

   ![Página de detalles de solicitud](assets/request-details-page.png)

1. (Condicional) Si el formulario de solicitud no está asociado a una aprobación, o si la solicitud se ha aprobado, haga clic en el nombre de la solicitud y, a continuación, haga clic en el nombre del registro en el campo **Registro**.

   La página del registro se abre en Workfront Planning.

   >[!TIP]
   >
   >* Si no se agregó el nombre del registro al formulario de solicitud, el nombre del registro en el campo Registro de la solicitud se mostrará como **Sin título**.
   >
   >* Si el formulario de solicitud está asociado a una aprobación, esta debe concederse antes de que pueda acceder al registro desde la página de solicitud.

1. (Opcional) Haga clic en el nombre de **Tipo de registro**.

   La página de tipo de registro se abre en Workfront Planning.




