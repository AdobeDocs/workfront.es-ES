---
title: Uso de colaboradores de tareas
content-type: reference
description: Aprenda a utilizar los colaboradores de tareas y los colaboradores de IA que se pueden asignar a tareas de Workfront.
author: Becky
feature: Work Management, Tasks
source-git-commit: 2070a27e18d768dd14ce4f5c681ab08669c81766
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 8%

---

# Uso de colaboradores de tareas

{{highlighted-preview-article-level}}

Los colaboradores de tareas son colaboradores de IA que se pueden asignar directamente a tareas de Workfront, además del colaborador de IA del tipo revisor existente que se utiliza para revisiones de documentos y recursos. Al igual que otros colaboradores de IA, los colaboradores de tareas se configuran en el área de Configuración y se asignan a tareas igual que un usuario.

Los colaboradores de tareas se conectan a los agentes que ha configurado, como un servidor MCP.

Para obtener información e instrucciones sobre cómo crear un colaborador de tareas en Workfront, consulte [Configuración de un colaborador de tareas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) en el artículo Configuración de colaboradores de IA.

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
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

* Debe configurar un agente en Copilot, Claude o Writer.ai para poder utilizarlo como colaborador de tareas.

## Información general de Task Collaborator

Los colaboradores de tareas son una forma de asignar agentes de MCP a tareas específicas en Workfront. El agente se configura en una aplicación como Copilot Studio, Claude o Writer.ai y, a continuación, se conecta a Workfront como colaborador de tareas. A continuación, puede asignarlo a tareas como lo haría con un usuario.

Algunos flujos de trabajo de ejemplo pueden incluir:

* Detectar imágenes cargadas en una tarea, generar variaciones basadas en criterios determinados al agente y cargar las nuevas imágenes en la tarea.
* Generar una copia a partir de una descripción de tarea, revisar la copia según las directrices configuradas en el agente y publicar una copia en el flujo de actualización.
* Leer los detalles de un evento, identificar los detalles que faltan y publicar preguntas en el flujo de actualización sobre los detalles que faltan.

>[!NOTE]
>
>* Los detalles específicos sobre las responsabilidades y capacidades de un agente se configuran en la aplicación en la que se crea el agente, no en Workfront.
>* Actualmente, los colaboradores de tareas admiten agentes creados en Copilot Studio, Claude y Writer.ai.
>* Al configurar un agente en Copilot Studio, debe establecer la seguridad en **Sin autenticación**.
>* Para obtener información e instrucciones sobre cómo crear un colaborador de tareas en Workfront, consulte [Configuración de un colaborador de tareas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) en el artículo Configuración de colaboradores de IA.

## Asignar un colaborador de tareas a una tarea

Los colaboradores de tareas se asignan a las tareas del mismo modo que se asignan a los usuarios.

Para obtener instrucciones, consulte [Asignar tareas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).
