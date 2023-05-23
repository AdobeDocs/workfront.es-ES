---
product-area: reporting
navigation-topic: reporting-elements
title: Uso de formato condicional en vistas
description: Cuando comparta los informes con otros usuarios de Adobe Workfront, considere la posibilidad de personalizar la vista de los informes para que cierta información sea más fácil de leer o simplemente destacar.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 2%

---

# Uso de formato condicional en vistas

Cuando comparta los informes con otros usuarios de Adobe Workfront, considere la posibilidad de personalizar la vista de los informes para que cierta información sea más fácil de leer o simplemente destacar.

Puede personalizar la pestaña Detalles de los informes añadiendo formato especial o condicional a la vista de los informes.

Debe tener permisos de administración en el informe para poder editarlo y agregar formato especial a la vista.

Para obtener más información sobre la creación de informes, consulte el artículo [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Al aplicar formato condicional a las columnas en la vista del informe, puede configurar reglas que afecten a la forma en que se muestra el informe. Cuando se cumplen esas condiciones o reglas, se aplica el formato especial.

Por ejemplo, si el porcentaje completado de una tarea es inferior al 20 por ciento, puede resaltar el campo mostrando el número de porcentaje en negrita, texto rojo y color de fondo amarillo.

Con una vista con formato condicional, puede:

* Cambie el encabezado de una columna.
* Cambie el valor de una columna a texto o imagen personalizados.
* Dar formato a la visualización de un campo cambiando el tipo de fuente, el color, la alineación o el color del fondo.

Los cambios que realice en la vista del informe sólo se aplicarán en la ficha Detalles del informe. Estos cambios no afectan a las pestañas Resumen, Matriz o Gráfico del informe.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitud o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Paneles y Calendarios para editar una vista de un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administración de permisos de un informe para crear o editar una vista de un informe</p> <p>Administración de permisos en una vista</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Debe crear un informe para poder agregarle formato condicional.

Para obtener información sobre cómo crear un informe, consulte [Creación de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Creación de una vista con formato condicional

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Informes**.

1. Haga clic en el nombre del informe en el que desee crear una vista con formato condicional.

   O

   Clic **Acciones de informe**, luego haga clic en **Editar**.

1. (Condicional) Si ha editado un informe, seleccione una columna existente o cree una nueva.
1. Clic **Opciones avanzadas**.

1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Etiqueta personalizada de columna</strong></td> 
      <td> <p>Especifique un nombre para la columna.</p> <p>Si está editando una columna existente, al especificar un nombre aquí se cambia el nombre de la columna existente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato de campo</strong></td> 
      <td>Elija el formato en el que se muestra el valor de la columna. En función del campo de columna, permite establecer cómo se muestran las fechas, los números o la moneda.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar esta columna en panel</strong></td> 
      <td>Seleccione este campo si desea que la columna se muestre cuando el informe se coloque en un panel. La columna siempre se muestra cuando se mira el informe fuera de un panel.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Agregar una regla para esta columna**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. En el **Cuando el:** , establezca una instrucción condition para la columna. Por ejemplo: cuando el porcentaje completado de la tarea es igual a (distingue mayúsculas de minúsculas) 50.
1. En el **Mostrar el campo de esta manera:** especifique el aspecto de este campo cuando se cumple la condición definida arriba.

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
      <td> <p>Seleccione esta opción para mostrar una etiqueta personalizada para esta columna, en lugar de su valor real. Especifique el texto que se va a mostrar en lugar del valor en el campo proporcionado.</p> <p>Importante: Seleccionar <strong>Mostrar texto</strong> deshabilita la capacidad de editar en línea el texto de esta columna.<br>Además, no se puede cambiar el valor de una columna Predecesora porque contiene lógica integrada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aplicar a toda la fila</strong></td> 
      <td>Seleccione esta opción para aplicar la configuración a toda la fila en lugar de aplicar la configuración únicamente a la columna seleccionada.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Agregar regla**.\
   Puede agregar reglas adicionales a la misma columna o a otras columnas.

   Las reglas se aplican en el orden en que se crearon. Se combinan pero no se sobrescriben entre sí, aunque una regla de columna tiene prioridad sobre una regla de fila en la misma celda.

   Ejemplo 1: Primero puede crear una regla que indique que cuando el estado del proyecto es Generando, el color del texto es morado y negrita. A continuación, cree una segunda regla que indique si el nombre de la tarea no está en blanco, si el color del texto es rojo y en cursiva y si el color de fondo es verde. En este ejemplo, ocurre lo siguiente:

   * Las tareas cuyo estado del proyecto sea Generando se mostrarán en texto morado y negrita. Si el nombre de la tarea no está en blanco, las tareas también tienen un fondo verde.
   * Las tareas cuyo estado del proyecto sea distinto de Generación (y cuyo nombre de tarea no esté en blanco) se mostrarán en rojo y en cursiva con fondo verde.

   Ejemplo 2: Cree una regla en la fecha planificada de finalización del proyecto que afecte a toda la fila y ponga el fondo gris si se cancela el proyecto (Estado = &quot;Inactivo&quot;). A continuación, cree una regla de columna que ponga el fondo rojo cuando la fecha planificada de finalización del proyecto sea menor que hoy (lo que significa que el proyecto está atrasado). En este ejemplo, si un proyecto cancelado tiene una fecha de finalización tardía, esa celda aparecerá en rojo aunque las demás celdas de la fila sean grises. Para corregir este formato:

   * Edite el formato de la fecha planificada de finalización y elimine la regla de columna para el fondo rojo de los proyectos retrasados.
   * Agregue una regla de columna con el mismo formato que la regla de fila (fondo gris cuando el estado del proyecto = &quot;Inactivo&quot;).
   * Vuelva a agregar la regla de columna para el fondo rojo en los proyectos posteriores.
   * Al guardar las reglas y la vista, el fondo rojo no se aplica a un proyecto cancelado.


1. Clic **Listo**.
1. Clic **Guardar + Cerrar**.\
   En el informe, los usuarios ven cambios en el formato si se cumplen las condiciones especificadas.
