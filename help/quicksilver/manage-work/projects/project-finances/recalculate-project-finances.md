---
title: Volver a calcular las finanzas del proyecto
product-area: projects
navigation-topic: financials
description: Las finanzas se calculan en un proyecto a medida que se producen cambios en las horas registradas para el proyecto o en las tasas utilizadas para calcular los costes y los ingresos.
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1590'
ht-degree: 0%

---

# Volver a calcular las finanzas del proyecto

Las finanzas se calculan en un proyecto a medida que se producen cambios en las horas registradas para el proyecto o en las tasas utilizadas para calcular los costes y los ingresos.

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
   <td> <p>Editar acceso a Proyectos y Datos Financieros</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para el proyecto con permisos para Administrar finanzas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre el cálculo de finanzas en Adobe Workfront

Las finanzas se calculan en Análisis mejorado de las siguientes maneras:

* Puede volver a calcular manualmente los costes e ingresos de un proyecto mediante la opción Recalcular finanzas de un proyecto.
* Además, algunas acciones déclencheur un nuevo cálculo automático.

Cuando la tasa de un usuario o una función cambia durante la vida de un proyecto, puede ocurrir lo siguiente:

* Cuando se realiza el cambio, la tasa actualizada se utiliza a partir de ese momento a medida que se registran las horas y se calcula la información financiera. Cambiar la tasa no afecta a cómo se calcularon las cosas antes de realizar el cambio. Para todas las horas existentes registradas, la antigua tasa se utiliza para calcular la información financiera.
* Puede obligar a Adobe Workfront a utilizar la nueva tasa de forma retroactiva para todas las horas registradas hasta el momento, mediante la opción Recalcular finanzas . Esto obliga a Workfront a volver a calcular de forma retroactiva todas las horas introducidas anteriormente, los costes planeados y los ingresos de acuerdo con la nueva información de tasa.

>[!CAUTION]
>
>Antes de volver a calcular manualmente las finanzas de un proyecto determinado, es posible que desee conservar los datos financieros que ya se hayan calculado a una tasa anterior. Se recomienda utilizar la opción Volver a calcular finanzas solo cuando esté seguro de que no está realizando cambios en la información existente, o solo cuando desea realizar dichos cambios.

## Conservar datos financieros para tareas con horas existentes {#preserve-financial-data-for-tasks-with-existing-hours}

Cuando se vuelven a calcular los datos financieros de un proyecto, Workfront vuelve a calcular de forma retroactiva todas las horas registradas anteriormente, los costes planeados, reales y los ingresos planeados y reales, de acuerdo con cualquier información financiera nueva o actualizada.

