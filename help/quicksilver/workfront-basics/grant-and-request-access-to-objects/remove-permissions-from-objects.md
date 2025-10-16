---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Quitar permisos de objetos
description: Es posible quitar los permisos de otros usuarios en los objetos a los que se tenga acceso de uso compartido. La eliminación de permisos de los objetos es idéntica para todos los objetos que se puedan compartir.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 82%

---

# Quitar permisos de objetos

<!--Audited: 01/2024-->

Es posible quitar los permisos de otros usuarios en los objetos a los que se tenga acceso de uso compartido. La eliminación de permisos de los objetos es idéntica para todos los objetos que se puedan compartir.

Consideraciones similares a las del uso compartido de objetos se aplican a la eliminación de permisos de los objetos. Para obtener más información, consulte la sección [Consideraciones sobre el uso compartido de objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) en el artículo [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p>
   <p><strong>Nota</strong>: algunos objetos requieren un acceso mayor que el de Solicitud.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior sobre los objetos que desea compartir</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores sobre los objetos que desea compartir</p> <p>Administración de permisos para eliminar permisos heredados en objetos</p>  </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminación de entidades de la lista de uso compartido de un objeto {#remove-entities-from-the-sharing-list-of-an-object}

Es posible quitar entidades (usuarios, funciones, equipos, grupos y empresas) de la lista de uso compartido de un objeto. Esto quita sus permisos sobre el objeto.

1. Vaya al objeto del que desee quitar permisos.

   Para obtener información acerca de los objetos que se pueden compartir, consulte [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Condicional) Para programas, portafolios y documentos, haga lo siguiente:

   1. Haga clic en el icono **Más** ![más icono](assets/more-icon.png)junto al nombre del objeto y, a continuación, haga clic en **Compartir** o **Compartir.**

      ![compartir](assets/share-a-document-350x160.png)

   1. Haga clic en la **x** que hay junto al nombre de un usuario, equipo, grupo, empresa o función para quitarlos en el cuadro de acceso a objetos.

      ![quitar permiso](assets/remove-permissions-on-portfolio.png)

   1. En el menú desplegable **[Nombre de usuario] se quitará el acceso a Workfront de este**, seleccione si desea que su acceso se quite sólo del objeto que ha seleccionado o de todos los objetos secundarios asociados a él.

1. (Condicional) Para proyectos, tareas y problemas, haga lo siguiente:

   1. Haga clic en **Compartir** a la derecha del nombre del objeto.

      ![compartir](assets/new-share-button.png)
   1. Busque el usuario, la función, el equipo, el grupo o la compañía que quiera quitar del objeto.
   1. Haga clic en **Quitar**.
En el menú desplegable **Quitar &lt; User Name > de**, seleccione si desea que su acceso se elimine solo del objeto seleccionado o de todos los objetos secundarios asociados a él.

      ![quitar](assets/remove-permissions-on-project-nwe-350x479.png)

   Se dan los siguientes escenarios:

   * Si quita la entidad solo del objeto, esa entidad perderá los permisos sobre el objeto y los permisos heredados sobre los objetos secundarios. Si anteriormente se les habían concedido permisos a los elementos secundarios de forma individual, conservarán los mismos permisos en todos los objetos secundarios asociados al seleccionar esta opción.
   * Si se quita la entidad del objeto y de todos los objetos secundarios, dicha entidad perderá los permisos sobre el objeto y sobre todos los objetos secundarios, incluso aunque anteriormente se les hubiera concedido permiso individual sobre cada objeto secundario.

1. Haga clic en **Guardar**.

<!--
## Remove permissions from several objects in bulk

You can remove entities (users, job roles, teams, groups, companies) from several objects at a time when you bulk select them in a list.

>[!NOTE]
>
>You cannot view what access entities have for all the objects selected when you select them in bulk. You must know which entity you want to remove from the sharing of the objects selected before removing their permissions.

1. Go to the list of objects that you want to share.

   For information about which objects can be shared, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Select several objects in the list, then click the **Share** icon ![share icon](assets/share-icon.png)at the top of the list. 
1. Type the name of the user, role, team, group, or company for which you want to remove the access in the **Edit `<Object Name>` access to** field. 
1. From the access drop-down menu, select **No Access**.

   ![remove in bulk](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. In the `<User Name>`'s Workfront access will be removed from this drop-down menu, select whether you want their access to be removed just from the objects that you have selected, or from all other children objects associated with it.  
   The following scenarios exist:

   * If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they were previously granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;
   * If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they were previously given individual permission on each child object.

   **Example:** Select whether to remove permissions to just the tasks you selected in a list, or to the issues and documents attached to the tasks as well.

   ![access](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Optional) To change permissions in bulk for several objects, select another level of sharing for the selected entity.

   For example, if they have Manage permissions, select Contribute or View instead. 

1. Click **Save**.

-->

## Quitar permisos heredados

Los permisos heredados se pueden eliminar de los objetos, lo que permite a los propietarios identificar específicamente quién tendrá acceso a objetos secundarios, independientemente del acceso que tenga un usuario a un objeto principal.

>[!IMPORTANT]
>
>Solo los usuarios con permiso de administración pueden quitar los permisos heredados.

Para quitar permisos heredados:

1. Vaya a un objeto para el que tenga permisos de administración. Por ejemplo, vaya a una tarea.
1. Vaya al cuadro de acceso a objetos como se describe en la sección [Quitar entidades de la lista de uso compartido de un objeto](#remove-entities-from-the-sharing-list-of-an-object) de este artículo.
1. Seleccione **Desactivar** junto a **Permiso heredado** para deshabilitar.

   Esto garantiza que nadie que tenga permisos concedidos para el objeto principal (por ejemplo, el proyecto) tenga permisos para esta tarea de forma predeterminada. Debe enumerar entidades individuales en la lista de uso compartido de la tarea para conceder permisos sobre la tarea.

   >[!TIP]
   >
   >No se pueden quitar entidades individuales de la lista Permisos heredados. Solo se pueden desactivar los permisos heredados para todas las entidades enumeradas.

1. Haga clic en **Guardar**.

## Hacer que un objeto pase a ser privado

Si ha compartido un objeto en todo el sistema o lo ha compartido con usuarios externos haciéndolo público, puede hacerlo privado de nuevo eliminando los permisos públicos o de todo el sistema. 

Para obtener más información sobre cómo hacer que un objeto esté disponible en todo el sistema o sea de uso público, vea [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Para hacer que un objeto pase a ser privado:

1. Vaya al objeto que desea que pase a ser privado.\
   Por ejemplo, vaya a un informe.
1. Haga clic en **Acciones de informe** y luego en **Uso compartido**.

   ![convertir en privado](assets/report-permissions-make-private-nwe-350x477.png)

1. Haga clic en el icono de engranaje y, a continuación, desmarque **Convertir esto en público para usuarios externos**.
1. En el menú desplegable **Que tiene acceso**, haz clic en **Solo las personas invitadas pueden acceder** para dejar de compartirlo con todos los usuarios de Workfront.
1. Haga clic en **Guardar**.
