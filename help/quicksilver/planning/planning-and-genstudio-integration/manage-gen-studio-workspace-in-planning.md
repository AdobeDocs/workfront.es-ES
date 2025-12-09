---
title: Administrar GenStudio Workspace en Adobe Workfront Planning
description: El espacio de trabajo de GenStudio for Performance Marketing está disponible en Adobe Workfront Planning cuando su empresa ha adquirido ambos productos y su instancia de Workfront está integrada con la instancia de GenStudio de su empresa. Puede ver el espacio de trabajo de GenStudio desde Planning y actualizar la información en ambos sistemas.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 4%

---


<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

<!--MUST update the access requirements below - not complete!!!!!!!!!-->

# Administrar el espacio de trabajo de GenStudio en Adobe Workfront Planning

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

El espacio de trabajo de Adobe GenStudio for Performance Marketing está disponible en Adobe Workfront Planning cuando su empresa ha adquirido ambos productos y su instancia de Workfront está integrada con la instancia de GenStudio de su empresa.

Puede ver el espacio de trabajo de GenStudio desde Planning y actualizar la información en ambos sistemas.

Para obtener información sobre cómo usar y administrar el espacio de trabajo de GenStudio desde GenStudio Performance Marketing, consulte [Guía del usuario de Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/home).

Para obtener información general acerca de la integración de GenStudio con Workfront Planning, consulte [Introducción a la integración de Adobe Workfront Planning y Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

>[!IMPORTANT]
>
>Los pasos descritos en este artículo ilustran cómo se puede actualizar el espacio de trabajo de GenStudio desde Workfront Planning cuando se tiene permisos de administración.
> No todas las funciones están disponibles si tiene permisos de contribución en el espacio de trabajo de GenStudio.
>
>Si su empresa tiene varias instancias de Workfront, todos los usuarios obtienen permisos de contribución en el espacio de trabajo de GenStudio en Workfront Planning.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront y cualquier paquete de Planning</p>
<p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
   <tr> 
<td> 
   <p> Productos adicionales</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Funciones de usuario de Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Cualquier función de usuario de GenStudio para acceder a campañas, productos y personas</li>
   <li>GenStudio System Manager para acceder a las activaciones <!--and Events--></li></ul>
   Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funciones de usuario y permisos</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  
   <p>En Workfront Planning: </p>
   <ul>
   <li><p>Administre permisos en GenStudio Workspace para agregar nuevos campos o tipos de registros a GenStudio Workspace</p></li>
   <li><p>Permisos de contribución para agregar, actualizar o eliminar registros en el espacio de trabajo de GenStudio GenStudio</p> </li>  
   </ul>
   <p>Ningún usuario puede quitar tipos de registros o campos de GenStudio for Performance Marketing del espacio de trabajo de GenStudio en Workfront Planning</p>
   <p>En Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Cualquier permiso de Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Crear permisos en Adobe GenStudio for Performance Marketing para crear elementos</p></li></ul>
   </td>  
</tbody> 
</table>

Para obtener información sobre el acceso a Adobe Workfront Planning, consulte [Información general sobre el acceso a Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Para obtener más información sobre Adobe GenStudio for Performance Marketing, consulte [Guía del usuario de Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/home).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations ****** and Events*********</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to add new fields or record types to the GenStudio workspace</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   </ul>
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Consideraciones para administrar un espacio de trabajo de GenStudio en Workfront Planning

* Su organización debe adquirir Adobe GenStudio for Performance Marketing para poder ver un espacio de trabajo de GenStudio en Workfront Planning.

* Según la cantidad de instancias de Workfront que tenga su organización, tendrá automáticamente los siguientes permisos para el espacio de trabajo de GenStudio en Planning:

  <!--this table is also in the Get started article-->

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
      <tr> 
      <td role="rowheader"><p>Una instancia de Workfront</p></td> 
      <td> 
   <p>El espacio de trabajo de GenStudio está visible en su instancia de Workfront Planning</p>
   <p>Los administradores de Workfront tienen permisos de administración en GenStudio Workspace, en Planning</p>
   <p>Todos los demás usuarios tienen acceso de contribución al espacio de trabajo de GenStudio en Planning</p>
   </td> </tr>
      <tr> 
   <td> 
      <p> Varias instancias de Workfront</p> </td> 
      <td> 
      <p>El espacio de trabajo de GenStudio es visible desde todas las instancias de Workfront</p>
   <p>Todos los usuarios con acceso a GenStudio for Performance Marketing y Workfront Planning tienen permisos de contribución en GenStudio en Planning</p> </td> 
   </tr>
      </tbody> 
   </table>

* La actualización de la configuración del espacio de trabajo, los tipos de registro, las vistas y los campos de un espacio de trabajo de GenStudio es idéntica a la actualización de un espacio de trabajo de Workfront Planning con sus elementos.

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Administrar el espacio de trabajo de GenStudio desde Workfront Planning

>[!NOTE]
>
>Antes de administrar el área de trabajo de GenStudio, consulte el artículo [Introducción a la integración de Workfront Planning y GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) para obtener más información.
>

1. Inicie sesión en Workfront como usuario que también tiene acceso a GenStudio.
1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Planificación]**.

   Se abrirá la página principal de Workfront Planning.

1. Haga clic en **Otros espacios de trabajo** y busque un espacio de trabajo que tenga una indicación creada por el **Sistema** y que tenga la etiqueta **GenStudio** en su tarjeta.

   ![tarjeta de espacio de trabajo de GenStudio con etiqueta](assets/genstudio-card-with-tag-highlighted.png)

1. Haga clic en la tarjeta de **GenStudio Workspace** para abrir GenStudio Workspace en Workfront Planning.
1. De forma predeterminada, los siguientes tipos de registros de GenStudio se crean y son visibles desde Workfront Planning:

   * Campañas
   * Productos
   * Personas
   * Activaciones
   * Canales
   * Regiones

   Hay una indicación en la tarjeta de tipo de registro de GenStudio de que se crearon originalmente en GenStudio.

   <!--check screen shot-->

   ![Tarjeta de tipo de registro GenStudio con etiqueta](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del área de trabajo y, a continuación, haga clic en una de las opciones siguientes:

   * **Editar**

     Para obtener más información, consulte [Edición de espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).
     <!--* **Delete** - this will generate an error message, per Iskuhi, so don't document as an option/ possibility-->

     <!--For information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). -->

1. Haga clic en **Compartir** en la esquina superior derecha para compartir el área de trabajo con otros usuarios.

   Para obtener más información, vea [Compartir espacios de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

   <!--
   >[!NOTE]
   >
   >You cannot remove GenStudio users from the GenStudio workspace, after you share that workspace with them.-->

1. Haga clic en cualquiera de las tarjetas de tipo de registro para ver los registros de ese tipo.

   Para administrar el tipo de registro, las vistas y los campos, consulte la sección [Administrar tipos de registros de GenStudio desde Workfront Planning](#manage-genstudio-record-types-from-workfront-planning) en este artículo.


## Administre tipos de registros, vistas y registros desde GenStudio Workspace en Workfront Planning

>[!NOTE]
>
>Antes de administrar el área de trabajo de GenStudio, consulte el artículo [Introducción a la integración de Workfront Planning y GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) para obtener más información.
>

1. Vaya al espacio de trabajo de GenStudio en Workfront Planning y abra una página de tipo de registro, tal como se describe en la sección [Administrar el espacio de trabajo de GenStudio desde Workfront Planning](#manage-the-genstudio-workspace-from-workfront-planning) en este artículo.

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre de un tipo de registro y, a continuación, haga clic en una de las opciones siguientes:

   * **Editar**

     Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).
   * **Administrar automatizaciones**

     Para obtener más información, consulte [Configuración de automatizaciones de Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).
   * **Administrar formularios de solicitud**

     Puede crear varios formularios de solicitud. Los formularios de solicitud estarán disponibles en el área de Solicitudes de Workfront y también puede compartirlos públicamente o con un vínculo.

     Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

1. Para compartir una vista o el tipo de registro, haga lo siguiente:

   * Haga clic en **Compartir** en la esquina superior derecha de la página de tipo de registro y, a continuación, haga clic en una de las siguientes opciones:
      * **Compartir el tipo de registro**
Para obtener más información, consulte [Compartir tipos de registros](/help/quicksilver/planning/access/share-record-types.md).
      * **Compartir la vista actual**
Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).
      * **Copiar el vínculo de vista**
Se copia un vínculo a la vista en el portapapeles.
      * **Exportar la vista actual**
Para obtener más información, vea [Exportar registros desde la vista de tabla](/help/quicksilver/planning/records/export-records-from-the-table-view.md).

        <!--
         >[!NOTE]
         >
         >You cannot remove GenStudio users from record types in the GenStudio workspace, after you share that workspace or the record types with them.-->

1. Para administrar las vistas de tipo de registro, haga lo siguiente:

   * Haga clic en **+ Vista** para crear una vista para el tipo de registro de GenStudio.

     Para obtener más información, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

   * Haga clic en el icono **Pantalla completa** ![Abrir vista completa en el icono de pantalla completa](assets/open-full-screen-icon.png) para abrir cualquier vista en modo de pantalla completa.

   * Administre los elementos de una vista desde cualquier vista.

     Por ejemplo, puede cambiar el filtro, las agrupaciones, el orden y la configuración de una vista, si está disponible.

     Para obtener más información, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

1. Para agregar registros, siga uno de estos procedimientos:

   * Haga clic en **Nuevo registro** desde cualquier vista para crear registros desde cero

   * Importación de registros mediante un archivo CSV o de Excel en la vista de tabla

   * Haga clic en cualquier lugar de la vista de calendario o de la cronología para agregar registros.

     Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).

     Los registros son visibles tanto desde Workfront como desde GenStudio.

     >[!NOTE]
     >
     >No puede agregar registros para el tipo de registro Activaciones.

1. Para editar registros, siga uno de estos procedimientos:

   * Editar registros en línea desde la vista de tabla

   * Haga clic en un registro desde cualquier vista para abrir su página de detalles.

     Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

     Los cambios que realice desde el espacio de trabajo de GenStudio en Planning son visibles inmediatamente desde GenStudio.

1. Seleccione un registro en la vista de tabla y luego haga clic en **Eliminar**.

   Para obtener más información, consulte [Eliminar registros](/help/quicksilver/planning/records/delete-records.md).

   Los registros eliminados se eliminan inmediatamente de GenStudio.

   >[!TIP]
   >
   >Los registros eliminados se pueden recuperar de la vista de tabla Archivos eliminados recientemente en Workfront Planning. Los registros eliminados de GenStudio también se pueden recuperar del grupo Eliminados recientemente en Workfront Planning.

   Para obtener más información, consulte [Restaurar registros eliminados](/help/quicksilver/planning/records/restore-deleted-records.md)

1. Haga clic en el icono + en la esquina superior derecha de la vista de tabla para crear lo siguiente:

   * Campos de registro

     Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md)

   * Registrar conexiones

     Para obtener más información, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md)

     Los campos creados desde GenStudio Workspace están visibles en las siguientes áreas:

      * Vistas de Workfront Planning
      * Detalles del registro de Workfront Planning
      * Detalles de registro de GenStudio

     >[!TIP]
     >
     >Los campos creados en Workfront Planning no son visibles en la vista de lista de GenStudio.

     <!--when this releases, replace the tip above with this: 
      
      >[!NOTE]
      >
      >* Fields created in Workfront Planning are not visible in the list view in GenStudio.
      >
      >* You can connect any GenStudio record type to the Brands GenStudio record type. 
      >  Products and Personas are connected to Brands by default. -->

1. Pase el ratón sobre un campo de la vista de tabla y, a continuación, haga clic en el menú desplegable para realizar una de las siguientes acciones:

   * Ordenar por él
   * Ocultar esto
   * Editar su configuración
     <!--* Delete it - not possible now, per Iskuhi; the link is there but it will generate an error-->

     <!--GenStudio-native fields are note removed from GenStudio. -->

     >[!NOTE]
     >
     >Puede editar la configuración de un campo y agregar más campos solo cuando tenga permisos de administración en GenStudio.

