---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vista: mostrar objetos que no están incluidos en la interfaz estándar"
description: Puede mostrar en una vista objetos que no están incluidos en la interfaz de modo estándar. Solo puede hacerlo haciendo referencia a ellos mediante el modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '451'
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

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ejemplo: agregar la columna Nombre del propietario del Portfolio a una vista de proyecto

1. Ir a una lista de proyectos.
1. En el menú desplegable **Vista**, haz clic en **Nueva vista**.

1. Haga clic en **Agregar columna** y, a continuación, empiece a escribir &quot;Identificador de propietario del Portfolio&quot; en el campo **Mostrar en esta columna** y, a continuación, selecciónelo cuando se muestre en la lista.

1. Haga clic en **Cambiar al modo de texto** y, a continuación, **Editar el modo de texto**.
1. Reemplace la línea `valuefield` (`valuefield=portfolio:ownerID`) con la siguiente línea:

   `valuefield=portfolio:owner:name`

   O

   Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

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

1. Haga clic en **Listo** y luego en **Guardar vista**.
