---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Eliminación de permisos de objetos
description: Puede quitar los permisos de otros usuarios en objetos a los que tenga acceso Compartir. La eliminación de permisos de los objetos es idéntica para todos los objetos que se pueden compartir.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# Eliminación de permisos de objetos

Puede quitar los permisos de otros usuarios en objetos a los que tenga acceso Compartir. La eliminación de permisos de los objetos es idéntica para todos los objetos que se pueden compartir. 

Consideraciones similares a las de compartir objetos se aplican para eliminar permisos de objetos. Para obtener más información, consulte la sección [Consideraciones sobre el uso compartido de objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) en el artículo [Información general sobre cómo compartir permisos en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Requisitos de acceso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or  
   <p>Legacy license: Request or higher</p>
   <p><b>NOTE</b></p>

   <p>Some objects require a higher access than Request. </p>
   
   <p>For example, for the current license, a Contributor can share issues, but only Standard-license users can share a project.</p>
   
   <p>For the legacy license, a Requestor can share issues, but only Workers or Planners can share a project.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>Manage permissions to remove inherited permissions on objects</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener lo siguiente para compartir objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Workfront*</td> 
   <td> <p>Solicitud o superior</p>
   <p><b>NOTA</b></p>

Algunos objetos requieren un acceso mayor que Solicitud. Por ejemplo, un solicitante puede compartir problemas, pero solo los trabajadores o los planificadores pueden compartir un proyecto.

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso o superior a los objetos que desea compartir</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos o superiores de los objetos que desea compartir</p> <p>Administrar permisos para quitar permisos heredados en objetos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Eliminación de entidades de la lista de uso compartido de un objeto {#remove-entities-from-the-sharing-list-of-an-object}

Puede quitar entidades (usuarios, funciones de trabajo, equipos, grupos y empresas) de la lista de uso compartido de un objeto. Esto elimina los permisos del objeto.

1. Vaya al objeto que desea compartir.

   Para obtener información sobre los objetos que se pueden compartir, consulte [Información general sobre cómo compartir permisos en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Haga clic en el **Más** icono ![](assets/more-icon.png)junto al nombre del objeto y, a continuación, haga clic en **Uso compartido** o **Compartir.**

   ![](assets/share-a-document-350x160.png)

1. Haga clic en el **x** junto al nombre de un usuario, equipo, grupo, empresa, función de trabajo para eliminarlos en el cuadro de acceso a objetos.

   ![](assets/remove-permissions-on-project-nwe-350x479.png)

1. En el `<User Name>`El acceso de Workfront de se eliminará de este menú desplegable, seleccione si desea que su acceso se elimine solo del objeto seleccionado o de todos los objetos secundarios asociados a él.\
   Existen los siguientes escenarios:

   * Si elimina la entidad solo del objeto, esa entidad pierde sus permisos en el objeto y sus permisos heredados en los objetos secundarios. Si anteriormente se les otorgaban permisos a los elementos secundarios de forma individual, conservan los mismos permisos en todos los objetos secundarios asociados a ella al seleccionar esta opción. 
   * Si elimina la entidad del objeto y todos los objetos secundarios, esa entidad perderá sus permisos para el objeto, así como todos los objetos secundarios, incluso cuando anteriormente se les había concedido permiso individual para cada objeto secundario. 

1. Haga clic en **Guardar**.

## Eliminación de permisos de varios objetos de forma masiva

Puede quitar entidades (usuarios, funciones de trabajo, equipos, grupos, empresas) de varios objetos a la vez que los selecciona por lotes en una lista. 

>[!NOTE]
>
>No puede ver qué entidades de acceso tienen para todos los objetos seleccionados cuando los selecciona de forma masiva. Debe saber qué entidad desea eliminar del uso compartido de los objetos seleccionados antes de eliminar sus permisos.

1. Vaya a la lista de objetos que desea compartir.

   Para obtener información sobre los objetos que se pueden compartir, consulte [Información general sobre cómo compartir permisos en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Seleccione varios objetos de la lista y, a continuación, haga clic en el **Compartir** icono ![](assets/share-icon.png)en la parte superior de la lista.
1. Escriba el nombre del usuario, rol, equipo, grupo o empresa para los que desea eliminar el acceso en la **Editar `<Object Name>` acceso a** campo .
1. En el menú desplegable de acceso, seleccione **Sin acceso**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. En el `<User Name>`El acceso de Workfront de se eliminará de este menú desplegable, seleccione si desea que su acceso se elimine solo de los objetos seleccionados o de todos los demás objetos secundarios asociados a él.\
   Existen los siguientes escenarios:

   * Si elimina la entidad solo del objeto, esa entidad pierde sus permisos en el objeto y sus permisos heredados en los objetos secundarios. Si anteriormente se les otorgaban permisos a los elementos secundarios de forma individual, conservan los mismos permisos en todos los objetos secundarios asociados a ella al seleccionar esta opción. 
   * Si elimina la entidad del objeto y todos los objetos secundarios, esa entidad perderá sus permisos para el objeto, así como todos los objetos secundarios, incluso cuando anteriormente se les había concedido permiso individual para cada objeto secundario.

   **Ejemplo:** Seleccione si desea quitar permisos solo para las tareas seleccionadas en una lista, o también para los problemas y documentos adjuntos a las tareas.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Opcional) Para cambiar permisos de forma masiva para varios objetos, seleccione otro nivel de uso compartido para la entidad seleccionada.

   Por ejemplo, si tienen permisos de gestión, seleccione Contribute o Ver en su lugar.

1. Haga clic en **Guardar**.

## Eliminación de permisos heredados

Los permisos heredados se pueden eliminar de los objetos, lo que permite a los propietarios identificar específicamente quién tendrá acceso a los objetos secundarios, independientemente del acceso de un usuario a un objeto principal.

>[!IMPORTANT]
>
>Solo los usuarios con permiso de administración pueden eliminar permisos heredados.

Para quitar permisos heredados:

1. Vaya a un objeto al que tenga permisos de gestión. Por ejemplo, vaya a una tarea.
1. Vaya al cuadro de acceso al objeto tal como se describe en la sección [Eliminación de entidades de la lista de uso compartido de un objeto](#remove-entities-from-the-sharing-list-of-an-object) en este artículo.
1. Seleccione el **x** junto a **Permiso heredado** en el cuadro para compartir para eliminar a cualquiera de los que aparecen allí.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   Esto garantiza que nadie a quien se le concedan permisos para el objeto principal (por ejemplo, el proyecto) tenga permisos para esta tarea de forma predeterminada. Debe enumerar entidades individuales en la lista de uso compartido de la tarea para conceder permisos sobre la tarea.

   >[!TIP]
   >
   >No se pueden quitar entidades individuales de la lista Permisos heredados. Solo puede deshabilitar los Permisos heredados para todas las entidades enumeradas.

1. Haga clic en **Guardar**. 

## Convertir un objeto en privado

Si ha compartido un objeto en todo el sistema o lo ha compartido con usos externos haciéndolo público, puede volver a hacerlo privado eliminando los permisos públicos o de todo el sistema. 

Para obtener más información sobre cómo hacer que un objeto esté disponible para todo el sistema o para el público, consulte [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Para convertir un objeto en privado:

1. Vaya al objeto que desea convertir en privado.\
   Por ejemplo, vaya a un informe.
1. Haga clic en **Acciones de informe**, luego **Uso compartido**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Haga clic en **Eliminación del acceso público** para eliminar el acceso de los usuarios externos a la visualización del informe.
1. Haga clic en **Eliminar el acceso a todo el sistema** para dejar de compartirlo con todos los usuarios de Workfront. 
1. Haga clic en **Guardar**.
