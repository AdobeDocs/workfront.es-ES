---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: Crear varias reglas de filtro que hagan referencia al mismo campo (instrucciones "AND")'
description: En la interfaz de modo estándar, al intentar crear varios filtros que hacen referencia al mismo campo (mediante el calificador AND), uno de los filtros se elimina al guardar el informe y salir del Report Builder.
author: Courtney
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/GkRwwb61-KuX14NsIAJVh0aG4CxipyKHymqI7eNAUEU
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
source-wordcount: 383
ht-degree: 24%

---

# Filtro: crear varias reglas de filtro que hagan referencia al mismo campo (instrucciones “AND“)

<!--Audited: 10/2024-->

En la interfaz de modo estándar, al intentar crear varios filtros que hacen referencia al mismo campo (mediante el calificador AND), uno de los filtros se elimina al guardar el informe y salir del Report Builder.

**Ejemplo:** Es posible que solo desee ver las tareas que contienen la palabra &quot;verde&quot; pero no la palabra &quot;rojo&quot; en el nombre. Adobe Workfront no permite guardar las siguientes reglas de filtrado mediante la interfaz de modo estándar porque hace referencia al mismo campo (Nombre de tarea) pero utiliza diferentes modificadores y hace referencia a valores diferentes:

* Nombre de tarea > Contiene > Verde
* Nombre de tarea > No contiene > Rojo

Sin embargo, puede crear este filtro con el modo de texto.

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

## Crear varias reglas de filtro que hagan referencia al mismo campo

1. Vaya a una lista de tareas.
1. Haga clic en el menú desplegable **Filtro** y seleccione **Nuevo filtro**.
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
