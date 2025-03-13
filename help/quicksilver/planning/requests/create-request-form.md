---
title: Creación y administración de un formulario de solicitud en Adobe Workfront Planning
description: Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede crear un formulario de solicitud y asociarlo a ese tipo de registro. A continuación, puede compartir un vínculo con otros usuarios internos o externos. Los usuarios con un vínculo al formulario pueden rellenar los valores de campo que contiene y, al enviarlo, pueden agregar un nuevo registro para el tipo de registro asociado a él.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: a3c82d8be6945a91a249d64923c6377a5edfa268
workflow-type: tm+mt
source-wordcount: '2084'
ht-degree: 10%

---

# Creación y administración de un formulario de solicitud en Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


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
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p>
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
   <li><p>Administrar permisos en un área de trabajo <!--<span class="preview">and record type</span>--> </p></li>
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

## Limitaciones de visualización de campos y valores en formularios de solicitud

Existen limitaciones en la forma en que se muestran ciertos campos en el formulario de solicitud y en la forma en que sus valores se muestran posteriormente en los registros o en la página de detalles de la solicitud después de enviar una solicitud.

Para obtener información sobre cómo enviar solicitudes de Workfront Planning, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

* Las siguientes son limitaciones de la forma en que se muestran ciertos campos en los formularios de solicitud, los registros creados por un formulario de solicitud o en la página de detalles de la solicitud:

   * No se pueden agregar campos de los siguientes tipos a un formulario de solicitud:

      * Creado por y modificado por última vez por
      * Fecha de creación y fecha de la última modificación
      * Fórmula. <span class="preview">Los campos de fórmula son compatibles con el entorno de vista previa.</span>
      * Campos de búsqueda de objetos Workfront
      * Campos de búsqueda de registros conectados de Workfront Planning

* Las siguientes son diferencias entre la forma en que se muestran los formatos de campo en el generador de formularios de solicitud y el formato de los valores de los campos en el registro o en la página de detalles de la solicitud:

   * Los campos Moneda, Número y Porcentaje se muestran como un campo de texto de una sola línea en el generador de formularios.

     Sin embargo, el formato de campo se conserva y los valores de los números de estos campos se mostrarán como Valores monetarios, numéricos y de porcentaje en el tipo de registro y en la página de detalles de la solicitud.

<div class="preview">

* A continuación se describe cómo se muestran algunos valores de campo en los formularios de solicitud y en las páginas de detalles de solicitud:

   * No se conserva el formato especial de los campos Moneda, Número y Porcentaje. Por ejemplo, la precisión decimal no se conserva para los valores de estos campos en estas áreas.
   * Los valores del campo Personas se muestran como ID.
   * Los campos de fórmula que no hacen referencia a otros campos o cálculos no muestran ningún valor. Por ejemplo, un campo con una fórmula `STRING` muestra un valor &quot;N/A&quot;.
   * Los campos de fórmula que hacen referencia a los campos Moneda muestran los valores sin tener en cuenta los tipos de cambio.
   * Los valores de los campos de párrafo muestran un valor &quot;N/A&quot; en el formulario de solicitud y muestran etiquetas html en lugar del texto con formato en la página de detalles de la solicitud.

</div>

## Creación de un formulario de solicitud para un tipo de registro

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee añadir registros.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro en el encabezado de la página y, a continuación, haga clic en **Crear formulario de solicitud** <span class="preview">o **Administrar formulario de solicitud**, si ya tiene un formulario y desea crear otros</span>.
1. Actualice el nombre del formulario de solicitud. De manera predeterminada, el nombre del formulario es **Formulario sin título**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Opcional) Agregue una **Descripción** para el formulario de solicitud.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Haga clic en **Crear**. El formulario de solicitud del tipo de registro seleccionado se abre en la pestaña Formulario.

   ![Modo de edición del formulario de solicitud de campañas](assets/campaigns-request-form-edit-mode.png)

   El formulario de solicitud contiene la siguiente información de forma predeterminada:

   * Campos de registro disponibles en la vista de tabla del tipo de registro seleccionado. <!--they are working on removing the limitation below-->

   * **Sección predeterminada**: Este es el salto de sección predeterminado que Workfront aplica al formulario de solicitud. Todos los campos de registro se muestran en el área **Sección predeterminada**.
   * Campo **Asunto**: Campo que identificará la solicitud en Workfront. La configuración y el valor del campo Subject no se pueden editar.

     >[!TIP]
     >
     >El campo **Asunto** requiere un valor cuando esté visible en el formulario de solicitud. Sin embargo, puede quitar el campo **Subject** si es necesario, y los solicitantes no lo verán en el formulario cuando envíen la solicitud.

   * Todos los campos asociados al tipo de registro.

     Los campos contenidos en el formulario de solicitud serán visibles para todos los que envíen una solicitud a este tipo de registro.

