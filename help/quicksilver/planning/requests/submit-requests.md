---
title: Envío de solicitudes de Adobe Workfront Planning
description: Una vez que alguien comparta un vínculo a un formulario de solicitud con usted desde una página de tipo de registro en Adobe Workfront Planning, puede agregar una solicitud para crear registros para el tipo de registro asociado al formulario de solicitud.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: bffa5992a530761afe57ec62b4cbba2bf03ad1e6
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 1%

---

# Envío de solicitudes de Adobe Workfront Planning para crear registros

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

{{planning-important-intro}}

Una vez que alguien comparta un vínculo a un formulario de solicitud con usted desde una página de tipo de registro en Adobe Workfront Planning, puede agregar una solicitud para crear registros para el tipo de registro asociado al formulario de solicitud.

Los usuarios de Workfront y los usuarios externos pueden enviar solicitudes a los tipos de registros de Planning y crear registros. <!--double check on the external users-->

Este artículo describe cómo puede enviar una solicitud para agregar nuevos registros a un tipo de registro.

Para obtener información sobre cómo un administrador del área de trabajo puede crear un formulario de solicitud y asociarlo a un tipo de registro, vea [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para poder acceder a Workfront Planning:

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
   <td role="rowheader"><p>plan Adobe Workfront*</p></td>
   <td>
<p>Cualquiera de los siguientes planes de Workfront:</p>
<ul><li>Seleccionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning no está disponible para planes Workfront heredados</p>
   </td>
<tr>
   <td role="rowheader"><p>Plan de planificación de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera </p>  
<p>Para obtener más información sobre lo que se incluye en cada plan de Workfront Planning, consulte <a href="https://business.adobe.com/products/workfront/pricing.html">Precios y empaquetado de Adobe Workfront</a>. </td>
<tr>
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td>
   <td>
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p>
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p>
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
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
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

* El formulario de solicitud debe compartirse con un vínculo para que pueda acceder a él. Existen los siguientes escenarios:

   * Si tiene una cuenta de Workfront, el vínculo solo se ha compartido con personas internas y tendrá acceso al espacio de trabajo. Las personas fuera de Workfront no pueden acceder a un vínculo compartido internamente.
   * Si no tiene una cuenta de Workfront, el vínculo se ha compartido con personas externas. Los usuarios de Workfront también pueden acceder a un vínculo compartido con personas externas.

* El vínculo al formulario no debe haber caducado.

## Consideraciones sobre el envío de solicitudes a Workfront Planning

* No puede acceder a los formularios de solicitud de las solicitudes de Workfront Planning sin un vínculo específico a los formularios.
* No puede editar una solicitud después de enviarla a Workfront Planning.
* Cada solicitud enviada crea un registro para el tipo de registro asociado al formulario que utiliza.
* Los registros creados al enviar formularios de solicitud no se pueden diferenciar de los registros agregados mediante ningún otro método. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).

## Envío de una solicitud a Workfront Planning

1. Vaya al vínculo compartido con usted desde un tipo de registro de Workfront Planning.

1. Actualice los campos disponibles en el formulario. Los campos con asterisco son obligatorios.

   >[!TIP]
   >
   >   Si el campo de Workfront **Subject** está disponible, es posible que no esté visible en Workfront Planning. Le recomendamos que actualice tantos campos de la solicitud como sea posible para que el nuevo registro sea identificable cuando se añada al tipo de registro.

1. Haga clic en **Enviar**.

   El formulario se enviará y se agregará un nuevo registro al tipo de registro asociado al formulario.





