---
title: Importar campos desde Adobe Workfront
description: En Adobe Workfront Planning, puede crear campos personalizados para cada tipo de registro. A continuación, puede asociar el campo con los registros de Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 0da877936ba8f52341a5b151f76710c979ce9294
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 7%

---


<!--add to TOC-->

# Importación de campos desde Adobe Workfront

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Puede importar copias de campos de Workfront existentes. Al importar campos desde Workfront, se crea una copia de cada campo para un tipo de registro de Workfront Planning.


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
   <td role="rowheader"><p>plan Adobe Workfront*</p></td> 
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
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar </p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administrar permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre la importación de campos desde Workfront

* Puede importar campos de Workfront nativos o personalizados a un tipo de registro en Workfront Planning.
* La importación de campos de Workfront crea copias de los mismos campos y conserva el nombre del campo en Workfront Planning. Una vez copiados en Workfront Planning, los campos son independientes de los campos originales de Workfront y no comparten información.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* Puede agregar campos nativos o personalizados desde los siguientes objetos de Workfront:
   * Portafolio
   * Programar
   * Proyecto
   * Tarea
   * Problema
   * Documento
   * Compañía
   * Grupo
   * Usuario
   * Función
   * Asignación
   * Hora
   * Registro de facturación
     <!--Available only to Preview, but might not come to Prod:* Rate card-->
   * Gasto
   * Iteración
     <!--* Non-labor resource-->
     <!--* Non-labour resource category-->
* Es posible que los campos de Workfront no conserven su tipo de campo después de importarse en Workfront Planning.

  La tabla siguiente muestra los tipos de campo de Workfront y su tipo de campo de Workfront Planning correspondiente.

  | Tipo de campo de Workfront | Tipo de campo de Workfront Planning |
  |------------------------------------------|-------------------------------|
  | Texto con formato de una sola línea | Texto de línea única |
  | Texto de una sola línea con formato de número | Número |
  | Texto de una sola línea con formato de moneda | Divisa |
  | Párrafo | Párrafo |
  | Texto con formato | Párrafo |
  | Lista desplegable de selección única | Selección única |
  | Lista desplegable de selección múltiple | Selección múltiple |
  | Los filtros de escritura anticipada de usuario no son compatibles | Personas |
  | Calculado* | Fórmula |
  | Fecha | Fecha |
  | Grupo de casillas de verificación | Selección múltiple |
  | Botón de opción | Selección múltiple |

  *Los campos calculados estarán disponibles más adelante.
Todos los demás tipos de campos de Workfront no son compatibles con Workfront Planning.


## Importar campos desde Workfront

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registro desee utilizar para crear campos.

   Se abre el espacio de trabajo y se muestran los tipos de registro.

1. Haga clic en la tarjeta de un tipo de registro.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.

   >[!TIP]
   >
   >    Algunos campos pueden estar ocultos. Haga clic en **Campos** y habilite la opción para los campos que desee ver como columnas en la vista de tabla.

1. Haga clic en el icono **+** en la esquina superior derecha de la vista de tabla

   O

   Pase el ratón sobre el encabezado de cualquier columna, haga clic en la flecha hacia abajo después del nombre del campo y, a continuación, haga clic en **Insertar a la izquierda** o **Insertar a la derecha** para agregar el nuevo campo.
1. Haga clic en **Agregar** existente en la esquina inferior derecha de la ficha **Nuevo campo**. <!--check UI - did they change this??-->

   ![](assets/add-existing-fields-from-workfront-modal.png)

1. Empiece a escribir el nombre de un campo de Workfront existente en el área de búsqueda y, a continuación, haga clic en **+** cuando se muestre en la lista.
1. (Opcional) Escriba otro campo y haga clic en **+** cuando se muestre en la lista.
1. (Opcional) Haga clic en el icono **Filtros** ![](assets/filters-in-import-fields-icon.png) y, a continuación, actualice uno o ambos de los campos siguientes:

   * Tipo de objeto: seleccione un tipo de objeto Workfront cuyos campos desee importar.
   * Formulario personalizado: seleccione uno o varios formularios personalizados de Workfront. Puede seleccionar un formulario personalizado sin seleccionar primero un tipo de objeto.
1. Haga clic en **+** y luego en **Agregar campos**.
Los campos se agregan a la vista de tabla y a las páginas de detalles de los registros.
