---
user-type: administrator
product-area: system-administration
keywords: KickStart, KickStart, KickStart, KickStart
navigation-topic: use-kick-starts
title: Exportar datos de Workfront mediante Kick-Starts
description: Como administrador de Adobe Workfront, puede utilizar el exportador de datos de KickStarts para exportar datos de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 8%

---

# Exportación de datos de Workfront mediante Kick-Starts

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador de Adobe Workfront, puede utilizar el exportador de datos de KickStarts para exportar datos de Workfront. Puede usarlo en otras aplicaciones después de exportarlo.

La exportación de datos mediante Kick-Starts también es útil para comprender qué campos están asociados con cada objeto, cómo se codifican estos campos, así como el formato que se da a los valores de estos campos en la base de datos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td>
   <p>Nuevo: estándar</p>
   O
   <p>Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ventajas y desventajas de utilizar kick-starts para exportar datos

Existen dos formas de exportar datos dentro de Workfront:

* Exportación de datos desde un informe o una lista

  Para obtener más información acerca de cómo exportar datos desde un informe o una lista, vea [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Exportación de datos mediante kick-starts

En la tabla siguiente se muestran las ventajas y desventajas de cada método:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>Los datos exportados incluyen valores de objetos y campos</p> </th> 
   <th> <p>Capacidad para exportar datos en torno a varios tipos de objetos simultáneamente</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exportación de datos desde una vista de lista</strong> </p> <p>Para obtener más información acerca de cómo exportar datos de una lista, vea <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar datos</a></p> </td> 
   <td> <p>Sí</p> <p>Se exportan tanto los campos nativos de Workfront como los campos personalizados asociados a los objetos.</p> </td> 
   <td> <p>No</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exportación de datos mediante Kick-Starts</strong> </p> </td> 
   <td> <p>Sí (limitado)</p> <p>La mayoría de los campos nativos de Workfront asociados con objetos se exportan, pero algunos no. Por ejemplo, no puede exportar los campos Programación, Propietario del proyecto o Patrocinador del proyecto a través de una exportación de inicio de proyecto.</p> <p>En un proyecto que tiene un formulario personalizado adjunto, los datos introducidos en los campos del formulario no se exportan.</p> <p>Pero puede exportar un formulario personalizado. El archivo resultante enumera los campos configurados en el formulario, como los cuadros de texto y los botones de opción.</p> </td> 
   <td> <p>Sí</p> <p>El uso de Kick-Starts para exportar datos de Workfront permite exportar datos relacionados con varios tipos de objetos en una sola exportación. Por ejemplo, puede incluir tareas, problemas y proyectos en una sola exportación.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Límites de exportación

Existen las siguientes limitaciones al exportar datos mediante kick-starts (los datos se exportan en formato de archivo de Excel):

* **50.000 filas:** El número de filas permitidas en el archivo.
* **65.530 hipervínculos:** Excel ha impuesto este límite a los documentos que contienen más de 65.530 hipervínculos. Estos documentos no se pueden abrir después de exportarse. Tenga en cuenta que un documento de Excel puede tener sólo 200 filas de datos, pero si hay más de 65.530 vínculos dentro del documento, éste no se abrirá.

## Exportación de datos mediante kick-starts

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Kick-Starts,** y, a continuación, haga clic en **Exportar datos.**

1. Seleccione el objeto que desea exportar. De manera predeterminada, los siguientes objetos se muestran en **Qué incluir**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objeto</strong> </p> </th> 
      <th> <p><strong>Hojas exportadas del archivo de Excel</strong> </p> </th> 
      <th> <p> <strong>Formato de exportación</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Panel de control</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parámetro<br>Opción de parámetro<br>Grupo de parámetros<br>Parámetro de categoría<br>Categoría<br>Informe<br>Sección de ficha de portal<br>Panel<br>Preferencias</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Informe</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parámetro<br>Opción de parámetro<br>Grupo de parámetros<br>Parámetro de categoría<br>Categoría<br>Informe<br>Preferencias</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Aprobación</p> </td> 
      <td scope="col" valign="top"> <p>Aprobador De Paso<br>Paso De Aprobación<br>Aprobación<br>Proceso De Aprobación<br>Preferencias</p> </td> 
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
      <td valign="top"> <p>Preferencias de <br>usuario</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Más opciones** para ver la lista completa de objetos.

   Todos los objetos enumerados aquí se pueden utilizar para importar también datos en Workfront.

   La única excepción es el objeto **Niveles de acceso**. La hoja de datos Niveles de acceso incluida en una exportación se proporciona únicamente con fines de referencia. Permite asignar un nivel de acceso a una nueva cuenta de usuario por ID.

   Para obtener más información sobre cómo importar datos en Workfront mediante kick-starts, consulte [Importar datos en Adobe Workfront mediante una plantilla de Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). A continuación se muestra una lista de todos los objetos que se pueden exportar mediante kick-starts:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Objeto</p> </th> 
      <th> <p>Hojas exportadas del archivo de Excel</p> </th> 
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
      <td scope="col" valign="top"> Compañía<br>Preferencias </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Plantilla de mensaje de correo electrónico</td> 
      <td scope="col" valign="top"> Plantilla de correo electrónico<br>Preferencias </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Gasto</td> 
      <td valign="top"> Preferencias de <br>gasto </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Página externa</td> 
      <td valign="top"> Página externa<br>Preferencias </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filtro</td> 
      <td valign="top"> Filtrar<br>preferencias </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Grupo</td> 
      <td valign="top"> Preferencias de grupo<br>0  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Agrupación</td> 
      <td valign="top"> Agrupando<br>Preferencias </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Hora</td> 
      <td valign="top"> Preferencias de hora<br> </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Problema</td> 
      <td valign="top"> Problema<br>Preferencias </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Función</td> 
      <td valign="top"> Función del puesto<br>Preferencias </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Ruta de hitos</td> 
      <td valign="top"> Milestone<br>Ruta de hitos<br>Preferencias </td> 
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
      <td valign="top"> Conjunto de recursos<br>Preferencias </td> 
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
      <td valign="top">Preguntas sobre el informe de valoración<br>Opción del informe de valoración<br>Preferencias<br> </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tarea</td> 
      <td valign="top"> Preferencias de la tarea <br> </td> 
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
      <td valign="top"> Preferencias de la tarea de plantilla<br> </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Hoja de horas</td> 
      <td valign="top"> Hoja de horas Perfil<br>Hoja de horas<br>Preferencias </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Ver </td> 
      <td valign="top"> Ver<br>preferencias  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Descargar.**

   El archivo de KickStart exportado se descarga en el equipo como archivo de Excel o como . archivo zip que contiene varios archivos de propiedades y de Excel. Cada archivo de Excel es una colección de hojas, donde cada hoja representa un campo asociado al objeto seleccionado. Hay una hoja **Properties** asociada con cada exportación.

   Las opciones **Tablero** e **Informe** le permiten seleccionar tableros e informes específicos para incluirlos en la descarga. Solo puede exportar paneles, que se comparten en todo el sistema.

   No se pueden exportar los informes de matriz. Para obtener más información acerca de los informes de matriz, vea [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Kick-Starts no admite filtros de modo de texto. Para que la exportación se realice correctamente, los filtros de creación de informes deben cambiarse al modo Estándar.

   Puede seleccionar hasta 100 paneles y 100 informes en una sola exportación.

   ![](assets/kickstart-export-350x381.png)

   Puede exportar varios objetos al mismo tiempo.

1. (Recomendado) Analice los datos exportados para asegurarse de que toda la información que espera ver se ha exportado.

   Para exportaciones grandes, Workfront trabaja en segundo plano para producir el archivo de Excel y le envía un mensaje de advertencia sobre el retraso. El archivo de KickStart se le enviará por correo electrónico cuando finalice la descarga.

   ![](assets/large-kick-start-file-warning-350x65.png)
