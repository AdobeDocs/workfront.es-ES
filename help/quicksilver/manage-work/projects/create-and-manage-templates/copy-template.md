---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiar una plantilla de proyecto
description: En lugar de crear una nueva plantilla de proyecto desde cero, puede copiar una plantilla existente y realizar cambios en ella, si es necesario.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# Copiar una plantilla de proyecto

En lugar de crear una nueva plantilla de proyecto desde cero, puede copiar una plantilla existente y realizar cambios en ella, si es necesario.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a plantillas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores a una plantilla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.


## Consideraciones sobre la copia de plantillas

Los siguientes elementos siempre se copian de un proyecto existente a uno nuevo:

* Tareas de plantilla
* Información predeterminada de tarea de plantilla (proceso de aprobación predeterminado de tarea, Forms personalizado predeterminado de tarea)
* Formularios personalizados
* Riesgos
* Información de configuración de cola
* Portfolio y programa
* Rutas de aprobación
* Documentos
* Los días de las tareas de plantilla originales se transfieren a la nueva plantilla. Debe cambiar el día de inicio o finalización de la plantilla (según su modo de programación) para actualizar los días de las tareas de plantilla, si es necesario.

Los siguientes elementos nunca se copian de un proyecto existente en uno nuevo:

* Tarifas de facturación
* Comentarios del usuario

## Copiar una plantilla

1. Vaya a la plantilla que desee copiar.
1. Haga clic en el menú **Más** ![](assets/qs-more-icon-on-an-object.png) y luego haga clic en **Copiar**.
1. Especifique un nombre para la plantilla en el campo **Nuevo nombre de plantilla**.

   De manera predeterminada, el nuevo nombre es **Copia de `<original template name>`.**

1. Seleccione si desea **Conservar asignaciones de usuarios en tareas y plantillas**: seleccione esta opción para transferir todas las asignaciones de tareas y plantillas de la plantilla original a la nueva plantilla.
1. Haga clic en **Guardar** para crear una copia de la plantilla.
