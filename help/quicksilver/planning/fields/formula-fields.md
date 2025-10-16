---
title: Información general sobre campos de fórmula
description: En Adobe Workfront Planning, puede crear campos de fórmula que utilicen funciones y campos existentes para calcular un nuevo valor personalizado.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 33%

---

# Información general sobre campos de fórmula

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede crear campos personalizados en Adobe Workfront Planning haciendo referencia a los campos existentes y conectándolos en un campo de tipo fórmula.

Los campos de fórmula generan un nuevo valor utilizando los valores existentes de otros campos en un tipo de registro y una función que indica cómo se deben calcular los valores existentes.

Para obtener más información, consulte la sección “Fórmula” en el artículo [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

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
<ul> 
<li><p>Cualquier Workfront y cualquier paquete de Planning</p></li>
O
<li><p>Cualquier flujo de trabajo y cualquier paquete de Planning</p></li></ul>
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
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
 
</tbody> 
</table> -->

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

<div class="preview">

* Al actualizar un campo de fórmula o un campo que pueda afectarlo, una alerta le notifica el impacto del cambio. La alerta se muestra en los siguientes casos:

   * Cuando se actualiza un campo de fórmula (sin incluir los cambios de nombre y descripción) cuando ese campo tiene campos de fórmula o búsqueda dependientes. La alerta muestra esos campos dependientes y le pregunta si desea continuar.

   * Cuando se elimina un campo que se utiliza en una expresión de fórmula o como campo de búsqueda. La alerta muestra los campos de fórmula y búsqueda dependientes y le pregunta si desea continuar con la eliminación.

</div>



<div class="preview">

## Limitaciones de los campos de fórmula

* Puede agregar un máximo de 20 campos de fórmula para un tipo de registro.

  Los campos de búsqueda de fórmulas agregados desde tipos de registros conectados no cuentan con este límite.

* La expresión de fórmula no puede superar los 50 000 caracteres.

* Los campos de fórmula podrían mostrarse como `#ERROR!` en los siguientes casos:
   * Cuando se elimina un campo utilizado en una fórmula.
   * Cuando un campo utilizado en un campo de búsqueda agregado se muestra como `#ERROR!`.

     Por ejemplo, si muestra un campo de búsqueda que contiene campos de fórmula de búsqueda agregados y uno de los campos de fórmula a los que se hace referencia se muestra como `#ERROR!`.
   * Cuando un valor de fórmula no se puede mostrar en el formato seleccionado.

     Por ejemplo, si selecciono Número para el formato de un campo de fórmula y los campos utilizados en la fórmula son campos de texto que sólo muestran valores de texto no numéricos, el resultado de la fórmula se mostrará como `#ERROR!`, ya que no puede analizar el texto en un número.

</div>

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
