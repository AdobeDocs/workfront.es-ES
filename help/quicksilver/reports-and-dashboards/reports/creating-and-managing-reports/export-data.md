---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exportar datos
description: Puede exportar datos de Adobe Workfront desde listas, informes, paneles y búsquedas.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: ae3fc73e93474c75fd03144b66af23f7142867c0
workflow-type: tm+mt
source-wordcount: '2264'
ht-degree: 82%

---

# Exportación de datos

<!-- Audited: 5/2025 -->

Puede exportar datos de Adobe Workfront desde listas, informes, paneles y búsquedas.

Algunos de los motivos para exportar datos son:

* Desea proporcionar una copia impresa de sus datos a alguien de fuera de Workfront.
* Desea enviar los resultados de un informe como datos adjuntos a un usuario externo.
* Desea crear una copia de seguridad externa de sus datos de Workfront.
* Hay un límite por el que solo se pueden mostrar 2000 resultados en una página dentro de la aplicación web de Workfront. Si el informe produce más de 2000, puede exportar el informe a cualquiera de los formatos disponibles y ver todos los resultados del informe en una sola lista.

Puede exportar un informe manualmente, desde la interfaz de Workfront, o programar el envío de un informe y ese informe se le enviará a usted más adelante. Para obtener más información sobre la programación de envío de informes, consulte [Información general sobre el envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

La información de este artículo no se aplica a las siguientes exportaciones:

* Exportación de información desde informes de gráficos.

  Para obtener más información sobre cómo exportar un informe de gráfico, consulte [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Exportación de información desde un gráfico Gantt.

  Para obtener más información acerca de cómo exportar un gráfico Gantt, consulte [Exportar un gráfico Gantt a PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Exportar información desde el Planificador de recursos.

  Para obtener más información sobre cómo exportar la información desde el Planificador de recursos, consulte “Opción de exportación” en [Información general sobre la navegación del Planificador de recursos](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
    <p>Nuevo:</p>
      <ul>
      <li>Ligero o superior</li>
      </ul>
    <p>Actual:</p>
      <ul>
      <li>Revisión o superior</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a informes, paneles de control y calendarios para exportar informes</p> <p>Acceso de visualización o superior a los objetos que se ven en una lista para exportar la lista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superior a un informe o panel de control para exportar el informe o el panel de control</p> <p>Permisos de visualización o superior a los objetos que se ven en una lista para exportar la lista</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Es imprescindible haber creado ya el informe para poder exportar sus datos.

Para obtener más información sobre la creación de informes, consulte [Crear un informe personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) o [Crear una copia de un informe](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Formatos y límites de exportación

### Formatos de exportación {#export-formats}

La información se puede exportar en los siguientes formatos:

* PDF (horizontal o vertical)
* Excel
* Excel (.xlsx)
* Delimitado por tabulaciones

>[!NOTE]
>
>Los paneles se pueden imprimir o exportar solo a un archivo PDF.

### Límites de exportación {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Existen varias limitaciones en la forma en que se muestran los informes en Workfront, así como en la forma en que se exportan a través de una exportación manual, un informe enviado o a través de la API.

* **50 000 celdas:** número máximo de celdas permitidas en la exportación de un informe para archivos de Excel.
* **50.000 filas:** Número de filas de datos permitidas en una exportación de informe para archivos PDF y delimitados por tabuladores.

   * Para archivos de Excel, este límite es de **65,000 filas**.
   * Para archivos de Excel(.xlsx), este límite es de **100.000 filas**.
   * Estos límites excluyen los encabezados de columna y las filas de las agrupaciones del informe. Por ejemplo, si tiene 6 agrupaciones en un informe y 50 000 filas de datos, el archivo exportado tendrá 50 000 filas.

  >[!IMPORTANT]
  >
  >La exportación de un informe que incluya una referencia de recopilación dentro de una columna puede dar lugar a un error, incluso si el informe se encuentra dentro de los límites de exportación indicados. Si la recopilación a la que se hace referencia es demasiado grande, se agota el tiempo de espera del proceso de exportación y, por lo tanto, se produce un error.
  >
  >Para evitar este error, excluya las columnas que hagan referencia a recopilaciones grandes o reduzca el tamaño de las recopilaciones a las que se hace referencia antes de exportarlas.

  Si el informe tiene más elementos que estos límites, recibirá un error que indica que la exportación no se ha realizado correctamente. Reduzca el número de elementos que ve en la pantalla a un número menor o igual que estos límites para poder exportar los resultados.

  Si el informe tiene más de 50 000/65 000/100 000 filas y desea exportar todos los datos, le sugerimos que utilice filtros o indicadores para obtener cargas de datos más pequeñas y realizar varias exportaciones.

  Para obtener información sobre el uso de filtros, consulte [Información general sobre los filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Para obtener información acerca del uso de las indicaciones, consulte [Añadir una indicación a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Estos límites se aplican a lo siguiente:

   * Exportación manual de un informe.
   * Un informe programado.
   * Una exportación a través de una integración de API.
   * Datos exportados mediante Kick-Start.

     Para obtener más información sobre la exportación de datos mediante Kick-Starts, consulte [Exportar datos de Adobe Workfront a través de Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >Puede exportar 50 000 filas en un archivo de KickStart, aunque solo puede exportar los datos a un archivo con formato de Excel.

   * Exportación de información de utilización para un proyecto.

     Para obtener más información sobre cómo exportar la información de utilización de un proyecto, consulte [Información general sobre el informe de utilización de recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **Tamaño de archivo de 10 MB:** límite de tamaño de archivo para cualquier informe exportado programado para su envío. Si un archivo exportado adjunto a un correo electrónico supera los 5 MB, se enviará por correo electrónico un vínculo donde se pueda descargar el archivo en lugar del informe exportado adjunto.
* **65 530 hipervínculos:** Excel ha impuesto este límite a los documentos que contienen más de 65 530 hipervínculos. Estos documentos no se pueden abrir cuando se exportan manualmente o cuando se envían en un informe enviado. Tenga en cuenta que un documento de Excel puede tener solo 200 filas de datos, pero si hay más de 65 530 vínculos dentro del documento, este no se abrirá. Este límite solo existe en archivos de Excel, no en los demás formatos admitidos.
* **256 columnas**: Excel ha impuesto este límite a los documentos que contienen más de 256 columnas. Estos documentos no se pueden exportar manualmente ni enviar en un informe enviado. Este límite solo existe en archivos de Excel, no en los demás formatos admitidos.

  >[!IMPORTANT]
  >
  >La exportación de un informe que incluya una columna Informes puede provocar un error incluso si el informe se encuentra dentro de los límites de exportación enumerados.
  >
  >Si utiliza la función de exportación para compartir un informe que contenga una columna Informes con otros usuarios, considere la posibilidad de compartir el informe haciéndolo público en su lugar. Para obtener más información sobre cómo hacer público un informe, vea [Compartir un informe en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
  >
  >Si utiliza la función de exportación para evaluar los datos externamente, le recomendamos que utilice Workfront Data Connect. Para obtener más información, consulte [Información general sobre Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

Si intenta exportar datos más allá del límite, es posible que no reciba todos los datos esperados en la exportación. En su lugar, se produce un informe modificado dentro del límite.

Además, se detendrán los informes que tarden más de 60 minutos en ejecutarse.

Si tiene dudas o problemas con respecto a su límite, póngase en contacto con el soporte técnico de Workfront.

## Exportación de datos

### Exportación de datos desde un informe o una lista {#export-data-from-a-report-or-list}

1. Vaya al informe o la lista que desea exportar.
1. Seleccione los elementos que desea exportar. Al seleccionar elementos individuales, se exportan únicamente los elementos seleccionados.

   Por ejemplo, en un proyecto, seleccione las tareas que desea exportar.

   O

   Deje todos los elementos sin seleccionar para exportar la lista completa.

1. Haga clic en **Exportar** y, a continuación, seleccione un formato.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![Export dashboard note](assets/nwe-dashboard-export-note-350x271.png)
   -->

   O

   Haga clic en el icono **Exportar** ![Icono Exportar](assets/export-icon-nwe.png) y, a continuación, seleccione un formato.

   Las opciones disponibles para la exportación de PDF dependen de la configuración Configuración regional de correo electrónico de la configuración de usuario de Workfront:

   * América del Norte - Carta - Horizontal, Carta - Vertical, Otros tamaños

   * Todas las ubicaciones fuera de América del Norte - A4 - Horizontal, A4 - Vertical, Otros tamaños

1. (Condicional) Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el disco duro.
1. Para comprender cómo se muestra la información en el archivo exportado, siga leyendo la sección [Use el documento exportado](#use-the-exported-document) en este artículo.

### Exportar datos desde un panel de control {#export-data-from-a-dashboard}

Puede imprimir la información desde un panel o exportarla como un archivo PDF.

Para obtener más información sobre la exportación de datos desde un panel, consulte [Exportar un panel de control](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Utilizar el documento exportado {#use-the-exported-document}

Las secciones siguientes describen cómo se muestra la información en un archivo exportado:

* [Nombres de archivo](#file-names)
* [Títulos](#titles)
* [Marcas de tiempo](#timestamps)
* [Formato](#formatting)
* [Vínculos](#links)
* [Personalización de marca](#branding)

### Nombres de archivo {#file-names}

Tanto si exporta una lista de objetos como un informe, el archivo exportado tendrá un nombre de archivo y un título. Puede encontrar el archivo exportado en su equipo haciendo referencia al nombre del archivo. El título del informe proporcionará a los usuarios una indicación de lo que representa el archivo exportado cuando lo comparta con ellos.

#### Nombres de archivo de las listas exportadas {#file-names-for-exported-lists}

Al exportar una lista de objetos, el tipo de objeto se muestra en el archivo exportado en el nombre del archivo y en el título de la lista.

Al exportar una lista de tareas o problemas, el **Nombre de archivo** puede ser uno de los siguientes:

* Al exportar listas de tareas y problemas en un proyecto:

   * *The_project_name_Exported_Tasks*(*en los formatos PDF, Excel, Excel (.xlsx) o delimitados por tabuladores)*
   * *The_project_name_Exported_Issues*(*en los formatos PDF, Excel, Excel (.xlsx) o delimitados por tabuladores)*

* Al exportar listas de tareas y problemas en una tarea (subtareas):

   * **The_project_name_the_task_name_Exported_Tasks**(*en los formatos PDF, Excel, Excel (.xlsx) o delimitados por tabuladores)*
   * **The_project_name_the_task_name_Exported_Issues**(*en los formatos PDF, Excel, Excel (.xlsx) o delimitados por tabuladores)*

Al exportar una lista de cualquier otro objeto de un proyecto a un archivo PDF, el nombre de archivo del documento exportado indica el tipo de objetos que ha exportado.\
Por ejemplo, el nombre de archivo puede ser:

* *Exported_Users* al exportar la pestaña Personas del proyecto (*en los formatos PDF, Excel, Excel (.xlsx) o delimitados por tabuladores)*
* *Exported_Risks* al exportar una lista de riesgos en el proyecto (*en los formatos PDF, Excel, Excel (.xlsx) o delimitados por tabuladores)*

#### Nombres de archivo de los informes exportados {#file-names-for-exported-reports}

Al exportar un informe, el nombre de archivo del informe exportado es:

*The_report_name*(*en los formatos PDF, Excel, Excel (.xlsx) o delimitado por tabuladores)*

### Títulos {#titles}

Al exportar una lista de objetos, solo el archivo con formato PDF tendrá un título. Si exporta una lista o un informe a formatos Excel, Excel (.xlsx) o delimitado por tabuladores, el archivo no tendrá título.

#### Títulos de las listas exportadas {#titles-for-exported-lists}

Al exportar listas de tareas y problemas de un proyecto a un archivo PDF, el título del documento exportado es uno de los siguientes:

* *Nombre de proyecto - Tareas exportadas*
* *Nombre de proyecto - Problemas exportados*

Al exportar listas de tareas y problemas de una tarea a un archivo PDF, el mosaico del documento exportado es uno de los siguientes:

* *Nombre de proyecto - Nombre de tarea - Tareas exportadas*
* *Nombre de proyecto - Nombre de tarea - Problemas exportados*

Cuando se exporta una lista de cualquier otro objeto de un proyecto a un archivo PDF, el título del documento exportado indica el tipo de objetos exportados.\
Por ejemplo, el título puede ser:

* *Usuarios exportados* al exportar la pestaña Personas del proyecto.
* *Riesgos exportados* al exportar una lista de riesgos en el proyecto.

#### Títulos de los informes exportados {#titles-for-exported-reports}

Un informe que se exporte a un archivo de PDF tendrá un título.

Si el informe se exporta a los formatos Excel, Excel (.xlsx) o delimitado por tabuladores, el informe exportado no tendrá título. El título del archivo exportado es el nombre del informe tal como aparece en la aplicación web de Workfront.

Si el informe tiene una descripción, se incluye en el archivo exportado.

### Marcas de tiempo {#timestamps}

Se muestra una marca de tiempo en el documento exportado desde el contexto del usuario que exportó el elemento.

La marca de tiempo incluye:

* Fecha
* Hora
* Huso horario en el que se exportó el elemento

Según el tipo de documento que exporte, las marcas de tiempo se mostrarán en varias ubicaciones:

* **PDF:** las marcas de tiempo se muestran en el pie de página de cada página y en el nombre de archivo.
* **Excel:** las marcas de tiempo se muestran en el nombre de archivo.

### Formato {#formatting}

Al exportar un proyecto a PDF, las subtareas se muestran con sangría respecto a sus tareas principales. Las listas exportadas no contraen ninguna tarea principal.

Siempre recibe la pestaña predeterminada de un informe cuando se envía un informe o cuando se programa su envío, a menos que el informe tenga una vista especial.

Si el informe tiene un formato especial en la aplicación web, el informe debe entregarse con el formato especial cuando se entreguen las pestañas Details y Matrix, solo para archivos de PDF y Excel.

>[!NOTE]
>
>Si los datos que está exportando contienen columnas compartidas y los exporta a un formato de Excel o Delimitado por tabulaciones, estas columnas se separarán en el archivo exportado.

Para obtener más información sobre cómo personalizar el formato de un informe, consulte [Usar formato condicional en vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Vínculos {#links}

Los vínculos pueden dirigir a cualquier objeto de Workfront que admita la vinculación. Al exportar una lista en Workfront a PDF, los vínculos admitidos que existan en el documento original permanecerán activos en el documento exportado.

>[!TIP]
>
>Si la línea `valueformat=HTML` aparece en modo de texto para una columna de campo personalizado y los valores del vínculo no se muestran en un archivo PDF exportado, debe introducir líneas de código adicionales en la columna en modo de texto.
>
>Por ejemplo, si tiene un campo personalizado llamado Abrir proyectos del primer trimestre que contiene vínculos, debe añadir el siguiente código:
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Al exportar a un formato de Excel, en el archivo exportado solo se incluyen los vínculos a objetos dentro de Workfront y solo se admiten en lugares en los que se puede seleccionar permitir vínculos en documentos de Excel exportados, como envíos de informes.

## Personalización de marca {#branding}

>[!IMPORTANT]
>
>La personalización de marca solo se aplica a las organizaciones que aún no se han incorporado a Adobe Experience Cloud.
>
>Si su organización ya se ha incorporado a Adobe Experience Cloud, la personalización de marca no está disponible.

Si el administrador de Workfront ha añadido una personalización de la marca a la instancia de Workfront para la barra de navegación global, los archivos PDF exportados también incluyen su logotipo personalizado.

Los datos exportados en cualquier otro formato no se pueden personalizar con el logotipo.

Para obtener más información sobre la personalización de marca de la instancia de Workfront y la barra de navegación global, consulte [Marcar instancia de Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
