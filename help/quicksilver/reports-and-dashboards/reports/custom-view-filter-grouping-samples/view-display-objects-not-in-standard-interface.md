---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Ver: mostrar objetos que no están incluidos en la interfaz estándar"'
description: 'Puede mostrar en objetos de vista que no estén incluidos en la interfaz de modo estándar. Esto solo se puede hacer haciendo referencia a ellos mediante el modo de texto. Puede determinar qué campos se pueden incluir en una vista de cualquiera de las siguientes maneras: EDITAR.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Vista: mostrar objetos que no están incluidos en la interfaz estándar

Puede mostrar en objetos de vista que no estén incluidos en la interfaz de modo estándar. Esto solo se puede hacer haciendo referencia a ellos mediante el modo de texto.\
Puede determinar qué campos se pueden incluir en una vista de cualquiera de estas formas:

* Utilice la variable [Explorador de API](https://one.workfront.com/s/api-explorer) para descubrir otros objetos a los que se puede hacer referencia mediante el modo de texto.\
   No todos los campos documentados en el Explorador de API son campos válidos para el modo de texto. Algunos campos solo se pueden registrar a través de la API.

* Busque el campo ID del objeto en una columna. La mayoría de los objetos que tienen un ID de campo también tienen un nombre de columna o campo correspondiente al que es posible que no se pueda acceder mediante la interfaz de modo estándar.

   Puede utilizar el modo de texto para incluir en una vista el nombre de columna o campo en lugar del ID reemplazando el valor `fieldnameID` con la variable `fieldname:name`.

   Por ejemplo, en la interfaz de modo estándar, la variable **ID del propietario del Portfolio** está disponible para una vista de proyecto, pero la variable **Nombre del propietario del Portfolio** no lo es. Puede utilizar el modo de texto para mostrar la variable **Nombre del propietario del Portfolio** en la columna de una vista.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ejemplo: agregar la columna Nombre del propietario del Portfolio a una vista de proyecto

1. Vaya a una lista de proyectos.
1. En el **Ver** menú desplegable, haga clic en **Nueva vista**.

1. Haga clic en **Agregar columna** a continuación, empiece a escribir &quot;ID del propietario del Portfolio&quot; en la **Mostrar en esta columna** y selecciónelo cuando aparezca en la lista.

1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Sustituya el `valuefield` línea (`valuefield=portfolio:ownerID`) con la siguiente línea:

   ```
   valuefield=portfolio:owner:name
   ```

   O

   Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   En este ejemplo concreto, el informe se clasificará por el ID del propietario del Portfolio, tal como indica el `querysort` línea.

   >[!TIP]
   >
   >Reemplazar cualquier campo `ID` con el campo `name` mediante el modo de texto, reemplazar siempre `ID` con `:name` en el `valuefield` línea.

1. Haga clic en **Guardar**, luego **Guardar vista**.