1. (Opcional) Pase el ratón sobre cualquier campo del formulario que quiera quitar y luego haga clic en el icono **x** para quitarlo. Se agregarán a la ficha **Campos** situada a la izquierda del formulario.

   Por ejemplo, quite el campo **Asunto**, ya que esto no es visible en Workfront Planning. <!--remove this example if this becomes visible in Planning?-->

1. (Opcional) Para quitar la **sección predeterminada** del formulario, haga lo siguiente:

   1. Elimine todos los campos de la sección predeterminada.
   1. Haga clic en **Elementos de contenido** y agregue una nueva sección; a continuación, agregue un nombre para la sección.
   1. Agregue campos a la nueva sección.
   1. Haga clic en el icono **x** para quitar la **sección predeterminada**.
1. Haga clic en cualquier campo y, a continuación, utilice los controles del panel derecho del formulario para definir su tamaño o cualquiera de las siguientes informaciones:

   * **Etiqueta**: este es el nombre del campo tal como aparecerá en el formulario de solicitud. Esto no cambia el nombre del campo de registro.
   * **Instrucciones**: Agregue más información sobre el campo.
   * **Crear un campo obligatorio**: cuando se selecciona, el campo debe tener un valor. De lo contrario, el formulario no se podrá enviar.
   * **Agregar lógica**: defina qué condiciones deben cumplirse para que el campo se muestre o se oculte.

   >[!TIP]
   >
   >   El tipo de campo de cada campo se muestra en la parte superior del panel derecho, después de seleccionar el campo en el formulario.
   >     

1. (Opcional) Haga clic en la pestaña **Elementos de contenido** de la parte izquierda del formulario y agregue cualquiera de los siguientes elementos:

   * **Texto descriptivo**
   * **Salto de sección**

   Para obtener más información sobre cómo crear un formulario personalizado, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Opcional) Haga clic en **Vista previa** para ver cómo se mostrará el formulario para otros usuarios cuando lo usen para enviar un nuevo registro.

