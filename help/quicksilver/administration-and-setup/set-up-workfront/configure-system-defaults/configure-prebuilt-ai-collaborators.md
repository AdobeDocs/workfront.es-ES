---
user-type: administrator
product-area: system-administration;setup
title: Configuración de colaboradores de IA pregenerados
description: Como administrador de Adobe Workfront, puede configurar los colaboradores de IA creados previamente desde Adobe, como el coordinador de admisión, como agentes de trabajo que los usuarios pueden asignar a tareas y problemas.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c95c5a71a2706d4ddbf3e53a579b348bd072a04e
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 8%
---
# Configuración de colaboradores de IA pregenerados

## Información general

Los colaboradores de IA creados previamente son agentes de trabajo listos para usar de Adobe que están configurados para hacer un trabajo específico, como comprobar solicitudes de información que falta. Están disponibles como agentes de trabajo nativos de Adobe, por lo que no es necesario configurar un agente en una plataforma externa ni proporcionar credenciales de plataforma externa.

Al configurar un agente de trabajo, se selecciona un Collaborator creado previamente como origen del agente. A continuación, puede asignar un nombre al agente de trabajo, establecer su nivel de acceso y elegir las acciones que puede realizar. Los usuarios asignan el agente de trabajo configurado a tareas o problemas de la misma manera que asignan cualquier otro agente de trabajo. Los usuarios no necesitan saber que el agente es un Collaborator creado previamente.

Para obtener más información acerca de los agentes de trabajo y otros tipos de colaboradores de IA, consulte [Configurar colaboradores de IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Seleccionar, Prime o Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema] o Administrador de grupo</td> 
  </tr> 
  </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Su organización debe tener Adobe CX Coworker habilitado. Para obtener más información, consulte [Información general sobre CX Enterprise Coworker en Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

## Configuración de un colaborador de IA creado previamente

Puede configurar un colaborador de IA creado previamente al configurar un agente de trabajo. En el área **Elegir el origen del agente**, seleccione **Adobe Native** y, a continuación, seleccione el Collaborator generado previamente que desee utilizar en la lista siguiente.

Para ver los pasos completos, consulte [Configurar un agente de trabajo en Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront).

Una vez configurado el Collaborator, los usuarios podrán asignarlo a tareas o problemas. Para obtener más información, vea [Usar agentes de trabajo](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

## Colaboradores de IA creados previamente disponibles

### CX Enterprise Coworker {#cx-enterprise-coworker}

Un agente de CX Enterprise Coworker con tecnología de Adobe Agent Orchestrator.

Para obtener más información, consulte [Información general sobre CX Enterprise Coworker en Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

### Coordinador de admisión {#intake-coordinator}

El coordinador de admisión comprueba los detalles, los formularios personalizados y los archivos adjuntos de las solicitudes en busca de información que falte, que no sea clara o incoherente. Publica comentarios o realiza cambios con la aprobación del usuario.

>[!NOTE]
>
>Puede asignar el coordinador de admisión a una regla de enrutamiento cuando se cree la regla, pero no puede asignarla posteriormente.

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
