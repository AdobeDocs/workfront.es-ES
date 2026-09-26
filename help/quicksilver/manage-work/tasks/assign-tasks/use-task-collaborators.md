---
title: Usar agentes de trabajo
content-type: reference
description: Aprenda a utilizar agentes de trabajo y colaboradores de IA que se pueden asignar a tareas de Workfront.
author: Becky
feature: Work Management, Tasks
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 3%
---
# Usar agentes de trabajo

Los agentes de trabajo son colaboradores de IA que se pueden asignar directamente a tareas de Workfront, además del revisor de IA existente que se utiliza para revisiones de documentos y recursos. Al igual que otros colaboradores de IA, los agentes de trabajo se configuran en el área de Configuración y se asignan a tareas igual que un usuario.

Los agentes de trabajo se conectan a los agentes configurados en Copilot Studio, Claude o Writer.

Para obtener información e instrucciones sobre cómo crear un agente de trabajo en Workfront, consulte [Configurar un agente de trabajo](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) en el artículo Configurar colaboradores de IA.

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

* Debe configurar un agente en Copilot, Claude o Writer.ai antes de poder utilizarlo como agente de trabajo.

## Introducción al agente de trabajo

Los agentes de trabajo son una forma de asignar agentes MCP a tareas específicas en Workfront. El agente se configura en una aplicación como Copilot Studio, Claude o Writer.ai y, a continuación, se conecta a Workfront como agente de trabajo. A continuación, puede asignarlo a tareas como lo haría con un usuario.

Algunos flujos de trabajo de ejemplo pueden incluir:

* Detectar imágenes cargadas en una tarea, generar variaciones basadas en criterios determinados al agente y cargar las nuevas imágenes en la tarea.
* Generar una copia a partir de una descripción de tarea, revisar la copia según las directrices configuradas en el agente y publicar una copia en el flujo de actualización.
* Leer los detalles de un evento, identificar los detalles que faltan y publicar preguntas en el flujo de actualización sobre los detalles que faltan.

>[!NOTE]
>
>* Los detalles específicos sobre las responsabilidades y capacidades de un agente se configuran en la aplicación en la que se crea el agente, no en Workfront.
>* No es necesario agregar el servidor MCP de Workfront al agente utilizado como agente de trabajo y no es necesario conectarse para que funcione el agente de trabajo.
>* Actualmente, los agentes de trabajo son compatibles con los agentes creados en Copilot Studio, Claude y Writer.ai.
>* Al configurar un agente en Copilot Studio, debe establecer la seguridad en **Sin autenticación**.
>* Para obtener información e instrucciones sobre cómo crear un agente de trabajo en Workfront, consulte [Configurar un agente de trabajo](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) en el artículo Configurar colaboradores de IA.

## Información que lee un agente de trabajo

Cuando un agente de trabajo comienza a trabajar en una tarea, lee automáticamente la siguiente información de la tarea como contexto:

* Título de tarea
* Descripción de la tarea
* Comentarios en el flujo de actualización de la tarea
* Información de cualquier formulario personalizado adjunto a la tarea

Esta información siempre se lee y no se puede configurar como ajuste de Workfront.

>[!TIP]
>
>Para obtener los mejores resultados, recomendamos:
>
>* Incluya cualquier información de fondo que desee que el agente utilice directamente en la descripción de la tarea o en un campo de formulario personalizado relevante.
>* Asegúrese de que la tarea coincida con lo que el agente debe hacer. Por ejemplo, si su agente tiene instrucciones para traducir texto de inglés a francés, incluya el texto que desea traducir en la descripción de la tarea.

## Déclencheur de inicio del agente de trabajo

Cuando se asigna un agente de trabajo a una tarea, comienza a trabajar cuando se cumple cualquiera de las siguientes situaciones:

* El agente de trabajo está asignado a una tarea que está lista para iniciarse. (Por ejemplo, si la tarea tiene predecesoras, las predecesoras están completas).
* El agente de trabajo y un usuario se asignan a una tarea y el agente de trabajo se asigna primero.
* Una tarea a la que ya se ha asignado un agente de trabajo como está lista para iniciarse y el agente de trabajo es el único o el principal asignado. (Por ejemplo, si la tarea tiene predecesoras, las predecesoras están completas).
* Una tarea a la que ya se han asignado un agente de trabajo y un usuario está lista para iniciarse y el agente de trabajo se ha asignado primero o es el principal asignado. (Por ejemplo, si la tarea tiene predecesoras, las predecesoras están completas).
* Se asignan un usuario y un agente de trabajo a una tarea y se elimina el usuario.
* Un usuario y un agente de trabajo se asignan a una tarea y el agente de trabajo se establece como el principal asignado a la tarea.

Las siguientes situaciones no hacen que el agente de trabajo comience a trabajar en la tarea:

* Se asigna un agente de trabajo a una tarea que ya tiene un usuario asignado.
* Se @mentioned un agente de trabajo en una tarea.
* Se asigna un agente de trabajo a una tarea que ya tiene asignado un agente de trabajo. En este caso, el primer agente de trabajo asignado ya habrá comenzado el trabajo y el segundo agente de trabajo no hará nada.
* Se asigna un agente de trabajo a una tarea que no está lista para iniciarse. (Por ejemplo, si la tarea tiene predecesoras, las predecesoras aún no están completas).

## Asignar un agente de trabajo a una tarea

Los agentes de trabajo se asignan a las tareas del mismo modo que se asignan a los usuarios.

Cuando esté buscando un agente de trabajo en la lista de usuarios asignados disponibles, el nombre del agente de trabajo es solo un nombre.

Para obtener instrucciones, consulte [Asignar tareas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).

>[!NOTE]
>
>No se pueden asignar agentes de trabajo para revisar o aprobar un documento.

## Solución de problemas de agentes de trabajo

Si su agente de trabajo no devuelve una respuesta o salida, compruebe lo siguiente:

* Asegúrese de que el agente esté publicado en el lado del proveedor de la plataforma de IA.
* Asegúrese de que tiene suficientes créditos de IA con la plataforma de su agente.
* Asegúrese de que la acción realizada en la tarea no requiera un nivel de acceso específico.
* Si utiliza Copilot como proveedor de agentes, asegúrese de utilizar la configuración &quot;sin autenticación&quot;.
* Si utiliza Copilot, asegúrese de que su agente está configurado en un entorno global. Actualmente, la funcionalidad del agente de trabajo no admite versiones regionales de Copilot Studio.
* Asegúrese de que Collaborator es el principal usuario asignado a la tarea.
* Asegúrese de que la tarea a la que está asignado el agente de trabajo se puede iniciar. Por ejemplo, compruebe que todas las tareas predecesoras de esa tarea estén completas.

>[!TIP]
>
>También puede ir a la plataforma del proveedor de agentes y pedirle que realice la tarea dentro de la plataforma. Si el agente no puede realizar la tarea dentro de la plataforma, el agente de trabajo también tendrá problemas en Workfront.
