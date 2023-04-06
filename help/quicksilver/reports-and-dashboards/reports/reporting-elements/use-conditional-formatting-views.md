---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizar el formato condicional en las vistas
description: A medida que comparta los informes con otros usuarios de Adobe Workfront, considere la posibilidad de personalizar la vista de los informes para facilitar la lectura o destacar cierta información.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1148'
ht-degree: 2%

---

# Utilizar el formato condicional en las vistas

A medida que comparta los informes con otros usuarios de Adobe Workfront, considere la posibilidad de personalizar la vista de los informes para facilitar la lectura o destacar cierta información.

Puede personalizar la pestaña Detalles de los informes agregando un formato especial o condicional a la vista de los informes.

Debe tener permisos de administración en el informe para poder editarlo y agregar formato especial a la vista.

Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Si aplica formato condicional a las columnas en la vista del informe, puede configurar reglas que afecten a la forma en que se muestra el informe. Cuando se cumplen esas condiciones o reglas, se aplica el formato especial.

Por ejemplo, si el porcentaje completado de una tarea es inferior al 20 por ciento, puede resaltar el campo mostrando el número de porcentaje en negrita, texto rojo y un color de fondo amarillo.

Con una vista con formato condicional, puede:

* Cambie el encabezado de una columna.
* Cambie el valor de una columna por texto personalizado o una imagen.
* Para dar formato a la visualización de un campo, cambie el tipo de fuente, el color, la alineación o el color del fondo.

Los cambios que realice en la vista del informe surtirán efecto únicamente en la pestaña Detalles del informe. Estos cambios no afectan a las pestañas Resumen, Matriz o Gráfico del informe.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios para editar una vista en un informe</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administrar permisos para un informe para crear o editar una vista en un informe</p> <p>Administrar permisos en una vista</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe crear un informe antes de poder agregarle formato condicional.

Para obtener información sobre la creación de informes, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Crear una vista con formato condicional

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Informes**.

1. Haga clic en el nombre de un informe en el que desea crear una vista con formato condicional.

   O

   Haga clic en **Acciones de informe** y haga clic en **Editar**.

1. (Condicional) Si ha editado un informe, seleccione una columna existente o cree una nueva.
1. Haga clic en **Opciones avanzadas**.

1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Etiqueta personalizada de columna</strong></td> 
      <td> <p>Especifique un nombre para la columna.</p> <p>Si está editando una columna existente, al especificar un nombre aquí se cambiará el nombre de la columna existente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato de campo</strong></td> 
      <td>Elija el formato en el que se muestra el valor en la columna . En función de lo que sea el campo de columna, esto le permite establecer cómo se muestran las fechas, los números o la moneda.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar esta columna en panel</strong></td> 
      <td>Seleccione este campo si desea que la columna se muestre cuando el informe se coloque en un tablero. La columna siempre se muestra al mirar el informe fuera de un tablero.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Agregar una regla para esta columna**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. En el **Cuando:** , defina una condición para la columna. Por ejemplo: cuando el porcentaje completado de la tarea es igual a (con distinción de mayúsculas y minúsculas) 50.
1. En el **Muestre el campo de esta manera:** especifique el aspecto del campo cuando se cumpla la condición definida anteriormente.

   Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Color de texto</strong></td> 
      <td> <p>Seleccione el color en el que se muestra el texto. Hay 8 colores disponibles.</p> <p>Nota: Si el campo contiene un hipervínculo, las selecciones de color de texto no se aplican a este campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato de texto</strong></td> 
      <td>Seleccione si desea mostrar el texto en negrita o en cursiva.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Alineación de texto</strong></td> 
      <td>Seleccione si desea alinear el texto a la derecha, al centro o a la izquierda dentro de la columna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fondo</strong></td> 
      <td>Seleccione el color del fondo del texto. Hay 8 colores disponibles.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar icono</strong></td> 
      <td>Seleccione uno de los 16 iconos si desea mostrar un icono en lugar del valor real de esta columna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar texto</strong></td> 
      <td> <p>Seleccione esta opción para mostrar una etiqueta personalizada para esta columna, en lugar de su valor real. Especifique el texto que desea mostrar en lugar del valor del campo proporcionado.</p> <p>Importante: Selección <strong>Mostrar texto</strong> deshabilita la posibilidad de editar en línea el texto de esta columna.<br>Además, no se puede cambiar el valor de una columna de Predecesor porque contiene lógica integrada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aplicar a toda la fila</strong></td> 
      <td>Seleccione esta opción para aplicar la configuración a toda la fila en lugar de aplicar la configuración solo a la columna seleccionada.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Agregar regla**.\
   Puede agregar reglas adicionales a la misma columna o agregar reglas a otras columnas.

   Las reglas se aplican en el orden en que se crearon. Se combinan, pero no se sobrescriben entre sí, aunque una regla de columna tiene prioridad sobre una regla de fila de la misma celda.

   Ejemplo 1: Primero puede crear una regla que indique que cuando el estado del proyecto está generando, el color del texto es morado y negrita. A continuación, se crea una segunda regla que indica que cuando el nombre de la tarea no está en blanco, el color del texto es rojo y cursiva y el color del fondo es verde. En este ejemplo, se produce lo siguiente:

   * Las tareas cuyo estado del proyecto es Generación se muestran en color morado y en negrita. Si el nombre de la tarea no está en blanco, las tareas también tienen un fondo verde.
   * Las tareas cuyo estado del proyecto es cualquier cosa que no sea la creación (y el nombre de la tarea no está en blanco) se muestran en un texto rojo y en cursiva con un fondo verde.

   Ejemplo 2: Cree una regla en la Fecha de Finalización Planificada del Proyecto que afecte a toda la fila, de modo que el fondo quede gris si se cancela el proyecto (Estado = &quot;Muerto&quot;). A continuación, cree una regla de columna que ponga el fondo en rojo cuando la Fecha de finalización planeada para el proyecto sea menor que hoy (lo que significa que el proyecto está atrasado). En este ejemplo, si un proyecto cancelado tiene una fecha de finalización tardía, esa celda aparecerá en rojo aunque las demás celdas de la fila estén grises. Para corregir este formato:

   * Edite el formato de la fecha de finalización planeada y elimine la regla de columna del fondo rojo en los proyectos atrasados.
   * Agregue una regla de columna con el mismo formato que la regla de fila (fondo gris cuando Estado del proyecto = &quot;Muerto&quot;).
   * Agregue de nuevo la regla de columna para el fondo rojo en los proyectos atrasados.
   * Al guardar las reglas y la vista, el fondo rojo no se aplica a un proyecto cancelado.


1. Haga clic en **Listo**.
1. Haga clic en **Guardar + Cerrar**.\
   En el informe, los usuarios ven cambios en el formato si se cumplen las condiciones especificadas.
