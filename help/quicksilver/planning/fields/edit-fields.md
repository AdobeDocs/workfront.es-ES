---
title: Editar configuración de campo
description: En Adobe Workfront Planning, puede editar la configuración de campo de los campos que ya se han creado. En este artículo se describe cómo editar la configuración de los campos de Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 73%

---


# Editar configuración de campo

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede editar la configuración de los campos existentes en Adobe Workfront Planning.

Para obtener información sobre la creación de campos de Adobe Workfront Planning, consulte [Creación de campos](/help/quicksilver/planning/fields/create-fields.md).

En este artículo se describe cómo editar la configuración de los campos de Workfront Planning. Para obtener información sobre cómo editar los valores de campo de los registros, consulte [Edición de registros](/help/quicksilver/planning/records/edit-records.md).

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
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
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
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Consideraciones sobre la edición de configuración de campo

Debe tener en cuenta lo siguiente antes de realizar cambios en la configuración de un campo:

* La configuración de campos solo se puede editar desde la tabla de tipo de registro.
* No puede editar ningún campo en la página de registro ni en ninguna otra vista, fuera de la vista de tabla.
* Una vez guardado el campo, no puede editar el tipo de campo.
* No puede anular la selección de la opción Permitir números negativos seleccionada anteriormente para un campo Número, Porcentaje o Moneda, si ya hay valores negativos almacenados en los registros a los que está asociada.
* Sí puede editar la configuración de los siguientes elementos de campo después de guardar el campo:

   * El nombre o la descripción de cualquier campo
   * Las opciones de un campo de selección única o de selección múltiple.
   * La expresión de un campo de fórmula.

  >[!WARNING]
  >
  >Cuando cambian las expresiones de fórmula, o se añaden o eliminan opciones de un campo de tipo de selección, se perderán datos de los registros que ya tienen información almacenada en los campos cuya configuración se modifica.
  >
  >No se muestra ninguna advertencia ni indicación de que esta pérdida de datos pueda producirse al cambiar la configuración de los campos.
  >
  >No se muestra ninguna notificación a otros usuarios de que la configuración del campo haya cambiado.

* Puede editar los campos de búsqueda existentes de los registros conectados.

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Editar configuración de campo

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos campos de registro desee editar.

   El espacio de trabajo se abre y todos los tipos de registros del espacio de trabajo se muestran en tarjetas.

1. Haga clic en la tarjeta de un tipo de registro.

   Se abre la página del tipo de registro.

1. (Condicional) Haga clic en la pestaña de una **vista de tabla**.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.
1. Pase el puntero por encima del encabezado de columna del campo que desee editar, a continuación haga clic en la flecha que apunta hacia abajo detrás del nombre del campo y por último haga clic en **Editar campo**

   O

   Haga doble clic en el encabezado de columna del campo.

   ![Menú de flecha después del nombre del campo en el encabezado de tabla resaltado](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Actualice la información sobre el campo y haga clic en **Guardar**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Una vez guardado el campo, no puede actualizar el tipo de campo.
   >
   >* Al modificar las configuraciones de campo (opciones de campo o expresiones de fórmula), los registros que ya contienen información en los campos modificados actualizarán sus valores en tiempo real. No se muestran advertencias ni registros de auditoría para los cambios de valor activados por los cambios en la configuración del campo. Todos los usuarios que vean los campos verán inmediatamente los nuevos valores con las modificaciones.

   La información de campo se actualiza para todos los que tengan acceso a la vista del espacio de trabajo.

1. (Condicional) Para los campos de registro conectados, haga clic en **Editar campos de búsqueda** y agregue o quite cualquiera de los campos de búsqueda del tipo de registro conectado.

   Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).