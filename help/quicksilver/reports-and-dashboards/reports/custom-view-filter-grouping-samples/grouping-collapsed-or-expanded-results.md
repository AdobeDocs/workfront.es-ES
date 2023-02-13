---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupación: indicar si los resultados de una agrupación deben contraerse o expandirse mediante el modo de texto.'
description: '"Agrupación: indicar si los resultados de una agrupación deben contraerse o expandirse mediante el modo de texto.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Agrupación: indicar si los resultados de una agrupación deben contraerse o expandirse mediante el modo de texto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Puede indicar si los resultados de una agrupación deben mostrarse contraídos o expandidos en una lista o informe utilizando el Creador de informes estándar. De forma predeterminada, los resultados de una agrupación se muestran expandidos. Para obtener información sobre cómo crear una agrupación, consulte [Crear agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Cuando ajusta las agrupaciones manualmente al ver una lista, Adobe Workfront recuerda su preferencia manual hasta que cierre la sesión. Cuando vuelve a iniciar sesión, la lista se muestra según esta configuración.
>* Los resultados de una agrupación siempre se muestran expandidos después de acceder a ellos desde un elemento de gráfico.
>


También puede indicar si una agrupación debe mostrarse expandida o contraída mediante el modo de texto.

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

## Indicar si los resultados de una agrupación deben contraerse o expandirse mediante el modo de texto

1. Ir a una lista de objetos.
1. En el **Agrupación** menú desplegable, seleccione **Nuevo grupo**.

1. Añada una agrupación y haga clic en **Cambiar al modo de texto**.

   O

   Si la agrupación ya está en modo de texto, agregue el siguiente código al nivel de agrupación que desea mostrar contraído:

   ```
   group.0.iscollapsed=true
   ```

1. (Opcional) Si desea que la agrupación se muestre ampliada, agregue el siguiente código al nivel de agrupación correspondiente:

   ```
   group.0.iscollapsed=false
   ```

1. Haga clic en **Listo**, luego **Guardar agrupación**.
