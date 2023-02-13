---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: crear varias reglas de filtro que hagan referencia al mismo campo (instrucciones 'AND')"
description: En la interfaz de modo estándar, al intentar crear varios filtros que hagan referencia al mismo campo (utilizando el calificador AND), uno de los filtros se elimina al guardar el informe y salir del Creador de informes.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Filtro: crear varias reglas de filtro que hagan referencia al mismo campo (instrucciones &quot;AND&quot;)

En la interfaz de modo estándar, al intentar crear varios filtros que hagan referencia al mismo campo (utilizando el calificador AND), uno de los filtros se elimina al guardar el informe y salir del Creador de informes.

**Ejemplo:** Puede que desee ver solo las tareas que contienen la palabra &quot;verde&quot; pero que no contienen la palabra &quot;rojo&quot; en el nombre. Adobe Workfront no permite guardar las siguientes reglas de filtro mediante la interfaz de modo estándar porque hace referencia al mismo campo (Nombre de tarea) pero utiliza modificadores diferentes y hace referencia a valores diferentes:

* Nombre de la tarea > Contiene > Verde
* Nombre de la tarea > No contiene > Rojo

Sin embargo, puede crear este filtro utilizando el modo de texto .

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

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear varias reglas de filtro que hagan referencia al mismo campo

1. Vaya a una lista de tareas.
1. En el **Filtro** menú desplegable, seleccione **Nuevo filtro**.
1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. En el área Definir reglas de filtro para el informe , agregue el siguiente código:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Para crear filtros similares, cree primero la primera instrucción . Por ejemplo:
   >
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copie y pegue la instrucción tantas veces como sea necesario. A continuación, puede agregar tantas instrucciones como necesite para hacer referencia al mismo campo (en nuestro caso, &quot;name&quot;) y realizar las siguientes modificaciones a las instrucciones adicionales:
   >
   >1. Antes de las dos líneas copiadas con &quot;AND&quot;:1:&quot;, &quot;Y:2:&quot;, &quot;Y:3:&quot;, etc para cada nuevo campo posible valor.
   >1. Reemplace la línea del campo con el nuevo valor del campo (después del signo &quot;=&quot;).
   >1. Reemplace la línea modificadora (_Mod) con el nuevo modificador.

   >   
   >Estas instrucciones distinguen entre mayúsculas y minúsculas.

1. Haga clic en **Listo**, luego **Guardar filtro**.
