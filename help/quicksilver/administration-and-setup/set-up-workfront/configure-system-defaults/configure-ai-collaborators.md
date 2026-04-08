---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Configuración de colaboradores de IA
description: Como administrador de Adobe Workfront, puede configurar los colaboradores de IA y asignarlos a proyectos y tareas.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: 25d5fef46bc8f02e92d778685c2ad6e93439f9ff
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 8%

---

# Configuración de colaboradores de IA

{{highlighted-preview-article-level}}

Los colaboradores de IA son una forma de incorporar agentes de IA en sus proyectos y tareas. Puede configurar un colaborador de IA y, a continuación, asignarlo como lo haría con un usuario.

Por ejemplo, puede configurar un colaborador de IA de tipo revisor con directrices de marca y, a continuación, asignar ese colaborador para que revise un documento.

Los tipos de AI Collaborator disponibles incluyen:

* Revisor: cree un colaborador con marcas<!-- or Adobe Brand Intelligence--> y, a continuación, asígnelo como revisor en los recursos.

  Para obtener más información, consulte [Introducción al Revisor de contenido de Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

  >[!NOTE]
  >
  >Actualmente, Revisor es el único tipo de colaborador de IA disponible. En el futuro habrá más funciones de AI Collaborator disponibles.


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Standard, Prime o Ultimate</p></td> 
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



* Su organización debe tener registrado un Contrato de IA de Adobe Gen firmado.

  Para obtener más información, consulte [Firmar el acuerdo de IA general de Adobe](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) en el artículo Asistente de IA en Workfront.
* Debe tener configurada una marca en Workfront para poder utilizarla en un colaborador de IA de tipo revisor.

  Para obtener instrucciones, consulte [Crear y administrar marcas para el revisor de contenido](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Crear un nuevo colaborador de IA de tipo revisor

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. Haga clic en **Nuevo colaborador** en la esquina superior derecha de la pantalla.
1. Haz clic en **Revisor** y luego haz clic en **Continuar**.

   >[!NOTE]
   >
   >Actualmente, solo está disponible el tipo Revisor. En el futuro habrá más tipos de colaborador de IA disponibles.

1. En el campo Nombre del colaborador, introduzca un nombre para el colaborador. Este es el nombre que aparece en la lista de usuarios asignados disponibles en una tarea.
   <!--1. Select whether the collaborator will use a brand or Adobe Brand Intelligence for its reviews.-->
   <!--1. (Conditional) If the AI Collaborator will use Adobe Brand Intelligence, select the tenant that it will use.-->
1. <!--(Conditional) If the AI Collaborator will use a Brand,-->Seleccione la marca y la guía de marca que utilizará.
1. Haga clic en **Guardar**.

## Administrar colaboradores de IA

Puede editar, copiar y eliminar colaboradores de IA existentes.

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. (Condicional) Para editar un Collaborator, haga clic en el nombre del Collaborator que desee editar, realice las modificaciones que desee en la ventana Editar Collaborator y haga clic en **Guardar**.
1. (Condicional) Para copiar un Collaborator, haga clic en el icono Copiar ![Icono Copiar](assets/copy-ai-collaborator.png) en la fila del AI Collaborator que desee copiar, haga clic en el nombre de la copia, realice las modificaciones que desee en la ventana Editar Collaborator y haga clic en **Guardar**.
1. (Condicional) Para eliminar un Collaborator, haga clic en el icono Eliminar ![Icono Eliminar](assets/delete-collaborator-icon.png) en la fila del AI Collaborator que desee eliminar y, a continuación, haga clic en **Eliminar**.
