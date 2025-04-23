---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definición de Tipos de Solicitudes para un Proyecto
description: Puede organizar el tipo de problemas o solicitudes que se registran en Adobe Workfront por tipos de solicitud.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 6311526ddf9143c4a979d8bbac96312a3b0e8151
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 22%

---

# Definición de tipos de solicitud para un proyecto

Puede organizar el tipo de problemas o solicitudes que se registran en Adobe Workfront por tipos de solicitud.

Esta organización resulta útil por motivos de creación de informes y para ayudar a los usuarios a comprender qué tipo de trabajo inesperado puede producirse durante la duración de un proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
    <p>Nuevo: estándar</p>
    <p>o</p>
    <p>Actual: plan</p></td>  
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

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de empezar, debe hacer lo siguiente:

* Tener o crear un proyecto

  Para obtener información sobre cómo crear proyectos, vea [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

## Consideraciones sobre los tipos de solicitud

* Puede especificar el tipo de problemas o solicitudes que se pueden registrar en un proyecto al configurar el área de **Detalles de la cola** para el proyecto.
* No es necesario habilitar el proyecto para que sea una cola de solicitudes y poder definir los tipos de solicitudes de un proyecto. Cualquier problema registrado para un proyecto puede etiquetarse con un tipo de solicitud diferente.
* Si agrega Temas de colas al proyecto, debe definir Tipos de solicitudes en cada tema de la cola para mostrarlo al agregar un nuevo problema o solicitud. Para obtener más información, consulte [Crear temas de la cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Definición del problema o los tipos de solicitud de un proyecto

{{step1-to-projects}}

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
