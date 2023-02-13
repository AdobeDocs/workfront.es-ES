---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definir tipos de solicitud para un proyecto
description: Puede organizar el tipo de problemas o solicitudes que se registran en Adobe Workfront mediante tipos de solicitud.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# Definir tipos de solicitud para un proyecto

Puede organizar el tipo de problemas o solicitudes que se registran en Adobe Workfront mediante tipos de solicitud.

Esta organización es útil para generar informes y para ayudar a los usuarios a comprender qué tipo de trabajo inesperado puede producirse durante la duración de un proyecto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan de Adobe Workfront</a>*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Licencia de Adobe Workfront</a>*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de empezar, debe

* Tener o crear un proyecto

   Para obtener información sobre la creación de proyectos, consulte [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

## Consideraciones sobre los tipos de solicitud

* Puede especificar el tipo de problemas o solicitudes que se pueden registrar en un proyecto al configurar la variable **Detalles de cola** para el proyecto.
* No es necesario permitir que el proyecto sea una cola de solicitudes para poder definir los tipos de solicitud de un proyecto. Los problemas registrados en un proyecto se pueden etiquetar con un tipo de solicitud diferente.
* Si agrega temas de cola al proyecto, debe definir los tipos de solicitud en cada tema de cola para mostrarlo al agregar un nuevo problema o solicitud. Para obtener más información, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definir los tipos de problema o solicitud de un proyecto

1. Haga clic en **Proyectos** en el menú principal. ![](assets/main-menu-icon.png)

1. Haga clic en el nombre del proyecto para abrirlo.
1. En el panel izquierdo, haga clic en **Detalles de cola**.
1. En el **Propiedades de cola** seleccione **Tipos de solicitud** para el proyecto.

   >[!NOTE]
   >
   >Debe tener seleccionado al menos un tipo de solicitud. Puede seleccionar varios tipos de solicitud.

   Seleccione entre los siguientes tipos:

   * Informe de errores
   * Solicitud de cambio
   * Problema
   * Solicitud

   >[!TIP]
   >
   >Es posible que el administrador de Workfront haya cambiado el nombre de algunas de estas opciones. Para obtener más información, consulte [Configurar tipos de solicitud](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Haga clic en **Guardar**.

   Los tipos de solicitud especificados estarán disponibles para seleccionarlos cuando introduzca un nuevo problema en una tarea o proyecto, o cuando envíe una nueva solicitud al proyecto, si el proyecto está habilitado como cola de solicitudes.
