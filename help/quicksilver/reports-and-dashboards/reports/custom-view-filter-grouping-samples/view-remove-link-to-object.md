---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Quitar vínculo a un objeto en una columna'
description: De forma predeterminada, algunos objetos que se muestran en una vista se vinculan a la página Detalles del objeto. Por ejemplo, la columna que muestra el nombre de un proyecto es un vínculo al proyecto; la columna que muestra el nombre de un usuario es un vínculo a la página de perfil del usuario.
author: Courtney
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/J-FHP3ySrleMgoRDrh5xzapQfqjtwraEAwX8xwvKTuk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 372
ht-degree: 76%

---

# Vista: quitar el vínculo a un objeto en una columna

<!--Audited: 11/2024-->

De forma predeterminada, algunos objetos que se muestran en una vista se vinculan a la página Detalles del objeto. Por ejemplo, la columna que muestra el nombre de un proyecto es un vínculo al proyecto; la columna que muestra el nombre de un usuario es un vínculo a la página de perfil del usuario.

Puede quitar este vínculo mediante el modo de texto en columnas que se muestran en todas las vistas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar una vista </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Edición del acceso a Filtros, Vistas y Agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## Ejemplo: Quitar el vínculo a una tarea de la columna Nombre de tarea en una vista de tareas:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista** para crear una nueva vista.

   O

   Haga clic en el **icono Editar** ![Icono Editar](assets/edit-icon.png) para editar una vista existente y, a continuación, seleccione la vista.

1. Haga clic en **Añadir columna** para añadir una columna nueva.

   O

   Haga clic en una columna existente con un vínculo a un objeto.

1. Haga clic en **Cambiar al modo de texto** > **Editar modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >Puede utilizar un código similar para otros objetos si ajusta lo siguiente:
   >
   >* Reemplace la línea `valuefield` del código por `valueexpression` y mantenga el mismo nombre incluido entre llaves después del signo igual.
   >* Elimine todas las líneas que comienzan con `link.` del texto original de la columna. Por ejemplo, elimine todas las líneas siguientes:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Haga clic en **Listo** y luego en **Guardar vista**.

