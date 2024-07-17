---
product-area: reporting
navigation-topic: report-usage
title: Ver uso del informe
description: Ver uso del informe
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 1%

---

# Ver uso del informe

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Para comprender la amplitud con la que se utilizan los informes en el sistema, puede ver la siguiente información en una lista de informes:

* Últimos 10 usuarios que vieron el informe
* Ver recuento en un lapso de tiempo especificado

  >[!NOTE]
  >
  >Adobe Workfront cuenta una vista por usuario y día. Si accede al mismo informe varias veces al día, Workfront lo cuenta como una vista para ese informe. Si otro usuario accede al mismo informe el mismo día, Workfront lo contabiliza como una vista nueva para el segundo usuario.

* Fecha de última visualización
* Última visualización por usuario
* Una lista de paneles que contienen el informe\
  Para obtener más información sobre cómo mostrar el nombre de los tableros en los que se pueden agregar informes en una lista de informes, consulte el artículo [Comprender cómo organizar informes en un tablero](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

Se puede crear una vista para una lista de informes en la que se puede mostrar esta información.\
Puede filtrar una lista de informes por algunos de estos campos.\
Para obtener más información sobre los campos por los que puede filtrar un informe, vea el artículo [Filtrar una lista de informes por información de uso](#filter-a-report-list-by-usage-information).

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
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar la información de uso del informe en la lista Vista de un informe

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront y luego haga clic en **Informes**.

1. En la lista de informes, haga clic en el menú desplegable **Ver**.
1. (Opcional) Seleccione la vista **Uso del informe** para mostrar la información de uso del informe más común.\
   O

1. Haga clic en **Nueva vista** para crear una vista personalizada.
1. Haga clic en **Añadir columna**.
1. Empiece a escribir cualquiera de los siguientes campos y selecciónelos cuando aparezcan en la lista debajo del objeto **Report** para agregarlos a una nueva columna:

   * **Últimos 10 usuarios**: Muestra los nombres de los últimos 10 usuarios que vieron el informe.
   * **Vistas**: muestra el número de vistas en cualquiera de los siguientes lapsos de tiempo:

      * **Este mes, trimestre, año**
      * **Último mes, trimestre, año**
      * **Todas las vistas**: muestra un recuento general de todas las vistas del informe

   * **Última visualización por**: muestra información sobre el usuario que vio el informe por última vez
   * **Fecha de la última visualización**: Muestra la fecha en la que se vio el informe por última vez

1. Pulse **Guardar vista**.\
   La información de uso sobre el informe se muestra en las columnas que agregó a la vista.\
   También puede crear un informe para el objeto de informe y utilizar esta vista en el informe.\
   Para obtener más información sobre cómo generar un informe, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Debe tener acceso de edición a los informes en su nivel de acceso para crear un informe.\
   Para obtener más información acerca del acceso a los informes, vea el artículo [Conceder acceso a informes, paneles y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrado de una lista de informes por información de uso {#filter-a-report-list-by-usage-information}

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront y luego haga clic en **Informes**.
1. En la lista de informes, haga clic en el menú desplegable **Filtro**.
1. Haga clic en **Nuevo filtro** y luego haga clic en **Agregar una regla de filtro**.
1. Empiece a escribir cualquiera de los siguientes campos y selecciónelos cuando aparezcan en la lista debajo del objeto **Report** para agregarlos como una nueva regla de filtro:

   * **Vistas**: muestra el número de vistas en cualquiera de los siguientes lapsos de tiempo:

      * **Este mes, trimestre, año**
      * **Último mes, trimestre, año**
      * **Todas las vistas**

   * **Última visualización por**: muestra información sobre el usuario que vio el informe por última vez
   * **Fecha de la última visualización**: Muestra la fecha en la que se vio el informe por última vez

1. Seleccione un modificador para el campo y, a continuación, especifique un valor cuando se le solicite.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Haga clic en **Guardar filtro**.\
   Muestra una lista de informes que cumplen con la información de uso definida.\
   También puede crear un informe para el objeto de informe y utilizar este filtro en el informe.\
   Para obtener más información sobre cómo generar un informe, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Debe tener acceso de edición a los informes en su nivel de acceso para crear un informe.\
   Para obtener más información acerca del acceso a los informes, vea el artículo [Conceder acceso a informes, paneles y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Excepciones al ver la información de uso del informe

>[!IMPORTANT]
>
>La información de uso del informe se ha recopilado desde marzo de 2018. No se encuentra disponible ninguna información anterior a esta fecha.

A continuación se indican algunas excepciones que deben tenerse en cuenta a la hora de trabajar con información de uso de informes:

* Cada vez que se muestra un informe en un tablero o en una pestaña personalizada, se cuenta como una vista. El usuario que muestra ese informe en su panel se muestra como el usuario Última vista por: Nombre y la fecha en la que se mostró el panel se muestra como la fecha Última visualización Activada.
* Workfront no recopila información de uso para informes integrados.\
  Para obtener más información acerca de los informes integrados de Workfront, consulte el artículo [Usar informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront no recopila información de uso sobre los informes enviados. Un informe enviado no cuenta como una vista.\
  Para obtener más información sobre los informes enviados, consulte el artículo [Resumen de entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Cuando un administrador de sistema o de grupo inicia sesión como otro usuario, las vistas se contabilizan y se asocian al administrador del sistema o del grupo.
* Workfront no recopila información de uso de los informes por trimestres personalizados. En los campos de uso del informe solo se hace referencia a los trimestres integrados estándar.
* Workfront no recopila información de uso de los informes compartidos y vistos públicamente. Cuando alguien ve un informe público sin iniciar sesión en Workfront, no se cuentan las vistas del informe.\
  Para obtener más información sobre cómo compartir informes, consulte el artículo [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
