---
title: Crear registros importando información desde un archivo CSV o de Excel
description: Los registros son instancias individuales de tipos de registros, que son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear registros importando información desde un archivo CSV o de Excel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 940945df-391c-4672-9d9d-180d5028509b
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 6%

---


# Crear registros importando información desde un archivo CSV o de Excel

<!--

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Los registros son instancias individuales de tipos de registros, que son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear registros importando información desde un archivo CSV o de Excel.

Para obtener más información sobre cómo crear registros, vea [Crear registros](/help/quicksilver/planning/records/create-records.md).

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
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront y cualquier paquete de Planning</p> <p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Permisos de contribución o superiores al espacio de trabajo y tipo de registro donde se importan registros. </p>
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
   </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, programs, and portfolios) as you connect them from new records  </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> -->


## Consideraciones acerca de la importación de registros mediante un archivo CSV o de Excel

* Los encabezados de las columnas de cada hoja se convierten en los campos asociados a los registros.
* Cada fila de cada hoja se convierte en un registro único asociado.
* Si el archivo de Excel contiene más de una hoja, sólo se importará la información de una hoja seleccionada durante el proceso de importación.
* El archivo no debe superar lo siguiente:
   * 25 000 filas
   * 500 columnas
* El archivo no debe superar los 5 MB.
* No se admiten hojas vacías.
* No se admiten los campos de los siguientes tipos y no se pueden asignar a campos de la hoja de importación:

   * Campos de conexión a Workfront y tipos de objeto de AEM Assets. Sólo se pueden asignar campos de conexión a tipos de registro de Planning.
   * Campos de búsqueda de registros de Planning conectados u objetos de Workfront y AEM Assets
   * Campos de fórmula
   * Fecha de creación, Creado por
   * Fecha de la última modificación, Última modificación por
   * Fecha de aprobación, Aprobado por
   * Personas
   * Si se importa un campo de selección múltiple o única y tiene más opciones que un campo similar en Planning, las opciones adicionales se crean durante la importación. Solo los usuarios con permisos de Administrar en el espacio de trabajo pueden importar nuevas opciones.

## Creación de registros importando un archivo CSV o de Excel

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee crear registros,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo situada a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y, a continuación, selecciónelo cuando se muestre en la lista.
1. Haga clic en la tarjeta del tipo de registro donde desee importar los registros.
1. Haga clic en **Nuevo registro** en la esquina superior derecha de la pantalla.

   ![Elija la forma de agregar registros en el cuadro de tres botones](assets/choose-way-to-add-records-three-button-box.png)
1. Haga clic en **Cargar desde el archivo** y, a continuación, **Continuar**. <!--add screen shot when all three buttons are added - with the Submit a request button-->
1. Arrastre y suelte un archivo de Excel o CSV guardado anteriormente en el equipo, o haga clic en **Seleccione un archivo CSV o de Excel** para buscar uno.
1. Haz clic en **Vista previa y edita**.
1. (Condicional) Si el archivo importado tiene más de una hoja, seleccione el botón de opción de la hoja que desea importar en el cuadro **Seleccione una hoja para importar** y, a continuación, haga clic en **Siguiente**. De lo contrario, continúe con el siguiente paso.

   ![Seleccione una hoja para importar registros](assets/select-a-sheet-to-import-box.png)
1. En **Asignar los campos de Planning a los encabezados de columna**, seleccione el **campo de Planning** que mejor coincida con la información de cada una de las columnas de la hoja.

   ![Asignar campos de Planning a columnas al importar registros](assets/map-planning-fields-to-columns-when-importing-records.png)

   Cada fila representa un nuevo registro. Solo se muestran los 10 primeros registros en el cuadro Vista previa y edición.

   >[!TIP]
   >
   >No se admiten todos los tipos de campo. Para obtener más información, vea la sección [Consideraciones acerca de la importación de registros mediante un archivo CSV o de Excel](#considerations-about-importing-records-using-an-excel-or-csv-file) en este artículo.


1. (Opcional y condicional) Si tiene permisos de administración en el área de trabajo, seleccione **Crear opciones que faltan** en la esquina inferior izquierda de la pantalla. Cuando se habilita, se agregan las opciones que faltan en los campos de selección única y múltiple.

   >[!NOTE]
   >
   >Por ejemplo, si el tipo de registro seleccionado tiene un campo de estado de selección única con las opciones Nuevo, En curso y Cerrado, y un campo de estado importado de un archivo también tiene una opción de estado Retenido, también se agrega la opción de estado Retenido.
   >
   >Si no tiene permisos de administración en el espacio de trabajo, puede importar registros, pero no se crearán las opciones adicionales. En su lugar, recibe el siguiente mensaje en la esquina superior derecha del cuadro Asignar los campos de Planning a los encabezados de columna: **Las opciones que no existen en los campos de conexión, de selección única o múltiple, no se agregarán**.

1. Haga clic en **Importar**.

   La siguiente información se importa en Workfront Planning:

   * Nuevos registros que se muestran en la parte inferior de la vista de tabla del tipo de registro seleccionado.
   * Valores de campo nuevos para campos existentes asociados a cada registro.
   * Nuevas opciones de un campo de selección múltiple o única que no existía en Planning.  <!--when we add connected records - add those here too-->

   Puede empezar a administrar campos y registros en la página de tipos de registros.

   Todas las personas con acceso a Workfront Planning y al espacio de trabajo ahora pueden ver y editar los registros importados y su información.

   <!--when we add connected records and the info icon in the tool changes, also add those items to the Import step and to the NOTE above it-->
