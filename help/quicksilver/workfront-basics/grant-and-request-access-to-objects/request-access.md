---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Solicitud de acceso a objetos
description: La visibilidad de los objetos en Adobe Workfront depende del acceso a ese tipo de objeto, así como de los permisos que tenga en un objeto individual.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 0%

---

# Solicitud de acceso a objetos

La visibilidad de los objetos en Adobe Workfront depende del acceso a ese tipo de objeto, así como de los permisos que tenga en un objeto individual.

>[!NOTE]
>
>En este artículo se describe cómo puede solicitar permisos a todos los objetos, excepto a los planes del Scenario Planner de Adobe Workfront. Para obtener información sobre cómo solicitar acceso a los planes, consulte [Solicitar acceso a un plan en el Scenario Planner](../../scenario-planner/request-access-to-plan.md). Esto requiere una licencia adicional.

El administrador de Workfront configura el acceso a un tipo de objeto en su nivel de acceso. Para obtener más información, vea [Cómo funcionan juntos los niveles de acceso y los permisos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Si necesita permisos para objetos específicos dentro de Workfront, puede solicitar acceso a ellos. En lugar de enviar un correo electrónico al administrador de Workfront o al propietario del objeto para explicarle sus necesidades, puede solicitar acceso (o permisos) adicional en Workfront.

Puede solicitar acceso inicial a los objetos si alguien comparte un vínculo con el objeto o puede solicitar acceso adicional a los objetos que puede ver al menos.

Por ejemplo, puede tener permisos de Vista en un proyecto, pero debe agregar tareas a ese proyecto. En este caso, puede solicitar permisos de Contribute para el proyecto.

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
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver el acceso o superior a los objetos para los que solicita permisos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Comprender las reglas de uso compartido estándar

Las siguientes reglas estándar de uso compartido se aplican automáticamente, ya que se establecen como opciones predeterminadas en el sistema de Workfront.

* Los usuarios asignados a una tarea o a un problema tienen acceso a Contribute en ella.
* Los jefes de proyecto, Portfolio y programa tienen acceso de administración a los objetos que poseen.
* Los usuarios incluidos en una conversación tienen acceso de visualización en el objeto en el que se produce la conversación.
* Los usuarios asignados como aprobadores tienen acceso de visualización en el objeto a la espera de ser aprobado.
* Al compartir un tablero, todos los informes del tablero se comparten también con el mismo acceso a los mismos usuarios.
* Los propietarios de objetos no pueden ampliar el acceso a un objeto más allá de su acceso en ese objeto, tal como lo ha definido el administrador.

## Solicitar acceso

Puede solicitar acceso inicial a objetos a los que actualmente no tiene acceso, o puede solicitar acceso adicional a objetos a los que sólo tiene acceso limitado.

* [Solicitar acceso inicial](#request-initial-access)
* [Solicitar acceso adicional](#request-additional-access)

### Solicitar acceso inicial  {#request-initial-access}

Si todavía no tiene acceso a un objeto y navega hasta ese objeto desde un vínculo, se muestra una pantalla que le informa de que no tiene acceso para ver la información.

Para solicitar acceso inicial a un objeto:

1. Haga clic en **Solicitar acceso**.\
   Se muestra el cuadro de diálogo **Solicitar acceso**.

1. (Condicional) Si más de un usuario tiene el acceso adecuado para otorgarle acceso adicional, se muestra una flecha desplegable junto al nombre del usuario.
1. Seleccione el usuario de la lista desplegable que desee que reciba su solicitud de acceso.\
   En la lista desplegable solo se muestran 10 usuarios. La lista se ordena alfabéticamente.\
   Para obtener más información sobre el orden de los usuarios enumerados en este menú desplegable, consulte [Jerarquía de los menús desplegables &quot;Solicitar acceso&quot; y &quot;Solicitar más acceso&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. En la lista desplegable, seleccione el tipo de acceso que desea solicitar.
1. (Opcional) En el campo **P.S.**, especifique una nota para el usuario sobre por qué necesita acceso adicional.

   ![](assets/request-access-dialog-350x314.png)

Si no tiene derechos de nivel de acceso a un objeto e intenta acceder a ese objeto desde un vínculo, se muestra una pantalla que le informa de que debe ponerse en contacto con el administrador de Workfront.

Por ejemplo, si no tiene acceso a la cartera, pero se le ha proporcionado un vínculo a una cartera, verá el siguiente mensaje:\
![](assets/permission-request-initial2-350x96.png)

### Solicitar acceso adicional {#request-additional-access}

Para solicitar acceso adicional a un objeto al que ya tiene acceso limitado:

1. Vaya al objeto para el que desea solicitar acceso adicional.

1. Haga clic en el menú **Más** a la derecha del nombre del proyecto y, a continuación, haga clic en **Solicitar más acceso**.

   ![](assets/request-access-in-project-350x201.png)

1. (Condicional) Si más de un usuario tiene el acceso adecuado para otorgarle acceso adicional, se muestra una flecha desplegable junto al nombre del usuario.
1. Seleccione el usuario de la lista desplegable que desee que reciba su solicitud de acceso.\
   En la lista desplegable solo se muestran 10 usuarios. La lista se ordena alfabéticamente.\
   Para obtener más información sobre el orden de los usuarios enumerados en este menú desplegable, consulte [Jerarquía de los menús desplegables &quot;Solicitar acceso&quot; y &quot;Solicitar más acceso&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. En la lista desplegable, seleccione el nivel de acceso que desee solicitar.
1. (Opcional) En el campo **P.S.**, especifique una nota con respecto a por qué necesita acceso adicional.
1. Haga clic en **Solicitar acceso**.\
   ![](assets/request-access-dialog-350x314.png)

## Jerarquía de los menús desplegables &quot;Solicitar acceso&quot; y &quot;Solicitar más acceso&quot; {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Comprenda la jerarquía de usuarios enumerados en los menús desplegables Solicitar acceso y Solicitar más acceso](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Explicación del propietario de un objeto](#understand-the-owner-of-an-object)

### Comprenda la jerarquía de usuarios enumerados en los menús desplegables Solicitar acceso y Solicitar más acceso {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Al rellenar las listas &quot;Solicitar acceso&quot; o &quot;Solicitar más acceso&quot; en los objetos, Workfront selecciona una lista de hasta diez usuarios que cumplen diversas funciones en el uso compartido del objeto, como se describe a continuación. Estos usuarios pueden conceder acceso al objeto al usuario que lo solicita.\
La lista resultante se ordenará por su nombre en orden alfabético ascendente.\
Workfront muestra hasta diez usuarios en las listas &quot;Solicitar acceso&quot; y &quot;Solicitar más acceso&quot;.

El orden de los usuarios en los menús desplegables &quot;Solicitar acceso&quot; o &quot;Solicitar más acceso&quot; viene determinado por las siguientes reglas:

* El primer usuario de la lista es el &quot;propietario&quot; del objeto, tal como se describe en [Comprenda el propietario de un objeto](#understand-the-owner-of-an-object).
* A continuación, la lista se rellena con los usuarios con los que se comparte el objeto de forma individual. Se muestran en orden alfabético.
* A continuación, la lista se rellena con los usuarios que obtienen el acceso necesario compartiendo con sus equipos, grupos o empresas. Se muestran en orden alfabético.
* Si la lista está vacía, se agregan los administradores de Workfront para que siempre haya alguien desde quien solicitar acceso. Se muestran en orden alfabético.
* Cada uno de los usuarios de la lista debe tener el acceso solicitado al objeto y el acceso para compartir el objeto.

### Explicación del propietario de un objeto {#understand-the-owner-of-an-object}

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
   <td>El propietario es el Propietario del proyecto o, si falta o no tiene el acceso necesario, el propietario del portafolio principal. <p>Es posible que no sean la misma persona que el creador del proyecto. </p></td> 
  </tr> 
  <tr> 
   <td>Tareas</td> 
   <td>El propietario es el Usuario asignado principal o, si falta o no tiene el acceso necesario, el propietario del proyecto en el que reside la tarea, según se ha definido anteriormente. <p>Es posible que no sean la misma persona que el creador de la tarea. </p></td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td> <p>El propietario es el contacto principal del problema o, si falta o no tiene el acceso necesario, el propietario del proyecto en el que reside el problema, según se ha definido anteriormente. </p> <p>Es posible que no sean la misma persona que el creador del problema. </p> </td> 
  </tr> 
  <tr> 
   <td>Portafolios</td> 
   <td>El propietario es el propietario Portfolio. <p>Es posible que no sean la misma persona que el creador del portafolio. </p></td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>El propietario es el propietario del documento (el usuario que lo ha cargado) o, si falta o no tiene el acceso necesario, el propietario del objeto en el que reside el documento.</td> 
  </tr> 
  <tr> 
   <td>Informes y paneles</td> 
   <td>El propietario es el creador, el informe o el tablero. </td> 
  </tr> 
  <tr> 
   <td>Calendarios</td> 
   <td>El propietario es el creador del calendario. Todos los usuarios tienen un calendario asignado de forma predeterminada. Se les considera propietarios de ese calendario. </td> 
  </tr> 
  <tr> 
   <td>Filtros, vistas y agrupaciones</td> 
   <td>El propietario de un filtro, vista o agrupación es el creador. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Planes</span> </td> 
   <td> <p><span>El propietario es el creador del plan.</span> </p> <p>Esto requiere una licencia adicional. </p> <p><span>Para obtener información acerca del Planificador de escenarios de Workfront, consulte</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Información general del Planificador de escenarios</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Metas</td> 
   <td> <p>El propietario es el usuario designado como Propietario. Es posible que no sean la misma persona que el creador del objetivo. </p> <p>Esto requiere una licencia adicional. </p> <p>Para obtener información acerca de Workfront Goals, vea <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Información general sobre Adobe Workfront Goals</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


