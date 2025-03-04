---
title: Crear registros importando información desde un archivo CSV o de Excel
description: Los registros son instancias individuales de tipos de registros, que son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear registros importando información desde un archivo CSV o de Excel.
hide: true
hidefromtoc: true
source-git-commit: 9f17fcab210768923e866d2f1596f40ddf8a558e
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 14%

---


<!-- add the following in the metadata when live:

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog-->

# Crear registros importando información desde un archivo CSV o de Excel

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Los registros son instancias individuales de tipos de registros, que son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear registros importando información desde un archivo CSV o de Excel.

Para obtener más información sobre cómo crear registros, vea [Crear registros](/help/quicksilver/planning/records/create-records.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td> Estándar
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p> 
   <p>Editar el acceso en Workfront para los tipos de objeto que desea crear (proyectos y portafolios) al conectar los registros a ellos. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Administre los permisos del espacio de trabajo al que desee agregar registros. </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
   <p>Administre permisos a objetos Workfront (portafolios) para agregar objetos secundarios (proyectos).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>Todos los usuarios, incluidos los administradores de Workfront, deben tener asignada una plantilla de diseño que incluya el área de Planning en el menú principal </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones acerca de la importación de tipos de registros mediante un archivo CSV o de Excel

* Los encabezados de las columnas de cada hoja se convierten en los campos asociados a los registros.
* Cada fila de cada hoja se convierte en un registro único asociado.
* Si el archivo de Excel contiene más de una hoja, sólo se importará la información de una hoja seleccionada durante el proceso de importación.
* El archivo no debe superar lo siguiente:
   * 10 000 filas
   * 500 columnas
* El archivo no debe superar los 5 MB.
* No se admiten hojas vacías.
* No se admiten los campos de los siguientes tipos y no se pueden asignar a campos de la hoja de importación:
   * Campos de búsqueda de registros conectados u objetos de Workfront conectados
   * Campos de fórmula
   * Fecha de creación, Creado por
   * Fecha de la última modificación, Última modificación por
   * Personas
* Si se importa un campo de selección múltiple o única y tiene más opciones que un campo similar en Planning, las opciones adicionales se crean durante la importación.

## Creación de registros importando un archivo CSV o de Excel

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee crear los tipos de registro,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo situada a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y, a continuación, selecciónelo cuando se muestre en la lista.
1. Haga clic en la tarjeta del tipo de registro donde desee importar los registros.
1. Haga clic en **Nuevo registro** en la esquina superior derecha de la pantalla.
1. Haga clic en **Cargar desde el archivo** y, a continuación, **Continuar**.
1. Arrastre y suelte un archivo de Excel o CSV guardado anteriormente en el equipo, o haga clic en **Seleccione un archivo CSV o de Excel** para buscar uno.
1. Haz clic en **Vista previa y edita**.
1. (Condicional) Si el archivo importado tiene más de una hoja, seleccione el botón de opción de la hoja que desea importar en el cuadro **Seleccione una hoja para importar** y, a continuación, haga clic en **Siguiente**. De lo contrario, continúe con el siguiente paso.

   ![Seleccione una hoja para importar registros](assets/select-a-sheet-to-import-box.png)
1. En **Asignar los campos de Planning a los encabezados de columna**, seleccione el **campo de Planning** que mejor coincida con la información de cada una de las columnas de la hoja.

   ![Asignar campos de Planning a columnas al importar registros](assets/map-planning-fields-to-columns-when-importing-records.png)

   Cada fila representa un nuevo registro. Solo se muestran los 10 primeros registros en el cuadro Vista previa y edición.

1. (Opcional) Seleccione **Crear opciones que faltan** en la esquina inferior izquierda de la pantalla. Cuando se habilita, se agregan las opciones que faltan en los campos de selección única y múltiple.

   Por ejemplo, si el tipo de registro seleccionado tiene un campo de estado de selección única con las opciones Nuevo, En curso y Cerrado, y un campo de estado importado de un archivo también tiene una opción de estado Retenido, también se agrega la opción de estado Retenido

   <!--when we add connected records and the info icon in the tool changes, also add those items to this step-->

1. Haga clic en **Importar**.

   La siguiente información se importa en Workfront Planning:

   * Nuevos registros que se muestran en la parte inferior de la vista de tabla del tipo de registro seleccionado.
   * Valores de campo nuevos para campos existentes asociados a cada registro.
   * Nuevas opciones de un campo de selección múltiple o única que no existía en Planning.

   Puede empezar a administrar campos y registros en la página de tipos de registros.

   Todas las personas con acceso a Workfront Planning y al espacio de trabajo ahora pueden ver y editar los registros importados y su información.