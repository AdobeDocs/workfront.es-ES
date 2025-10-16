---
product-area: projects
navigation-topic: financials
title: Administrar gastos del proyecto
description: El proceso de creación y administración de gastos es el mismo para los gastos relacionados con el proyecto y las tareas. Todos los gastos que se agregan al proyecto en el caso comercial se agregan a la pestaña Gastos como gastos planificados.
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 36%

---

# Administrar gastos del proyecto

<!-- Audited: 6/2025 -->

El proceso de creación y administración de gastos es el mismo para los gastos relacionados con el proyecto y las tareas. Todos los gastos que se añaden al proyecto en el caso empresarial se añaden a la pestaña Gastos como gastos planificados. Para obtener más información, vea [Crear un caso comercial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

La cantidad total de los gastos de todas las tareas y proyectos que contribuye al costo total del proyecto. El importe planificado de los gastos contribuye al coste planificado del proyecto y el importe real de los gastos contribuye al coste real del proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Trabajo o superior</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Acceso de edición a proyectos y datos financieros</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Aportar o permisos superiores al proyecto, con permisos para Ver o Administrar finanzas</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agregar gastos

1. Vaya al proyecto o tarea para el que desee introducir gastos.
1. Haga clic en **Gastos** en el panel izquierdo.
1. Haga clic en **Agregar un gasto**. Aparece el cuadro de diálogo **Agregar un gasto**.
1. Introduzca la siguiente información:

   * **Descripción:** Escriba una descripción del gasto.
   * **Tipo de gasto:** (obligatorio) seleccione la categoría que mejor describa el gasto.
   * **Tarea:** Escriba el nombre de la tarea a la que está asociado este gasto y haga clic en ella cuando aparezca en la lista desplegable.
   * **Importe planificado:** Escriba el importe presupuestado planificado para el gasto. Esto afecta al coste presupuestado del proyecto.

   * **Importe real:** Escriba el importe que representa el costo real del gasto. Esto afecta al coste real del proyecto.

   * **Fecha planificada:** Escriba la fecha esperada para que se produzca el gasto. Puede escribir la fecha en el campo con el formato *mm/dd/aa*, o bien puede hacer clic en el icono **Calendario** ![Icono del calendario](assets/calendar-icon.png) y seleccionar la fecha de forma dinámica.

   * **Fecha de pago:** Escriba o seleccione la fecha en que se pagó el gasto.
   * **Facturable:** Seleccione esta opción si desea facturar este gasto. Categorizar un gasto como facturable es importante al crear registros de facturación.
   * **Reembolsable:** Seleccione esta opción si es necesario reembolsar el gasto. A continuación, puede marcar el gasto como reembolsado después de que se haya reembolsado el gasto.

1. Seleccione un **formulario personalizado** y especifique la información adicional que necesite.

   >[!NOTE]
   >
   >Debe crear un formulario personalizado para poder asociarlo a un gasto. En la lista solo se muestran los formularios personalizados activos. Para obtener información acerca de cómo crear formularios personalizados, vea el artículo [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en **Guardar**.

## Eliminar gastos

1. Vaya al proyecto para el que desea eliminar un gasto.
1. Haga clic en **Gastos** en el panel izquierdo.
1. Seleccione el gasto que desea eliminar y luego haga clic en el icono **Eliminar** ![Eliminar](assets/delete.png).
1. En el diálogo **Eliminar gasto**, haga clic en **Sí, eliminarlo**.
