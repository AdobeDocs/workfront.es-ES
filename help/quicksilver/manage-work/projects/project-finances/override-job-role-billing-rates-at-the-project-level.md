---
product-area: projects
navigation-topic: financials
title: Anular tasas de facturación de rol de trabajo en el nivel de proyecto
description: Como administrador de proyectos, puede especificar la tasa de facturación de una función de trabajo en un proyecto específico. Esta tasa de facturación a nivel de proyecto anula la tasa de facturación a nivel del sistema para esta función de trabajo. Workfront utiliza la tasa de facturación a nivel de proyecto de la función de trabajo para calcular los ingresos, en lugar de utilizar la tasa de facturación a nivel de sistema.
author: Alina
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Anular tasas de facturación de rol de trabajo en el nivel de proyecto

Como administrador de proyectos, puede especificar la tasa de facturación de una función de trabajo en un proyecto específico. Esta tasa de facturación a nivel de proyecto anula la tasa de facturación a nivel del sistema para esta función de trabajo. Workfront utiliza la tasa de facturación a nivel de proyecto de la función de trabajo para calcular los ingresos, en lugar de utilizar la tasa de facturación a nivel de sistema.

En este artículo se describe cómo puede anular las tasas de facturación del rol de trabajo del sistema para un proyecto.

Para obtener información general sobre cómo anular las tasas de facturación de la función de trabajo para proyectos y calcular los ingresos del proyecto, consulte [Información general sobre la anulación de la función de trabajo Tasas de facturación y el cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Para obtener más información sobre la función de trabajo que se utiliza para calcular los ingresos del proyecto, consulte la sección &quot;Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuario y función&quot; del artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>En el caso de los ingresos reales, las tasas de facturación aplicadas a las horas que se agregan a un registro de facturación marcado como Facturado no deben verse afectadas por las anulaciones de las tasas de facturación que se produzcan después de facturar el registro de facturación.

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
   <td> <p>Editar acceso a Proyectos y Datos Financieros</p> <p>Acceso administrativo para funciones de trabajo</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para el proyecto que incluye Editar datos financieros </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Anular tasas de facturación de rol de trabajo en el nivel de proyecto

Puede anular la tasa de facturación de una función de trabajo en un proyecto de las siguientes maneras:

* Una vez, seleccionando una nueva tasa para la función de trabajo.\
   La nueva tasa se utiliza durante toda la duración del proyecto para calcular los ingresos.

* Varias veces, seleccionando varias tasas nuevas para intervalos de fechas específicos.\
   Se puede utilizar una tasa diferente durante cada intervalo de fechas especificado.

>[!TIP]
>
>No puede anular las tasas de facturación de los usuarios de un proyecto.

Para anular una tasa de facturación de un proyecto:

1. Vaya al proyecto para el que desea anular las tasas de facturación.
1. Haga clic en **Tasas de facturación** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más**.
1. Haga clic en **Agregar tasa de facturación** > **Nueva tasa de facturación**.

   Se abre la casilla Tasa de Facturación Nueva.

1. En el **Función del trabajo** , seleccione la función de trabajo para la que desea cambiar la tasa de facturación.

   ![](assets/override-billing-rate-on-project-nwe-350x310.png)

   La variable **Tasa de facturación predeterminada** muestra la tasa a nivel del sistema para esta función de trabajo.

1. En el **Tasas de facturación 1** , introduzca la anulación única de la tasa de facturación y haga clic en **Guardar** para anular la tasa de facturación una vez

   O

   Haga clic en **Agregar tasa** para agregar más anulaciones de la tasa de facturación.

1. (Condicional) Si está agregando más de una anulación de la tasa de facturación, especifique la siguiente información:

   * **Tasas de facturación 1**: el valor de la tasa de facturación desde el principio del proyecto hasta la primera fecha de la primera anulación. Normalmente es la misma cantidad que la variable **Tasa predeterminada**.
   * **Fecha de inicio**: es la fecha en la que finaliza la tasa predeterminada.
   * **Fecha final**: la fecha en la que finaliza la anulación de la nueva tasa de facturación.

   ![new_billing_rate_with_adapt_dates.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. La zona horaria de las fechas seleccionadas se muestra en la parte inferior del cuadro Tasa de facturación nueva. Esta es la zona horaria asociada a su instancia de Workfront, tal como se muestra en el área Información del cliente de Configuración. Para obtener más información, consulte [Configurar información básica para el sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront aplica la tasa de rol de trabajo de invalidación a las horas que se producen durante los lapsos de tiempo especificados al calcular los ingresos en el proyecto.
1. No debe haber espacios entre los lapsos de tiempo de dos tasas de anulación. La variable **Fecha de inicio** de una tasa de anulación debe ser el día inmediatamente siguiente a la **Fecha final** de la fecha de anulación anterior.

1. No se puede especificar una fecha de inicio para la primera tasa de anulación ni una fecha de finalización para la última tasa de anulación.\
   Se recomienda utilizar la Tasa predeterminada para la primera tasa de anulación.\
   Workfront supone que la primera tasa de anulación se aplica a todas las horas con una fecha anterior a la fecha de finalización de la primera anulación y que la última tasa de anulación se aplica a todas las horas con una fecha posterior a la fecha de inicio de la última anulación.\
   Si se registra una hora antes de la fecha de inicio planeada del proyecto, se utiliza la primera tasa de facturación.\
   Si se registra una hora después de la Fecha de Finalización Planificada del proyecto, se utiliza la última tasa de facturación.

1. Haga clic en **Guardar**.
