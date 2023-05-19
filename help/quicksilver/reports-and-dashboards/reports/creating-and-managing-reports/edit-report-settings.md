---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Editar configuración del informe
description: Puede editar la configuración de un informe para definir cómo se muestra a los demás usuarios o qué tipo de información pueden solicitar los usuarios antes de ejecutar el informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 9%

---

# Editar configuración del informe

Puede editar la configuración de un informe para definir cómo se muestra a los demás usuarios o qué tipo de información pueden solicitar los usuarios antes de ejecutar el informe.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Pasos a seguir

1. Comience a crear un informe accediendo a la **Menú principal** > **Informes**, luego seleccione el objeto del informe.

   O

   Abra un informe existente y haga clic en **Acciones de informe** > **Editar**.

1. Clic **Configuración de informes** en la esquina superior derecha de report builder.
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
      <td role="rowheader">Ejecutar este informe con los derechos de acceso de</td> 
      <td>Seleccione el usuario cuyos derechos de acceso desea que utilice este informe cuando se muestre a otros usuarios. Para obtener más información sobre cómo ejecutar un informe con los derechos de acceso de otro usuario, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Ejecutar y entregar un informe con los derechos de acceso de otro usuario</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando el informe se cargue, mostrar</td> 
      <td>Seleccione la pestaña predeterminada que se muestra para todos los usuarios cuando se carga el informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando se cargue el informe en un panel, mostrar elementos...</td> 
      <td>Especifique el número de elementos que se muestran para todos los usuarios cuando el informe se carga en un panel. El valor predeterminado es 15 elementos y el número máximo de elementos es 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar la vista Cuadrícula de recursos en la ficha Detalles</td> 
      <td> <p>(Solo informe de usuario) Seleccione esta opción para mostrar la cuadrícula de recursos en la pestaña Detalles del informe.</p> <p>Nota: Al aplicar la vista Cuadrícula de recursos a un informe de usuario, el informe sólo muestra los proyectos que se encuentran en el estado Actual. Si desea ver proyectos en cualquier otro estado, puede utilizar la ficha Utilización de usuarios en el área Personas de la barra de exploración global y aplicar allí la vista Cuadrícula de recursos. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar una vista especial en la ficha Detalles</td> 
      <td>(Solo informe de proyecto) Especifique el tipo de vista que los usuarios verán cuando accedan a esta información en la pestaña Detalles. Por ejemplo, puede seleccionar una vista de Hito o Gantt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar este informe en una vista Gantt de forma predeterminada</td> 
      <td>(Solo informe de proyecto e informe de tareas) Seleccione esta opción para que la vista Gantt se active automáticamente cuando los usuarios vean la ficha Detalles en este informe.<br>Para obtener más información sobre la visualización del gráfico Gantt en los informes de proyecto y de tarea, consulte la sección "Visualización de información de tarea en la lista de proyectos del gráfico Gantt" en el artículo <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Ver información en el gráfico Gantt </a>.</td> 
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

1. Clic **Indicadores de informe** para configurar cualquier solicitud de informe.\
   Para obtener más información sobre cómo agregar indicadores a un informe, vea el artículo [Agregar una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Clic **Listo,** luego haga clic en **Guardar + Cerrar**.

## Información adicional

Consulte también:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Introducción a los informes en Adobe Workfront](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Uso de informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
