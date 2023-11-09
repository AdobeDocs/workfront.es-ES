---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exportación de datos
description: Obtenga información sobre cómo exportar datos de informes
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '2177'
ht-degree: 0%

---

# Exportación de datos

Puede exportar datos de Adobe Workfront desde varias listas, informes, paneles y búsquedas.
La información de este artículo no se aplica a las siguientes exportaciones:

* Exportación de información desde informes de gráficos.

  Para obtener más información sobre cómo exportar un informe de gráfico, consulte [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Exportación de información desde el diagrama de Gantt.

  Para obtener más información sobre cómo exportar el gráfico Gantt, consulte [Exportar el gráfico Gantt a PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Exportar información desde el Planificador de recursos.

  Para obtener más información sobre cómo exportar la información desde el Planificador de recursos, consulte &quot;Opción de exportación&quot; en [Resumen de navegación del Planificador de recursos](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Algunos de los motivos para exportar datos son:

* Desea proporcionar una copia impresa de sus datos a alguien fuera de Workfront.
* Desea enviar los resultados de un informe como datos adjuntos a un usuario externo.
* Desea crear una copia de seguridad externa de los datos de Workfront.
* Hay un límite para mostrar solo 2000 resultados en una página dentro de la aplicación web de Workfront. Si el informe produce más de 2000, puede exportarlo a cualquiera de los formatos mencionados a continuación y obtener todos los resultados del informe en una sola lista.

Puede exportar un informe manualmente desde la interfaz de Workfront o programar una entrega para un informe que se le enviará más adelante. Para obtener más información sobre la programación de informes enviados, consulte [Resumen de entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización o superior a informes, tableros y calendarios para exportar informes</p> <p>Permite ver o acceder a los objetos que se visualizan en una lista para exportar la lista</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o aumentar los permisos de un informe o panel para exportar el informe o el panel</p> <p>Ver o permisos superiores a los objetos que se ven en una lista para exportar la lista</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requisitos previos

Debe crearse el informe antes de poder exportar sus datos.

Para obtener más información sobre la creación de informes, consulte [Creación de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Exportar formatos y límites

* [Formatos de exportación](#export-formats)
* [Límites de exportación](#export-limits)

### Formatos de exportación {#export-formats}

La información se puede exportar en los siguientes formatos:

* PDF (carta horizontal o vertical, legal, contable y A4)
* Excel (.xls)
* Excel (.xlsx)
* Delimitado por tabulaciones

>[!NOTE]
>
>Los paneles se pueden imprimir o exportar únicamente a un archivo .pdf.

### Límites de exportación {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Existen varias limitaciones en la forma en que se muestran los informes en Workfront, así como en la forma en que se exportan a través de una exportación manual, un informe enviado o a través de la API.

* **50 000 filas:** Número de filas de datos permitidas en una exportación de informe para archivos .pdf y delimitados por tabuladores.

   * Para archivos .xls de Excel, este límite es **65 000 filas**.
   * Para archivos .xlsx de Excel, este límite es **100 000 filas**.
   * Estos límites excluyen los encabezados de columna y las filas de las agrupaciones del informe. Por ejemplo, si tiene 6 agrupaciones en un informe y 50 000 filas o datos, el archivo exportado tendrá 50 000 filas.

  >[!IMPORTANT]
  >
  >La exportación de un informe que incluya una referencia de recopilación dentro de una columna puede dar lugar a un error, incluso si el informe se encuentra dentro de los límites de exportación enumerados. Si la colección a la que se hace referencia es demasiado grande, se agota el tiempo de espera del proceso de exportación y, por lo tanto, se produce un error.
  >
  >Para evitar este error, excluya las columnas que hagan referencia a colecciones grandes o reduzca el tamaño de las colecciones a las que se hace referencia antes de exportarlas.
  >

  Si el informe tiene más elementos que estos límites, recibirá un error que indica que la exportación no se ha realizado correctamente. Reduzca el número de elementos que ve en la pantalla a un número inferior o igual a estos límites para poder exportar los resultados.

  Si el informe tiene más de 50 000/ 65 000/ 100 000 filas y desea exportar todos los datos, le sugerimos que utilice filtros o indicadores para obtener cargas de datos más pequeñas y realizar varias exportaciones.

  Para obtener información sobre el uso de filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Para obtener información sobre el uso de indicadores, consulte [Agregar una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Estos límites se aplican a:

   * Exportación manual de un informe.
   * Un informe programado.
   * Una exportación a través de una integración de API.
   * Datos exportados mediante un KickStart.

     Para obtener más información sobre la exportación de datos mediante kick-starts, consulte [Exportación de datos de Adobe Workfront mediante Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)

     >[!NOTE]
     >
     >Puede exportar 50 000 filas en un archivo de KickStart, aunque solo puede exportar los datos a un archivo con formato de Excel. 

   * Exportación de información de utilización para un proyecto.

     Para obtener más información sobre cómo exportar la información de utilización de un proyecto, consulte [Descripción general del informe Utilización de los recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **Tamaño de archivo de 10 MB:** Límite de tamaño de archivo para cualquier informe exportado programado para su envío. Si un archivo exportado adjunto a un correo electrónico supera los 5 MB, se enviará por correo electrónico un vínculo donde se pueda descargar el archivo en lugar del informe exportado adjunto.
* **65.530 hipervínculos:** Se trata de un límite impuesto por Excel a los documentos que contienen más de 65.530 hipervínculos. Estos documentos no se pueden abrir cuando se exportan manualmente o cuando se envían en un informe enviado. Tenga en cuenta que un documento de Excel puede tener sólo 200 filas de datos, pero si hay más de 65.530 vínculos dentro del documento, éste no se abrirá. Este límite solo existe en archivos de Excel, no en los demás formatos admitidos. 
* **256 columnas**: Se trata de un límite impuesto por Excel a los documentos que contienen más de 256 columnas. Estos documentos no se pueden exportar manualmente ni enviar en un informe enviado. Este límite solo existe en archivos de Excel, no en los demás formatos admitidos.

Si intenta exportar datos más allá del límite, es posible que no reciba todos los datos esperados en la exportación. En su lugar, se produce un informe modificado dentro del límite.

Además, se detendrán los informes que tarden más de 60 minutos en ejecutarse.

Si tiene dudas o problemas con respecto a su límite, póngase en contacto con el soporte técnico de Workfront.

## Exportación de datos

* [Exportación de datos desde un informe o una lista](#export-data-from-a-report-or-list)
* [Exportación de datos desde un tablero](#export-data-from-a-dashboard)

### Exportación de datos desde un informe o una lista {#export-data-from-a-report-or-list}

1. Vaya al informe o la lista que desee exportar.
1. Seleccione los elementos que desea exportar. (Al seleccionar elementos individuales, sólo se exportan los elementos seleccionados.)

   Por ejemplo, en un proyecto, seleccione las tareas que desee exportar.

   O

   Deje todos los elementos sin seleccionar para exportar la lista completa.

1. Clic **Exportar**, luego seleccione un formato.

   >[!NOTE]
   >
   Para exportar un informe de panel, debe tener una licencia de planificación.\
   ![](assets/nwe-dashboard-export-note-350x271.png)

   O

   Haga clic en **Exportar** icono ![](assets/export-icon-nwe.png), luego seleccione un formato.

   Las opciones disponibles para la exportación de PDF dependen de la configuración regional de la configuración de usuario de Workfront:

   * Norteamérica: carta (predeterminada), legal, contable, A4

     <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * Todas las ubicaciones fuera de Norteamérica: A3, A4 (predeterminado), carta, legal, libro mayor

     <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. (Condicional) Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el disco duro.
1. Continuar con [Utilizar el documento exportado](#use-the-exported-document).

### Exportación de datos desde un tablero {#export-data-from-a-dashboard}

Puede imprimir la información desde un panel o exportarla como un archivo .pdf.

Para obtener más información sobre la exportación de datos desde un panel, consulte [Exportar un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Utilizar el documento exportado {#use-the-exported-document}

* [Nombres de archivo](#file-names)
* [Títulos](#titles)
* [Marcas de hora](#timestamps)
* [Formato](#formatting)
* [Vínculos](#links)
* [Personalización de marca](#branding)

### Nombres de archivo {#file-names}

Tanto si exporta una lista de objetos como un informe, el archivo exportado tendrá un nombre de archivo y un título. Puede encontrar el archivo exportado en el equipo haciendo referencia al nombre del archivo. El título del informe proporcionará a los usuarios una indicación de lo que representa el archivo exportado cuando lo comparta con ellos.

* [Nombres de archivo para listas exportadas](#file-names-for-exported-lists)
* [Nombres de archivo para informes exportados](#file-names-for-exported-reports)

#### Nombres de archivo para listas exportadas {#file-names-for-exported-lists}

Al exportar una lista de objetos, el tipo de objeto se muestra en el archivo exportado en el nombre del archivo y en el título de la lista.

Cuando exporta una lista de tareas o problemas, la variable **Nombre de archivo** puede ser uno de los siguientes:

* Al exportar listas de tareas y problemas en un proyecto:

   * *Tareas_exportadas_nombre_proyecto*(*en formato de PDF, Excel, Excel (.xlsx) o delimitado por tabuladores)*
   * *The_project_name_Exported_Issues*(*en formato de PDF, Excel, Excel (.xlsx) o delimitado por tabuladores)*

* Al exportar Listas de tareas y problemas en una tarea (subtareas):

   * **The_project_name_the_task_name_Exported_Tasks**(*en formato de PDF, Excel, Excel (.xlsx) o delimitado por tabuladores)*
   * **The_project_name_the_task_name_Exported_Issues**(*en formato de PDF, Excel, Excel (.xlsx) o delimitado por tabuladores)*

Cuando se exporta una lista de cualquier otro objeto de un proyecto a un fichero de PDF, el nombre del fichero del documento exportado indica el tipo de objetos exportados.\
Por ejemplo, el nombre de archivo puede ser:

* *Exported_Users*, al exportar la pestaña Personas en el proyecto(*en formato de PDF, Excel, Excel (.xlsx) o delimitado por tabuladores)*
* *Riesgos_exportados*, al exportar una lista de riesgos en el proyecto *en formato de PDF, Excel, Excel (.xlsx) o delimitado por tabuladores)*

#### Nombres de archivo para informes exportados {#file-names-for-exported-reports}

Al exportar un informe, el nombre de archivo del informe exportado es:

*The_report_name*(*en formato de PDF, Excel, Excel (.xlsx) o delimitado por tabuladores)*

### Títulos {#titles}

Al exportar una lista de objetos, sólo el archivo con formato de PDF tendrá título. Si exporta una lista o un informe a formatos de Excel, Excel (.xlsx) o delimitados por tabuladores, el archivo no tendrá título.

* [Títulos para listas exportadas](#titles-for-exported-lists)
* [Títulos de los informes exportados](#titles-for-exported-reports)

#### Títulos para listas exportadas {#titles-for-exported-lists}

Cuando exporta Listas de tareas y problemas de un proyecto a un archivo de PDF, el título del documento exportado es uno de los siguientes:

* *Nombre del proyecto - Tareas exportadas*
* *Nombre del proyecto - Problemas exportados*

Cuando exporta listas de tareas y problemas de una tarea a un archivo de PDF, el mosaico del documento exportado es uno de los siguientes:

* *Nombre del proyecto - Nombre de tarea - Tareas exportadas*
* *Nombre de proyecto - Nombre de tarea - Problemas exportados*

Cuando se exporta una lista de cualquier otro objeto de un proyecto a un fichero de PDF, el título del documento exportado indica el tipo de objetos exportados.\
Por ejemplo, el título puede ser:

* *Usuarios exportados*, al exportar la pestaña Personas en el proyecto.
* *Riesgos exportados*, al exportar una lista de riesgos en el proyecto.

#### Títulos de los informes exportados {#titles-for-exported-reports}

Un informe que se exporta a un archivo de PDF tendrá un título.

Si el informe se exporta a formatos de Excel, Excel (.xlsx) o delimitado por tabuladores, el informe exportado no tendrá título. El título del archivo exportado es el nombre del informe tal como aparece en la aplicación web de Workfront.

Si el informe tiene una descripción, se incluirá en el archivo exportado.

### Marcas de hora {#timestamps}

Se muestra una marca de tiempo en el documento exportado desde el contexto del usuario que exportó el elemento.

La marca de tiempo incluye:

* Fecha
* Hora
* Zona horaria en la que se exportó el elemento

Según el tipo de documento que exporte, las marcas de tiempo se mostrarán en varias ubicaciones:

* **PDF:** Las marcas de tiempo se muestran al pie de cada página y en el nombre del archivo.
* **Excel:** Las marcas de tiempo se muestran en el nombre del archivo.

### Formato {#formatting}

Al exportar un proyecto a .pdf, las subtareas se muestran con sangría respecto a sus tareas principales. Las listas exportadas no contraen ninguna tarea principal.

Siempre recibe la pestaña predeterminada de un informe cuando se envía un informe o cuando se programa una entrega, a menos que el informe tenga una vista especial.

Si el informe tiene un formato especial en la aplicación web, el informe debe entregarse con el formato especial cuando las pestañas Detalles y Matriz solo se entregan para archivos .pdf y Excel.

>[!NOTE]
>
Si los datos que está exportando contienen columnas compartidas y los exporta a un formato de Excel o Delimitado por tabuladores, estas columnas se separarán en el archivo exportado.

Para obtener más información sobre cómo personalizar el formato en un informe, consulte [Uso de formato condicional en vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Vínculos {#links}

Los vínculos pueden señalar a cualquier objeto de Workfront que admita la vinculación. Al exportar una lista en Workfront a .pdf, los vínculos admitidos que existan en el documento original permanecerán activos en el documento exportado.

>[!TIP]
>
>Si la línea `valueformat=HTML` aparece en modo texto para una columna de campo personalizado y los valores del vínculo no se muestran en un archivo .pdf exportado. debe introducir líneas de código adicionales en la columna en modo texto.
>
>Por ejemplo, si tiene un campo personalizado llamado Abrir proyectos del primer trimestre que contiene vínculos, debe agregar el siguiente código:
>
>```
>link.url=customDataLabelsAsString(Open Q1 Projects)
>linkedname=direct
>```

Al exportar a un formato de Excel, solo se incluyen en el archivo exportado los vínculos a objetos dentro de Workfront y solo se admiten en lugares en los que se puede seleccionar permitir vínculos en documentos de Excel exportados, como envíos de informes.

## Personalización de marca {#branding}

Si el administrador de Workfront ha agregado personalización de marca a la instancia de Workfront para la barra de navegación global, los archivos .pdf exportados también incluyen el logotipo personalizado.

Los datos exportados en cualquier otro formato no se pueden personalizar con el logotipo.

Para obtener más información sobre la personalización de la marca de la instancia de Workfront y la barra de navegación global, consulte [Marca su instancia de Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