1. (Opcional) Haga clic en la ficha **Configuración** y, a continuación, agregue al menos un usuario al campo **Aprobadores** para aprobar nuevas solicitudes para este formulario de registro.

   ![Ficha de configuración](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Al asociar un formulario de solicitud con los aprobadores, cualquier nueva solicitud debe ser aprobada primero por todos los aprobadores antes de que genere un nuevo registro.
   * Puede agregar uno o varios aprobadores a un formulario de solicitud.
   * Si al menos un aprobador rechaza la solicitud, esta se rechaza y no se crea el registro.
   * Todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.

     Para obtener más información sobre cómo agregar aprobaciones a los formularios de solicitud, consulte [Agregar aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Opcional) Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del formulario en el encabezado y, a continuación, haga clic en **Editar** para actualizar el nombre del formulario.
1. Haga clic en **Publicar** para publicar el formulario y obtener un vínculo único para él.

   Ocurren lo siguiente:

   * Se ha quitado el botón **Publicar**.
   * Se agrega el botón **Cancelar publicación** al formulario. Si hace clic en él, se impedirá el acceso al formulario.
   * Se agrega un botón **Compartir** al formulario.

1. Haga clic en **Compartir** para compartir el formulario con otros usuarios.

   ![Compartir la casilla del formulario de solicitud](assets/share-box-for-request-form.png)

1. Seleccione entre las siguientes opciones para indicar qué tipos de usuarios pueden acceder a este formulario:

   * Cualquiera con acceso de visualización o más alto al espacio de trabajo
   * Cualquiera con acceso de aportación o más alto al espacio de trabajo
   * Cualquiera con el vínculo

   >[!WARNING]
   >
   >* Si selecciona **Cualquier persona que tenga el vínculo**, cualquier persona podrá obtener acceso al formulario y enviar un nuevo registro, incluso las personas que no pertenezcan a su organización y que no tengan una cuenta de Workfront.
   >
   >* Un formulario que contenga los siguientes tipos de campo no se puede compartir públicamente:
   >
   >     * Conexiones de Workfront o AEM Assets
   >     * Personas
   >

1. (Condicional) Si seleccionó **Cualquier persona con el vínculo** en el paso anterior, seleccione **Fecha de caducidad del vínculo** del calendario disponible. <!--take out this tip when we release to production as in multiple forms this is no longer happening-->

   >[!TIP]
   >
   >Hay indicios de que el vínculo se comparte públicamente cuando este es el caso.
   >![Vínculo compartido públicamente al formulario en el menú de tipo de registro](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)

   Las personas recibirán un error una vez que caduque el vínculo y debe actualizar la fecha del vínculo y generar un nuevo vínculo para compartirlo antes de que las personas puedan acceder al formulario de nuevo.

   Puede seleccionar fechas futuras en un plazo de 180 días a partir de la fecha actual.

   >[!TIP]
   >
   ><span class="preview">Una vez que caduca la fecha de uso compartido, el formulario de solicitud ya no está disponible en el área de solicitudes de Workfront.</span>


1. <span class="preview">(Opcional)</span> Haga clic en **Guardar y copiar vínculo** para guardar los detalles de uso compartido del formulario. Si el formulario se guardó anteriormente, haga clic en **Copiar vínculo**.

   Las opciones de uso compartido de formularios se guardan y el vínculo se copia en el portapapeles. Ahora puede compartirlo con otros usuarios.

   Para obtener información sobre cómo crear registros mediante un vínculo a un formulario de solicitud, consulte [Enviar solicitudes de Adobe Workfront Planning](/help/quicksilver/planning/requests/submit-requests.md).

1. Haga clic en **Guardar** en la esquina inferior derecha de la pestaña **Formulario** para guardar el formulario.

1. Haga clic en la flecha que señala a la izquierda del nombre del formulario en el encabezado para cerrar el formulario.

   <span class="preview">Se abre la vista de tabla de **Formularios de solicitud** y se agrega el formulario.</span>

1. <span class="preview">(Opcional) Pase el ratón sobre el nombre de un formulario de solicitud en la vista de tabla, luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png) a la derecha del nombre del formulario y haga clic en una de las siguientes opciones:</span>

   * <span class="preview">**Editar formulario**: haga clic aquí para editar más información en el formulario. </span>
   * <span class="preview"> **Cancelar publicación**: haga clic aquí para cancelar la publicación del formulario que lo quita del área de solicitudes en Workfront. </span>
   * <span class="preview">**Compartir**: haga clic aquí para modificar quién tiene acceso al formulario. </span>
   * <span class="preview">**Copiar vínculo**: haga clic aquí para copiar rápidamente el vínculo del formulario de solicitud sin abrir el formulario. </span>
   * <span class="preview">**Eliminar**: haga clic aquí para eliminar el formulario. No se eliminan todas las solicitudes y registros agregados mediante el formulario. El formulario no se puede recuperar. </span>

   ![Menú más en el formulario de solicitud de la lista de formularios de solicitud](assets/more-menu-on-request-form-from-request-forms-list.png)


1. <span class= "preview">Haga clic en la flecha que señala a la izquierda de **Solicitar formularios** en el encabezado para cerrar la tabla de formularios de solicitud.   </span>

   <span class= "preview">Se abre la página de tipo de registro. </span>
1. (Opcional y condicional) En el entorno Producción, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) a la derecha del nombre del tipo de registro en el encabezado y, a continuación, siga uno de estos procedimientos:
   * Haga clic en **Actualizar formulario de solicitud** para realizar cualquier cambio en el formulario de solicitud.
   * Haga clic en **Copiar vínculo al formulario de solicitud** para compartir el vínculo al formulario con otros usuarios.

1. <span class="preview"> (opcional y condicional) En el entorno de vista previa, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) a la derecha del nombre del tipo de registro en el encabezado y, a continuación, haga clic en **Administrar formularios de solicitud**. </span>

   <span class="preview">Se abrirá la vista de tabla de formularios de solicitud. </span>
1. <span class="preview">Haga clic en un formulario de solicitud para abrirlo y editarlo.</span>
1. <span class= "preview">(Opcional) Vaya al área de **Solicitudes** en Workfront y busque el formulario compartido para enviar una solicitud. Para obtener más información, vea [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).</span>
