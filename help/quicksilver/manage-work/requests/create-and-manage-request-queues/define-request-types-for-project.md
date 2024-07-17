---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definición de tipos de solicitud para un proyecto
description: Puede organizar el tipo de problemas o solicitudes que se registran en Adobe Workfront por tipos de solicitud.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 2%

---

# Definición de tipos de solicitud para un proyecto

Puede organizar el tipo de problemas o solicitudes que se registran en Adobe Workfront por tipos de solicitud.

Esta organización resulta útil por motivos de creación de informes y para ayudar a los usuarios a comprender qué tipo de trabajo inesperado puede producirse durante la duración de un proyecto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan Adobe Workfront</a>*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Resumen de licencias</a>*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en un proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de empezar, debe hacer lo siguiente:

* Tener o crear un proyecto

  Para obtener información sobre cómo crear proyectos, vea [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

## Consideraciones sobre los tipos de solicitud

* Puede especificar el tipo de problemas o solicitudes que se pueden registrar en un proyecto al configurar el área de **Detalles de la cola** para el proyecto.
* No es necesario habilitar el proyecto para que sea una cola de solicitudes y poder definir los tipos de solicitudes de un proyecto. Cualquier problema registrado para un proyecto puede etiquetarse con un tipo de solicitud diferente.
* Si agrega Temas de colas al proyecto, debe definir Tipos de solicitudes en cada tema de la cola para mostrarlo al agregar un nuevo problema o solicitud. Para obtener más información, vea [Crear temas de colas](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definición del problema o los tipos de solicitud de un proyecto

1. Haga clic en **Proyectos** en el menú principal. ![](assets/main-menu-icon.png)

1. Haga clic en el nombre del proyecto para abrirlo.
1. En el panel izquierdo, haga clic en **Detalles de cola**.
1. En la sección **Propiedades de cola**, seleccione los **tipos de solicitud** que desee para el proyecto.

   >[!NOTE]
   >
   >Debe haber seleccionado al menos un tipo de solicitud. Puede seleccionar varios tipos de solicitud.

   Seleccione entre los siguientes tipos:

   * Informe de errores
   * Solicitud de cambio
   * Problema
   * Solicitud

   >[!TIP]
   >
   >Es posible que el administrador de Workfront haya cambiado el nombre de algunas de estas opciones. Para obtener más información, consulte [Configurar tipos de solicitudes](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Haga clic en **Guardar**.

   Los tipos de solicitud especificados estarán disponibles para seleccionarlos cuando se escriba un nuevo problema en una tarea o proyecto, o cuando se envíe una nueva solicitud al proyecto, si el proyecto está habilitado como cola de solicitudes.
