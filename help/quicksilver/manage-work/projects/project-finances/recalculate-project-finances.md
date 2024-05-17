---
title: Recalcular finanzas del proyecto
product-area: projects
navigation-topic: financials
description: Las finanzas se calculan en un proyecto a medida que se producen cambios en las horas registradas para el proyecto o en las tasas utilizadas para calcular los costes y los ingresos.
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 0%

---

# Recalcular finanzas del proyecto

Las finanzas se calculan en un proyecto a medida que se producen cambios en las horas registradas para el proyecto o en las tasas utilizadas para calcular los costes y los ingresos.

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
   <td> <p>Editar acceso a Proyectos y datos financieros</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto con permisos para Administrar finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Consideraciones sobre el cálculo de finanzas en Adobe Workfront

Las finanzas se calculan en el análisis mejorado de las siguientes maneras:

* Puede recalcular manualmente los costes e ingresos de un proyecto mediante la opción Recalcular finanzas en un proyecto.
* Además, algunas acciones almacenan en déclencheur un nuevo cálculo automático.

Cuando la tasa de un usuario o un rol cambia durante la duración de un proyecto, puede ocurrir lo siguiente:

* Cuando se realiza el cambio, la tasa actualizada se utiliza a partir de ese momento, a medida que se registran las horas y se calcula la información financiera. Cambiar la tasa no afecta a cómo se calcularon las cosas antes de realizar el cambio. Para todas las horas existentes registradas, se utiliza la tarifa antigua para calcular la información financiera.
* Puede obligar a Adobe Workfront a utilizar la nueva tasa de forma retroactiva para todas las horas registradas hasta el momento, utilizando la opción Recalcular finanzas. Esto obliga a Workfront a volver a calcular de forma retroactiva todas las horas introducidas anteriormente, los costes planificados y los ingresos de acuerdo con la nueva información de tarifas.

>[!CAUTION]
>
>Antes de recalcular manualmente las finanzas de un proyecto determinado, es posible que desee conservar los datos financieros que ya se hayan calculado a una tasa anterior. Se recomienda utilizar la opción Recalcular finanzas solo cuando esté seguro de que no está realizando cambios en la información existente o solo cuando dichos cambios sean deseados.
>
>Tenga en cuenta que al ejecutar un informe de proyecto (datos financieros) se vuelven a calcular los datos financieros y, como tal, debe tener en cuenta las mismas consideraciones antes de ejecutar el informe.

## Conservar datos financieros de tareas con horas existentes {#preserve-financial-data-for-tasks-with-existing-hours}

Cuando se vuelven a calcular los datos financieros de un proyecto, Workfront vuelve a calcular de forma retroactiva todas las horas registradas anteriormente, los costes planificados, los costes reales y los ingresos planificados y reales, de acuerdo con cualquier información financiera nueva o actualizada.

