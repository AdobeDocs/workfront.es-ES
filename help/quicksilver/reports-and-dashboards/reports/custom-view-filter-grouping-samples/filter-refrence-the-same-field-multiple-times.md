---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: Crear varias reglas de filtro que hagan referencia al mismo campo (instrucciones 'AND')"
description: En la interfaz de modo estándar, al intentar crear varios filtros que hacen referencia al mismo campo (mediante el calificador AND), uno de los filtros se elimina al guardar el informe y salir del Report Builder.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Filtro: crear varias reglas de filtro que hagan referencia al mismo campo (instrucciones &quot;AND&quot;)

<!--Audited: 10/2024-->

En la interfaz de modo estándar, al intentar crear varios filtros que hacen referencia al mismo campo (mediante el calificador AND), uno de los filtros se elimina al guardar el informe y salir del Report Builder.

**Ejemplo:** Es posible que solo desee ver las tareas que contienen la palabra &quot;verde&quot; pero no la palabra &quot;rojo&quot; en el nombre. Adobe Workfront no permite guardar las siguientes reglas de filtrado mediante la interfaz de modo estándar porque hace referencia al mismo campo (Nombre de tarea) pero utiliza diferentes modificadores y hace referencia a valores diferentes:

* Nombre de tarea > Contiene > Verde
* Nombre de tarea > No contiene > Rojo

Sin embargo, puede crear este filtro con el modo de texto.

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

## Crear varias reglas de filtro que hagan referencia al mismo campo

1. Ir a una lista de tareas.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.
1. Haga clic en **Modo de texto**.
1. En el cuadro que se muestra, agregue el siguiente código:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Para generar filtros similares, genere primero la primera instrucción. Por ejemplo:
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copie y pegue la instrucción tantas veces como sea necesario. A continuación, puede agregar tantas instrucciones como necesite para hacer referencia al mismo campo (en nuestro caso, &quot;name&quot;) y realizar las siguientes modificaciones en las instrucciones adicionales:
   >
   >1. Precede las dos líneas copiadas con &quot;AND:1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot;, etc. para cada nuevo valor posible de campo.
   >1. Reemplace la línea del campo por el nuevo valor del campo (después del signo &quot;=&quot;).
   >1. Reemplace la línea de modificador (_Mod) por el nuevo modificador.
   >   
   >Estas instrucciones distinguen entre mayúsculas y minúsculas.

1. Haga clic en **Aplicar** y luego en **Guardar como nuevo**.
