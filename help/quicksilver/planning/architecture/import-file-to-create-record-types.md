---
title: Crear tipos de registro importando información desde un archivo CSV o de Excel
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustren los elementos de trabajo necesarios en el ciclo vital de su organización mediante la importación de información desde un archivo CSV o de Excel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 16%

---

# Crear tipos de registros importando información desde un archivo CSV o de Excel

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustren los elementos de trabajo necesarios en el ciclo vital de su organización mediante la importación de información desde un archivo CSV o de Excel.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

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
   <td><p> Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>En el entorno de producción, todos los usuarios, incluidos los administradores del sistema, deben estar asignados a una plantilla de diseño que incluya Planning.</p>
<p><span class="preview">En el entorno de vista previa, los usuarios estándar y los administradores del sistema tienen Planning habilitado de forma predeterminada.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Consideraciones acerca de la importación de tipos de registros mediante un archivo CSV o de Excel

* Cada hoja del archivo de Excel se convierte en un tipo de registro. El nombre de la hoja se convierte en el nombre del tipo de registro.
* Si sólo hay una hoja o si importa un archivo CSV, el nombre del archivo se convierte en el nombre del tipo de registro.
* Los encabezados de las columnas de cada hoja se convierten en los campos asociados a cada tipo de registro.
* Los campos son únicos para sus respectivos tipos de registros.
* Cada fila de cada hoja se convierte en un registro único asociado a su tipo de registro respectivo.
* Cada hoja del archivo de Excel no debe superar lo siguiente:
   * 25 000 filas
   * 500 columnas
* El archivo no debe superar los 5 MB.
* No se admiten hojas vacías.
* No se admiten los campos de los siguientes tipos y no se pueden asignar a campos de la hoja de importación:
   * Conexiones y campos de búsqueda de registros conectados <!--or connected Workfront objects-->
   * Campos de fórmula
   * Fecha de creación, Creado por
   * Fecha de la última modificación, Última modificación por
   * Personas

Para importar tipos de registros mediante un archivo CSV o de Excel:

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee crear los tipos de registro,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo situada a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y, a continuación, selecciónelo cuando se muestre en la lista.
1. Haga clic en **Agregar tipo de registro**.
1. Haga clic en **Desde el archivo**.
1. Arrastre y suelte un archivo de Excel o CSV guardado anteriormente en el equipo, o haga clic en **Seleccione un archivo CSV o de Excel** para buscar uno.
1. Haz clic en **Vista previa y edita**.

   Se muestra el cuadro **Previsualizar y editar** con la siguiente información:

   * Los nombres de las hojas o de los futuros tipos de registros se muestran en el panel izquierdo. De forma predeterminada, Workfront Planning selecciona un icono y un color para cada nuevo tipo de registro.
   * Se selecciona el primer tipo de hoja o registro y los nombres de los campos asociados a él se muestran como encabezados de columna. El tipo de cada campo está seleccionado de forma predeterminada.
   * Cada fila representa un nuevo registro. Solo se muestran los 10 primeros registros en el cuadro Vista previa y edición.

   ![Cuadro de vista previa y edición](assets/preview-and-edit-box.png)

1. (Opcional) Haga clic en el nombre de cada hoja en el panel izquierdo para revisar la información que contiene.

   >[!NOTE]
   >
   >Las hojas vacías no son compatibles y aparecen atenuadas.

1. (Opcional) Anule la selección de las hojas que no quiera importar del panel izquierdo.

   ![Seleccione las hojas que desea importar en la lista desplegable sin seleccionar](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Las hojas que no haya seleccionado se muestran con un fondo gris.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del encabezado de la columna para realizar una de las siguientes acciones:

   * Cambie el nombre de uno de los campos
   * Cambiar **tipo de campo**
   * Actualizar el campo **Descripción**

1. (Condicional) Después de actualizar la información del campo, haga clic en **Guardar**.

1. Haga clic en **Importar** cuando esté listo para importar el archivo.

   La siguiente información se importa en Workfront Planning:

   * Nuevos tipos de registros
   * Nuevos campos asociados a cada tipo de registro
   * Nuevos registros asociados a cada tipo de registro

   Puede empezar a administrar campos y registros en las páginas de tipos de registros.

   Todas las personas con acceso a Workfront Planning y al espacio de trabajo ahora pueden ver y editar los tipos de registro importados y su información.
