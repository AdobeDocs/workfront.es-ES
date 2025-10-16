---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vista: Muestra objetos que no están incluidos en la interfaz estándar'
description: Puede mostrar en una vista objetos que no están incluidos en la interfaz de modo estándar. Solo puede hacerlo haciendo referencia a ellos mediante el modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 86%

---

# Vista: mostrar objetos que no están incluidos en la interfaz estándar

Puede mostrar en una vista objetos que no están incluidos en la interfaz de modo estándar. Solo puede hacerlo haciendo referencia a ellos mediante el modo de texto.\
Puede determinar qué campos se pueden incluir en una vista de cualquiera de las siguientes maneras:

* Use el [explorador de la API](../../../wf-api/general/api-explorer.md) para descubrir otros objetos a los que se puede hacer referencia mediante el modo de texto.\
  No todos los campos documentados en el explorador de la API son campos válidos para el modo de texto. Algunos campos solo se pueden notificar a través de la API.

* Busque el campo ID del objeto en una columna. La mayoría de los objetos que tienen un ID de campo también tienen una columna o un nombre de campo correspondiente que puede no ser accesible a través de la interfaz de modo estándar.

  Puede utilizar el modo de texto para incluir en una vista el nombre de columna o campo en lugar del ID reemplazando `fieldnameID` por el `fieldname:name`.

  Por ejemplo, en la interfaz de modo estándar, el campo **Identificador de propietario de portafolio** está disponible para una vista de proyecto, pero el campo **Nombre de propietario de portafolio** no lo está. Puede usar el modo de texto para mostrar el **Nombre del propietario de portafolio** en la columna de una vista.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ejemplo: añadir la columna Nombre del propietario de portafolio a una vista de proyecto

1. Ir a una lista de proyectos.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista**.

1. Haga clic en **Añadir columna** y, a continuación, empiece a escribir el “ID del propietario de portafolio” en el campo **Mostrar en esta columna** y, a continuación, selecciónelo cuando se muestre en la lista.

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

   En este ejemplo concreto, el informe ordenará el informe por el identificador de propietario del portafolio, tal como indica la línea `querysort`.

   >[!TIP]
   >
   >Para reemplazar cualquier campo `ID` con el campo `name` mediante el modo de texto, reemplace siempre `ID` por `:name` en la línea `valuefield`.

1. Haga clic en **Listo** y luego en **Guardar vista**.
