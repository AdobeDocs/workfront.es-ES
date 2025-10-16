---
product-area: reporting
navigation-topic: reporting-elements
title: Usar formato condicional en vistas
description: Cuando compartas tus informes con otros usuarios en Adobe Workfront, considera personalizar la vista de los informes para hacer que cierta información sea más fácil de leer o simplemente resalte.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 96%

---

# Usar formato condicional en vistas

<!-- Audited: 11/2024 -->

Cuando compartas tus informes con otros usuarios en Adobe Workfront, considera personalizar la vista de los informes para hacer que cierta información sea más fácil de leer o simplemente resalte.

Puede personalizar la pestaña Detalles de los informes añadiendo formato especial o condicional a la vista de los informes.

Para obtener más información sobre la creación de informes, consulte el artículo [Creación de un informe simple](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Al aplicar formato condicional a las columnas en la vista del informe, puedes configurar reglas que afecten la forma en que se muestra el informe. Cuando se cumplen esas condiciones o reglas, se aplica el formato especial.

Por ejemplo, si el porcentaje de finalización de una tarea es inferior al 20 por ciento, puedes resaltar el campo mostrando el número de porcentajes en negrita, texto rojo y con un fondo de color amarillo.

Con una vista con formato condicional, puede hacer lo siguiente:

* Cambie el encabezado de una columna.
* Cambie el valor de una columna a texto o imagen personalizados.
* Dar formato a la visualización de un campo cambiando el tipo de fuente, el color, la alineación o el color del fondo.

Los cambios que realices en la vista del informe solo se aplican en la pestaña Detalles del informe. Estos cambios no afectan las pestañas Resumen, Matriz o Gráfico del informe.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</strong></td> 
   <td> 
    <p>Estándar o Plan para vistas de informes</p>
    <p>Colaborador o solicitud de vistas de lista</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a filtros, vistas y agrupaciones</p> <p>Acceso de Edición de acceso a Informes, tableros y calendarios para editar una vista en un informe</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
    <td> <p>Gestionar permisos de un informe para crear o editar una vista en un informe</p> <p>Permisos de administración de una vista</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe crear un informe antes de poder añadir formato condicional a su vista.

Para obtener información sobre cómo crear un informe, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Creación de una vista con formato condicional

{{step1-to-reports}}

1. Haga clic en el nombre del informe donde desee crear una vista con formato condicional

   O

   Haga clic en **Nuevo informe**, luego selecciona un tipo de objeto para crear un nuevo informe.

1. (Condicional) Si edita un informe existente, haga clic en **Acciones del informe**, y luego en **Editar**.

1. En la pestaña **Columnas (Vista)** haga clic para seleccionar una columna existente o haga clic en **Añadir columna** para crear una columna.
1. En el campo **Mostrar en esta columna** de la esquina superior izquierda de Report Builder, seleccione el campo que desee mostrar en la nueva columna.
1. Haga clic en **Opciones avanzadas**.

1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Etiqueta personalizada de columna</strong></td> 
      <td> <p>Especifique un nombre para la columna.</p> <p>Si estás editando una columna existente, al especificar un nombre aquí se cambia el nombre de la columna existente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato de campo</strong></td> 
      <td>Elija el formato en el que se muestra el valor de la columna. Dependiendo de cuál sea el campo de columna, se permite configurar cómo se muestran las fechas, los números o la moneda. No todas las columnas muestran esta opción.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar esta columna en panel de control</strong></td> 
      <td>Seleccione este campo si desea que la columna se muestre cuando el informe se coloque en un tablero. La columna siempre se muestra cuando se mira el informe fuera de un panel de control.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Añadir una regla para esta columna**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. En la sección **Cuando:** establece una declaración condicional para la columna.

   Por ejemplo: “cuando el Porcentaje completado de la tarea sea Igual (distingue entre mayúsculas y minúsculas) a 50”.
1. En la sección **Mostrar el campo de esta forma:** especifica cómo se verá este campo cuando se cumpla la condición definida anteriormente.

   Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Color de texto</strong></td> 
      <td> <p>Seleccione el color en el que se muestra el texto mediante el selector de color.</p> <p><b>NOTA</b></p> <p> Si el campo contiene un hipervínculo, las selecciones de color del texto no se aplican a este campo.</p> </td> 
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
      <td role="rowheader"><strong>Contexto</strong></td> 
      <td>Seleccione el color del fondo del texto con el selector de color.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar icono</strong></td> 
      <td>Seleccione uno de los 16 iconos si desea mostrar un icono en lugar del valor real de esta columna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostrar texto</strong></td> 
      <td> <p>Selecciona esta opción para mostrar una etiqueta personalizada para esta columna, en lugar de su valor real. Especifique el texto que se va a mostrar en lugar del valor en el campo proporcionado.</p> <p><b>IMPORTANTE</b></p> <p>Seleccionar <strong>Mostrar texto</strong> desactiva la capacidad de editar el texto en línea en esta columna.<br>Tampoco puede cambiar el valor de una columna Predecesora porque contiene lógica integrada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aplicar a toda la fila</strong></td> 
      <td>Selecciona esta opción para aplicar la configuración a toda la fila en lugar de aplicarla solo a la columna seleccionada.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Añadir regla**.\
   Puede añadir reglas adicionales a la misma columna o a otras columnas.

   Las reglas se aplican en el orden en que se crearon. Se combinan, pero no se sobrescriben entre sí, aunque una regla de columna tiene prioridad sobre una regla de fila en la misma celda.

   **EJEMPLO 1**

   En primer lugar, puede crear una regla que indique que, cuando un proyecto se encuentra en estado de compilación, el color del texto sea morado y negrita. A continuación, cree una segunda regla que indique que cuando el nombre de una tarea no en blanco, el color del texto es rojo y en cursiva, y el color de fondo es verde. En este ejemplo, ocurre lo siguiente:

   * Las tareas cuyo estado del proyecto sea Generando se mostrarán en texto morado y negrita. Si el nombre de la tarea no en blanco, las tareas también tienen un fondo verde.
   * Las tareas cuyo estado del proyecto sea distinto de Generación (y cuyo nombre de tarea no en blanco) se mostrarán en rojo y en cursiva con fondo verde.

   **EJEMPLO 2**

   Cree una regla en la columna Fecha planificada de finalización del proyecto que afecte a toda la fila y ponga el fondo gris si se cancela el proyecto (por ejemplo, cuando el estado del proyecto es Inactivo). A continuación, cree una regla de columna que ponga el fondo rojo cuando la fecha planificada de finalización del proyecto sea menor que hoy (lo que significa que el proyecto está atrasado). En este ejemplo, si un proyecto cancelado tiene una fecha de finalización tardía, esa celda aparecerá en rojo, aunque las demás celdas de la fila sean grises. Para corregir este formato:

   * Edita el formato de la Fecha planificada de finalización y elimina la regla de la columna para el fondo rojo en proyectos atrasados.
   * Añada una regla de columna con el mismo formato que la regla de fila (fondo gris cuando el Estado del Proyecto = Finalizado)
   * Añada nuevamente la regla de columna para el fondo rojo en proyectos atrasados.
   * Al guardar las reglas y la vista, el fondo rojo no se aplica a un proyecto cancelado.

1. Haga clic en **Guardar**.
1. Haga clic en **Guardar + Cerrar**.\
   En el informe, los usuarios ven cambios en el formato si se cumplen las condiciones especificadas.
