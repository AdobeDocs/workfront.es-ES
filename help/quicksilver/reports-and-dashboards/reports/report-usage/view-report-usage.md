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
source-wordcount: '997'
ht-degree: 0%

---

# Ver uso del informe

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Para comprender la amplitud con la que se utilizan los informes en su sistema, puede ver la siguiente información en una lista de informes:

* Últimos 10 usuarios que vieron el informe
* Ver recuento dentro de un lapso de tiempo especificado

   >[!NOTE]
   >
   >Adobe Workfront cuenta una vista por usuario y día. Si accede al mismo informe varias veces al día, Workfront lo contará como una vista para ese informe. Si otro usuario accede al mismo informe en el mismo día, Workfront lo considera una nueva vista para el segundo usuario.

* Fecha de última visualización
* Última visualización por usuario
* Una lista de tableros que contienen el informe\
   Para obtener más información sobre cómo mostrar el nombre de los tableros en los que se pueden agregar informes en una lista de informes, consulte el artículo [Cómo organizar informes en un tablero](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

Puede crear una vista para una lista de informes en la que pueda mostrar esta información.\
Puede filtrar una lista de informes por algunos de estos campos.\
Para obtener más información sobre los campos por los que puede filtrar un informe, consulte el artículo [Filtrado de una lista de informes por información de uso](#filter-a-report-list-by-usage-information).

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

## Mostrar la información de uso del informe en la Vista de una lista de informes

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Informes**.

1. En la lista de informes, haga clic en el botón **Ver** menú desplegable.
1. (Opcional) Seleccione el **Uso del informe** para mostrar la información de uso de informes más común.\
   O

1. Haga clic en **Nueva vista** para crear una vista personalizada.
1. Haga clic en **Agregar columna**.
1. Comience a escribir cualquiera de los campos siguientes y selecciónelos cuando aparezcan en la lista debajo de la **Informe** para agregarlos a una nueva columna:

   * **Últimos 10 usuarios**: Muestra los nombres de los últimos 10 usuarios que vieron el informe.
   * **Vistas**: Muestra el número de vistas dentro de cualquiera de los siguientes lapsos de tiempo:

      * **Este mes, trimestre, año**
      * **Último mes, trimestre, año**
      * **Todas las vistas**: Muestra un recuento general de todas las vistas del informe
   * **Última visualización por**: Muestra información sobre el usuario que vio el último informe
   * **Última fecha de visualización**: Muestra la última fecha en la que se visualizó el informe


1. Haga clic en **Guardar vista**.\
   La información de uso del informe se muestra en las columnas que agregó a la vista.\
   También puede crear un informe para el objeto de informe y utilizar esta vista en el informe.\
   Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Debe tener acceso de edición a los informes en el nivel de acceso para crear un informe.\
   Para obtener más información sobre el acceso a los informes, consulte el artículo [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrado de una lista de informes por información de uso {#filter-a-report-list-by-usage-information}

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Informes**.
1. En la lista de informes, haga clic en el botón **Filtro** menú desplegable.
1. Haga clic en **Nuevo filtro** y haga clic en **Agregar una regla de filtro**.
1. Comience a escribir cualquiera de los campos siguientes y selecciónelos cuando aparezcan en la lista debajo de la **Informe** para añadirlos como una nueva regla de filtro:

   * **Vistas**: Muestra el número de vistas dentro de cualquiera de los siguientes lapsos de tiempo:

      * **Este mes, trimestre, año**
      * **Último mes, trimestre, año**
      * **Todas las vistas**
   * **Última visualización por**: Muestra información sobre el usuario que vio el último informe
   * **Última fecha de visualización**: Muestra la última fecha en la que se visualizó el informe


1. Seleccione un modificador para el campo y, a continuación, especifique un valor cuando se le solicite.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Haga clic en **Guardar filtro**.\
   Se muestra una lista de informes que cumplen la información de uso definida.\
   También puede crear un informe para el objeto de informe y utilizar este filtro en el informe.\
   Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Debe tener acceso de edición a los informes en el nivel de acceso para crear un informe.\
   Para obtener más información sobre el acceso a los informes, consulte el artículo [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Excepciones al ver la información de uso del informe

>[!IMPORTANT]
>
>La información sobre el uso del informe se ha recopilado desde marzo de 2018. La información anterior a esta fecha no está disponible.

A continuación se indican algunas excepciones que deben tenerse en cuenta al trabajar con información de uso de informes:

* Cada vez que un informe se muestra en un tablero o en una ficha personalizada, se cuenta como una vista. El usuario que muestra ese informe en su tablero se muestra como Última vista de: Asigne un nombre al usuario y la fecha en la que se ha mostrado el tablero se muestre como la fecha de último visitado en.
* Workfront no recopila información de uso para informes integrados.\
   Para obtener más información sobre los informes integrados de Workfront, consulte el artículo [Uso de los informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront no recopila información de uso en informes entregados. Un informe enviado no cuenta como una sola vista.\
   Para obtener más información sobre los informes entregados, consulte el artículo [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Cuando un administrador de sistemas o grupos inicia sesión como otro usuario, las vistas se cuentan para el administrador del sistema o del grupo y se asocian a él.
* Workfront no recopila información de uso para informes por trimestres personalizados. En los campos de uso del informe solo se hace referencia a los trimestres integrados estándar.
* Workfront no recopila información de uso para informes que se comparten y visualizan públicamente. Cuando alguien ve un informe público sin iniciar sesión en Workfront, las vistas del informe no se cuentan.\
   Para obtener más información sobre cómo compartir informes, consulte el artículo [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
