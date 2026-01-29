---
title: Creación y administración de un formulario de solicitud en Adobe Workfront Planning
description: Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede crear un formulario de solicitud y asociarlo a ese tipo de registro. A continuación, puede compartir un vínculo con otros usuarios internos o externos. Los usuarios con un vínculo al formulario pueden rellenar los valores de campo que contiene y, al enviarlo, pueden agregar un nuevo registro para el tipo de registro asociado a él.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '3518'
ht-degree: 4%

---

# Creación y administración de un formulario de solicitud en Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Puede crear un formulario de solicitud y asociarlo a un tipo de registro en Adobe Workfront Planning. A continuación, puede compartir el formulario con otros usuarios y estos pueden enviar solicitudes para crear registros de ese tipo.

Este artículo describe cómo un administrador del espacio de trabajo puede crear un formulario de solicitud asociado a un tipo de registro.

Para obtener información sobre cómo enviar una solicitud a un tipo de registro para crear un registro, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

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
   <td><p>Estándar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administrar permisos a un espacio de trabajo o tipo de registro</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limitaciones de visualización de campos y valores en formularios de solicitud

Existen limitaciones en la forma en que se muestran ciertos campos en el formulario de solicitud y en la forma en que sus valores se muestran posteriormente en los registros o en la página de detalles de la solicitud después de enviar una solicitud.

Para obtener información sobre cómo enviar solicitudes de Workfront Planning, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

* Las siguientes son limitaciones de la forma en que se muestran ciertos campos en los formularios de solicitud, los registros creados por un formulario de solicitud o en la página de detalles de la solicitud:

   * No se pueden agregar campos de los siguientes tipos a un formulario de solicitud:

      * Creado por, Última modificación por, Aprobado por
      * Fecha de creación, Fecha de la última modificación, Fecha de aprobación
      * Campos de búsqueda de objetos Workfront
      * Campos de búsqueda de registros conectados de Workfront Planning

* Las siguientes son diferencias entre la forma en que se muestran los formatos de campo en el generador de formularios de solicitud y el formato de los valores de los campos en el registro o en la página de detalles de la solicitud:

   * Los campos Moneda, Número y Porcentaje se muestran como un campo de texto de una sola línea en el generador de formularios.

     Sin embargo, el formato de campo se conserva y los valores de campo se muestran como moneda, números y porcentajes después de enviar la solicitud, en el tipo de registro y en la página de detalles de la solicitud.

* A continuación se describe cómo se muestran algunos valores de campo en los formularios de solicitud y en las páginas de detalles de solicitud:

   * No se conserva el formato especial de los campos Moneda, Número y Porcentaje. Por ejemplo, la precisión decimal no se conserva para los valores de estos campos en estas áreas.
   * Los valores del campo Personas se muestran como ID.
   * Los campos de fórmula que no hacen referencia a otros campos o cálculos no muestran ningún valor. Por ejemplo, un campo con una fórmula `STRING` muestra un valor &quot;N/A&quot;.
   * Los campos de fórmula que hacen referencia a los campos Moneda muestran los valores sin tener en cuenta los tipos de cambio.
   * Los valores de los campos de párrafo muestran un valor &quot;N/A&quot; en el formulario de solicitud y muestran etiquetas html en lugar del texto con formato en la página de detalles de la solicitud.

## Creación de un formulario de solicitud

Para crear un formulario de solicitud, debe empezar a crearlo, configurar los detalles del formulario y terminar publicándolo y compartiéndolo.

### Empezar a crear un formulario de solicitud

Puede crear un formulario de solicitud a partir del tipo de registro asociado al formulario <!--span class="preview">, or from the Requests area of Workfront.</span>-->.

#### Creación de un formulario de solicitud a partir de un tipo de registro

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee añadir registros.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro en el encabezado de la página y, a continuación, haga clic en **Crear formulario de solicitud** o **Administrar formularios de solicitud**, si ya tiene un formulario y desea crear otros.
1. (Condicional) Si desea agregar otro formulario, haga clic en **Nuevo formulario de solicitud**.

   Se abrirá el cuadro de diálogo Crear formulario de solicitud.

