---
title: Crear tipos de registro importando información desde un archivo CSV o de Excel
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustren los elementos de trabajo necesarios en el ciclo vital de su organización mediante la importación de información desde un archivo CSV o de Excel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 9%

---

# Crear tipos de registros importando información desde un archivo CSV o de Excel

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustren los elementos de trabajo necesarios en el ciclo vital de su organización mediante la importación de información desde un archivo CSV o de Excel.

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
<p>Cualquier Workfront y cualquier paquete de Planning</p>
<p>O</p>
<p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
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
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
 
</tbody> 
</table>-->


## Consideraciones acerca de la importación de tipos de registros mediante un archivo CSV o de Excel

* Cada hoja del archivo de Excel se convierte en un tipo de registro. El nombre de la hoja se convierte en el nombre del tipo de registro.
* Si sólo hay una hoja o si importa un archivo CSV, el nombre del archivo se convierte en el nombre del tipo de registro.
* Los encabezados de las columnas de cada hoja se convierten en los campos asociados a cada tipo de registro.
* Los campos son únicos para sus respectivos tipos de registros.
* Cada fila de cada hoja se convierte en un registro único asociado a su tipo de registro respectivo.
* Cada hoja del archivo de Excel no debe superar lo siguiente:
   * 25 000 filas
   * 500 columnas
* El archivo no debe superar los 5 MB.
* No se admiten hojas vacías.
* No se admiten los campos de los siguientes tipos y no se pueden asignar a campos de la hoja de importación:

   * Campos de conexión a Workfront, tipos de objetos de AEM Assets o GenStudio Brands.
   * Campos de búsqueda de registros de Planning conectados, Workfront, objetos de AEM Assets o marcas de GenStudio.
   * Campos de fórmula
   * Fecha de creación, Creado por
   * Fecha de la última modificación, Última modificación por
   * Fecha de aprobación, Aprobado por
   * Personas

Para importar tipos de registros mediante un archivo CSV o de Excel:

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee crear los tipos de registro,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo situada a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y, a continuación, selecciónelo cuando se muestre en la lista.
1. Haga clic en **Agregar tipo de registro**.
1. Haga clic en **Cargar desde el archivo**.
1. Arrastre y suelte un archivo de Excel o CSV guardado anteriormente en el equipo, o haga clic en **Seleccione un archivo CSV o de Excel** para buscar uno y, a continuación, selecciónelo.
1. Haz clic en **Vista previa y edita**.

   Se muestra el cuadro **Previsualizar y editar** con la siguiente información:

   * Los nombres de las hojas o de los futuros tipos de registros se muestran en el panel izquierdo. De forma predeterminada, Workfront Planning selecciona un icono y un color para cada nuevo tipo de registro.
   * Se selecciona el primer tipo de hoja o registro y los nombres de los campos asociados a él se muestran como encabezados de columna. El tipo de cada campo está seleccionado de forma predeterminada.
   * Cada fila representa un nuevo registro. Solo se muestran los 10 primeros registros en el cuadro Vista previa y edición.

   ![Cuadro de vista previa y edición](assets/preview-and-edit-box.png)

1. (Opcional) Haga clic en el nombre de cada hoja en el panel izquierdo para revisar la información que contiene.

   >[!NOTE]
   >
   >Las hojas vacías no son compatibles y aparecen atenuadas.

1. (Opcional) Anule la selección de las hojas que no quiera importar del panel izquierdo.

   ![Seleccione las hojas que desea importar en la lista desplegable sin seleccionar](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Las hojas que no haya seleccionado se muestran con un fondo gris.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del encabezado de una columna para realizar una de las siguientes acciones, en la ficha **Campo**:

   ![Ficha Campo en el cuadro de importación de asignación de tipo de registro](assets/field-tab-on-record-type-import-mapping-box.png)

   * Cambie el nombre de uno de los campos
   * Cambiar **tipo de campo**
   * Actualizar el campo **Descripción**

1. (Opcional) Haga clic en la ficha **Conexión** para asignar la información de la columna a un campo conectado desde otros tipos de registros.

   ![Ficha Conexión en el cuadro de asignación de importación de tipo de registro](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >Solo puede asignar a campos desde registros conectados de Workfront Planning. No se puede asignar a campos desde conexiones de Workfront, AEM Assets o GenStudio Brands. Para obtener más información, vea la sección [Consideraciones acerca de la importación de tipos de registros mediante un archivo CSV o de Excel](#considerations-about-importing-record-types-using-an-excel-or-csv-file) en este artículo.

1. (Condicional) Después de actualizar la información del campo, haga clic en **Guardar**.

1. Haga clic en **Importar** cuando esté listo para importar el archivo.

   La siguiente información se importa en Workfront Planning:

   * Nuevos tipos de registros
   * Nuevos campos asociados a cada tipo de registro
   * Nuevos registros asociados a cada tipo de registro

   Puede empezar a administrar campos y registros en las páginas de tipos de registros.

   Todas las personas con acceso a Workfront Planning y al espacio de trabajo ahora pueden ver y editar los tipos de registro importados y su información.
