---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Resumen de la conciliación de asignaciones de recursos entre proyectos e iniciativas
description: Resumen de la conciliación de asignaciones de recursos entre proyectos e iniciativas
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Resumen de la conciliación de asignaciones de recursos entre proyectos e iniciativas

>[!IMPORTANT]
>
>Su organización debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para poder ver la información de la iniciativa de un proyecto. Para obtener información sobre la obtención de [!DNL Workfront Scenario Planner], consulte [Acceso necesario para utilizar el Scenario Planner](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Puede conectar proyectos con iniciativas para garantizar que sus planes estratégicos y el trabajo real estén sincronizados. A medida que esboza sus planes estratégicos e iniciativas en la [!DNL Scenario Planner] además de planificar el trabajo real de un proyecto, puede asegurarse de que los recursos tanto del proyecto como de las iniciativas coincidan, de modo que no se sobreasignen ni se infrautilicen.

## Requisitos previos

Antes de empezar, debe tener lo siguiente:

* Un plan en la [!DNL Scenario Planner] con una iniciativa conectada a un proyecto.
* Asignaciones de funciones requeridas para la iniciativa.
* Tareas o problemas en el proyecto que tienen horas planificadas y están asignados a una de las siguientes opciones:

   * Roles
   * Usuarios asociados con roles

## Conectar proyectos e iniciativas

>[!NOTE]
>
>Puede crear iniciativas y conectarlas a proyectos solo si su organización ha adquirido una licencia adicional para [!DNL Workfront Scenario Planner].

Puede conectar proyectos con iniciativas mediante una de las siguientes acciones:

* Importar proyectos a un plan como nuevas iniciativas

   Para obtener más información, consulte [Proyectos importados a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publicación de iniciativas en proyectos

   Para obtener más información, consulte [Actualice o cree proyectos publicando iniciativas en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Ambos procesos crean una conexión entre los proyectos y sus iniciativas correspondientes. Después de conectarlos, puede administrar sus asignaciones de recursos comparándolos y asegurándose de que coincidan.

## Consideraciones sobre la reconciliación de recursos en proyectos e iniciativas vinculados

>[!NOTE]
>
>Puede ver iniciativas, conectarlas a proyectos y ver sus asignaciones de recursos en un proyecto solo si su organización ha adquirido una licencia adicional para [!DNL Workfront Scenario Planner].

* Puede asignar usuarios, equipos y funciones de trabajo a elementos de trabajo en un proyecto, así como funciones de trabajo a iniciativas. Como resultado, solo puede reconciliar funciones del puesto entre proyectos e iniciativas.

   >[!TIP]
   >
   >Para reconciliar el tiempo de los usuarios en un proyecto con las asignaciones de roles en las iniciativas, debe asociar los usuarios con los roles.

* Puede ver la asignación de funciones de iniciativa en un proyecto vinculado en las siguientes áreas del proyecto:

   * [!DNL Scenario Planner] de la sección [!UICONTROL Detalles del proyecto] área de un proyecto. Para obtener más información, consulte los siguientes artículos:

      * [Actualice o cree proyectos publicando iniciativas en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Administrar información en el proyecto [!UICONTROL Información general] área](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >No puede ver la información de funciones del proyecto y de la iniciativa en paralelo en [!DNL Scenario Planner] de la sección [!UICONTROL Detalles del proyecto].

   * El [!UICONTROL Asignación de funciones] Panel en las siguientes áreas:

      * [!UICONTROL Distribuidor de cargas de trabajo] del proyecto

         Para obtener información sobre cómo ver y reconciliar las asignaciones de funciones entre la iniciativa y el proyecto vinculado en la [!UICONTROL Distribuidor de cargas de trabajo], consulte [Mostrar la asignación de funciones para proyectos e iniciativas en [!UICONTROL Distribuidor de cargas de trabajo]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL Tareas] sección

         Para obtener información sobre cómo reconciliar las asignaciones de funciones entre la iniciativa y el proyecto vinculado en la [!UICONTROL Tareas] sección, consulte [Mostrar la asignación de funciones para proyectos e iniciativas en la lista de tareas](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >Puede ver la información de funciones del proyecto y de la iniciativa en paralelo en [!UICONTROL Asignación de funciones] panel.



* No puede ver la asignación de funciones de un proyecto en una iniciativa vinculada. Para obtener más información, consulte [Proyectos importados a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
