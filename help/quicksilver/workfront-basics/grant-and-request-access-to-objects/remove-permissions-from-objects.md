---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Eliminación de permisos de objetos
description: Puede quitar los permisos de otros usuarios en los objetos a los que tiene acceso para compartir. La eliminación de permisos de los objetos es idéntica para todos los objetos que se pueden compartir.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

# Eliminación de permisos de objetos

<!--Audited: 01/2024-->

Puede quitar los permisos de otros usuarios en los objetos a los que tiene acceso para compartir. La eliminación de permisos de los objetos es idéntica para todos los objetos que se pueden compartir.

Consideraciones similares a las de los objetos compartidos se aplican a la eliminación de permisos de los objetos. Para obtener más información, vea la sección [Consideraciones sobre cómo compartir objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) en el artículo [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Requisitos de acceso

Debe tener lo siguiente para compartir objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Workfront*</td> 
   <td> <p>Nueva licencia: Colaborador o superior</p>
   O  
   <p>Licencia actual: Solicitud o superior</p>
   <p><b>NOTA</b></p>

<p>Algunos objetos requieren un acceso mayor que el de Solicitud. </p>

<p>Por ejemplo, para la nueva licencia, un colaborador puede compartir problemas, pero solo los usuarios con licencia estándar pueden compartir un proyecto.</p>

<p>Para la licencia actual, un solicitante puede compartir problemas, pero solo los trabajadores o los planificadores pueden compartir un proyecto.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Ver el acceso o superior a los objetos que desea compartir</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permite ver los permisos o superior de los objetos que desea compartir</p> <p>Administración de permisos para eliminar permisos heredados en objetos</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront. Para obtener más información, consulte [Requisitos de acceso para la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Eliminación de entidades de la lista de uso compartido de un objeto {#remove-entities-from-the-sharing-list-of-an-object}

Puede quitar entidades (usuarios, funciones, equipos, grupos y empresas) de la lista de uso compartido de un objeto. Quita sus permisos para el objeto.

1. Vaya al objeto del que desee quitar permisos.

   Para obtener información acerca de los objetos que se pueden compartir, vea [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Condicional) Para programas, portafolios y documentos, haga lo siguiente:

   1. Haga clic en el icono **Más** ![](assets/more-icon.png)junto al nombre del objeto y, a continuación, haga clic en **Compartir** o en **Compartir.**

      ![](assets/share-a-document-350x160.png)

   1. Haga clic en **x** junto al nombre de un usuario, equipo, grupo, empresa o rol para quitarlos en el cuadro de acceso a objetos.

      ![](assets/remove-permissions-on-portfolio.png)

   1. En el acceso Workfront de **&lt; Nombre de usuario > se eliminará de este menú desplegable de**, seleccione si desea que su acceso se elimine únicamente del objeto que ha seleccionado o de todos los objetos secundarios asociados a él.

1. (Condicional) Para proyectos, tareas y problemas, haga lo siguiente:

   1. Haga clic en **Compartir** a la derecha del nombre del objeto.

      ![](assets/new-share-button.png)
   1. Busque el usuario, la función, el equipo, el grupo o la compañía que desee quitar del objeto.
   1. Haga clic en **Quitar**.
En el menú desplegable **Quitar &lt; Nombre de usuario > de**, seleccione si desea que su acceso se elimine sólo del objeto que ha seleccionado, o de todos los objetos secundarios asociados a él.

      ![](assets/remove-permissions-on-project-nwe-350x479.png)

   Existen los siguientes escenarios:

   * Si quita la entidad sólo del objeto, esa entidad pierde sus permisos sobre el objeto y sus permisos heredados sobre los objetos secundarios. Si anteriormente se les habían concedido permisos para los elementos secundarios de forma individual, conservan los mismos permisos en todos los objetos secundarios asociados a él al seleccionar esta opción.
   * Si se quita la entidad del objeto y de todos los objetos secundarios, dicha entidad pierde sus permisos sobre el objeto y sobre todos los objetos secundarios, incluso cuando anteriormente se les había concedido permiso individual sobre cada objeto secundario.

1. Haga clic en **Guardar**.

## Eliminación de permisos de varios objetos de forma masiva

Puede eliminar entidades (usuarios, funciones, equipos, grupos y empresas) de varios objetos a la vez cuando los selecciona por lotes en una lista.

>[!NOTE]
>
>No puede ver qué entidades de acceso tienen para todos los objetos seleccionados cuando los selecciona de forma masiva. Debe saber qué entidad desea eliminar del uso compartido de los objetos seleccionados antes de eliminar sus permisos.

1. Vaya a la lista de objetos que desea compartir.

   Para obtener información acerca de los objetos que se pueden compartir, vea [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Seleccione varios objetos de la lista y, a continuación, haga clic en el icono **Compartir** ![](assets/share-icon.png)en la parte superior de la lista.
1. Escriba el nombre del usuario, rol, equipo, grupo o compañía para el que desea quitar el acceso en el campo **Editar acceso de `<Object Name>` a**.
1. En el menú desplegable de acceso, seleccione **Sin acceso**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. En el elemento Workfront del elemento `<User Name>` se quitará el acceso a este menú desplegable, seleccione si desea que su acceso se quite sólo de los objetos que ha seleccionado, o de todos los objetos secundarios asociados a él.\
   Existen los siguientes escenarios:

   * Si quita la entidad sólo del objeto, esa entidad pierde sus permisos sobre el objeto y sus permisos heredados sobre los objetos secundarios. Si anteriormente se les habían concedido permisos para los elementos secundarios de forma individual, conservan los mismos permisos en todos los objetos secundarios asociados a él al seleccionar esta opción. 
   * Si se quita la entidad del objeto y de todos los objetos secundarios, dicha entidad pierde sus permisos sobre el objeto y sobre todos los objetos secundarios, incluso cuando anteriormente se les había concedido permiso individual sobre cada objeto secundario.

   **Ejemplo:** Seleccione si desea quitar permisos sólo a las tareas seleccionadas en una lista o a los problemas y documentos adjuntos a las tareas.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Opcional) Para cambiar los permisos de forma masiva para varios objetos, seleccione otro nivel de uso compartido para la entidad seleccionada.

   Por ejemplo, si tienen permisos de administración, seleccione Contribute o Ver en su lugar.

1. Haga clic en **Guardar**.

## Eliminación de permisos heredados

Los permisos heredados se pueden eliminar de los objetos, lo que permite a los propietarios identificar específicamente quién tendrá acceso a los objetos secundarios, independientemente del acceso de un usuario a un objeto principal.

>[!IMPORTANT]
>
>Solo los usuarios con permiso de administración pueden quitar los permisos heredados.

Para eliminar permisos heredados:

1. Vaya a un objeto para el que tenga permisos de administración. Por ejemplo, ir a una tarea.
1. Vaya al cuadro de acceso a objetos como se describe en la sección [Quitar entidades de la lista de uso compartido de un objeto](#remove-entities-from-the-sharing-list-of-an-object) de este artículo.
1. Seleccione **x** junto a **Permiso heredado** en el cuadro para compartir para quitar a cualquiera que aparezca allí.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   Esto garantiza que nadie que tenga permisos concedidos para el objeto principal (por ejemplo, el proyecto) tenga permisos para esta tarea de forma predeterminada. Debe enumerar  entidades individuales en la lista de uso compartido de la tarea para conceder permisos sobre la tarea.

   >[!TIP]
   >
   >No se pueden quitar entidades individuales de la lista Permisos heredados. Solo puede desactivar los Permisos heredados para todas las entidades enumeradas.

1. Haga clic en **Guardar**. 

## Convertir un objeto en privado

Si ha compartido un objeto en todo el sistema o lo ha compartido con usuarios externos haciéndolo público, puede hacerlo privado de nuevo eliminando los permisos públicos o de todo el sistema. 

Para obtener más información sobre cómo hacer que un objeto esté disponible en todo el sistema o de manera pública, vea [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Para convertir un objeto en privado:

1. Vaya al objeto que desea convertir en privado.\
   Por ejemplo, navegue hasta un informe.
1. Haga clic en **Acciones de informe** y luego en **Compartir**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Haga clic en **Eliminar acceso público** para eliminar el acceso de los usuarios externos a la visualización del informe.
1. Haga clic en **Eliminar acceso en todo el sistema** para dejar de compartirlo con todos los usuarios de Workfront. 
1. Haga clic en **Guardar**.
