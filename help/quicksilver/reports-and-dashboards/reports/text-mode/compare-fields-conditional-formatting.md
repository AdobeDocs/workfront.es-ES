---
product-area: reporting
navigation-topic: text-mode-reporting
title: Comparar campos en formato condicional
description: Puede utilizar el formato condicional para comparar dos campos diferentes en una vista y resaltarlos cuando se cumplan determinados criterios entre los campos.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Comparar campos en formato condicional

Puede utilizar el formato condicional para comparar dos campos diferentes en una vista y resaltarlos cuando se cumplan determinados criterios entre los campos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Paneles y Calendarios para editar la vista de un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe para editar la vista en un informe</p> <p>Administración de permisos en una vista</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ejemplo: Comparar Fecha de Inicio Real y Fecha de Inicio Planificada

Por ejemplo, si la fecha de inicio real de una tarea es posterior a la fecha de inicio planificada, puede resaltar la columna Fecha de inicio planificada con formato condicional.

Para comparar la fecha planificada de inicio y la fecha real de inicio de la tarea mediante un formato condicional:

1. Ir a una vista de tareas o a un informe.
1. (Condicional) Si está trabajando con un informe, en la ficha **Columnas (Ver)**, haga clic en el encabezado de la columna a la que desea dar formato condicional para seleccionarla.\
   Por ejemplo, seleccione la columna **Fecha de inicio real** si desea agregarle el formato condicional comparando los campos Fecha de inicio planificada y Fecha de inicio real.

1. Haga clic en **Opciones avanzadas** y, a continuación, haga clic en Agregar una regla **para esta columna**.

1. Introduzca los criterios de comparación utilizando los valores existentes encontrados en el generador y especifique el formato condicional.\
   Por ejemplo, se desea resaltar las tareas en las que la fecha de inicio real sea posterior ( o posterior) a la fecha de inicio planificada. Seleccione el modificador Greater Than y seleccione una fecha real en el campo de fecha.\
     ![](assets/cond-format-1-350x84.png)

1. (Opcional) Seleccione **Aplicar a toda la fila** si desea aplicar el formato a toda la fila.
1. Haga clic en **Agregar regla** y después en **Listo**.

1. Seleccione la columna **Fecha real de inicio** y, a continuación, haga clic en **Cambiar al modo de texto**.

1. **Haga clic para editar el modo texto** y después agregue la siguiente línea de texto:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   En nuestro ejemplo: 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Si está comparando un campo nativo de Workfront, utilice la sintaxis en minúscula para el nombre del campo. Si está comparando un campo personalizado, use **DE:Nombre real del campo** para el campo de nombre que está comparando con el primer campo.\
   >Por ejemplo, si está comparando la **Fecha real de inicio** con un campo personalizado denominado **Fecha de entrega**, agregue la siguiente instrucción al código de modo de texto:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Asegúrese de que la línea de código `righttext` coincida con la instrucción de la línea de código `rightmethod`.

   ![](assets/cond-format-2-350x171.png)

1. Haga clic en **Guardar**.
1. Haga clic en **Guardar + Cerrar**.

   La columna resalta los campos que cumplen los criterios.
