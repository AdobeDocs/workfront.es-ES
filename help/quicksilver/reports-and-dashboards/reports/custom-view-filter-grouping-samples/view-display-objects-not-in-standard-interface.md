---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vista: muestra objetos que no están incluidos en la interfaz estándar"
description: 'Puede mostrar en una vista objetos que no están incluidos en la interfaz de modo estándar. Solo puede hacerlo haciendo referencia a ellos mediante el modo de texto. Puede determinar qué campos se pueden incluir en una vista de cualquiera de las siguientes maneras: EDITARME.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Ver: muestra los objetos que no están incluidos en la interfaz estándar

Puede mostrar en una vista objetos que no están incluidos en la interfaz de modo estándar. Solo puede hacerlo haciendo referencia a ellos mediante el modo de texto.\
Puede determinar qué campos se pueden incluir en una vista de cualquiera de las siguientes maneras:

* Utilice el [Explorador de API](../../../wf-api/general/api-explorer.md) para descubrir otros objetos a los que se puede hacer referencia mediante el modo de texto.\
   No todos los campos documentados en el Explorador de API son campos válidos para el modo de texto. Algunos campos solo se pueden registrar a través de la API.

* Busque el campo ID del objeto en una columna. La mayoría de los objetos que tienen un ID de campo también tienen una columna o un nombre de campo correspondiente al que puede que no se pueda acceder mediante la interfaz de modo estándar.

   Puede utilizar el modo de texto para incluir en una vista el nombre de la columna o del campo en lugar del ID reemplazando el `fieldnameID` con el `fieldname:name`.

   Por ejemplo, en la interfaz de modo estándar, la variable **Identificador de propietario del Portfolio** está disponible para una vista de proyecto, pero el campo **Nombre del propietario del Portfolio** el campo no. Puede utilizar el modo de texto para mostrar el **Nombre del propietario del Portfolio** en la columna de una vista.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Ejemplo: agregar la columna Nombre del propietario del Portfolio a una vista de proyecto

1. Ir a una lista de proyectos.
1. Desde el **Ver** , haga clic en **Nueva vista**.

1. Clic **Agregar columna** a continuación, empiece a escribir &quot;ID de propietario del Portfolio&quot; en la **Mostrar en esta columna** y, a continuación, selecciónelo cuando se muestre en la lista.

1. Clic **Cambiar a modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic en **Haga clic para editar el texto**.
1. Reemplace el `valuefield` línea (`valuefield=portfolio:ownerID`) con la línea siguiente:

   ```
   valuefield=portfolio:owner:name
   ```

   O

   Elimine el texto que encuentre en la **Modo de texto** y reemplácelo por el siguiente código:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   En este ejemplo concreto, el informe ordenará el informe por el ID del propietario del Portfolio, tal como indica la variable `querysort` línea.

   >[!TIP]
   >
   >Para reemplazar cualquier campo `ID` con el campo `name` con el modo texto, reemplazar siempre `ID` con `:name` en el `valuefield` línea.

1. Clic **Guardar**, entonces **Guardar vista**.
