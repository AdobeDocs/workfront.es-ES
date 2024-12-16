---
title: Envío de solicitudes de Adobe Workfront Planning
description: Una vez que alguien comparta un vínculo a un formulario de solicitud con usted desde una página de tipo de registro en Adobe Workfront Planning, puede añadir una solicitud para crear registros para el tipo de registro asociado al formulario de solicitud.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 9b5ba629fa2f50f0425f4afbfd4faa891d917845
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 19%

---

# Envío de solicitudes de Adobe Workfront Planning para crear registros

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Una vez que alguien comparta un vínculo a un formulario de solicitud con usted desde una página de tipo de registro en Adobe Workfront Planning, puede añadir una solicitud para crear registros para el tipo de registro asociado al formulario de solicitud.

Los usuarios de Workfront y los usuarios externos pueden enviar solicitudes a los tipos de registros de Planning y crear registros. <!--double check on the external users-->

Este artículo describe cómo puede enviar una solicitud para agregar nuevos registros a un tipo de registro.

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
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p>
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
   <p>Permisos de vista o superiores de un espacio de trabajo, si es un usuario de Workfront</p> 
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
   * Un tipo de registro asociado a un formulario de solicitud. Para obtener más información, consulte [Crear un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* El formulario de solicitud debe compartirse con un vínculo para que pueda acceder a él. Se dan los siguientes escenarios:

   * Si tiene una cuenta de Workfront, el vínculo se ha compartido únicamente con personas internas y tendrá acceso de contribución o superior al espacio de trabajo. Las personas fuera de Workfront no pueden acceder a un vínculo compartido internamente.
   * Si no tiene una cuenta de Workfront, el vínculo se ha compartido con personas externas. Los usuarios de Workfront también pueden acceder a un vínculo compartido con personas externas.

* El vínculo al formulario no debe haber caducado.

## Consideraciones sobre el envío de solicitudes a Workfront Planning

* Solo puede acceder a un formulario de solicitud de solicitudes de Workfront Planning desde un vínculo específico al formulario.
* No puede editar una solicitud después de enviarla a Workfront Planning.
* Cada solicitud enviada crea un registro para el tipo de registro asociado con el formulario que utiliza <span class="preview">si el formulario no está asociado a una aprobación, o si la aprobación ha sido concedida por todos los aprobadores.</span>
* Los registros creados al enviar formularios de solicitud no se pueden diferenciar de los registros agregados mediante ningún otro método. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
* <span class="preview">Las solicitudes enviadas se muestran en la ficha Planificación de la sección Enviadas del área Solicitudes de Workfront </span>.

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Envío de una solicitud a Workfront Planning

1. Vaya al vínculo compartido con usted desde un tipo de registro de Workfront Planning.

1. Actualice los campos disponibles en el formulario. Los campos con asterisco son obligatorios.

   >[!TIP]
   >
   >   Si el campo **Asunto** está disponible, no será visible en Workfront Planning una vez enviada la solicitud.
   >
   >Se recomienda actualizar tantos campos de la solicitud como sea posible para que el nuevo registro sea identificable cuando se añada al tipo de registro en Workfront Planning.

1. Haga clic en **Enviar**.

   El formulario se enviará y se producirán los siguientes eventos:

   * Si el formulario de solicitud no estaba asociado a una aprobación, o <span class="preview">si la aprobación fue concedida por todos los aprobadores,</span> se agrega un nuevo registro al tipo de registro asociado al formulario.

   * Si el formulario de solicitud no estaba asociado a una aprobación, la solicitud <span class="preview"> se agrega a la ficha Planificación de la sección Enviados del área Solicitudes de Workfront y se agrega un nuevo registro a la página de tipo de registro.</span>

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     ><span class="preview">Todos los usuarios que tengan acceso al menos a un área de trabajo podrán ver la ficha Planificación en el área Solicitudes. Solo puede ver las solicitudes enviadas por usted o por cualquier otra persona a los espacios de trabajo para los que tiene al menos permisos de Vista. Los administradores de Workfront pueden ver todas las solicitudes enviadas a cualquier espacio de trabajo del sistema. </span> <!--ensure this is correct; asking team in slack-->

   * <span class="preview">Si el formulario de solicitud estaba asociado a una aprobación, la solicitud se guarda temporalmente en la pestaña Planificación de la sección Enviado del área Solicitudes de Workfront. No se ha creado ningún registro para el tipo de registro asociado al formulario de solicitud.</span>

     <span class="preview">Para obtener más información, consulte [Agregar una aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).</span>
   * <span class="preview">Recibe una notificación en la aplicación y por correo electrónico que indica que la solicitud se ha enviado correctamente o que se ha enviado para su revisión.</span>
   * <span class="preview">Si el formulario de solicitud estaba asociado con una aprobación, los aprobadores recibirán una notificación en la aplicación y por correo electrónico para revisar y aprobar la solicitud.</span>

     >[!NOTE]
     >
     ><span class="preview">Las notificaciones por correo electrónico y en la aplicación solo son visibles cuando la instancia de Workfront de su organización está integrada en la experiencia unificada de Adobe.</span>




