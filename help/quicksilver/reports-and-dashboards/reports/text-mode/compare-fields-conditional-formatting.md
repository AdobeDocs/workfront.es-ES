---
product-area: reporting
navigation-topic: text-mode-reporting
title: Comparar campos con formato condicional
description: Puede utilizar el formato condicional para comparar dos campos diferentes en una vista y resaltarlos cuando se cumplen ciertos criterios entre los campos.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Comparar campos con formato condicional

Puede utilizar el formato condicional para comparar dos campos diferentes en una vista y resaltarlos cuando se cumplen ciertos criterios entre los campos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios para editar la vista en un informe</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe para editar la vista en un informe</p> <p>Administrar permisos en una vista</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ejemplo: Comparar fecha de inicio real y fecha de inicio planeada

Por ejemplo, si la Fecha de inicio real de una tarea es posterior a la Fecha de inicio planeada, puede resaltar la columna Fecha de inicio planeada con el formato condicional.

Para comparar la fecha de inicio planeada y la fecha de inicio real de la tarea con el formato condicional:

1. Vaya a una vista de tarea o a un informe.
1. (Condicional) Si está trabajando con un informe, desde la **Columnas (Vista)** , haga clic en el encabezado de la columna a la que desea dar formato condicionalmente para seleccionarla.\
   Por ejemplo, seleccione la **Fecha de inicio real** si desea agregar el formato condicional comparando los campos Fecha de inicio planeada y Fecha de inicio real .

1. Haga clic en **Opciones avanzadas** A continuación, haga clic en Añadir un **Regla para esta columna**.

1. Introduzca los criterios de comparación utilizando los valores existentes encontrados en el generador y especifique el formato condicional.\
   Por ejemplo, deseamos resaltar las tareas en las que la Fecha de inicio real es posterior ( o buena) a la Fecha de inicio planeada. Seleccione el modificador Bueno que es y, en el campo de fecha, seleccione una fecha real.\
     ![](assets/cond-format-1-350x84.png)

1. (Opcional) Seleccione **Aplicar a toda la fila** si desea aplicar el formato a toda la fila.
1. Haga clic en **Agregar regla**, luego **Listo**.

1. Seleccione el **Fecha de inicio real** y, a continuación, haga clic en **Cambiar al modo de texto**.

1. **Haga clic para editar texto** a continuación, agregue la línea de texto siguiente:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   En nuestro ejemplo: 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Si está comparando un campo nativo de Workfront, utilice la sintaxis de mayúsculas y minúsculas para el nombre del campo. Si está comparando un campo personalizado, utilice **DE:Nombre real del campo** para el campo de nombre que está comparando con el primer campo.\
   >Por ejemplo, si está comparando la variable **Fecha de inicio real** con un campo personalizado etiquetado **Fecha de envío**, agregue la siguiente instrucción en el código de modo de texto:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Asegúrese de que la variable `righttext` la línea de código coincide con la instrucción del `rightmethod` línea de código.

   ![](assets/cond-format-2-350x171.png)

1. Haga clic en **Guardar**.
1. Haga clic en **Guardar + Cerrar**.

   La columna resalta los campos que cumplen sus criterios.
