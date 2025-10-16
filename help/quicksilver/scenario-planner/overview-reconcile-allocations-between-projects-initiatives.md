---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Visión General de Reconciliación de Asignaciones de Recursos entre Proyectos e Iniciativas
description: Información general sobre la conciliación de asignaciones de recursos entre proyectos e iniciativas
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 98%

---

# Información general sobre la conciliación de asignaciones de recursos entre proyectos e iniciativas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Puede conectar proyectos con iniciativas para garantizar que sus planes estratégicos y el trabajo real estén sincronizados. A medida que esquematiza sus planes estratégicos e iniciativas en [!DNL Scenario Planner] y planea el trabajo real en un proyecto, puede asegurarse de que los recursos del proyecto y de las iniciativas coincidan, de manera que no los sobreasigne ni los infrautilice.

## Requisitos previos

Antes de comenzar, debe tener lo siguiente:

* Un plan en [!DNL Scenario Planner] con una iniciativa conectada a un proyecto.
* Asignaciones de las funciones requeridas para la iniciativa.
* Tareas o problemas en el proyecto que tienen horas planificadas y están asignados a una de las siguientes opciones:

   * Roles
   * Usuarios asociados con funciones

## Conectar proyectos e iniciativas

>[!NOTE]
>
>Puede crear iniciativas y conectarlas a proyectos solamente si su organización ha adquirido una licencia adicional para [!DNL Workfront Scenario Planner].

Puede conectar proyectos con iniciativas mediante una de las siguientes acciones:

* Importar proyectos a un plan como nuevas iniciativas

  Para obtener más información, consulte [Importar proyectos a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publicar iniciativas en proyectos

  Para obtener más información, consulte [Actualizar o crear proyectos publicando iniciativas en  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Ambos procesos crean una conexión entre los proyectos y sus iniciativas correspondientes. Después de conectarlas, puede administrar sus asignaciones de recursos comparándolas y asegurándose de que coincidan.

## Consideraciones sobre la reconciliación de recursos en proyectos e iniciativas vinculados

>[!NOTE]
>
>Es posible ver iniciativas, conectarlas a los proyectos y ver sus asignaciones de recursos en un proyecto solamente si su organización ha adquirido una licencia adicional para [!DNL Workfront Scenario Planner].

* Puede asignar usuarios, equipos y funciones de trabajo a elementos de trabajo en un proyecto, así como funciones de trabajo a iniciativas. Como resultado, solo puede reconciliar funciones entre proyectos e iniciativas.

  >[!TIP]
  >
  >Para reconciliar el tiempo de los usuarios en un proyecto con las asignaciones de funciones en las iniciativas, debe asociar los usuarios con las funciones.

* Puede ver la asignación de funciones de iniciativa en un proyecto vinculado en las siguientes áreas del proyecto:

   * Sección [!DNL Scenario Planner] del área [!UICONTROL Detalles del proyecto] en un proyecto. Para obtener más información, consulte los siguientes artículos:

      * [Actualice o cree proyectos publicando iniciativas en  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Administrar información en el área [!UICONTROL Información general] del proyecto](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >No puede ver información sobre la función desde el proyecto y la iniciativa en paralelo en la sección [!DNL Scenario Planner] de [!UICONTROL Detalles del proyecto].

   * El panel [!UICONTROL Asignación de funciones] se encuentra en las siguientes áreas:

      * [!UICONTROL Distribuidor de cargas de trabajo] del proyecto

        Para obtener información sobre cómo ver y reconciliar las asignaciones de funciones entre la iniciativa y el proyecto vinculado en el [!UICONTROL Distribuidor de cargas de trabajo], consulte [Mostrar la asignación de funciones para proyectos e iniciativas en el [!UICONTROL Distribuidor de cargas de trabajo]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * Sección [!UICONTROL Tareas]

        Para obtener información acerca de cómo reconciliar las asignaciones de funciones entre la iniciativa y el proyecto vinculado en la sección [!UICONTROL Tareas], consulte [Mostrar asignación de funciones para proyectos e iniciativas en la lista de tareas](../scenario-planner/show-role-allocation-task-list-nwe.md).

     >[!TIP]
     >
     >Puede ver la información sobre la función desde el proyecto y la iniciativa en paralelo en el panel [!UICONTROL Asignación de funciones].

* No puede ver la asignación de funciones de un proyecto en una iniciativa vinculada. Para obtener más información, consulte [Importar proyectos a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
