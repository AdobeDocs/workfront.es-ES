---
title: Filtrado de una tabla en el lienzo de informes
description: Filtrado de una tabla en el lienzo de informes
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: ca70952bf0acd71f748b042852d434b560727a83
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---


# Filtrado de una tabla en el lienzo de informes

Después de agregar un bloque de tabla a un informe, puede configurar filtros para limitar la información que se muestra en la tabla.

Hay 3 componentes en una regla de filtro:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campo</td> 
   <td> <p>El campo que contiene la información con la que desea filtrar la tabla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operador</td> 
   <td> <p>La forma en que el filtro determina qué valores de campo se incluyen o excluyen de la tabla. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Valor</td> 
   <td> <p>Los valores dentro del campo seleccionado que se evalúan según el operador.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** Si desea limitar los resultados del informe para que solo muestren los proyectos que sean propiedad de Jane Doe, puede crear una regla de filtro con el campo &quot;Propietario del proyecto&quot;, el operador &quot;Igual a&quot; y el valor &quot;Jane Doe&quot;.

O puede mostrar solo los proyectos que tengan un propietario de proyecto asignado, que tendría el campo &quot;Propietario del proyecto&quot; y el operador &quot;No está en blanco&quot;.

## Requisitos previos

Antes de empezar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Resumen de Lienzo de informes beta](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configuración de reglas de filtro para una tabla

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.

1. Clic **Nuevo informe**.

   O

   Vaya a un informe existente y haga clic en **Menú Más** icono ![](assets/more-icon.png) en el encabezado del informe, seleccione **Editar**.

1. Para agrupar filas en una tabla nueva, arrastre o haga doble clic en un bloque de tabla hasta el lienzo.

   O

   Para agrupar filas en una tabla existente, haga clic en **Editar** icono ![](assets/edit-icon.png) en el encabezado de la tabla.

1. En el panel derecho, busque el campo por el que desea filtrar la tabla y, a continuación, arrástrelo a la sección Filtro.

   Se muestra un conjunto de reglas de filtro con el nombre del campo seleccionado.

1. Seleccione el operador que desee en el menú desplegable:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Equal To</strong> </td> 
      <td> <p>Esto solo devuelve una coincidencia exacta del valor buscado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Not Equal To</strong> </td> 
      <td> <p>Esto solo devuelve resultados que no coinciden exactamente con el valor buscado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>En blanco</strong> </td> 
      <td> <p>El campo existe para el objeto, pero aún no se ha dado un valor al campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>No en blanco</strong> </td> 
      <td> <p>El campo por el que está filtrando existe y se le ha dado un valor.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than</strong> </td> 
      <td> <p>Esto busca todos los resultados con un valor menor que el introducido, sin incluir el valor introducido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Es Menor Que O Igual A</strong> </td> 
      <td> <p>Esto busca todos los resultados con un valor menor o igual que el valor introducido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Es Bueno que</strong> </td> 
      <td> <p>Esto busca todos los resultados con un valor bueno al valor introducido, sin incluir el valor introducido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Es Bueno que o igual a</strong> </td> 
      <td> <p>Esto busca todos los resultados con valores buenos o iguales al valor introducido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Entre</strong> </td> 
      <td> <p>Proporciona 2 valores de campo obligatorios y busca todos los resultados dentro del intervalo de ambos campos, incluidos los valores introducidos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contiene</strong> </td> 
      <td> <p>Esto busca el texto especificado en toda una cadena de texto.</p> <p>Por ejemplo, si utiliza "Contiene Inf", se captura todo lo que contenga "Inf" o "inf", como la palabra "Infinity".</p> <p>Nota: Adobe Workfront busca la palabra o frase completa introducida para cada regla de filtrado. Por ejemplo, si está buscando campos con la frase "nuevo proyecto" en su nombre, Workfront no muestra los proyectos que tienen únicamente "nuevo" o "proyecto" en sus nombres, ni las frases que contienen palabras adicionales intermedias como "nuevo proyecto principal". El filtro solo encuentra proyectos con la frase exacta "nuevo proyecto" en el nombre.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>No contiene</strong> </td> 
      <td> <p>Esto filtra los elementos a los que les falta texto especificado.</p> <p>Por ejemplo, "no contiene inf" devuelve ningún campo sin "inf" ni "inf" en sus nombres.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Introduzca el último valor para completar la regla de filtrado, según el operador seleccionado.

   >[!NOTE]
   >
   >Los valores introducidos aquí son **no** distingue mayúsculas de minúsculas.

1. (Opcional) Para agregar otra regla de filtro al conjunto de reglas, haga lo siguiente:

   1. Arrastre otro campo a **Soltar para agregar otra regla** en la sección Filtros debajo de la otra regla.
   1. Repita los pasos 4-6.
   1. En la lista desplegable de operadores que se encuentra a la izquierda de la nueva regla, seleccione **Y** o **O**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>Y</p> </td> 
         <td> <p>Al unir reglas de filtro o conjuntos de reglas con el operador AND, indica que desea que se cumplan todas las reglas del mismo nivel.</p> <p>De forma predeterminada, las instrucciones de un filtro se unen mediante el operador AND.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>O</p> </td> 
         <td> <p>Cuando una reglas de filtro o un conjunto de reglas con el operador OR, indica que desea <strong>al menos</strong> se debe cumplir una regla (o conjunto de reglas) en ese nivel.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >Los operadores AND y OR del mismo nivel (que conectan varias reglas de un conjunto de reglas o conjuntos de reglas completos) siempre coincidirán. Por ejemplo, si cambia el operador entre dos reglas dentro de un conjunto de reglas, todos los demás operadores de ese conjunto de reglas cambiarán automáticamente para coincidir con él.

1. (Condicional) Para agregar un conjunto de reglas de filtro adicional, haga lo siguiente:

   1. Arrastre el campo que desee agregar al **Agregar un conjunto de reglas** debajo de los demás conjuntos de reglas de filtro.
   1. Repita los pasos 4-7.
   1. En la lista desplegable de operadores que se encuentra a la izquierda del nuevo conjunto de reglas, seleccione **Y** o **O**. Estos operadores funcionan igual que los enumerados en el paso 7, pero se aplican a conjuntos de reglas completos en contraposición a reglas individuales dentro de un conjunto****.
