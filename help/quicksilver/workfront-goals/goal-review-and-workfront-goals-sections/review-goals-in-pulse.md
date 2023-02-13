---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Revise los objetivos en la sección Pulso de objetivos de Adobe Workfront
description: Puede ver todos los objetivos de su organización, independientemente de quién sea el propietario. Para obtener información sobre la creación de objetivos, consulte Crear objetivos en Objetivos de Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 33873797-183d-4efc-9099-26eb907ca799
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 1%

---

# Revise los objetivos en la sección Pulso de objetivos de Adobe Workfront

>[!IMPORTANT]
> 
>La funcionalidad descrita en este artículo se ha eliminado de Workfront, a partir de la versión 23.1.\
>Este artículo también se eliminará poco después de la versión 23.1, a principios de 2023. En este momento, le recomendamos que actualice los marcadores según corresponda.


Puede ver todos los objetivos de su organización, independientemente de quién sea el propietario. Para obtener información sobre la creación de objetivos, consulte [Crear objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Puede utilizar la sección Pulse de Objetivos de Adobe Workfront como herramienta de colaboración, donde puede revisar y participar en un flujo de actualizaciones sobre objetivos actuales que le pertenecen, a sus equipos, grupos u organización, y asegurarse de que los objetivos se mantienen actualizados. Los objetivos de Workfront agrupan las actualizaciones de progreso, los comentarios y el historial de edición por objetivos en la sección Pulso .

## Requisitos de acceso

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>Debe adquirir una licencia adicional para los objetivos de Adobe Workfront para acceder a la funcionalidad que se describe en este artículo. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para utilizar los objetivos de Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver o tener más acceso a los objetivos</p> <p>Nota:  <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Conceder acceso a los objetivos de Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> 
    <div> 
     <p>Ver o permisos superiores en objetivos</p> 
     <p>Para obtener información sobre cómo compartir objetivos, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir un objetivo en los objetivos de Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe tener lo siguiente para poder iniciar:

* Plantilla de diseño que incluye el área Objetivos del menú principal.

## Administrar actualizaciones y comentarios de objetivo en la sección Pulse 

>[!TIP]
>
>En la sección Pulse solo aparecen los objetivos que se han marcado en al menos una vez.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) > **Objetivos** en la esquina superior derecha de la pantalla.

   Se abrirá el área Objetivos de Workfront .

   Todos los objetivos se muestran de forma predeterminada.

1. Haga clic en **Pulse** en el panel izquierdo.

   <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: see the numbering in the procedure)
      </MadCap:conditionalText>
      -->

   Se muestra una lista de objetivos. La lista contiene las columnas siguientes con información sobre cada objetivo:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Metas</td> 
         <td>El nombre del objetivo.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Propietario</td> 
         <td>Nombre del propietario del objetivo.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Periodo</td> 
         <td>Período de tiempo para el que se programa el objetivo.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Progreso</td> 
         <td>El indicador de progreso del objetivo que suele ser un valor de porcentaje.</td> 
      </tr> 
      <tr> 
         <td role="rowheader"> <p>Estado (incluye icono de alineación)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
         <td> <p>El estado del objetivo que puede ser uno de los siguientes:</p> 
         <ul> 
         <li>Activo</li> 
         <li>Borrador</li> 
         <li>Inactivo</li> 
         <li>Cerrado</li> 
         </ul> <p>El icono de alineación aparece en los objetivos alineados con otros objetivos. Para obtener información sobre la alineación de objetivos, consulte <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Alinear objetivos conectándolos en los objetivos de Adobe Workfront</a>.</p>

   <p>La columna Estado también incluye las actualizaciones incrementales realizadas para cada resultado o actividad con cada registro en el objetivo.</p>

   Por ejemplo, si el objetivo tiene una actividad de barra de progreso manual y usted se fija en el objetivo y actualiza la actividad al 50 %, la columna Estado muestra el 50 % para la actividad de ese objetivo. Más adelante, podría actualizar la misma actividad al 60 %. En este caso, se muestra una nueva línea bajo el mismo objetivo para la misma actividad durante el 10 %, porque acaba de añadir el 10 % al progreso de la actividad.
   </td>
   </tr> 
      </tbody> 
      </table>

1. (Opcional) Para seleccionar el tipo de información que desea mostrar, actualice los filtros de la esquina superior derecha de la sección Pulso .

   La lista Pulse muestra los objetivos y su historial actualizado que coinciden con los criterios del filtro seleccionado.

   Para obtener más información sobre los objetivos de filtrado, consulte [Filtrar información en objetivos de Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Haga clic en la flecha hacia la derecha situada a la izquierda del nombre del objetivo para expandir un objetivo y ver información adicional sobre las actualizaciones de cada objetivo.

   La siguiente información se muestra en la sección Pulse debajo de cada objetivo:

   * Nombres de resultados y propietarios. Para obtener información sobre los resultados, consulte [Agregar resultados a objetivos en Objetivos de Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * Nombres y propietarios de actividades. Para obtener información sobre las actividades, consulte [Agregar actividades a objetivos en Objetivos de Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * Barras de progreso y estados de progreso de resultados y actividades. Para obtener información sobre cómo calculan los objetivos los objetivos de Workfront, consulte [Resumen del progreso y la condición del objetivo en los objetivos de Adobe Workfront](../../workfront-goals/goal-management/calculate-goal-progress.md).

1. Haga clic en **Añadir un comentario** para agregar un comentario para el objetivo, haga clic en **Publicación**. El comentario se puede ver en el área de facturación, así como en la pestaña Actualizaciones del panel Detalles del objetivo . Le recomendamos que utilice la sección Pulso para comentar sobre los objetivos que no se han actualizado en poco tiempo y pedir al propietario del objetivo que actualice.

1. (Opcional) Haga clic en **Mostrar todas las actualizaciones** para mostrar todas las actualizaciones de objetivos. Se abre la pestaña Actualizaciones en el panel Detalles del objetivo de la derecha.
1. Haga clic en el nombre de un objetivo para abrir el **Detalles del objetivo** panel de la derecha y revise más información sobre el objetivo, así como administrarlo y sus resultados y actividades. Para obtener información sobre la revisión de objetivos individuales, consulte [Actualizar objetivos en la sección Detalles del objetivo de los objetivos de Adobe Workfront](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Opcional y condicional) Haga clic en **el icono de alineación** ![](assets/align-icon.png) para abrir el objetivo en la sección Alineación de objetivo , si el objetivo está alineado con otros objetivos.

1. (Opcional) Expanda el **Objetivos por página** menú desplegable y seleccione entre las siguientes opciones para mostrar objetivos adicionales:

   * 20. Esta es la selección predeterminada.
   * 50
   * 100


