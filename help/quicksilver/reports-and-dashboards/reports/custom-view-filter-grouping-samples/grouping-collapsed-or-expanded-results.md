---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: indique si los resultados de una agrupación deben contraerse o expandirse en modo de texto"
description: "Agrupación: indique si los resultados de una agrupación deben contraerse o expandirse mediante el modo de texto"
author: Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Grouping: indica si los resultados de una agrupación deben contraerse o expandirse mediante el modo de texto

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Se puede indicar si los resultados de una agrupación deben mostrarse contraídos o expandidos en una lista o informe con Report Builder estándar. De forma predeterminada, los resultados de una visualización de agrupación se expanden. Para obtener información sobre cómo crear una agrupación, consulte [Crear agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Cuando ajusta manualmente las agrupaciones al ver una lista, Adobe Workfront recuerda su preferencia manual hasta que cierre la sesión. Cuando vuelva a iniciar sesión, la lista se mostrará según esta configuración.
>* Los resultados de una agrupación siempre se muestran expandidos después de acceder a ellos desde un elemento de gráfico.
>

También puede indicar si una agrupación debe mostrarse expandida o contraída mediante el modo de texto.

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

## Indique si los resultados de una agrupación deben contraerse o expandirse utilizando el modo de texto

1. Ir a una lista de objetos.
1. En el menú desplegable **Agrupación** seleccione **Nueva agrupación**.

1. Agregue una agrupación y haga clic en **Cambiar al modo de texto**.

   O

   Si la agrupación ya está en modo de texto, agregue el código siguiente al nivel de agrupación que desee mostrar contraído:

   `group.0.iscollapsed=true`

1. (Opcional) Si desea que la agrupación se muestre expandida, agregue el siguiente código al nivel de agrupación adecuado:

   `group.0.iscollapsed=false`

1. Haga clic en **Listo** y luego en **Guardar agrupación**.
1. (opcional) Actualice el nombre de la agrupación y, a continuación, haga clic en **Guardar agrupación**.
