---
title: Información general sobre campos de fórmula
description: En Adobe Workfront Planning, puede crear campos de fórmula que utilicen funciones y campos existentes para calcular un nuevo valor personalizado.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: b27b01e1efacc3fc459cec0a53b2c11cbe5e132b
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 50%

---

# Información general sobre campos de fórmula

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede crear campos personalizados en Adobe Workfront Planning haciendo referencia a los campos existentes y conectándolos en un campo de tipo fórmula.

Los campos de fórmula generan un nuevo valor utilizando los valores existentes de otros campos en un tipo de registro y una función que indica cómo se deben calcular los valores existentes.

Para obtener más información, consulte la sección “Fórmula” en el artículo [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

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
   <td><p> Estándar</p>
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
   <td>   <p>Administrar permisos a un espacio de trabajo y tipo de registro </a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
  </tr>

</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre los campos de fórmula

* Los campos de fórmula hacen referencia a campos que pertenecen al mismo tipo de registro.
* Sólo se puede hacer referencia a campos de otros tipos de registro cuando se conecta otro tipo de registro con el campo de fórmula para el que se está creando.
* La referencia a los tipos de registros conectados o a sus campos de búsqueda en una fórmula depende de los permisos que tenga para los tipos de registros conectados. Si no tiene permisos para ver el tipo de registro, no puede hacer referencia a sus campos en una fórmula.
* No puede cambiar el tipo de campo de un campo Fórmula después de guardarlo.
* Puede actualizar el cálculo de un campo de fórmula después de guardarlo, y los resultados del cálculo se actualizan automáticamente para todos los registros del mismo tipo.
* Debe añadir los campos a los que hace referencia en las fórmulas tal y como aparecen en la interfaz de Workfront Planning.
* Sólo puede hacer referencia a campos que se muestran en la vista de tabla de un tipo de registro o en la página de detalles del registro.
* Puede definir el formato para el valor de un cálculo de fórmula eligiendo entre las siguientes opciones de formato:

   * Texto
   * Número
   * Porcentaje
   * Divisa
   * Etiquetas
   * Fecha

  Para obtener más información, consulte la sección &quot;Fórmula&quot; en el artículo [Crear campos](/help/quicksilver/planning/fields/create-fields.md).
* Puede hacer referencia a los campos de fórmula en las fórmulas nuevas. Una vez que el valor se actualiza en un campo al que se hace referencia en un campo de fórmula, todos los campos subsiguientes que hagan referencia a ese campo o a los campos de fórmula que contengan ese campo se actualizarán automáticamente.

## Fórmulas compatibles

Los campos de fórmula de Adobe Workfront Planning admiten la mayoría de las expresiones de los campos calculados de Workfront.

>[!NOTE]
>
>Las siguientes expresiones de Workfront no son compatibles con los campos de fórmula de Workfront Planning:
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* AÑADIR HORA
>* SWITCH
>* FORMATO

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

Para obtener una lista completa de expresiones de Workfront, consulte [Información general sobre expresiones de datos calculados](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Además, se admiten las siguientes expresiones para los campos de fórmula de Workfront Planning. Las expresiones siguientes no son compatibles con las expresiones Workfront:

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

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
   <td> <p>Devuelve la cadena concatenada por el delimitador.</p> <p>La expresión tiene el siguiente formato:

<code>ARRAYJOIN(delimiter,array)</code>
</p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Devuelve una matriz con valores únicos.</p> <p>La expresión tiene el siguiente formato:

<code>ARRAYUNIQUE(array)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Devuelve el ID de un registro. Cada registro tiene un ID único.</p> <p>La expresión tiene el siguiente formato:

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>Devuelve los datos de JSON según la ruta JSONPath proporcionada. Si JSONPath no existe en el JSON, se devuelve un resultado vacío. </p> <p>La expresión tiene el siguiente formato:
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Establece la zona horaria de una fecha y la hora en una zona horaria especificada.</p> <p>La expresión tiene el siguiente formato:

<code>SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>Devuelve el número de la semana en un año. De forma opcional, puede indicar en qué día comienza la semana (utilice 1 para el domingo o 2 para el lunes). Si se omite, las semanas comienzan de forma predeterminada en domingo.</p> <p>La expresión tiene el siguiente formato:

<code>WEEKOFYEAR(date,2)</code>
o
<code>WEEKOFYEAR(date)</code>
</p>
   </td></tr>

</table>
