---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vista: muestra objetos que no están incluidos en la interfaz estándar"
description: Puede mostrar en una vista objetos que no están incluidos en la interfaz de modo estándar. Solo puede hacerlo haciendo referencia a ellos mediante el modo de texto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Ver: muestra los objetos que no están incluidos en la interfaz estándar

Puede mostrar en una vista objetos que no están incluidos en la interfaz de modo estándar. Solo puede hacerlo haciendo referencia a ellos mediante el modo de texto.\
Puede determinar qué campos se pueden incluir en una vista de cualquiera de las siguientes maneras:

* Use el [Explorador de API](../../../wf-api/general/api-explorer.md) para descubrir otros objetos a los que se puede hacer referencia mediante el modo de texto.\
  No todos los campos documentados en el Explorador de API son campos válidos para el modo de texto. Algunos campos solo se pueden registrar a través de la API.

* Busque el campo ID del objeto en una columna. La mayoría de los objetos que tienen un ID de campo también tienen una columna o un nombre de campo correspondiente al que puede que no se pueda acceder mediante la interfaz de modo estándar.

  Puede utilizar el modo de texto para incluir en una vista el nombre de columna o campo en lugar del ID reemplazando `fieldnameID` por `fieldname:name`.

  Por ejemplo, en la interfaz de modo estándar, el campo **Identificador de propietario del Portfolio** está disponible para una vista de proyecto, pero el campo **Nombre de propietario del Portfolio** no lo está. Puede usar el modo de texto para mostrar el **Nombre del propietario del Portfolio** en la columna de una vista.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar una vista </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ejemplo: agregar la columna Nombre del propietario del Portfolio a una vista de proyecto

1. Ir a una lista de proyectos.
1. En el menú desplegable **Vista**, haz clic en **Nueva vista**.

1. Haga clic en **Agregar columna** y, a continuación, empiece a escribir &quot;Identificador de propietario del Portfolio&quot; en el campo **Mostrar en esta columna** y, a continuación, selecciónelo cuando se muestre en la lista.

1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic **Haga clic para editar el texto**.
1. Reemplace la línea `valuefield` (`valuefield=portfolio:ownerID`) con la siguiente línea:

   ```
   valuefield=portfolio:owner:name
   ```

   O

   Elimine el texto que encuentre en el cuadro **Modo de texto** y reemplácelo por el siguiente código:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   En este ejemplo concreto, el informe ordenará el informe por el identificador de propietario del Portfolio, tal como indica la línea `querysort`.

   >[!TIP]
   >
   >Para reemplazar cualquier campo `ID` con el campo `name` mediante el modo de texto, reemplace siempre `ID` por `:name` en la línea `valuefield`.

1. Haz clic en **Guardar** y luego en **Guardar vista**.
