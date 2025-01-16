---
title: Creación y administración de un formulario de solicitud en Adobe Workfront Planning
description: Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede crear un formulario de solicitud y asociarlo a ese tipo de registro. A continuación, puede compartir un vínculo con otros usuarios internos o externos. Los usuarios con un vínculo al formulario pueden rellenar los valores de campo que contiene y, al enviarlo, pueden agregar un nuevo registro para el tipo de registro asociado a él.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 14%

---

# Creación y administración de un formulario de solicitud en Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Puede crear un formulario de solicitud y asociarlo a un tipo de registro en Adobe Workfront Planning. A continuación, puede compartir un vínculo con otros usuarios internos o externos.

Los usuarios con un vínculo al formulario pueden actualizar los valores de campo que contiene y agregar nuevos registros enviándolo.

Este artículo describe cómo un administrador del espacio de trabajo puede crear un formulario de solicitud asociado a un tipo de registro.

Para obtener información sobre cómo enviar una solicitud a un tipo de registro para crear un registro, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

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
   <p>Estándar</p>
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
   <ul>
   <li><p>Administración de permisos en un espacio de trabajo</p></li>
    <li><p>Los administradores del sistema pueden administrar los espacios de trabajo que no hayan creado. </p></li>
    </ul>
   <p>Para obtener información acerca de los permisos de uso compartido para objetos de Workfront Planning, consulte 
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Información general sobre los permisos de uso compartido en Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de un formulario de solicitud para un tipo de registro

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee añadir registros.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.

1. Haga clic en el menú **Más** ![](assets/more-menu.png) a la derecha del nombre del tipo de registro en el encabezado de la página y, a continuación, haga clic en **Crear formulario de solicitud**.
1. Actualice el nombre del formulario de solicitud. De manera predeterminada, el nombre del formulario es **Formulario sin título**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Opcional) Agregue una **Descripción** para el formulario de solicitud.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Haga clic en **Crear**. El formulario de solicitud del tipo de registro seleccionado se abre en la pestaña Formulario.

   ![](assets/campaigns-request-form-edit-mode.png)

   El formulario de solicitud contiene la siguiente información de forma predeterminada:

   * Campos de registro disponibles en la vista de tabla del tipo de registro seleccionado. <!--they are working on removing the limitation below-->

   <!-- when we go to prod, the Preview batch below will become the only batch-->

   >[!IMPORTANT]
   >
   >Los campos de los siguientes tipos no se muestran en el formulario de solicitud:
   >
   >* Creado por y modificado por última vez por
   >* Fecha de creación y fecha de la última modificación
   >* Fórmula
   >* Campos de búsqueda de objetos Workfront
   >* Campos de búsqueda de registros conectados de Workfront Planning
   >

   <!--before release to prod: 
    > Depending on what environment you use to create a request form, the following scenarios exist:
   >
   >* Fields of the following types do not display in the request form in the Production environment: 
   >
   >    * Created by and Last modified by
   >    * Created date and Last modified date
   >    * Formula
   >    * People 
   >    * Workfront connected fields
   >    * Workfront objects' lookup fields
   >    * Workfront Planning records' connected fields
   >    * Workfront Planning connected records' lookup fields
   >    * AEM Assets connection fields-->

   * **Sección predeterminada**: Este es el salto de sección predeterminado que Workfront aplica al formulario de solicitud. No se puede cambiar el nombre de la sección predeterminada ni eliminarla.
   * Campo **Asunto**: Campo que identificará la solicitud en Workfront. La configuración y el valor del campo Subject no se pueden editar.

     >[!TIP]
     >
     >El campo **Asunto** requiere un valor cuando esté visible en el formulario de solicitud. Sin embargo, puede quitar el campo **Subject** si es necesario, y los solicitantes no lo verán en el formulario cuando envíen la solicitud.

   * Todos los campos asociados al tipo de registro.

     Los campos contenidos en el formulario de solicitud serán visibles para todos los que envíen una solicitud a este tipo de registro.

1. (Opcional) Pase el ratón sobre cualquier campo del formulario que quiera quitar y luego haga clic en el icono **x** para quitarlo. Se agregarán a la ficha **Campos** situada a la izquierda del formulario.

   Por ejemplo, quite el campo **Asunto**, ya que esto no es visible en Workfront Planning. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Haga clic en cualquier campo y, a continuación, utilice los controles del panel derecho del formulario para definir su tamaño o cualquiera de las siguientes informaciones:

   * **Etiqueta**: este es el nombre del campo tal como aparecerá en el formulario de solicitud. Esto no cambia el nombre del campo de registro.
   * **Instrucciones**: Agregue más información sobre el campo.
   * **Crear un campo obligatorio**: cuando se selecciona, el campo debe tener un valor. De lo contrario, el formulario no se podrá enviar.
   * **Agregar lógica**: defina qué condiciones deben cumplirse para que el campo se muestre o se oculte.

   >[!NOTE]
   >
   >   El tipo de campo de cada campo se muestra en la parte superior del panel derecho, después de seleccionar el campo en el formulario.
   >   
   >
   >   Los campos Moneda, Número y Porcentaje se muestran como un campo de texto de una sola línea. Sin embargo, el formato de campo se conserva y los valores dentro de estos campos se mostrarán como Valores monetarios, numéricos y de porcentaje.

