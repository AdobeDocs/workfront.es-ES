---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: mostrar solo los elementos en un estado de aprobación"
description: Solo puede mostrar elementos con un estado determinado que esté actualmente en Aprobación pendiente. Esto funciona igual para cualquier otro objeto con un estado de aprobación.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---

# Filtro: mostrar solo los elementos en un estado de aprobación

Solo puede mostrar elementos con un estado determinado que esté actualmente en Aprobación pendiente. Esto funciona igual para cualquier otro objeto con un estado de aprobación.

Puede colocar los siguientes objetos en un estado de aprobación:

* Tareas
* Problemas
* Proyectos

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

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Mostrar solo los elementos en estado de aprobación

1. Vaya al filtro que desee personalizar para una lista de proyectos, por ejemplo.
1. Clic **Agregar una regla de filtro** para el **Estado** del objeto de la lista.\
   Por ejemplo, en un informe de proyecto, añada **Estado Igual Planificación**, si desea mostrar solo los proyectos con un estado de **Planificación - Aprobación pendiente**.

1. Clic **Cambiar a modo de texto**.
1. Modifique la

   ```
   status
   ```

   línea al añadir **:A** a la clave de 3 letras del estado:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Clic **Listo**, entonces **Guardar filtro**.

   La lista solo muestra los proyectos que están en estado de Planificación - Aprobación pendiente.
