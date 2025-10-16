---
title: Editar agrupaciones existentes
description: Editar agrupaciones existentes
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 51%

---

# Editar agrupaciones existentes

<!-- Audited: 11/2024 -->

<!--NOTE: This is the third part of a former article split in 3: two how-tos and one reference article about creating and customizing groupings)-->

Puede personalizar una agrupación existente que haya creado originalmente o que se haya compartido con usted. A continuación, puede guardarlo como una nueva agrupación.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</strong></td> 
   <td> 
    <p>Colaborador o superior</p>
    <p>Solicitud o superior</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Paneles y Calendarios para editar una agrupación en un informe</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
    <td> <p>Permisos de administración a un informe para editar una agrupación en este</p> <p>Administración de permisos en una agrupación</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Requisitos previos

Debe crear una agrupación para poder editarla.

Para obtener información sobre cómo crear una agrupación, consulte [Crear agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Pasos a seguir

1. Vaya a una lista de objetos que contiene la agrupación que desea personalizar.
1. Haga clic en el icono **Agrupación**.
1. Seleccione la agrupación que desee personalizar y luego haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).

   ![Seleccione el icono de edición.](assets/customizegrouping-nwe-standard-350x291.png)

   Se abre el Generador de interfaces para personalizar la agrupación.

1. En la sección **Vista previa de la agrupación**, haga clic en **Añadir agrupación** para organizar la información en el informe. A continuación, se muestra una vista previa del aspecto de la agrupación en el informe.

1. Empiece a escribir el nombre del campo que representa la forma en que desea organizar la información en el informe y, a continuación, haga clic en él cuando aparezca en la lista desplegable.
1. (Opcional y condicional) Cuando vea una lista actualizada, seleccione **Contraer esta agrupación de forma predeterminada** si desea que los resultados de la agrupación se muestren contraídos en lugar de expandidos. Esta configuración está deshabilitada de forma predeterminada y los resultados de la agrupación siempre se muestran en la lista expandida.

   Para obtener información acerca de las listas actualizadas y heredadas, consulte la sección &quot;La diferencia entre las listas actualizadas y heredadas&quot; en el artículo [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Cuando ajusta manualmente las agrupaciones al ver una lista, Workfront recuerda su preferencia manual hasta que cierre la sesión. Cuando vuelva a iniciar sesión, la lista se mostrará según esta configuración.
   >* Los resultados de una agrupación siempre se muestran expandidos tras acceder a ellos desde un elemento de gráfico o en una lista heredada. En estos casos, se ignora esta configuración.

1. Repita los pasos 4, 5 y 6 para definir agrupaciones adicionales.\
   Puede definir hasta tres agrupaciones para organizar la información. Puede organizar todavía más la información con hasta cuatro agrupaciones creando un informe de matriz. Para obtener más información sobre los informes de matriz, consulte [Creación de un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Haga clic en **Guardar agrupación** para reemplazar la agrupación actual con los cambios.