1. (Opcional) Haga clic en la pestaña **Elementos de contenido** de la parte izquierda del formulario y agregue cualquiera de los siguientes elementos:

   * **Texto descriptivo**
   * **Salto de sección**

   Para obtener más información sobre cómo crear un formulario personalizado, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Opcional) Haga clic en **Vista previa** para ver cómo se mostrará el formulario para otros usuarios cuando lo usen para enviar un nuevo registro.

1. (Opcional) Haga clic en la ficha **Configuración** y, a continuación, agregue al menos un usuario al campo **Aprobadores** para aprobar nuevas solicitudes para este formulario de registro.

   ![](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Al asociar un formulario de solicitud con los aprobadores, cualquier nueva solicitud debe ser aprobada primero por todos los aprobadores antes de que genere un nuevo registro.
   * Puede agregar uno o varios aprobadores a un formulario de solicitud.
   * Si al menos un aprobador rechaza la solicitud, esta se rechaza y no se crea el registro.
   * Todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.

     Para obtener más información sobre cómo agregar aprobaciones a los formularios de solicitud, consulte [Agregar aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Opcional) Haga clic en el menú **Más** ![](assets/more-menu.png) que se encuentra a la derecha del nombre del formulario en el encabezado y, a continuación, haga clic en **Editar** para actualizar el nombre del formulario.
1. Haga clic en **Publish** para publicar el formulario y obtener un vínculo único para él.

   Ocurren lo siguiente:

   * Se ha quitado el botón **Publish**.
   * Se agrega el botón **Cancelar publicación** al formulario. Si hace clic en él, se impedirá el acceso al formulario.
   * Se agrega un botón **Compartir** al formulario.

1. Haga clic en **Compartir** para compartir el formulario con otros usuarios.

   ![](assets/share-box-for-request-form.png)

1. Seleccione entre las siguientes opciones para indicar qué tipos de usuarios pueden acceder a este formulario:

   * Cualquiera con acceso de visualización o más alto al espacio de trabajo
   * Cualquiera con acceso de aportación o más alto al espacio de trabajo
   * Cualquiera con el vínculo

   >[!WARNING]
   >
   >* Si selecciona **Cualquier persona que tenga el vínculo**, cualquier persona podrá obtener acceso al formulario y enviar un nuevo registro, incluso las personas que no pertenezcan a su organización y que no tengan una cuenta de Workfront.
   >
   > * Un formulario que contenga los siguientes tipos de campo no se puede compartir públicamente:
   >
   >     * Conexiones de Workfront o AEM Assets
   >     * Personas
   >

1. (Condicional) Si seleccionó **Cualquier persona con el vínculo** en el paso anterior, seleccione **Fecha de caducidad del vínculo** del calendario disponible. Las personas recibirán un error una vez que caduque el vínculo y debe actualizar la fecha del vínculo y generar un nuevo vínculo para compartirlo antes de que las personas puedan acceder al formulario de nuevo.

   Puede seleccionar fechas futuras en un plazo de 180 días a partir de la fecha actual.

1. Haga clic en **Guardar y copiar vínculo** para guardar los detalles de uso compartido del formulario. Si el formulario se guardó anteriormente, haga clic en **Copiar vínculo**.

   Las opciones de uso compartido de formularios se guardan y el vínculo se copia en el portapapeles. Ahora puede compartirlo con otros usuarios.

   Para obtener información sobre cómo crear registros mediante un vínculo a un formulario de solicitud, consulte [Enviar solicitudes de Adobe Workfront Planning](/help/quicksilver/planning/requests/submit-requests.md).

1. Haga clic en **Guardar** en la esquina inferior derecha de la pestaña **Formulario** para guardar el formulario.
1. Haga clic en la flecha que señala a la izquierda del nombre del formulario en el encabezado para cerrar el formulario.

   Se abre la página de tipo de registro.
1. (Opcional) Haga clic en el menú **Más** ![](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro en el encabezado y, a continuación, siga uno de estos procedimientos:
   * Haga clic en **Actualizar formulario de solicitud** para realizar cualquier cambio en el formulario de solicitud.
   * Haga clic en **Copiar vínculo al formulario de solicitud** para compartir el vínculo al formulario con otros usuarios.

   >[!TIP]
   >
   >Hay indicios de que el vínculo se comparte públicamente cuando este es el caso.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
