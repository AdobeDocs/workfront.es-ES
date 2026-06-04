---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definición de Tipos de Solicitudes para un Proyecto
description: Puede organizar el tipo de problemas o solicitudes que se registran en Adobe Workfront por tipos de solicitud.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fOdoie2wI-EHoKmQTHy0cDaVipi6XYE1JgMHdX6-Tbo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 21%

---

# Definir tipos de solicitud para un proyecto

<!-- Audited: 6/2025 -->

Puede organizar el tipo de problemas o solicitudes que se registran en Adobe Workfront por tipos de solicitud. Esto resulta útil por motivos de creación de informes y para ayudar a los usuarios a comprender qué tipo de trabajo inesperado puede producirse durante la duración de un proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
    <p>Estándar</p>
    <p>Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en un proyecto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de empezar, debe hacer lo siguiente:

* Tener o crear un proyecto.

  Para obtener información sobre cómo crear proyectos, vea [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

## Consideraciones sobre los tipos de solicitud

* Puede especificar el tipo de problemas o solicitudes que se pueden registrar en un proyecto al configurar el área Detalles de cola del proyecto.
* No es necesario habilitar el proyecto para que sea una cola de solicitudes y poder definir los tipos de solicitudes de un proyecto. Cualquier problema registrado para un proyecto puede etiquetarse con un tipo de solicitud diferente.
* Si agrega Temas de colas al proyecto, debe definir Tipos de solicitudes en cada tema de la cola para mostrarlo al agregar un nuevo problema o solicitud. Para obtener más información, consulte [Crear temas de la cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definición del problema o los tipos de solicitud de un proyecto

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.
1. En el panel izquierdo, haga clic en **Detalles de cola**.
1. En la sección **Propiedades de cola**, seleccione los **tipos de solicitud** que desee para el proyecto:
   * Informe de errores
   * Solicitud de cambio
   * Problema
   * Solicitud

   >[!NOTE]
   >
   >* Debe haber seleccionado al menos un tipo de solicitud. Puede seleccionar varios tipos.
   >* Es posible que el administrador de Workfront haya cambiado el nombre de algunas de estas opciones. Para obtener más información, consulte [Configurar tipos de solicitudes](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Haga clic en **Guardar**. Los tipos de solicitud especificados estarán disponibles para seleccionarlos cuando se escriba un nuevo problema en una tarea o proyecto, o cuando se envíe una nueva solicitud al proyecto (si el proyecto está habilitado como cola de solicitudes).
