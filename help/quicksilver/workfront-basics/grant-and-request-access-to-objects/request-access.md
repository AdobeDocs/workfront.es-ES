---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Solicitar acceso a objetos
description: La visibilidad de los objetos en Adobe Workfront depende del acceso a ese tipo de objeto, así como de los permisos que tenga en un objeto individual.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%

---

# Solicitar acceso a objetos

La visibilidad de los objetos en Adobe Workfront depende del acceso a ese tipo de objeto, así como de los permisos que tenga en un objeto individual.

>[!NOTE]
>
>En este artículo se describe cómo se pueden solicitar permisos para todos los objetos, excepto para los planes del planificador de escenarios de Adobe Workfront. Para obtener información sobre la solicitud de acceso a los planes, consulte [Solicitar acceso a un plan en el planificador de escenarios](../../scenario-planner/request-access-to-plan.md). Esto requiere una licencia adicional.

El administrador de Workfront configura el acceso a un tipo de objeto en el nivel de acceso. Para obtener más información, consulte [Cómo funcionan juntos los niveles de acceso y los permisos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Si necesita permisos para objetos específicos dentro de Workfront, puede solicitar acceso a ellos. En lugar de enviar un correo electrónico al administrador de Workfront o al propietario del objeto para explicar sus necesidades, puede solicitar acceso (o permisos) adicional dentro de Workfront.

Puede solicitar acceso inicial a los objetos si alguien comparte un vínculo con el objeto con usted o puede solicitar acceso adicional a los objetos que active al menos en la vista.

Por ejemplo, puede tener permisos de visualización para un proyecto, pero debe agregar tareas a ese proyecto. En este caso, puede solicitar permisos de Contribute al proyecto.

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso o superior a los objetos a los que solicita permisos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Comprender las reglas de uso compartido estándar

Las siguientes reglas de uso compartido estándar surten efecto automáticamente, ya que están configuradas como opciones predeterminadas en el sistema Workfront. 

* Los usuarios asignados a una tarea o a un problema tienen acceso de Contribute. 
* Los administradores de proyectos, Portfolio y programas tienen acceso de gestión en los objetos que poseen.
* Los usuarios incluidos en una conversación tienen acceso de visualización en el objeto en el que se produce la conversación.
* Los usuarios asignados como aprobadores tienen acceso de visualización en el objeto que está a la espera de ser aprobado.
* Al compartir un tablero, todos los informes del tablero también se comparten con el mismo acceso a los mismos usuarios. 
* Los propietarios de objetos no pueden ampliar el acceso a un objeto más allá de su acceso en ese objeto, tal como lo define el administrador.

## Solicitud de acceso

Puede solicitar acceso inicial a objetos a los que no tiene acceso actualmente, o bien solicitar acceso adicional a objetos a los que solo tiene acceso limitado.

* [Solicitar acceso inicial](#request-initial-access)
* [Solicitar acceso adicional](#request-additional-access)

### Solicitar acceso inicial  {#request-initial-access}

Si todavía no tiene acceso a un objeto y se desplaza a él desde un vínculo, aparece una pantalla que le informa de que no tiene acceso para ver la información.  

Para solicitar acceso inicial a un objeto:

1. Haga clic en **Solicitar acceso**.\
   La variable **Solicitar acceso** se muestra.

1. (Condicional) Si más de un usuario tiene el acceso adecuado para otorgarle acceso adicional, aparece una flecha desplegable junto al nombre del usuario. 
1. Seleccione el usuario de la lista desplegable que desea que reciba su solicitud de acceso.\
   Solo se muestran 10 usuarios en la lista desplegable. La lista se ordena alfabéticamente.\
   Para obtener más información sobre el orden de los usuarios enumerados en este menú desplegable, consulte  [Jerarquía de los menús desplegables &quot;Solicitar acceso&quot; y &quot;Solicitar más acceso&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. En la lista desplegable, seleccione el tipo de acceso que desea solicitar.
1. (Opcional) En la **P.S.** especifique una nota al usuario sobre por qué necesita acceso adicional.

   ![](assets/request-access-dialog-350x314.png)

Si no tiene derechos de nivel de acceso a un objeto e intenta acceder a él desde un vínculo, aparece una pantalla que le informa de que debe ponerse en contacto con el administrador de Workfront. 

Por ejemplo, si no tiene acceso de portafolio, pero se le ha dado un vínculo a un portafolio, verá el siguiente mensaje:\
![](assets/permission-request-initial2-350x96.png)

### Solicitar acceso adicional {#request-additional-access}

Para solicitar acceso adicional a un objeto al que ya tiene acceso limitado:

1. Vaya al objeto para el que desea solicitar acceso adicional.

1. Haga clic en el **Más** en línea con el nombre del proyecto y, a continuación, haga clic en **Solicitar más acceso**.\
   ![](assets/request-access-in-project-350x201.png)

1. (Condicional) Si más de un usuario tiene el acceso adecuado para otorgarle acceso adicional, aparece una flecha desplegable junto al nombre del usuario.
1. Seleccione el usuario de la lista desplegable que desea que reciba su solicitud de acceso.\
   Solo se muestran 10 usuarios en la lista desplegable. La lista se ordena alfabéticamente.\
   Para obtener más información sobre el orden de los usuarios enumerados en este menú desplegable, consulte  [Jerarquía de los menús desplegables &quot;Solicitar acceso&quot; y &quot;Solicitar más acceso&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. En la lista desplegable, seleccione el nivel de acceso que desea solicitar.
1. (Opcional) En la **P.S.** especifique una nota sobre por qué necesita acceso adicional.
1. Haga clic en **Solicitar acceso**.\
   ![](assets/request-access-dialog-350x314.png)

## Jerarquía de los menús desplegables &quot;Solicitar acceso&quot; y &quot;Solicitar más acceso&quot; {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Comprender la jerarquía de usuarios que aparece en los menús desplegables Solicitar acceso y Solicitar más acceso](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Comprender el propietario de un objeto](#understand-the-owner-of-an-object)

### Comprender la jerarquía de usuarios que aparece en los menús desplegables Solicitar acceso y Solicitar más acceso {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Al rellenar las listas &quot;Solicitar acceso&quot; o &quot;Solicitar más acceso&quot; en los objetos, Workfront selecciona una lista de hasta diez usuarios que cumplen varias funciones en el uso compartido del objeto, como se describe a continuación. Estos usuarios pueden conceder acceso al objeto al usuario que lo solicite.\
La lista resultante se ordena por su nombre en orden alfabético ascendente.\
Workfront muestra hasta 10 usuarios en las listas &quot;Solicitar acceso&quot; y &quot;Solicitar más acceso&quot;. 

El orden de los usuarios en los menús desplegables &quot;Solicitar acceso&quot; o &quot;Solicitar más acceso&quot; está dictado por las siguientes reglas: 

* El primer usuario de la lista es el objeto &quot;propietario&quot;, tal como se describe en [Comprender el propietario de un objeto](#understand-the-owner-of-an-object). 
* A continuación, la lista se rellena con usuarios con los que el objeto se comparte individualmente. Se muestran en orden alfabético.
* A continuación, la lista se rellena con usuarios que obtienen el acceso necesario compartiendo con sus equipos, grupos o empresas. Se muestran en orden alfabético.
* Si la lista está vacía, se añaden los administradores de Workfront para que siempre haya alguien desde el que solicitar el acceso. Se muestran en orden alfabético. 
* Cada uno de los usuarios de la lista debe tener el acceso solicitado al objeto y el acceso para compartir el objeto. 

### Comprender el propietario de un objeto {#understand-the-owner-of-an-object}

El propietario de un objeto se define de la siguiente manera:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objeto</strong> </th> 
   <th><strong>Definición del propietario del objeto</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Proyectos</td> 
   <td>El propietario es el propietario del proyecto o, si falta o no tiene el acceso necesario, el propietario del portafolio principal. <p>Puede que no sean la misma persona que el creador del proyecto. </p></td> 
  </tr> 
  <tr> 
   <td>Tareas</td> 
   <td>El propietario es el usuario asignado principal o, si falta o no tiene el acceso necesario, el propietario del proyecto en el que reside la tarea, tal como se ha definido anteriormente. <p>Puede que no sean la misma persona que el creador de la tarea. </p></td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td> <p>El propietario es el contacto principal del problema o, si falta o no tiene acceso necesario, el propietario del proyecto en el que reside el problema, tal como se ha definido anteriormente. </p> <p>Puede que no sean la misma persona que el creador del problema. </p> </td> 
  </tr> 
  <tr> 
   <td>Portafolios</td> 
   <td>El propietario es el propietario del Portfolio. <p>Es posible que no sean la misma persona que el creador del portafolio. </p></td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>El propietario es el propietario del documento (el usuario que cargó el documento) o, si falta o no tiene acceso necesario, el propietario del objeto en el que reside el documento.</td> 
  </tr> 
  <tr> 
   <td>Informes y tableros</td> 
   <td>El propietario es el creador o el informe o el tablero. </td> 
  </tr> 
  <tr> 
   <td>Calendarios</td> 
   <td>El propietario es el creador del calendario. Todos los usuarios tienen un calendario asignado de forma predeterminada. Se consideran los propietarios de ese calendario. </td> 
  </tr> 
  <tr> 
   <td>Filtros, vistas y agrupaciones</td> 
   <td>El propietario de un filtro, vista o agrupación es el creador. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Planes</span> </td> 
   <td> <p><span>El propietario es el creador del plan.</span> </p> <p>Esto requiere una licencia adicional. </p> <p><span>Para obtener información sobre el planificador de escenarios de Workfront, consulte</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Información general del planificador de escenarios</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Metas</td> 
   <td> <p>El propietario es el usuario designado como propietario. Puede que no sean la misma persona que el creador del objetivo. </p> <p>Esto requiere una licencia adicional. </p> <p>Para obtener información sobre los objetivos de Workfront, consulte <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Información general sobre los objetivos de Adobe Workfront</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

 
