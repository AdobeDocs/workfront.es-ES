---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: indique si los resultados de una agrupación deben contraerse o expandirse mediante el modo de texto"
description: "Agrupación: indique si los resultados de una agrupación deben contraerse o expandirse mediante el modo de texto"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Grouping: indica si los resultados de una agrupación deben contraerse o expandirse mediante el modo de texto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Se puede indicar si los resultados de una agrupación deben mostrarse contraídos o expandidos en una lista o informe con Report Builder estándar. De forma predeterminada, los resultados de una visualización de agrupación se expanden. Para obtener información sobre cómo crear una agrupación, consulte [Creación de agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

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
   <td> <p>Solicitud para modificar una agrupación </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una agrupación</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Indique si los resultados de una agrupación deben contraerse o expandirse utilizando el modo de texto

1. Ir a una lista de objetos.
1. Desde el **Agrupación** menú desplegable, seleccione **Nueva agrupación**.

1. Añada una agrupación y haga clic en **Cambiar a modo de texto**.

   O

   Si la agrupación ya está en modo de texto, agregue el código siguiente al nivel de agrupación que desee mostrar contraído:

   ```
   group.0.iscollapsed=true
   ```

1. (Opcional) Si desea que la agrupación se muestre expandida, agregue el siguiente código al nivel de agrupación adecuado:

   ```
   group.0.iscollapsed=false
   ```

1. Clic **Listo**, entonces **Guardar agrupación**.
