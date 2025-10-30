---
title: Crear o personalizar gravedades de problemas
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Los usuarios pueden usar gravedades para definir la gravedad de un problema. Puede personalizar cualquiera de las cinco gravedades predeterminadas existentes en Adobe Workfront o crear una nueva gravedad para los usuarios.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 5c80dca8a9f7dd5a693db9bf22738602da8b521b
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 65%

---

# Crear o personalizar la gravedad de los problemas

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Los usuarios pueden usar gravedades para definir la gravedad de un problema. Puede personalizar cualquiera de las cinco gravedades predeterminadas existentes en Adobe Workfront o crear una nueva gravedad para los usuarios.

>[!NOTE]
>
>Las tareas y los proyectos no tienen gravedades.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Gravedades de problemas integradas

Workfront tiene cinco gravedades de problemas integradas:

* Cosmético
* Causa confusión
* Error con solución
* Error sin solución
* Error fatal

Puede editar lo siguiente para estas gravedades:

* Nombre
* Color

  El color de una gravedad se conserva en un informe de gráfico si se agrupan los resultados por Gravedad del problema. Para obtener información sobre los informes de gráficos, consulte [Añadir un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Qué gravedad es la predeterminada

  Para obtener más información acerca de las gravedades predeterminadas, consulte [Crear o editar una gravedad de problema](#create-or-edit-an-issue-severity) en este artículo.

* Descripción
* Si una gravedad está oculta en Workfront

  Para obtener más información acerca de cómo ocultar una gravedad, vea [Crear o editar una gravedad de problema](#create-or-edit-an-issue-severity) en este artículo.

* Eliminar una gravedad

  Al hacerlo, debe seleccionar una gravedad de reemplazo.

## Crear o editar una gravedad de problema {#create-or-edit-an-issue-severity}

Como administrador de Workfront, puede crear y editar gravedades de problemas para adaptarlas a las necesidades de los usuarios.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Preferencias del proyecto** > **Gravedades**.

1. Si está creando una nueva gravedad, haga clic en **Nueva fila** en la parte inferior de la tabla.
1. Configure las siguientes opciones para la nueva gravedad o edítelas para una gravedad existente:

   * **Nombre de gravedad**: escriba un nombre para la gravedad.
   * **Importancia**: aumente o reduzca el nivel de gravedad asignado originalmente por Workfront para la gravedad.

     El número de importancia de cada gravedad debe ser único. El número más alto corresponde al nivel más alto de gravedad.

     No puede editar este número después de guardar la gravedad.

   * **Color**: elija un color para la gravedad.

     El color de la gravedad se utiliza en los informes de gráficos al agrupar los resultados por gravedad del problema. Para obtener información sobre los informes de gráficos, consulte [Añadir un gráfico a un informe](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

   * **Gravedad predeterminada**: seleccione la gravedad que desea que Workfront aplique automáticamente a todos los problemas recién creados.

     **Cosmético** es la gravedad predeterminada para los problemas en Workfront.

     No puede convertir una gravedad oculta en la predeterminada.

     La gravedad predeterminada se indica con un icono ![Icono de gravedad predeterminada](assets/default-icon.png). Para elegir un nuevo valor predeterminado, siga uno de estos procedimientos:

      * Seleccione la casilla de verificación situada junto al nombre de la gravedad y seleccione **Establecer como predeterminado** en la barra de acciones de la parte inferior de la pantalla.
      * Pase el ratón sobre el nombre de la gravedad y haga clic en el menú **Más** que aparece. A continuación, seleccione **Establecer como predeterminado**.

        La nueva gravedad predeterminada se etiqueta con el icono.

   * **Descripción**: escriba una descripción de la gravedad para explicar su función.
   * **Ocultar opción**: seleccione **Sí** para ocultar una gravedad que ya no sea necesaria.

     Una gravedad oculta no aparecerá en ninguna parte de Workfront, por lo que los usuarios no pueden elegirla para sus problemas.

     >[!IMPORTANT]
     >
     >En lugar de eliminar gravedades que ya no desee utilizar, le sugerimos que las oculte. De este modo, se conservan todos los datos históricos de los objetos ya completados con la gravedad, mientras que se evita que los usuarios utilicen la gravedad en el futuro.

1. (Opcional) Para cambiar el orden en que aparecen las gravedades, arrastre y suéltelas en el orden que desee.

   Esto cambia el orden en el que se muestran en los problemas. No cambia el número **Importancia**.

1. Haga clic en **Guardar**.

Para obtener más información sobre cómo usar gravedades mientras se trabaja con problemas, consulte [Actualizar la gravedad del problema](../../../manage-work/issues/issue-information/update-issue-severity.md).
