---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Visión general de la conciliación de las asignaciones de recursos entre proyectos e iniciativas
description: Visión general de la conciliación de las asignaciones de recursos entre proyectos e iniciativas
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Visión general de la conciliación de las asignaciones de recursos entre proyectos e iniciativas

>[!IMPORTANT]
>
>Su organización debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para que pueda ver la información de la iniciativa de un proyecto. Para obtener información sobre cómo obtener la variable [!DNL Workfront Scenario Planner], consulte [Acceso necesario para utilizar el planificador de escenarios](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Puede conectar proyectos con iniciativas para garantizar que sus planes estratégicos y el trabajo real estén sincronizados. A medida que describe sus planes e iniciativas estratégicos en el [!DNL Scenario Planner] y si planifica el trabajo real en un proyecto, puede asegurarse de que sus recursos tanto en el proyecto como en las iniciativas coincidan, de modo que no los sobreasignará ni los usará insuficientemente.

## Requisitos previos

Antes de comenzar, debe tener lo siguiente:

* Un plan en el [!DNL Scenario Planner] con una iniciativa relacionada con un proyecto.
* Se necesitan asignaciones de funciones para la iniciativa.
* Tareas o problemas en el proyecto que tengan horas planificadas y que se asignen a uno de los siguientes elementos:

   * Roles
   * Usuarios asociados a funciones de trabajo

## Conectar proyectos e iniciativas

>[!NOTE]
>
>Puede crear iniciativas y conectarlas a proyectos solo si su organización ha adquirido una licencia adicional para [!DNL Workfront Scenario Planner].

Puede conectar proyectos con iniciativas realizando una de las siguientes acciones:

* Importar proyectos en un plan como nuevas iniciativas

   Para obtener más información, consulte [Importar proyectos a planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publicar iniciativas en proyectos

   Para obtener más información, consulte [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Ambos procesos crean una conexión entre los proyectos y sus iniciativas correspondientes. Después de conectarlos, puede administrar sus asignaciones de recursos comparándolas y asegurándose de que coincidan.

## Consideraciones sobre la conciliación de recursos en proyectos e iniciativas vinculados

>[!NOTE]
>
>Puede ver iniciativas, conectarlas a proyectos y ver sus asignaciones de recursos en un proyecto solo si su organización ha adquirido una licencia adicional para [!DNL Workfront Scenario Planner].

* Puede asignar usuarios, equipos y funciones de trabajo a elementos de trabajo de un proyecto y asignar funciones de trabajo a iniciativas. Como resultado, solo puede reconciliar funciones de trabajo entre proyectos e iniciativas.

   >[!TIP]
   >
   >Para reconciliar el tiempo de los usuarios en un proyecto con las asignaciones de funciones en las iniciativas, debe asociar usuarios con funciones de trabajo.

* Puede ver la asignación de funciones de trabajo de iniciativa en un proyecto vinculado en las siguientes áreas del proyecto:

   * [!DNL Scenario Planner] de la sección [!UICONTROL Detalles del proyecto] de un proyecto. Para obtener más información, consulte los siguientes artículos:

      * [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Administrar información en el proyecto [!UICONTROL Información general] area](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >No puede ver la información de la función de trabajo del proyecto y de la iniciativa en paralelo en la [!DNL Scenario Planner] de la sección [!UICONTROL Detalles del proyecto].

   * La variable [!UICONTROL Asignación de funciones] en las siguientes áreas:

      * [!DNL Workload Balancer] del proyecto

         Para obtener información sobre cómo ver y reconciliar las asignaciones de funciones entre la iniciativa y el proyecto vinculado en la variable [!DNL Workload Balancer], consulte [Mostrar la asignación de funciones para proyectos e iniciativas en el [!DNL Workload Balancer]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL Tareas] sección

         Para obtener información sobre cómo reconciliar las asignaciones de funciones entre la iniciativa y el proyecto vinculado en la variable [!UICONTROL Tareas] consulte [Mostrar la asignación de funciones para proyectos e iniciativas en la lista de tareas](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >Puede ver la información de funciones del trabajo del proyecto y de la iniciativa en paralelo en [!UICONTROL Asignación de funciones] panel.



* No puede ver la asignación de funciones de trabajo para un proyecto en una iniciativa vinculada. Para obtener más información, consulte [Importar proyectos a planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
