---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Editar la configuración del informe
description: Puede editar la configuración de un informe para definir cómo se muestra para otros usuarios o qué tipo de información pueden solicitar los usuarios antes de ejecutar el informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 9%

---

# Editar la configuración del informe

Puede editar la configuración de un informe para definir cómo se muestra para otros usuarios o qué tipo de información pueden solicitar los usuarios antes de ejecutar el informe.

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

## Pasos prácticos

1. Comience a crear un informe en la sección **Menú principal** > **Informes** y, a continuación, seleccione el objeto del informe.

   O

   Abra un informe existente y haga clic en **Acciones de informe** > **Editar**.

1. Haga clic en **Configuración de informes** en la esquina superior derecha del Creador de informes.
1. Configure las siguientes opciones de informes:

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
      <td>Especifique una declaración que describa el propósito y los usos del informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ejecutar este informe con los derechos de acceso de</td> 
      <td>Seleccione el usuario cuyos derechos de acceso desee que utilice este informe al mostrarlo a otros usuarios. Para obtener más información sobre cómo ejecutar un informe con los derechos de acceso de otro usuario, consulte el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Ejecutar y enviar un informe con los derechos de acceso de otro usuario</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando el informe se cargue, mostrar</td> 
      <td>Seleccione la pestaña predeterminada que se muestra para todos los usuarios cuando se carga el informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando el informe se carga en un tablero, mostrar ... elementos</td> 
      <td>Especifique el número de elementos que se muestran para todos los usuarios cuando el informe se carga en un tablero. El valor predeterminado es 15 elementos y el número máximo de elementos es 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar la vista Cuadrícula de recursos en la ficha Detalles</td> 
      <td> <p>(Solo informe de usuario) Seleccione esta opción para mostrar la cuadrícula de recursos en la ficha Detalles del informe.</p> <p>Nota: Al aplicar la vista Cuadrícula de recursos a un informe de usuario, el informe solo muestra los proyectos que están en estado actual. Si desea ver proyectos en cualquier otro estado, puede utilizar la ficha Uso del usuario en el área Personas de la barra de navegación global y aplicar allí la vista Cuadrícula de recursos. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar una vista especial en la ficha Detalles</td> 
      <td>(Solo informe de proyecto) Especifique el tipo de vista que verán los usuarios cuando accedan a esta información en la ficha Detalles. Por ejemplo, puede seleccionar una vista Milestone o Gantt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar este informe en una vista Gantt de forma predeterminada</td> 
      <td>(Solo informe de proyecto y solo informe de tarea) Seleccione esta opción para que la vista Gantt se active automáticamente cuando los usuarios vean la ficha Detalles en este informe.<br>Para obtener más información sobre la visualización del diagrama de Gantt en los informes de proyectos y de tareas, consulte la sección "Ver información de tareas en la lista de proyectos Diagrama de Gantt" en el artículo <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Ver información en el diagrama de Gantt </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir cambiar la vista en el informe</td> 
      <td>Seleccione esta opción para permitir que los usuarios cambien la vista al ejecutar el informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir cambiar el grupo en el informe</td> 
      <td>Seleccione esta opción para permitir que los usuarios cambien el grupo al ejecutar el informe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir cambiar el filtro del informe</td> 
      <td>Seleccione esta opción para permitir que los usuarios cambien el filtro al ejecutar el informe.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Mensajes del informe** para configurar cualquier mensaje del informe.\
   Para obtener más información sobre la adición de mensajes a un informe, consulte el artículo [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Haga clic en **Listo,** a continuación, haga clic en **Guardar + Cerrar**.

## Información adicional

Consulte también:

* [Programa básico de creación de informes para la nueva experiencia de Workfront](https://one.workfront.com/s/basic-report-creation-program)
* [Introducción a los informes en Adobe Workfront](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Uso de los informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
