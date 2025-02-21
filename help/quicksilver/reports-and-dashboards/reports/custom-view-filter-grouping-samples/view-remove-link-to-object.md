---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Quitar vínculo a un objeto en una columna'
description: De forma predeterminada, algunos objetos que se muestran en una vista se vinculan a la página Detalles del objeto. Por ejemplo, la columna que muestra el nombre de un proyecto es un vínculo al proyecto; la columna que muestra el nombre de un usuario es un vínculo a la página de perfil del usuario.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 83%

---

# Vista: quitar el vínculo a un objeto en una columna

<!--Audited: 11/2024-->

De forma predeterminada, algunos objetos que se muestran en una vista se vinculan a la página Detalles del objeto. Por ejemplo, la columna que muestra el nombre de un proyecto es un vínculo al proyecto; la columna que muestra el nombre de un usuario es un vínculo a la página de perfil del usuario.

Puede quitar este vínculo mediante el modo de texto en columnas que se muestran en todas las vistas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p> Actual: 
   <ul>
   <li>Solicitud para modificar una vista</li> 
   <li>Plan para modificar un informe</li>
   </ul>
     </p>
     <p> Nuevo: 
   <ul>
   <li>Colaborador para modificar una vista</li> 
   <li>Estándar para modificar un informe</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Edición del acceso a Filtros, Vistas y Agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Ejemplo: Quitar el vínculo a una tarea de la columna Nombre de tarea en una vista de tareas:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista** para crear una nueva vista.

   O

   Haga clic en el **icono Editar** ![icono Editar](assets/edit-icon.png)

   para editar una vista existente y, a continuación, seleccione la vista.

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