* [Conservar ingresos del proyecto](#preserve-project-revenue)
* [Mantener costo del proyecto](#preserve-project-cost)

### Conservar ingresos del proyecto  {#preserve-project-revenue}

Las tasas de ingresos pueden cambiar durante la duración de un proyecto.

Para obtener más información sobre tasas de facturación e ingresos, consulte el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Las tasas de ingresos pueden variar en los siguientes niveles:

* Nivel del sistema (para funciones de trabajo)\
   Para obtener más información sobre la creación de funciones de trabajo con tasas de facturación a nivel de sistema, consulte el artículo [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* El nivel de usuario\
   Para obtener más información sobre cómo cambiar la información de la tasa de facturación de los usuarios, consulte el artículo [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Nivel de empresa (para funciones de trabajo)\
   Para obtener más información, consulte [Anular las tasas de facturación de funciones de trabajo a nivel de empresa](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* Nivel de proyecto (para funciones de trabajo)\
   Para obtener más información sobre cómo anular las tasas de rol de trabajo en el nivel de proyecto, consulte el artículo [Información general sobre la anulación de la función de trabajo Tasas de facturación y el cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Por ejemplo, la tasa de facturación de un usuario cambia durante el curso de un proyecto de 50 a 75 dólares la hora y desea que todos los datos existentes se mantengan calculados a la tasa antigua (50 dólares y hora). Sin embargo, cuando se recalculen las finanzas del proyecto, las tareas que ya tengan datos financieros existentes tendrán los ingresos actualizados para reflejar la nueva tasa de facturación (de 75 dólares por hora).

* [Mantener ingresos del proyecto creando un registro de facturación](#preserve-project-revenue-by-creating-a-billing-record)
* [Mantener ingresos del proyecto mediante varias anulaciones de tasa de facturación](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Mantener ingresos del proyecto creando un registro de facturación {#preserve-project-revenue-by-creating-a-billing-record}

Cuando las tasas de facturación cambian en cualquier nivel mencionado anteriormente, puede conservar los ingresos existentes que ya se han calculado en el proyecto evitando utilizar la opción de recalcular finanzas manual o bloqueando el tiempo registrado en el proyecto y calculado mediante la tasa antigua en un registro de facturación con el estado Facturado.

Cuando no vuelva a calcular las finanzas del proyecto o cuando bloquee las horas registradas en un registro de facturación facturado, las horas registradas después de los cambios de tasa se calcularán con la nueva tasa y las horas registradas antes de los cambios de tasa de coste se calcularán con la tasa antigua.

Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

#### Mantener ingresos del proyecto mediante varias anulaciones de tasa de facturación {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

Cuando las tasas de facturación cambian para las funciones de los trabajos en el nivel de proyecto, puede conservar los ingresos existentes que ya se han calculado en el proyecto mediante el uso de varias anulaciones de las tasas de facturación que están bloqueadas en un lapso de tiempo especificado.

Para obtener más información sobre el uso de las anulaciones de tasas de facturación múltiples, consulte el artículo [Información general sobre la anulación de la función de trabajo Tasas de facturación y el cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Esto solo se aplica a las tasas de facturación de funciones de trabajo que se cambian a nivel de proyecto.

### Mantener costo del proyecto {#preserve-project-cost}

Las tasas de coste pueden variar en los siguientes niveles:

* Nivel del sistema (para funciones de trabajo)\
   Para obtener más información sobre la creación de funciones de trabajo con tasas de coste en el nivel del sistema, consulte el artículo [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Nivel de usuario\
   Para obtener más información sobre cómo cambiar la información de la tasa de costo en los usuarios, consulte el artículo [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Cuando las tasas de facturación cambian en cualquier nivel mencionado anteriormente, puede conservar los costes existentes que ya se han calculado en el proyecto bloqueando el tiempo registrado en el proyecto y calculándolo con la tasa antigua en un registro de facturación con el estado Facturado. Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

También puede evitar utilizar la opción Recalcular finanzas manual, si no desea crear un registro de facturación, como se describe en la sección [Volver a calcular manualmente las finanzas de un proyecto](#manually-recalculate-finances-for-a-project) en este artículo.

Cuando no vuelva a calcular las finanzas del proyecto o cuando bloquee las horas registradas en un registro de facturación facturado, las horas registradas después de los cambios de tasa se calcularán con la nueva tasa y las horas registradas antes de los cambios de tasa de coste se calcularán con la tasa antigua.

## Volver a calcular manualmente las finanzas de un proyecto {#manually-recalculate-finances-for-a-project}

Si las tasas cambian durante la vida de un proyecto y desea que los cálculos de costes e ingresos reflejen las nuevas tasas, debe volver a calcular manualmente las finanzas del proyecto.

>[!NOTE]
>
>Puede evitar que los valores de los ingresos se actualicen para reflejar las nuevas tasas cuando vuelva a calcular manualmente las finanzas siguiendo los pasos de la sección [Conservar datos financieros para tareas con horas existentes](#preserve-financial-data-for-tasks-with-existing-hours) de este artículo. Los valores de coste siempre se actualizan para reflejar las nuevas tasas cuando se vuelven a calcular manualmente las finanzas de un proyecto.

Puede volver a calcular las finanzas de los proyectos en Workfront desde la página del proyecto o desde una lista de proyectos o un informe.

Puede volver a calcular las finanzas mientras las edita de forma masiva. Para obtener más información, consulte la [Volver a calcular manualmente las finanzas de forma masiva en el cuadro Editar proyectos](#manually-recalculate-finances-in-bulk-in-the-edit-projects-box) en este artículo.

1. Vaya al proyecto en el que desea volver a calcular las finanzas y haga clic en el botón **Más** icono ![](assets/qs-more-icon-on-an-object.png) a la derecha del nombre del proyecto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   O

   Vaya a una lista de proyectos o a un informe y seleccione uno o varios proyectos. A continuación, haga clic en el **Más** icono ![](assets/qs-more-icon-on-an-object.png) en la parte superior de la lista.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >En función de la complejidad de sus proyectos, le recomendamos que no seleccione un gran número de proyectos al volver a calcular sus finanzas de forma masiva para garantizar un rendimiento óptimo. Algunas cosas que podrían hacer que un proyecto sea demasiado complejo pueden ser varias dependencias o asignaciones o un gran número de campos personalizados.

1. Haga clic en **Volver a calcular finanzas**.

   Todos los costos e ingresos planeados en el proyecto se vuelven a calcular con cualquier información nueva.

   Debe recibir una confirmación en la parte superior del explorador de que las finanzas del proyecto se han recalculado correctamente.\
   Los valores de coste existentes y algunos valores de ingresos que no se han bloqueado se actualizan para reflejar las nuevas tasas.

## Volver a calcular manualmente las finanzas de forma masiva en el cuadro Editar proyectos {#manually-recalculate-finances-in-bulk-in-the-edit-projects-box}

Puede volver a calcular manualmente las finanzas de varios proyectos editándolos de forma masiva. Esto hace que los ingresos de los proyectos se vuelvan a calcular de forma retroactiva.

>[!IMPORTANT]
>
>Puede evitar que los valores de los ingresos se actualicen para reflejar las nuevas tasas cuando vuelva a calcular manualmente las finanzas siguiendo los pasos de la sección [Conservar datos financieros para tareas con horas existentes](#preserve-financial-data-for-tasks-with-existing-hours) de este artículo. Los valores de coste siempre se actualizan para reflejar las nuevas tasas cuando se vuelven a calcular manualmente las finanzas de los proyectos.

Para volver a calcular manualmente las finanzas de varios proyectos:

1. Vaya a una lista de proyectos.
1. Seleccione varios proyectos de la lista y haga clic en **Editar**.

   >[!TIP]
   >
   >En función de la complejidad de sus proyectos, se recomienda no seleccionar un gran número de proyectos al editarlos de forma masiva para garantizar un rendimiento óptimo. Algunas cosas que podrían hacer que un proyecto sea demasiado complejo pueden ser varias dependencias o asignaciones o un gran número de campos personalizados.

1. Haga clic en **Configuración** y, a continuación, seleccione **Volver A Calcular Los Costes Y Los Ingresos**.

1. Haga clic en **Guardar cambios**.

## Acciones que déclencheur un nuevo cálculo automático de las finanzas

Las siguientes acciones déclencheur el cálculo financiero de los proyectos en Workfront:

* Cambio del estado de una tarea
* Mover una tarea con horas a otro proyecto
* Cambio del estado del proyecto de Completado a un estado activo

>[!NOTE]
>
>Al cambiar el estado del proyecto, solo se vuelven a calcular los valores planificados.

También puede volver a calcular las finanzas manualmente en la sección **Más** menú ![](assets/qs-more-menu.png) en el nivel de proyecto, haciendo clic en **Volver a calcular finanzas**.
