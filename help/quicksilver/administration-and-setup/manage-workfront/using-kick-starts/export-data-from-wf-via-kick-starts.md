---
user-type: administrator
product-area: system-administration
keywords: inicio rápido,inicio inicial,inicio rápido,inicio inicial
navigation-topic: use-kick-starts
title: Exportar datos de Adobe Workfront mediante Kick-Starts
description: Como administrador de Adobe Workfront, puede utilizar el exportador de datos Kick-Starts para exportar datos desde Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 9%

---

# Exportar datos de Adobe Workfront mediante Kick-Starts

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador de Adobe Workfront, puede utilizar el exportador de datos Kick-Starts para exportar datos desde Workfront. Puede utilizarlo en otras aplicaciones después de exportarlo.

La exportación de datos a través de Kick-Starts también es útil para comprender qué campos están asociados a cada objeto, cómo se codifican estos campos y cómo se da formato a los valores de estos campos en la base de datos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ventajas y desventajas de utilizar los primeros pasos para exportar datos

Existen dos maneras de exportar datos dentro de Workfront:

* Exportación de datos de un informe o una lista

   Para obtener más información sobre la exportación de datos desde un informe o una lista, consulte [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Exportación de datos mediante inicios

La tabla siguiente muestra las ventajas y desventajas de cada método:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>Los datos exportados incluyen valores de objeto y campo</p> </th> 
   <th> <p>Capacidad de exportar datos en varios tipos de objetos simultáneamente</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exportación de datos desde una vista de lista</strong> </p> <p>Para obtener más información sobre cómo exportar datos de una lista, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar datos</a></p> </td> 
   <td> <p>Sí</p> <p>Se exportan los campos nativos de Workfront y los campos personalizados asociados con los objetos.</p> </td> 
   <td> <p>No</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exportación de datos mediante Kick-Starts</strong> </p> </td> 
   <td> <p>Sí (limitado)</p> <p>La mayoría de los campos nativos de Workfront asociados a objetos se exportan, pero algunos no. Por ejemplo, no se pueden exportar los campos Programación, Propietario del proyecto o Patrocinador del proyecto a través de una exportación inicial del proyecto.</p> <p>En un proyecto que tiene un formulario personalizado adjunto, los datos introducidos en los campos del formulario no se exportan.</p> <p>Sin embargo, puede exportar un formulario personalizado. El archivo resultante enumera los campos configurados en el formulario, como los cuadros de texto y los botones de opción.</p> </td> 
   <td> <p>Sí</p> <p>El uso de Kick-Starts para exportar datos de Workfront permite exportar datos relacionados con varios tipos de objetos en una sola exportación. Por ejemplo, puede incluir tareas, problemas y proyectos en una sola exportación.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Límites de exportación

Las siguientes limitaciones existen al exportar datos mediante el inicio (los datos se exportan en formato de archivo de Excel):

* **50 000 filas:** Número de filas permitidas en el archivo.
* **65.530 hipervínculos:** Este es un límite impuesto por Excel a los documentos que contienen más de 65.530 hipervínculos. Estos documentos no se pueden abrir después de exportarlos. Tenga en cuenta que un documento de Excel puede tener solo 200 filas de datos, pero si hay más de 65.530 vínculos dentro del documento, el documento no se abre.

## Exportación de datos mediante el inicio

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Comienzo de Kick,** a continuación, haga clic en **Exportar datos.**

1. Seleccione el objeto que desea exportar.
1. Haga clic en **Más opciones** para ver la lista completa de objetos.

   Todos los objetos enumerados aquí se pueden utilizar para importar también datos en Workfront.

   La única excepción es la **Niveles de acceso** objeto. La hoja de datos Niveles de acceso que se incluye en una exportación solo se proporciona con fines de referencia. Permite asignar un nivel de acceso a una nueva cuenta de usuario por ID.

   Para obtener más información sobre la importación de datos en Workfront mediante inicios, consulte [Importar datos en Adobe Workfront mediante una plantilla de inicio rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). A continuación se muestra una lista de todos los objetos que se pueden exportar mediante el inicio:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Objeto</p> </th> 
      <th> <p>Hojas exportadas del archivo Excel</p> </th> 
      <th> <p>Formato de exportación</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">Nivel de acceso</td> 
      <td scope="col" valign="top">Nivel de acceso<br>Preferencias</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Asignación</td> 
      <td scope="col" valign="top">Asignación<br>Preferencias</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Compañía</td> 
      <td scope="col" valign="top"> Empresa<br>Preferencias </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Plantilla de mensaje de correo electrónico</td> 
      <td scope="col" valign="top"> Plantilla de correo electrónico<br>Preferencias </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Gasto</td> 
      <td valign="top"> Gastos<br>Preferencias </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Página externa</td> 
      <td valign="top"> Página externa<br>Preferencias </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filtro</td> 
      <td valign="top"> Filtro<br>Preferencias </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Grupo</td> 
      <td valign="top"> Grupo<br>Preferencias  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Agrupación</td> 
      <td valign="top"> Agrupación<br>Preferencias </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Hora</td> 
      <td valign="top"> Hora<br>Preferencias </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Problema</td> 
      <td valign="top"> Problema<br>Preferencias </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Función</td> 
      <td valign="top"> Función del trabajo<br>Preferencias </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Ruta de hitos</td> 
      <td valign="top"> Milestone<br>Ruta de Milestone<br>Preferencias </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Nota</td> 
      <td valign="top"> Nota<br>Preferencias </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Portafolio</td> 
      <td valign="top"> Portfolio<br>Preferencias  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Proyecto</td> 
      <td valign="top"> Cola<br>Proyecto<br>Regla de enrutamiento<br>Tema de cola<br>Preferencias </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Estimación de recursos</td> 
      <td valign="top"> Estimación de recursos<br>Preferencias </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Conjunto de recursos</td> 
      <td valign="top"> Grupo de recursos<br>Preferencias </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Riesgo</td> 
      <td valign="top"> Riesgo<br>Preferencias  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Tipo de riesgo</td> 
      <td valign="top"> Tipo de riesgo<br>Preferencias  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tarjeta de puntuación</td> 
      <td valign="top">Preguntas sobre el informe de valoración<br>Opción informe de valoración<br>Informe de valoración<br>Preferencias </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tarea</td> 
      <td valign="top"> Tarea<br>Preferencias </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Plantilla</td> 
      <td valign="top"> Cola<br>Plantilla<br>Regla de enrutamiento<br>Tema de cola<br>Preferencias </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Asignación de plantilla</td> 
      <td valign="top"> Asignación de plantilla<br>Preferencias </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tarea de plantilla</td> 
      <td valign="top"> Tarea de plantilla<br>Preferencias </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Hoja de horas</td> 
      <td valign="top"> Perfil de hoja de horas<br>Hoja de horas<br>Preferencias </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Vista </td> 
      <td valign="top"> Ver<br>Preferencias  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Descargar.**

   El archivo inicial exportado se descarga en el equipo como archivo de Excel o como . archivo zip que contiene varios archivos de propiedades y Excel. Cada archivo de Excel es una colección de hojas, cada una de las cuales representa un campo asociado al objeto seleccionado. Hay un **Propiedades** hoja asociada a cada exportación.

   La variable **Panel** y **Informe** permite seleccionar tableros e informes específicos para incluirlos en la descarga. Solo puede exportar los tableros que se comparten en todo el sistema.

   No se pueden exportar informes de matriz. Para obtener más información sobre los informes de matriz, consulte [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Puede seleccionar hasta 100 paneles y 100 informes en una sola exportación.

   ![](assets/kickstart-export-350x381.png)

   Puede exportar varios objetos al mismo tiempo.

   De forma predeterminada, los siguientes objetos se muestran en la sección **Qué incluir** (antes de hacer clic en **Más opciones**):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objeto</strong> </p> </th> 
      <th> <p><strong>Hojas exportadas del archivo Excel</strong> </p> </th> 
      <th> <p> <strong>Formato de exportación</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Panel</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parámetro<br>Opción de parámetro<br>Grupo de parámetros<br>Parámetro de categoría<br>Categoría<br>Informe<br>Sección de pestañas del portal<br>Panel<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Informe</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parámetro<br>Opción de parámetro<br>Grupo de parámetros<br>Parámetro de categoría<br>Categoría<br>Informe<br>Preferencias</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Ruta de aprobación</p> </td> 
      <td scope="col" valign="top"> <p>Aprobador de pasos<br>Paso de aprobación<br>Aprobación<br>Proceso de aprobación<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Datos personalizados</p> </td> 
      <td scope="col" valign="top"> <p>Parámetro<br>Opción de parámetro<br>Grupo de parámetros<br>Parámetro de categoría<br>Categoría<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Tipo de gasto</p> </td> 
      <td valign="top"> <p>Tipo de gasto<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Tipo de hora</p> </td> 
      <td valign="top"> <p>Tipo de hora<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Equipo</p> </td> 
      <td valign="top"> Miembro del equipo<br>Equipo<br>Preferencias </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Usuario</p> </td> 
      <td valign="top"> <p>Usuario<br>Preferencias</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong></strong> </p> </th> 
      <th> <p><strong>Hojas exportadas del archivo Excel</strong> </p> </th> 
      <th> <p> <strong>Formato de exportación</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Panel</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parámetro<br>Opción de parámetro<br>Grupo de parámetros<br>Parámetro de categoría<br>Categoría<br>Informe<br>Sección de pestañas del portal<br>Panel<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Informe</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parámetro<br>Opción de parámetro<br>Grupo de parámetros<br>Parámetro de categoría<br>Categoría<br>Informe<br>Preferencias</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Ruta de aprobación</p> </td> 
      <td scope="col" valign="top"> <p>Aprobador de pasos<br>Paso de aprobación<br>Aprobación<br>Proceso de aprobación<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Datos personalizados</p> </td> 
      <td scope="col" valign="top"> <p>Parámetro<br>Opción de parámetro<br>Grupo de parámetros<br>Parámetro de categoría<br>Categoría<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Tipo de gasto</p> </td> 
      <td valign="top"> <p>Tipo de gasto<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Tipo de hora</p> </td> 
      <td valign="top"> <p>Tipo de hora<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Equipo</p> </td> 
      <td valign="top"> Miembro del equipo<br>Equipo<br>Preferencias </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Usuario</p> </td> 
      <td valign="top"> <p>Usuario<br>Preferencias</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Recomendado) Analice los datos exportados para asegurarse de que se exportó toda la información que espera ver.

   Para exportaciones grandes, Workfront trabaja en segundo plano para producir el archivo de Excel y le envía un mensaje de advertencia sobre el retraso. El archivo de inicio se le enviará por correo electrónico cuando termine la descarga.

   ![](assets/large-kick-start-file-warning-350x65.png)
