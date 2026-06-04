---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Editar la configuración de los informes
description: Puede editar la configuración de un informe para definir cómo se muestra a los demás usuarios o qué tipo de información pueden solicitar los usuarios antes de ejecutar el informe.
author: Courtney
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/GqhjJ-aQZfDJq4RYEtJoleC41CQtEJ-38aiSI43FHLE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 582
ht-degree: 95%

---

# Editar la configuración de los informes

<!-- Audited: 11/2024 -->

Puede editar la configuración de un informe para definir cómo se muestra a los demás usuarios o qué tipo de información pueden solicitar los usuarios antes de ejecutar el informe.

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
      <p>Estándar</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuración de nivel de acceso</td> 
   <td> <p>Acceso de Edición a informes, paneles de control y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
 <td> <p>Permisos de administración para un informe</p></td>  
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pasos a seguir

1. Comience a crear un informe yendo al **Menú principal** > **Informes**, y luego seleccione el objeto del informe.

   O

   Abra un informe existente y luego haga clic en **Acciones de informe** > **Editar**.

1. Haga clic en **Configuración de informes** en la esquina superior derecha del creador de informes.
1. Configure las siguientes opciones del informe:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Título del informe</td> 
      <td>Especifique un título para el informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Especifique una instrucción que describa el propósito y los usos del informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ejecute este informe con los derechos de acceso de</td> 
      <td>Seleccione el usuario cuyos derechos de acceso desea que utilice este informe cuando se muestre a otros usuarios. Para obtener más información acerca de cómo ejecutar un informe con los derechos de acceso de otro usuario, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Ejecutar y entregar un informe con los derechos de acceso de otro usuario</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando el informe se cargue, mostrar</td> 
      <td>Seleccione la pestaña predeterminada que se muestra para todos los usuarios cuando se carga el informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando se cargue el informe en un panel de control, mostrar ... elementos</td> 
      <td>Especifique el número de elementos que se muestran para todos los usuarios cuando el informe se carga en un panel de control. El valor predeterminado es 15 elementos y el número máximo de elementos es 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar la vista Cuadrícula de recursos en la ficha Detalles</td> 
      <td> <p>(Solo informe de usuario) Seleccione esta opción para mostrar la Cuadrícula de recursos en la ficha Detalles del informe.</p> <p>Nota: Al aplicar la vista Cuadrícula de recursos a un informe de usuario, el informe sólo muestra los proyectos que se encuentran en el estado Actual. Si desea ver proyectos en cualquier otro estado, puede utilizar la ficha Utilización de usuarios en el área Personas de la barra de exploración global y aplicar allí la vista Cuadrícula de recursos.
      <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        -->
        </p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar una vista especial en la ficha Detalles:</td> 
      <td>(Solo informe de proyecto) Especifique el tipo de vista que los usuarios verán cuando accedan a esta información en la pestaña Detalles. Por ejemplo, puede seleccionar una vista de Hito o Gantt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar este informe en una vista Gantt de forma predeterminada</td> 
      <td>(Solo informe de proyecto e informe de tareas) Seleccione esta opción para que la vista Gantt se habilite automáticamente cuando los usuarios vean la ficha Detalles en este informe.<br>Para obtener más información acerca de cómo ver el gráfico Gantt en los informes de proyectos y tareas, consulte la sección “Ver información de tareas en la lista de proyectos del gráfico Gantt” en el artículo <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Ver información en el gráfico Gantt </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir cambiar la vista en el informe</td> 
      <td>Seleccione esta opción para permitir que los usuarios cambien la Vista al ejecutar el informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir cambiar el grupo en el informe</td> 
      <td>Seleccione esta opción para permitir que los usuarios cambien el grupo al ejecutar el informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir cambiar el filtro del informe</td> 
      <td>Seleccione esta opción para permitir que los usuarios cambien el filtro cuando ejecuten el informe.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Solicitudes de informe** para configurar cualquier solicitud del informe.\
   Para obtener más información sobre cómo añadir solicitudes a un informe, consulte el artículo [Añadir una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Haz clic en **Listo,** y luego haz clic en **Guardar + Cerrar**.

## Más información

Consulte también lo siguiente:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Introducción a los informes](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Uso de informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
