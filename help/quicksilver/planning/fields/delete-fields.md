---
title: Eliminar campos
description: En Adobe Workfront Planning, puede eliminar campos personalizados que ya no sean relevantes.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 52%

---



# Eliminación de campos

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

En Adobe Workfront Planning, puede crear campos personalizados para almacenar información sobre registros.

Para obtener información acerca de cómo crear campos personalizados en Workfront Planning, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

Puede eliminar los campos de Workfront Planning que ya no sean relevantes.

## Consideraciones sobre la eliminación de campos de Workfront Planning:

* Solo puede eliminar un campo en la vista de tabla de tipo de registro.
* No se puede eliminar el campo principal de un registro.
* La información almacenada en el campo se elimina y no se puede recuperar.
* Al eliminar un campo de registro conectado, todos los campos de búsqueda conectados también se eliminan del tipo de registro desde el que se conecta. Los campos de registro conectados de los tipos de registro a los que se conecta también se eliminan del registro al que se conecta.

  Por ejemplo, cuando conecta campañas a otro tipo de registro llamado producto y elimina el campo Producto conectado y el campo de búsqueda Estado del producto de la campaña, se eliminan los siguientes elementos:

   * El campo Product connected de la campaña
   * El campo de búsqueda Estado del producto de la campaña
   * El campo conectado a Campaign desde el producto.

  Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

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
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
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
   <td><p> Estándar </p>
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
   <td>   <p>Administrar permisos para un área de trabajo <span class="preview">y tipo de registro</span> </a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>En el entorno de producción, todos los usuarios, incluidos los administradores del sistema, deben estar asignados a una plantilla de diseño que incluya Planning.</p>
<p><span class="preview">En el entorno de vista previa, los usuarios estándar y los administradores del sistema tienen Planning habilitado de forma predeterminada.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminación de campos

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos campos de registro desee eliminar.

   Se abre el espacio de trabajo y se muestran los tipos de registro.

1. Haga clic en la tarjeta de un tipo de registro.

1. (Condicional) Si aún no está seleccionado, haga clic en la pestaña de una **Vista de tabla** en la página de tipo de registro.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.

1. Busque el campo que desea eliminar en los encabezados de columna, pase el puntero por encima del encabezado de columna y, a continuación, haga clic en la flecha hacia abajo situada después del nombre del campo.

   ![Menú de flecha después del nombre del campo en el encabezado de tabla resaltado](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Haga clic en **Eliminar**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Haga clic en **Eliminar** para confirmar.

   El campo se elimina, no se puede recuperar y ya no se puede asociar a ningún registro.
