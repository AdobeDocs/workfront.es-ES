---
product-area: projects
navigation-topic: financials
title: Anular tarifas de facturación de rol en el nivel de proyecto
description: Como gerente del proyecto, puede especificar cuál es la tarifa de facturación de una función en un proyecto específico. Esta tarifa de facturación en el nivel de proyecto anula la tarifa de facturación en el nivel de sistema para esta función. Workfront utiliza la tarifa de facturación en el nivel de proyecto de la función de trabajo para calcular los ingresos, en lugar de utilizar la tarifa de facturación en el nivel de sistema.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: eb3db3b056cea359f77e56f77d6e9520954e2abb
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 31%

---

# Anular tarifas de facturación de funciones a nivel de proyecto

Como gerente del proyecto, puede especificar cuál es la tarifa de facturación de una función en un proyecto específico. Esta tarifa de facturación en el nivel de proyecto anula la tarifa de facturación en el nivel de sistema para esta función. Workfront utiliza la tarifa de facturación en el nivel de proyecto de la función de trabajo para calcular los ingresos, en lugar de utilizar la tarifa de facturación en el nivel de sistema.

Este artículo describe cómo puede anular las tarifas de facturación de funciones del sistema para un proyecto.

Para obtener información general acerca de la anulación de tarifas de facturación de roles de trabajo para proyectos y el cálculo de ingresos de proyectos, consulte [Información general sobre la anulación de tarifas de facturación de roles de trabajo y el cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Para obtener más información sobre qué rol se usa para calcular los ingresos del proyecto, consulte la sección &quot;Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuarios y roles&quot; en el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>En el caso de los ingresos reales, las tarifas de facturación aplicadas a las horas que se añaden a un Registro de facturación que está marcado como Facturado, no deben verse afectadas por las anulaciones de tarifas de facturación que ocurren después de que se haya facturado el Registro de facturación.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos y datos financieros</p> <p>Acceso administrativo para funciones del puesto</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administrar permisos para el proyecto que incluye Editar datos financieros </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anular tarifas de facturación de funciones a nivel de proyecto

Puede anular la tasa de facturación de un rol en un proyecto de las siguientes maneras:

* Una vez, seleccionando una nueva tasa para el rol.\
  La nueva tarifa se utiliza durante toda la duración del proyecto para calcular los ingresos.

* Varias veces, seleccionando varias tasas nuevas para intervalos de fechas específicos.\
  Se puede utilizar una tasa diferente durante cada intervalo de fechas especificado.

* Puede agregar nuevas tarifas de facturación a una plantilla de proyecto, que se convertirán en tarifas de facturación del proyecto cuando cree el proyecto a partir de esa plantilla. Para obtener información sobre cómo editar plantillas, consulte [Editar plantillas del proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!TIP]
>
>No puede anular las tarifas de facturación de un usuario en un proyecto.

Para sustituir una tarifa de facturación para un proyecto:

1. Vaya al proyecto para el que desea anular las tarifas de facturación.
1. Haga clic en **Tarifas de facturación** en el panel de la izquierda.
1. Haga clic en **Agregar tarifa de facturación** > **Nueva tarifa de facturación**.

   Se abre la casilla Nueva tarifa de facturación.

1. En el campo **Rol**, seleccione el rol para el cual desea cambiar la tarifa de facturación.

   ![Anular tarifa de facturación en el proyecto](assets/override-billing-rate-on-project-nwe-350x310.png)

   El campo **Tarifa de facturación predeterminada** muestra la tarifa a nivel del sistema para este rol.

1. En el campo **Tasas de facturación 1**, ingrese la anulación de tarifa de facturación única y luego haga clic en **Guardar** para anular la tarifa de facturación una vez

   O

   Haga clic en **Agregar tarifa** para agregar más anulaciones de tarifas de facturación.

1. (Condicional) Si agrega más de una anulación de tarifa de facturación, especifique la siguiente información:

   * **Tarifas de facturación 1**: el valor de la tarifa de facturación desde el comienzo del proyecto hasta la primera fecha de la primera anulación. Generalmente es la misma cantidad que la **tarifa predeterminada**.
   * **Fecha de inicio**: esta es la fecha en la que finaliza la tarifa predeterminada.
   * **Fecha de finalización**: la fecha en la que finaliza la nueva anulación de tarifa de facturación.

   ![new_billing_rate_with_adjustment_dates.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. La zona horaria de las fechas que seleccione se mostrará en la parte inferior del cuadro Nueva tarifa de facturación. Esta es la zona horaria asociada a la instancia de Workfront, como se muestra en el área de Información del cliente de la Configuración. Para obtener más información, consulte [Configurar información básica para el sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront aplica la tasa de rol de reemplazo a las horas que ocurren durante los lapsos de tiempo especificados al calcular los ingresos en el proyecto.
1. No debe haber espacios entre los marcos de tiempo de dos tasas de anulación. La **fecha de inicio** de una tasa de invalidación debe ser el día inmediatamente posterior a la **fecha de finalización** de la fecha de invalidación anterior.

1. No puede especificar una fecha de inicio para la primera tasa de sustitución ni una fecha de finalización para la última tasa de sustitución.\
   Le recomendamos que utilice la Tasa predeterminada para la primera tasa de anulación.\
   Workfront supone que la primera tasa de anulación se aplica a todas las horas con una fecha anterior a la fecha de finalización de la primera anulación y que la última tasa de anulación se aplica a todas las horas con una fecha posterior a la fecha de inicio de la última anulación.\
   Si se registra una hora antes de la fecha planificada de inicio del proyecto, se usa la primera tarifa de facturación.\
   Si se registra una hora después de la fecha planificada de finalización del proyecto, se utiliza la última tarifa de facturación.

1. Haga clic en **Guardar**.
