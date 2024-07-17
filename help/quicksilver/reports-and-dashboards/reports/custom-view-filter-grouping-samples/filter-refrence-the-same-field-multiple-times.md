---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: crear varias reglas de filtro que hagan referencia al mismo campo (instrucciones 'AND')"
description: En la interfaz de modo estándar, al intentar crear varios filtros que hacen referencia al mismo campo (mediante el calificador AND), uno de los filtros se elimina al guardar el informe y salir del Report Builder.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Filtro: crear varias reglas de filtro que hagan referencia al mismo campo (instrucciones &quot;AND&quot;)

En la interfaz de modo estándar, al intentar crear varios filtros que hacen referencia al mismo campo (mediante el calificador AND), uno de los filtros se elimina al guardar el informe y salir del Report Builder.

**Ejemplo:** Es posible que solo desee ver las tareas que contienen la palabra &quot;verde&quot; pero no la palabra &quot;rojo&quot; en el nombre. Adobe Workfront no permite guardar las siguientes reglas de filtrado mediante la interfaz de modo estándar porque hace referencia al mismo campo (Nombre de tarea) pero utiliza diferentes modificadores y hace referencia a valores diferentes:

* Nombre de tarea > Contiene > Verde
* Nombre de tarea > No contiene > Rojo

Sin embargo, puede crear este filtro con el modo de texto.

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
   <td> <p>Solicitud para modificar un filtro </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Crear varias reglas de filtro que hagan referencia al mismo campo

1. Ir a una lista de tareas.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.
1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic **Haga clic para editar el texto**.
1. En el área Definir reglas de filtro para el informe, agregue el siguiente código:

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

1. Haga clic en **Listo** y luego en **Guardar filtro**.
