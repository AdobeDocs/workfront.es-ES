---
title: Editar agrupaciones existentes
description: Editar agrupaciones existentes
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Editar agrupaciones existentes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

Puede personalizar una agrupación existente que haya creado originalmente o que se haya compartido con usted. A continuación, puede guardarlo como una nueva agrupación.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitud o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Paneles y Calendarios para editar una agrupación en un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administración de permisos de un informe para editar una agrupación en un informe</p> <p>Administración de permisos en una agrupación </p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe crear una agrupación para poder editarla.

Para obtener información sobre cómo crear una agrupación, consulte [Crear agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Pasos a seguir

1. Vaya a una lista de objetos que contiene la agrupación que desea personalizar.
1. Haga clic en el icono **Agrupación**.
1. Seleccione la agrupación que desee personalizar y, a continuación, haga clic en el icono **Editar**.

   ![Seleccione el icono de edición.](assets/customizegrouping-nwe-standard-350x291.png)

   Se abre el Generador de interfaces para personalizar la agrupación.

1. En la sección **Vista previa de la agrupación**, haga clic en **Agregar agrupación** para definir cómo desea que se organice la información en el informe. A continuación, se muestra una vista previa del aspecto de la agrupación en el informe.

1. Comience a escribir el nombre del campo que representa la forma en que desea organizar la información en el informe y, a continuación, haga clic en él cuando aparezca en la lista desplegable.
1. (Opcional y condicional) Cuando vea una lista actualizada, seleccione **Contraer esta agrupación de forma predeterminada** si desea que los resultados de la agrupación se muestren contraídos en lugar de expandidos. Esta configuración está deshabilitada de forma predeterminada y los resultados de la agrupación siempre se muestran en la lista expandida.

   Para obtener información acerca de las listas actualizadas y heredadas, consulte la sección &quot;La diferencia entre las listas actualizadas y heredadas&quot; en el artículo [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Cuando ajusta manualmente las agrupaciones al ver una lista, Workfront recuerda su preferencia manual hasta que cierre la sesión. Cuando vuelva a iniciar sesión, la lista se mostrará según esta configuración.
   >* Los resultados de una agrupación siempre se muestran expandidos después de acceder a ellos desde un elemento de gráfico o en una lista heredada. En estos casos, se ignora esta configuración.

1. Repita los pasos 4, 5 y 6 para definir agrupaciones adicionales.\
   Puede definir hasta tres agrupaciones para organizar la información. Puede organizar aún más la información con hasta cuatro agrupaciones creando un informe de matriz. Para obtener más información sobre los informes de matriz, consulte [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Haga clic en **Guardar como nueva agrupación** para reemplazar la agrupación actual con los cambios.
