---
product-area: projects
navigation-topic: use-predecessors
title: Crear relaciones de predecesor encadenando tareas
description: Puede crear relaciones predecesoras de varias formas en Adobe Workfront. Un método es encadenar tareas.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 1%

---

# Crear relaciones de predecesor encadenando tareas

Puede crear relaciones predecesoras de varias formas en Adobe Workfront. Un método es encadenar tareas.

Para obtener información sobre las tareas predecesoras, consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Al encadenar tareas, puede permitir que el sistema cree automáticamente las relaciones predecesoras en las tareas seleccionadas, en lugar de crear manualmente una relación en cada tarea. Se pueden seguir utilizando diferentes tipos de relaciones predecesoras entre tareas.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Tareas de cadena para crear relaciones de predecesor

1. Vaya al proyecto que contiene las tareas que desea encadenar.
1. Haga clic en **Tareas** en el panel izquierdo.
1. (Condicional) Seleccione **Autoguardar** en la esquina superior derecha de la lista de tareas, seleccione las tareas que desea encadenar.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >No es posible encadenar tareas en una lista de tareas cuando se guardan manualmente cambios en tareas o se utiliza el modo de planificación de línea de tiempo para guardar tareas.

1. Haga clic con el botón derecho en las tareas seleccionadas y, a continuación, haga clic en **Cadena**.
1. Seleccione entre los siguientes tipos de dependencia:

   * **Finalizar-Iniciar**
   * **Finalizar-Finalizar**
   * **Iniciar-Iniciar**
   * **Iniciar-Finalizar**

   Para obtener más información sobre los tipos de dependencias predecesores, consulte [Descripción general de los tipos de dependencia de tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Opcional) Haga clic en **Desencadenar** si algunas de las tareas se han encadenado anteriormente.

   >[!CAUTION]
   >
   >Solo se eliminan los predecesores secuenciales mediante la opción unchain al editar tareas masivas.

   Las tareas seleccionadas ahora están vinculadas por relaciones predecesoras.