1. En el cuadro Crear formulario de solicitud, actualice el nombre del formulario de solicitud. De manera predeterminada, el nombre del formulario es **Formulario sin título**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Opcional) Agregue una **Descripción** para el formulario de solicitud.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Haga clic en **Crear**.

   El formulario de solicitud del tipo de registro seleccionado se abre en la pestaña Formulario.
1. Continúe con [Configurar detalles para el formulario de solicitud](#set-up-details-for-the-request-form).

<!--

<div class="preview">

#### Create a request form from the Requests area of Workfront

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Requests**.
1. In the upper-right corner of the screen, click **Request forms**.
1. (Conditional) If you are editing an existing request form, select it from the list, then continue to [Configure the form](#confgure-the-form).
1. If you are creating a new request form, in the upper-right corner of the screen, click **New request form**.

   The Create request form box opens

1. In the Create request form box, update the name of the request form. By default, the name of the form is **Untitled form**. 
1. In the Object types field, select the record type that the request form will be associated with. Record types are grouped into the workspace that they exist within.
1. (Optional) Add a **Description** for the request form. 

1. Click **Create**. 

   The request form for the selected record type opens in the Form tab.
1. Continue to [Set up details for the request form](#set-up-details-for-the-request-form).



</div>

-->

### Configuración de detalles para el formulario de solicitud

Los detalles del formulario se dividen en pestañas.

* La pestaña **Formulario** le permite agregar campos y elementos de contenido al formulario
* La ficha **Configuración** le permite establecer un proceso de aprobación para el formulario y establecer opciones de finalización de solicitudes.

  >[!NOTE]
  >
  ><span class="preview">En el entorno de vista previa, la ficha Configuración reemplaza a la ficha Configuración.</span>
  <!--* <span class="preview">The **Automations** tab allows you to automate what will occur based on features of the request made with the form.</span>-->

#### Configuración de detalles del formulario

1. Comience a crear o editar un formulario de solicitud, tal como se describe en la sección [Comience a crear un formulario de solicitud](#begin-creating-a-request-form).

   O

   Busque el formulario de solicitud en la lista Formularios de solicitud, haga clic en el cuadro situado junto al nombre del formulario y, a continuación, haga clic en **Editar formulario** en la barra azul de la parte inferior de la pantalla.

   El formulario de solicitud del tipo de registro seleccionado se abre en la pestaña Formulario.

   ![Modo de edición del formulario de solicitud de campañas](assets/campaigns-request-form-edit-mode.png)

   El formulario de solicitud contiene la siguiente información de forma predeterminada:

   * Campos de registro disponibles en la vista de tabla del tipo de registro seleccionado. <!--they are working on removing the limitation below-->

   * **Sección predeterminada**: Este es el salto de sección predeterminado que Workfront aplica al formulario de solicitud. Todos los campos de registro se muestran en el área **Sección predeterminada**.
   * Campo **Asunto**: Campo que identificará la solicitud en Workfront. La configuración y el valor del campo Subject no se pueden editar.

     >[!NOTE]
     >
     >* El campo **Asunto** requiere un valor cuando esté visible en el formulario de solicitud. Sin embargo, puede quitar el campo **Subject** si es necesario, y los solicitantes no lo verán en el formulario cuando envíen la solicitud.
     >* Cuando falta el campo Subject en un formulario de solicitud, pero hay un campo Name para el nombre del registro futuro, se asigna automáticamente el mismo nombre a la solicitud que al registro creado.
     >* Cuando faltan los campos Asunto y Nombre en el formulario de solicitud, se asigna un nombre a la solicitud según el siguiente patrón: `< Record name > request form < Entry date of the request >`; el registro se denomina **Sin título**.

   * Todos los campos asociados al tipo de registro.

     Los campos contenidos en el formulario de solicitud serán visibles para todos los que envíen una solicitud a este tipo de registro.

1. (Opcional) Pase el ratón sobre cualquier campo del formulario que quiera quitar y luego haga clic en el icono **x** para quitarlo. Se agregarán a la ficha **Campos** situada a la izquierda del formulario.

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
1. Continúe con una de las siguientes acciones:

   * [Configurar detalles de configuración](#set-up-configuration-details) si desea configurar más detalles para el formulario en el entorno de producción
   * <span class="preview">[Configurar opciones](#configure-settings) si desea configurar más detalles para el formulario en el entorno de producción</span>
   * [Complete la creación del formulario de solicitud](#complete-request-form-creation) si no desea configurar más opciones.

#### Configurar los detalles de configuración

>[!NOTE]
>
>Esta pestaña solo está disponible en el entorno de producción.

En la pestaña Configuración, puede establecer el proceso de aprobación y configurar cuándo se marcará como Completada una solicitud creada a partir de este formulario.

1. Comience a crear o editar un formulario de solicitud, tal como se describe en la sección [Comience a crear un formulario de solicitud](#begin-creating-a-request-form).

   El formulario de solicitud del tipo de registro seleccionado se abre en la pestaña Formulario.
1. (Opcional) Configure cualquier detalle del formulario, tal como se describe en [Configurar detalles del formulario](#set-up-form-details).

1. (Opcional) Si desea agregar aprobadores, haga clic en la ficha **Configuración** y, a continuación, agregue al menos un usuario o equipo al campo **Aprobadores** para aprobar nuevas solicitudes para este formulario de registro.

   ![Ficha de configuración](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Puede agregar uno o varios aprobadores a un formulario de solicitud.
   * Si al menos un aprobador rechaza la solicitud, esta se rechaza y no se crea el registro. La solicitud permanece en el área de solicitudes de Workfront.
   * Si añade más de un aprobador y la opción Only one decision is required no está activada, todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.
   * Si un equipo se establece como aprobador, solo se requiere una decisión del equipo.

   Para obtener más información sobre cómo agregar aprobaciones a los formularios de solicitud, consulte [Agregar aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Condicional) Si desea que el registro se cree después de que cualquiera de los aprobadores lo haya aprobado, marque la casilla **Solo se requiere una decisión**.

1. Seleccione si desea que una solicitud creada a partir de este formulario se marque como completada cuando se cree el objeto solicitado o cuando se complete el objeto solicitado.
1. (Condicional) Si ha seleccionado que la solicitud se marque como completada cuando se complete el objeto solicitado, seleccione el campo y el valor que indican cuándo se completa el objeto. Por ejemplo, puede seleccionar el campo Estado y el valor Completar para completar la solicitud cuando el estado del objeto creado se establece en Completar.
1. Continuar a <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[Completar la creación del formulario de solicitud](#complete-request-form-creation).

<div class="preview">

### Configurar opciones

>[!NOTE]
>
>Esta pestaña solo está disponible en el entorno de vista previa.

En la pestaña Settings, puede establecer reglas de aprobación y configurar cuándo una solicitud creada a partir de este formulario se marcará como Completada.

#### Configuración de reglas de aprobación

Las reglas de aprobación definen el proceso de aprobación en función de los valores de campo en las solicitudes enviadas.

Por ejemplo, si un formulario de solicitud tiene el campo &quot;Tipo de campaña&quot;, se puede crear una regla que envíe la solicitud a una persona cuando el campo tenga el valor &quot;Digital&quot; y a una persona diferente cuando tenga el valor &quot;Imprimir&quot;.

Tenga en cuenta lo siguiente al añadir reglas de aprobación:

* Las reglas se priorizan por orden. Si se cumplen las primeras condiciones de regla, se aplica esa regla, incluso si también se cumplen las condiciones para reglas que se encuentran más abajo en la lista.
* Si no se cumple ninguna condición, se aplica la regla predeterminada.
* Puede añadir uno o varios aprobadores a una regla de aprobación.
* Si al menos un aprobador rechaza la solicitud, esta se rechaza y no se crea el registro. La solicitud permanece en el área de solicitudes de Workfront.
* Si añade más de un aprobador y la opción Only one decision is required no está activada, todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.
* Si un equipo se establece como aprobador, solo se requiere una decisión del equipo.

Para obtener más información sobre cómo agregar aprobaciones, consulte [Agregar aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

Para definir reglas de aprobación para un formulario de solicitud:

1. Comience a crear o editar un formulario de solicitud, tal como se describe en la sección [Comience a crear un formulario de solicitud](#begin-creating-a-request-form).

   El formulario de solicitud del tipo de registro seleccionado se abre en la pestaña Formulario.
1. (Opcional) Configure cualquier detalle del formulario, tal como se describe en [Configurar detalles del formulario](#set-up-form-details).

1. Para comenzar a configurar las reglas de aprobación, haga clic en el icono ![Aprobaciones](assets/approvals-icon-on-form.png) de aprobaciones en el panel de navegación izquierdo.

1. (Opcional) Si desea establecer un proceso de aprobación predeterminado, agregue al menos un usuario o equipo al campo **Aprobadores** del área Regla de aprobación predeterminada y, a continuación, haga clic en la casilla de verificación **Solo se requiere una decisión** si desea que el registro se cree después de que cualquiera de los aprobadores predeterminados lo haya aprobado.

   ![Área de regla de aprobación predeterminada](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. (Opcional) Para cada regla de aprobación adicional, haga lo siguiente:

   1. Haga clic en **Agregar regla de aprobación**
   1. Haga clic en el título del marcador de posición &quot;Regla de aprobación sin título&quot; e introduzca un nombre para la regla de aprobación.
   1. Haga clic en **Seleccionar un campo** y seleccione el campo que activa la regla.
   1. Seleccione el operador de la regla. Los operadores varían según el tipo de campo.
   1. Si el operador seleccionado requiere un valor, haga clic en el icono de signo más y añada uno o más valores.
   1. (Opcional) Agregue más condiciones con AND u OR haciendo clic en Agregar condición y configurando la condición adicional.
   1. En el área Acciones de la regla de aprobación, en el campo **Aprobadores**, agregue al menos un usuario o equipo que se establecerá en el aprobador cuando se cumpla la condición.
   1. (Condicional) Si desea que el registro se cree después de que cualquiera de los aprobadores lo haya aprobado, marque la casilla **Solo se requiere una decisión**.

1. (Opcional) Para reordenar las reglas de enrutamiento, haga clic en el controlador de arrastre situado en el lado izquierdo de la regla y arrástrela a la ubicación deseada.

   No se puede reordenar la regla predeterminada.

1. (Opcional) Para eliminar una regla de enrutamiento, haga clic en **X** a la derecha de la regla.
1. Haga clic en **Guardar** para guardar las reglas de aprobación.
1. Continuar a [Establecer opciones de finalización de solicitud](#set-request-completion-options)

#### Establecer opciones de finalización de solicitud

Las opciones de finalización permiten establecer si una solicitud se marca como completada cuando se crea el objeto solicitado o cuando se completa el objeto creado. El usuario define cuándo se completa el objeto en función de una condición especificada.

1. Comience a crear o editar un formulario de solicitud, tal como se describe en la sección [Comience a crear un formulario de solicitud](#begin-creating-a-request-form).

   El formulario de solicitud del tipo de registro seleccionado se abre en la pestaña Formulario.
1. (Opcional) Configure cualquier detalle del formulario, tal como se describe en [Configurar detalles del formulario](#set-up-form-details).

1. Seleccione si desea que una solicitud creada a partir de este formulario se marque como completada cuando se cree el objeto solicitado o cuando se complete el objeto solicitado.
1. (Condicional) Si ha seleccionado que la solicitud se marque como completada cuando se complete el objeto solicitado, seleccione el campo y el valor que indican cuándo se completa el objeto. Por ejemplo, puede seleccionar el campo Estado y el valor Completar para completar la solicitud cuando el estado del objeto creado se establece en Completar.
1. Continuar a <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[Completar la creación del formulario de solicitud](#complete-request-form-creation).

</div>

<!--
 
<div class="preview">

#### Set up Automations

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. 

For information on creating automations in other areas of Workfront Planning, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. Currently, the only available trigger for request form automation is `When request object status equals pending creation`.

1. Update the following fields in the **Actions** section: 

   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Currently, the only available Action for request form automation is `Create record`.

     >[!TIP]
     >
     >After you saved the automation, you can no longer change the action selected in this field.
1. Continue to  [Complete request form creation](#complete-request-form-creation).


</div>

-->

### Completar creación de formulario de solicitud

1. Cree y configure el formulario como se describe en [Comience a crear un formulario de solicitud](#begin-creating-a-request-form) y [configure los detalles del formulario de solicitud](#set-up-details-for-the-request-form).
1. (Opcional) Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del formulario en el encabezado y, a continuación, haga clic en **Editar** para actualizar el nombre del formulario.

1. Haga clic en **Publicar** para publicar el formulario y obtener un vínculo único para él.

   Ocurren lo siguiente:

   * Se ha quitado el botón **Publicar**.
   * Se agrega el botón **Cancelar publicación** al formulario. Si hace clic en él, se impedirá el acceso al formulario.
   * Se agrega un botón **Compartir** al formulario.
   * El formulario está disponible en el área de Solicitudes del menú principal de Workfront.

1. Haga clic en **Compartir** para compartir el formulario con otros usuarios.

   Para obtener información sobre cómo compartir un formulario de solicitud, consulte la sección [Compartir un formulario de solicitud](#share-a-request-form) en este artículo
1. Haga clic en la flecha que señala a la izquierda del nombre del formulario en el encabezado para cerrar el formulario.

   Se abre la vista de tabla **Formularios de solicitud** y se agrega el formulario.

## Administrar formularios de solicitud existentes


1. Haga clic en el espacio de trabajo donde desee administrar los formularios de solicitud.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro. Para obtener información acerca de cómo crear un tipo de registro, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   La página de tipo de registro se abre en la vista a la que se accedió por última vez. De forma predeterminada, se abre una página de tipo de registro en la vista de tabla.

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro en el encabezado de la página y, a continuación, haga clic en **Administrar formularios de solicitud**.

   Todos los formularios de solicitud asociados al tipo de registro se muestran en una vista de tabla.

1. (Opcional) Pase el ratón sobre el nombre de un formulario de solicitud en la vista de tabla, luego haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) a la derecha del nombre del formulario y haga clic en una de las siguientes opciones:

   * **Editar formulario**: haga clic aquí para editar más información en el formulario.
   * **Cancelar publicación**: haga clic aquí para cancelar la publicación del formulario que lo quita del área de solicitudes en Workfront.
   * **Compartir**: haga clic aquí para modificar quién tiene acceso al formulario.
   * **Copiar vínculo**: haga clic aquí para copiar rápidamente el vínculo del formulario de solicitud sin abrir el formulario.
   * **Eliminar**: haga clic aquí para eliminar el formulario. No se eliminan todas las solicitudes y registros agregados mediante el formulario. El formulario no se puede recuperar.

   ![Menú más en el formulario de solicitud de la lista de formularios de solicitud](assets/more-menu-on-request-form-from-request-forms-list.png)

1. Haga clic en la flecha que señala a la izquierda de **Formularios de solicitud** en el encabezado para cerrar la tabla de Formularios de solicitud.

   Se abre la página de tipo de registro.
1. (Opcional y condicional) Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro en el encabezado y, a continuación, siga uno de estos procedimientos:

   1. Haga clic en **Actualizar formulario de solicitud** para realizar cambios en el formulario de solicitud y, a continuación, haga clic en un formulario de solicitud para abrirlo y editarlo.
   1. Haga clic en **Copiar vínculo al formulario de solicitud** para compartir el vínculo al formulario con otros usuarios.

1. (Opcional) Vaya al área de **Solicitudes** en Workfront y busque el formulario compartido para enviar una solicitud. Para obtener más información, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Compartir un formulario de solicitud

1. Cree un formulario de solicitud como se describe en la sección [Crear un formulario de solicitud para un tipo de registro](#create-a-request-form-for-a-record-type) de este artículo.
1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del formulario de solicitud en la página del tipo de registro.
1. Haga clic en **Compartir** para compartir el formulario con otros usuarios.

1. Para compartir el formulario internamente, seleccione la pestaña **Uso compartido interno**, busque el nombre de un usuario, equipo, rol de trabajo, grupo o compañía en el campo **Conceder acceso para enviar este formulario** y, a continuación, selecciónelo cuando aparezca en la lista. El permiso **Enviar** está seleccionado de forma predeterminada para cada entidad.

   ![Compartir la casilla del formulario de solicitud](assets/share-box-for-request-form.png)

1. (Opcional) Haga clic en el menú desplegable situado después del nombre de una entidad y, a continuación, haga clic en **Quitar** para quitarlos de la lista y dejar de compartir el formulario con ellos.

   >[!NOTE]
   >
   >Además de los equipos, grupos, empresas y funciones del puesto, solo puede compartir con los usuarios que se han añadido a Adobe Admin Console. No puede agregar usuarios solo de Workfront. Para obtener más información, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

1. En la sección **Quién puede enviar solicitudes a través de este formulario**, seleccione entre las siguientes opciones para indicar qué tipos de usuarios pueden acceder a este formulario:

   * Solo pueden acceder las personas invitadas
   * Cualquiera con acceso de visualización o más alto al espacio de trabajo
   * Cualquiera con acceso de aportación o más alto al espacio de trabajo
1. (Opcional) Haga clic en **Copiar vínculo** para compartir el vínculo al formulario con las personas que tengan acceso para hacerlo. El vínculo se copia en el portapapeles.
1. Para compartir el formulario públicamente, selecciona la pestaña **Uso compartido público** y, a continuación, habilita la configuración **Crear vínculo público**.

   ![Uso compartido público del formulario de solicitud](assets/share-request-form-publicly-tab.png)

   >[!WARNING]
   >
   >* Al habilitar la configuración **Crear vínculo público**, cualquier persona podrá obtener acceso al formulario y enviar un nuevo registro, incluso las personas que no pertenezcan a su organización y que no tengan una cuenta de Workfront.
   >
   >* Un formulario que contenga los siguientes tipos de campo no se puede compartir públicamente:
   >
   >     * Conexiones de Workfront o AEM Assets
   >     * Personas
   >

1. Elija una **fecha de caducidad del vínculo**.

   Puede seleccionar fechas futuras en un plazo de 180 días a partir de la fecha actual.

   >[!TIP]
   >
   >Una vez que caduca la fecha de uso compartido, el formulario de solicitud ya no está disponible en el área de Solicitudes de Workfront y ya no se puede acceder a los vínculos compartidos con otros usuarios.

   Las personas recibirán un error una vez que caduque el vínculo y debe actualizar la fecha del vínculo y generar un nuevo vínculo para compartirlo antes de que las personas puedan acceder al formulario de nuevo.


1. (Opcional y condicional) Haga clic en **Guardar** para guardar los detalles de uso compartido del formulario.
1. (Condicional) Si el formulario se guardó anteriormente, haga clic en **Copiar vínculo**.

   Las opciones de uso compartido de formularios se guardan y el vínculo se copia en el portapapeles. Ahora puede compartirlo con otros usuarios.

   Para obtener información sobre cómo crear registros mediante un vínculo a un formulario de solicitud, consulte [Enviar solicitudes de Adobe Workfront Planning](/help/quicksilver/planning/requests/submit-requests.md).

1. Haga clic en **Guardar** en la esquina inferior derecha de la pestaña **Formulario** para guardar el formulario.
