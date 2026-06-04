---
product-area: projects
navigation-topic: financials
title: Anular tarifas de facturación de rol en el nivel de proyecto
description: Este artículo describe cómo puede anular las tarifas de facturación de funciones del sistema para un proyecto.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/zCRX2XunBvSbVd0-pr0evZlpMftnDb8QjBxOvDL-djo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 812
ht-degree: 22%

---

# Anular tarifas de facturación de funciones a nivel de proyecto

Como gerente del proyecto, puede especificar cuál es la tarifa de facturación de una función en un proyecto específico. Esta tarifa de facturación en el nivel de proyecto anula la tarifa de facturación en el nivel de sistema para esta función. Workfront utiliza la tarifa de facturación en el nivel de proyecto de la función de trabajo para calcular los ingresos, en lugar de utilizar la tarifa de facturación en el nivel de sistema.

Este artículo describe cómo puede anular las tarifas de facturación de funciones del sistema para un proyecto.

Para obtener información general acerca de cómo anular las tarifas de facturación de rol para los proyectos y calcular los ingresos del proyecto, vea [Información general sobre cómo anular las tarifas de facturación y calcular los ingresos en un proyecto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Para obtener más información sobre qué rol se usa para calcular los ingresos del proyecto, consulte [Información general sobre la jerarquía de ingresos y costos](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) y la sección [Cálculos de ingresos para tareas basados en asignaciones de usuarios y roles](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) del artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>En el caso de los ingresos reales, las tarifas de facturación aplicadas a las horas que se añaden a un Registro de facturación que está marcado como Facturado, no deben verse afectadas por las anulaciones de tarifas de facturación que ocurren después de que se haya facturado el Registro de facturación.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td> <p>Para anular una tasa de facturación de rol para un proyecto: Cualquier paquete de Workfront o de flujo de trabajo</p>
        <p>Para aplicar atributos al rol: Workflow Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos y datos financieros</p> <p>Acceso administrativo para funciones del puesto</p></td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administre permisos al proyecto que incluya Editar tarifas de facturación </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anular tarifas de facturación de funciones a nivel de proyecto

Al sustituir la tasa de facturación de un trabajo en un proyecto, puede asignar fechas en vigor y cada intervalo de fechas tiene una tasa diferente. Si no asigna fechas en vigor, la anulación de la tarifa de facturación que introduzca se utilizará durante toda la duración del proyecto para calcular los ingresos.

Puede agregar nuevas tarifas de facturación a una plantilla de proyecto, que se convertirán en tarifas de facturación del proyecto cuando cree el proyecto a partir de esa plantilla. Para obtener información sobre cómo editar plantillas, consulte [Editar plantillas del proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!TIP]
>
>No puede anular las tarifas de facturación del usuario de un proyecto a menos que tenga el paquete Workflow Ultimate.

Para sustituir una tarifa de facturación para un proyecto:

1. Vaya al proyecto para el que desea anular las tarifas de facturación.
1. Haga clic en **Tarifas de facturación** en el panel de la izquierda.

   O

   Haga clic en **Tarifas** en el panel izquierdo y luego haga clic en la ficha **Facturación** si aún no está seleccionada.

1. Haga clic en **Agregar tarifa de facturación > Nueva tarifa de facturación del rol**.

   Se abre la casilla Nueva tarifa de facturación.

1. En el campo **Rol**, seleccione el rol para el cual desea cambiar la tarifa de facturación.

1. (Opcional) Seleccione cualquier atributo para la tasa de facturación, como agencia o ubicación.

   El administrador del sistema define los atributos de tasa en el área de Configuración.

1. Seleccione la **Moneda** para la anulación de tarifa de facturación.
1. En el campo **Tarifa de facturación**, ingresa la anulación de tarifa de facturación y luego haz clic en **Guardar** para anular la tarifa de facturación una vez

   O

   Haga clic en **Agregar tarifa** para agregar más anulaciones de tarifas de facturación.

1. (Condicional) Para las sustituciones de ratios de facturación con fecha en vigor, introduzca la siguiente información para cada fila:

   * **Tarifa de facturación**: Valor de la tarifa de facturación desde el comienzo del proyecto hasta la primera fecha de la primera anulación.
   * **Fecha de inicio**: La fecha en la que comienza la anulación de la tarifa de facturación.
   * **Fecha de finalización**: La fecha en la que finaliza la anulación de la tarifa de facturación.

   ![Tarifas de facturación con fechas de anulación](assets/new-job-role-billing-rate-on-project2.png)

   Workfront aplica la tasa de funciones de reemplazo a las horas que se producen durante estos lapsos de tiempo al calcular los ingresos del proyecto.

   Workfront le permite dejar espacios entre marcos de tiempo de anulación, pero recibirá una advertencia para confirmar que esto es intencional.

   No es necesario especificar una fecha de inicio para la primera tasa de sustitución, ni una fecha de finalización para la última tasa de sustitución.

   Si introduce solo una anulación de tarifa de facturación, esa tarifa se aplica a toda la duración del proyecto. Si agrega varias anulaciones con fecha en vigor, Workfront supone que la primera anulación se aplica a todas las horas antes de su fecha de finalización y la última anulación se aplica a todas las horas después de su fecha de inicio.

   Workfront supone que la primera tasa de anulación se aplica a todas las horas con una fecha anterior a la fecha de finalización de la primera anulación y que la última tasa de anulación se aplica a todas las horas con una fecha posterior a la fecha de inicio de la última anulación.

   Si se registra una hora antes de la fecha planificada de inicio del proyecto, se usa la primera tarifa de facturación.

   Si se registra una hora después de la fecha planificada de finalización del proyecto, se utiliza la última tarifa de facturación.

1. Haga clic en **Guardar**.
