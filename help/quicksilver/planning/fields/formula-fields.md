---
title: Información general sobre campos de fórmula
description: En Adobe Workfront Planning, puede crear campos de fórmula que utilicen funciones y campos existentes para calcular un nuevo valor personalizado.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 8%

---

# Información general sobre campos de fórmula

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--this article is linked to the UI in the formula box, "Learn more..."-->

<!---
title: Formula fields overview
description: In Adobe Workfront Planning, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{planning-important-intro}}

Puede crear campos personalizados en Adobe Workfront Planning haciendo referencia a campos existentes y conectándolos en un campo de tipo fórmula.

Los campos de fórmula generan un nuevo valor utilizando valores existentes de otros campos en un tipo de registro y una función que indica cómo se deben calcular los valores existentes.

Para obtener más información, consulte la sección &quot;Fórmula&quot; en el artículo [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en la fase de acceso anticipado para Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Nuevo: estándar</p>
   <p>Actual: plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de acceso para la planificación de Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administrar permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## Consideraciones sobre los campos de fórmula

* Los campos de fórmula hacen referencia a campos que pertenecen al mismo tipo de registro.
* Sólo se puede hacer referencia a campos de otros tipos de registro cuando se conecta otro tipo de registro con el campo de fórmula para el que se está creando.
* No se puede cambiar el tipo de campo de un campo Formula después de guardarlo.
* Puede actualizar el cálculo de un campo de fórmula después de guardarlo, y los resultados del cálculo se actualizan automáticamente para todos los registros del mismo tipo.
* Debe agregar los campos a los que hace referencia en las fórmulas tal y como aparecen en la interfaz de Workfront Planning.
* Sólo puede hacer referencia a campos que se muestran en la vista de tabla de un tipo de registro o en la página de detalles del registro.
<!--* You can format the result of a formula calculation by choosing from the following options:

   * Text
   * Number
   * Percent
   * Currency
   * Tags
   * Date

   For more information, see the "Formula" section in the article [Create fields](/help/quicksilver/planning/fields/create-fields.md). -->


## Fórmulas compatibles

Los campos de fórmula de Adobe Workfront Planning admiten todas las expresiones de los campos calculados de Workfront. Para obtener más información, vea [Información general sobre expresiones de datos calculados](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Además, se admiten las siguientes expresiones para los campos de fórmula de Workfront Planning:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expresión</th> 
   <th>Explicación y ejemplo</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Devuelve una cadena concatenada por delimitador.</p> <p>La expresión tiene el siguiente formato:

<code>ARRAYJOIN(delimitador,matriz)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Devuelve una matriz con valores únicos.</p> <p>La expresión tiene el siguiente formato:

<code>ARRAYUNIQUE(matriz)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Devuelve el ID de un registro. Cada registro tiene un ID único.</p> <p>La expresión tiene el siguiente formato:

<code>{ID}</code>
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Establece la zona horaria de una fecha y hora en una zona horaria específica.</p> <p>La expresión tiene el siguiente formato:

<code>SETTIMEZONE(fecha,&#39;América/Los_Ángeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>Devuelve el número de la semana en un año. De forma opcional, puede indicar en qué día comienza la semana (utilice 1 para el domingo o 2 para el lunes). Si se omite, las semanas comienzan de forma predeterminada en domingo.</p> <p>La expresión tiene el siguiente formato:

<code>WEEKOFYEAR(fecha,2)</code>
o
<code>WEEKOFYEAR(fecha)</code>
</p>
   </td></tr>

</table>