* [Conservar ingresos del proyecto](#preserve-project-revenue)
* [Conservar costo del proyecto](#preserve-project-cost)

### Conservar ingresos del proyecto  {#preserve-project-revenue}

Las tasas de ingresos pueden cambiar durante la duración de un proyecto.

Para obtener más información sobre las tarifas de facturación y los ingresos, consulte el artículo [Resumen de facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Las tasas de ingresos pueden cambiar en los siguientes niveles:

* El nivel del sistema (para los roles)\
  Para obtener más información sobre la creación de funciones con tarifas de facturación en el sistema, consulte el artículo [Crear y administrar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* El nivel de usuario\
  Para obtener más información acerca de cómo cambiar la información sobre la tarifa de facturación de los usuarios, consulte el artículo [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* El nivel de compañía (para los roles)\
  Para obtener más información, consulte [Anular las tarifas de facturación de funciones en el nivel de compañía](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* El nivel de proyecto (para los roles)\
  Para obtener más información sobre la anulación de tasas de rol en el nivel de proyecto, consulte el artículo [Resumen de anulación de Tarifas de facturación de rol y cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Por ejemplo, la tarifa de facturación de un usuario cambia durante el transcurso de un proyecto de 50 a 75 dólares la hora y desea que todos los datos existentes permanezcan calculados a la tarifa antigua (50 dólares y hora). Sin embargo, cuando se recalculen las finanzas del proyecto, los ingresos de las tareas que ya tengan datos financieros se actualizarán para reflejar la nueva tasa de facturación (de 75 dólares la hora).

* [Conservar ingresos del proyecto creando un registro de facturación](#preserve-project-revenue-by-creating-a-billing-record)
* [Conservar ingresos del proyecto mediante el uso de varias anulaciones de tarifa de facturación](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Conservar ingresos del proyecto creando un registro de facturación {#preserve-project-revenue-by-creating-a-billing-record}

Cuando las tarifas de facturación cambian en cualquier nivel mencionado anteriormente, puede conservar los ingresos existentes que ya se han calculado en el proyecto evitando usar la opción Recalcular finanzas manualmente o bloqueando el tiempo registrado en el proyecto y calculado usando la tarifa antigua en un registro de facturación con un estado de Facturado.

Cuando no recalcula las finanzas en el proyecto o cuando bloquea las horas registradas en un registro de facturación facturada, las horas registradas después de los cambios de tarifa se calcularán con la nueva tarifa y las horas registradas antes de que cambie la tarifa de costo permanecerán calculadas con la tarifa antigua.

Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

#### Conservar ingresos del proyecto mediante el uso de varias anulaciones de tarifa de facturación {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

Cuando cambian las tarifas de facturación para los roles en el nivel de proyecto, puede conservar los ingresos existentes que ya se han calculado en el proyecto mediante el uso de varias anulaciones de tarifas de facturación que están bloqueadas dentro de un lapso de tiempo especificado.

Para obtener más información sobre cómo usar varias anulaciones de tarifas de facturación, consulte el artículo [Resumen de anulación de Tarifas de facturación de rol y cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Esto solo se aplica a las tarifas de facturación de roles de trabajo que se cambian en el nivel de proyecto.

### Conservar costo del proyecto {#preserve-project-cost}

Las tasas de coste pueden cambiar en los siguientes niveles:

* Nivel del sistema (para roles)\
  Para obtener más información sobre la creación de funciones con tasas de coste a nivel de sistema, consulte el artículo [Crear y administrar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Nivel de usuario\
  Para obtener más información sobre cómo cambiar la información de tasa de costo de los usuarios, vea el artículo [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Cuando las tarifas de facturación cambian en cualquier nivel mencionado anteriormente, puede conservar los costos existentes que ya se han calculado en el proyecto bloqueando el tiempo registrado en el proyecto y calculado usando la tarifa antigua en un registro de facturación con un estado de Facturado. Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

También puede evitar utilizar la opción Recalcular finanzas manualmente si no desea crear un registro de facturación, tal como se describe en la sección [Recalcular manualmente las finanzas de un proyecto](#manually-recalculate-finances-for-a-project) en este artículo.

Cuando no recalcula las finanzas en el proyecto o cuando bloquea las horas registradas en un registro de facturación facturada, las horas registradas después de los cambios de tarifa se calcularán con la nueva tarifa y las horas registradas antes de que cambie la tarifa de costo permanecerán calculadas con la tarifa antigua.

## Recalcular manualmente las finanzas de un proyecto {#manually-recalculate-finances-for-a-project}

Si las tarifas cambian durante la duración de un proyecto y desea que los cálculos de costos e ingresos reflejen las nuevas tarifas, debe recalcular manualmente las finanzas en el proyecto.

>[!NOTE]
>
>Puede evitar que los valores de ingresos se actualicen para reflejar las nuevas tasas cuando recalcule manualmente las finanzas siguiendo los pasos de la sección [Conservar datos financieros de tareas con horas existentes](#preserve-financial-data-for-tasks-with-existing-hours) de este artículo. Los valores de costo siempre se actualizan para reflejar las nuevas tasas cuando se recalculan manualmente las finanzas en un proyecto.

Puede recalcular las finanzas de los proyectos en Workfront desde la página del proyecto o desde una lista de proyectos o un informe.

Puede recalcular las finanzas mientras las edita por lotes. Para obtener más información, consulte [Recalcular finanzas manualmente de forma masiva](#manually-recalculate-finances-in-bulk) de este artículo.

1. Vaya al proyecto donde desea volver a calcular las finanzas y haga clic en el **Más** icono ![](assets/qs-more-icon-on-an-object.png) a la derecha del nombre del proyecto.

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   O

   Vaya a una lista de proyectos o a un informe, seleccione uno o varios proyectos y, a continuación, haga clic en **Más** icono ![](assets/qs-more-icon-on-an-object.png) al principio de la lista.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Según la complejidad de sus proyectos, recomendamos no seleccionar un gran número de proyectos al recalcular sus finanzas de forma masiva para garantizar un rendimiento óptimo. Algunas cosas que podrían hacer que un proyecto sea demasiado complejo podrían ser varias dependencias o asignaciones o un gran número de campos personalizados.

1. Clic **Recalcular finanzas**.

   Todos los costes e ingresos planificados del proyecto se recalculan con la información nueva.

   Debería recibir una confirmación en la parte superior del explorador de que las finanzas del proyecto se han recalculado correctamente.
Los valores de coste existentes y algunos valores de ingresos que no se han bloqueado se actualizan para reflejar las nuevas tasas.

## Recalcular finanzas manualmente de forma masiva{#manually-recalculate-finances-in-bulk}

Puede recalcular manualmente las finanzas de varios proyectos editándolos por lotes. Esto hace que los ingresos de los proyectos se recalculen de forma retroactiva.

>[!IMPORTANT]
>
>Puede evitar que los valores de ingresos se actualicen para reflejar las nuevas tasas cuando recalcule manualmente las finanzas siguiendo los pasos de la sección [Conservar datos financieros de tareas con horas existentes](#preserve-financial-data-for-tasks-with-existing-hours) de este artículo. Los valores de costo siempre se actualizan para reflejar las nuevas tasas cuando se recalculan manualmente las finanzas en los proyectos.

Para volver a calcular manualmente las finanzas de varios proyectos:

1. Ir a una lista de proyectos.
1. Seleccione varios proyectos en la lista y haga clic en **Más** icono ![](assets/qs-more-icon-on-an-object.png) al principio de la lista.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Según la complejidad de sus proyectos, recomendamos no seleccionar un gran número de proyectos al editarlos por lotes para garantizar un rendimiento óptimo. Algunas cosas que podrían hacer que un proyecto sea demasiado complejo podrían ser varias dependencias o asignaciones o un gran número de campos personalizados.

1. Clic **Recalcular finanzas**.

   Todos los costes e ingresos planificados de los proyectos seleccionados se vuelven a calcular con la información nueva.

   Debería recibir una confirmación en la parte superior del navegador de que las finanzas de los proyectos se han recalculado correctamente.

## Acciones que afectan al déclencheur de un nuevo cálculo automático de las finanzas

Las siguientes acciones almacenan como déclencheur el recálculo financiero de los proyectos en Workfront:

* Cambiar el estado de tarea
* Mover una tarea con horas a otro proyecto
* Cambio del estado del proyecto de Completo a Activo

>[!NOTE]
>
>Al cambiar el estado del proyecto, solo se vuelven a calcular los valores planificados.

También puede recalcular las finanzas manualmente en la sección **Más** menú ![](assets/qs-more-menu.png) en el nivel de proyecto, haciendo clic en **Recalcular finanzas**.
