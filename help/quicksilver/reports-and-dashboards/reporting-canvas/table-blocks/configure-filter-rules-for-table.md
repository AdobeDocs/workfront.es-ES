---
title: Filtrado de una tabla en el Lienzo de informes
description: Filtrado de una tabla en el Lienzo de informes
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---


# Filtrado de una tabla en el Lienzo de informes

Después de agregar un bloque de tabla a un informe, puede configurar filtros para limitar la información que se muestra en la tabla.

Hay 3 componentes en una regla de filtro:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campo</td> 
   <td> <p>El campo que contiene la información por la que desea filtrar la tabla .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operador</td> 
   <td> <p>La forma en que el filtro determina qué valores de campo se incluyen o excluyen de la tabla. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Valor</td> 
   <td> <p>Los valores del campo seleccionado que se evalúan según el operador.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** Si desea limitar los resultados del informe para que solo se muestren los proyectos que son propiedad de Jane Doe, puede crear una regla de filtro con el campo &quot;Propietario del proyecto&quot;, el operador &quot;Igual a&quot; y el valor &quot;Jane Doe&quot;.

O puede mostrar solo los proyectos que tengan un propietario de proyecto asignado, que tendrían el campo &quot;Propietario del proyecto&quot; y el operador &quot;No está en blanco&quot;.

## Requisitos previos

Antes de comenzar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Reporting Canvas beta: información general](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Configuración de reglas de filtro para una tabla

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.

1. Haga clic en **Nuevo informe**.

   O

   Vaya a un informe existente y haga clic en el botón **Más menú** icono ![](assets/more-icon.png) en el encabezado del informe, seleccione **Editar**.

1. Para agrupar filas en una tabla nueva, arrastre o haga doble clic en un bloque de tabla hasta el lienzo.

   O

   Para agrupar filas en una tabla existente, haga clic en el botón **Editar** icono ![](assets/edit-icon.png) en el encabezado de tabla.

1. En el panel derecho, busque el campo mediante el cual desea filtrar la tabla y arrástrelo a la sección Filtro .

   Se muestra un conjunto de reglas de filtro con el nombre del campo seleccionado.

1. Seleccione el operador que desee en el menú desplegable:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Igual a</strong> </td> 
      <td> <p>Esto solo devuelve una coincidencia exacta del valor buscado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Distinto a</strong> </td> 
      <td> <p>Esto solo devuelve resultados que no son coincidencias exactas del valor buscado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>En blanco</strong> </td> 
      <td> <p>El campo existe para el objeto, pero aún no se ha dado un valor al campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>No en blanco</strong> </td> 
      <td> <p>El campo que está filtrando existe y se le ha dado un valor.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than</strong> </td> 
      <td> <p>Esto busca todos los resultados con un valor inferior al introducido, sin incluir el valor introducido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than Or Equal To</strong> </td> 
      <td> <p>Esto busca todos los resultados con un valor menor o igual que el valor introducido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Es Bueno que</strong> </td> 
      <td> <p>Esto busca todos los resultados con un valor bueno al valor introducido, sin incluir el valor introducido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Bueno Que O Igual A</strong> </td> 
      <td> <p>Esto busca todos los resultados con valores buenos o iguales al valor introducido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Entre</strong> </td> 
      <td> <p>Proporciona 2 valores de campo requeridos y busca todos los resultados dentro del rango de ambos campos, incluidos los valores introducidos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contiene</strong> </td> 
      <td> <p>Esto busca el texto especificado en toda una cadena de texto.</p> <p>Por ejemplo, si utiliza "Contiene información", se capturará cualquier cosa que contenga "Inf" o "inf", como la palabra "Infinity".</p> <p>Nota: Adobe Workfront busca toda la palabra o frase que escriba para cada regla de filtro. Por ejemplo, si está buscando campos con la frase "nuevo proyecto" en su nombre, Workfront no muestra proyectos que solo tengan "nuevo" o "proyecto" en sus nombres, ni frases que contengan palabras adicionales entre ellas, como "nuevo proyecto principal". El filtro encuentra solo proyectos con la frase exacta "nuevo proyecto" en el nombre.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>No contiene</strong> </td> 
      <td> <p>Esto filtra los elementos que no tienen texto especificado.</p> <p>Por ejemplo, "no contiene inf" devuelve cualquier campo sin "Inf" o "inf" en sus nombres.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Introduzca el último valor para completar la regla de filtro, según el operador seleccionado.

   >[!NOTE]
   >
   >Los valores introducidos aquí son **not** distingue entre mayúsculas y minúsculas.

1. (Opcional) Para agregar otra regla de filtro al conjunto de reglas, haga lo siguiente:

   1. Arrastre otro campo a la **Soltar para agregar otra regla** en la sección Filtros debajo de la otra regla.
   1. Repita los pasos 4-6.
   1. En la lista desplegable del operador situada a la izquierda de la nueva regla, seleccione **Y** o **O**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>Y</p> </td> 
         <td> <p>Cuando se unen reglas de filtro o conjuntos de reglas con el operador AND, debe indicar que desea que se cumplan todas las reglas del mismo nivel.</p> <p>De forma predeterminada, las instrucciones de un filtro se unen mediante el operador AND.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>O</p> </td> 
         <td> <p>Cuando se unen reglas de filtro o conjunto de reglas con el operador OR, debe indicar que desea <strong>al menos</strong> una regla (o conjunto de reglas) a ese nivel que se va a cumplir.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >Los operadores AND y OR del mismo nivel (que conectan varias reglas dentro de un conjunto de reglas o conjuntos de reglas completos) siempre coincidirán. Por ejemplo, si cambia el operador entre dos reglas dentro de un conjunto de reglas, todos los demás operadores de ese conjunto de reglas cambiarán automáticamente para que coincidan.

1. (Condicional) Para agregar un conjunto de reglas de filtro adicional, haga lo siguiente:

   1. Arrastre el campo que desee añadir al **Agregar un conjunto de reglas** debajo de los demás conjuntos de reglas de filtro.
   1. Repita los pasos del 4 al 7.
   1. En la lista desplegable de operadores situada a la izquierda del nuevo conjunto de reglas, seleccione **Y** o **O**. Estos operadores funcionan igual que los enumerados en el paso 7, pero se aplican a conjuntos de reglas completos en lugar de a reglas individuales dentro de un conjunto.****
