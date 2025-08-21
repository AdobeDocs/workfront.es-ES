---
title: Creación y administración de un formulario de solicitud en Adobe Workfront Planning
description: Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede crear un formulario de solicitud y asociarlo a ese tipo de registro. A continuación, puede compartir un vínculo con otros usuarios internos o externos. Los usuarios con un vínculo al formulario pueden rellenar los valores de campo que contiene y, al enviarlo, pueden agregar un nuevo registro para el tipo de registro asociado a él.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 359131cef04fdb46def64428a7a693c3f00b2cd4
workflow-type: tm+mt
source-wordcount: '2568'
ht-degree: 7%

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

+++ Amplíe para ver los requisitos de acceso. 

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
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p>
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
   <li><p>Administración de permisos de un espacio de trabajo y tipo de registro</p></li>
    <li><p>Los administradores del sistema pueden administrar los espacios de trabajo que no hayan creado. </p></li>
    </ul>
   <p>Para obtener información acerca de los permisos de uso compartido para objetos de Workfront Planning, consulte 
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Información general sobre los permisos de uso compartido en Adobe Workfront Planning</a> 
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

      * Creado por, modificado por última vez por, <span class="preview">Aprobado por</span>
      * Fecha de creación, Fecha de la última modificación, <span class="preview">Fecha de aprobación</span>
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

## Empezar a crear un formulario de solicitud

Puede crear un formulario de solicitud a partir del tipo de registro asociado al formulario <span class="preview"> o del área de solicitudes de Workfront.</span>

### Creación de un formulario de solicitud a partir de un tipo de registro

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
1. Continúe a [Configurar el formulario](#configure-the-form).

<div class="preview">

### Cree un formulario de solicitud desde el área Solicitudes de Workfront

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Solicitudes**.
1. En la esquina superior derecha de la pantalla, haga clic en **Solicitar formularios**.
1. (Condicional) Si está editando un formulario de solicitud existente, selecciónelo en la lista y, a continuación, [configure el formulario](#confgure-the-form).
1. Si está creando un nuevo formulario de solicitud, en la esquina superior derecha de la pantalla, haga clic en **Nuevo formulario de solicitud**.

   Se abrirá el cuadro de diálogo Crear formulario de solicitud

1. En el cuadro Crear formulario de solicitud, actualice el nombre del formulario de solicitud. De manera predeterminada, el nombre del formulario es **Formulario sin título**.
1. En el campo Object types, seleccione el tipo de registro al que se asociará el formulario de solicitud. Los tipos de registro se agrupan en el espacio de trabajo en el que existen.
1. (Opcional) Agregue una **Descripción** para el formulario de solicitud.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Haga clic en **Crear**.

   El formulario de solicitud del tipo de registro seleccionado se abre en la pestaña Formulario.
1. Continúe a [Configurar el formulario](#configure-the-form).

</div>

## Configuración del formulario

1. Comience a crear o editar un formulario de solicitud, tal como se describe en una de las siguientes secciones:

   * [Creación de un formulario de solicitud a partir de un tipo de registro](#create-a-request-form-from-a-record-type)
   * <span class="preview">[Crear un formulario de solicitud desde el área de solicitudes de Workfront](#create-a-request-form-from-the-requests-area-of-workfront)</span>

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

1. (Opcional) Haga clic en la ficha **Configuración** y, a continuación, agregue al menos un usuario <span class="preview">o equipo</span>al campo **Aprobadores** para aprobar nuevas solicitudes para este formulario de registro.

   ![Ficha de configuración](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Al asociar un formulario de solicitud con los aprobadores, cualquier nueva solicitud debe ser aprobada primero por todos los aprobadores antes de que genere un nuevo registro.
   * Puede agregar uno o varios aprobadores a un formulario de solicitud.
   * Si al menos un aprobador rechaza la solicitud, esta se rechaza y no se crea el registro.
   * Todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.
   * <span class="preview">Si un equipo se establece como aprobador, solo se requiere una decisión del equipo.</span>

     Para obtener más información sobre cómo agregar aprobaciones a los formularios de solicitud, consulte [Agregar aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

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
