---
title: Creación o edición de un estado
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: Como administrador de Adobe Workfront, puede crear estados personalizados para proyectos, tareas y problemas.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 2%

---

# Creación o edición de un estado

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

Como administrador de Adobe Workfront, puede crear estados personalizados para proyectos, tareas y problemas. Pueden ser para usuarios de todo el sistema de Workfront o para grupos o subgrupos específicos. Para obtener más información sobre los estados, consulte [Resumen de estados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Los administradores de grupo también pueden crear sus propios estados de grupo para usarlos únicamente en sus grupos. Para obtener más información, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
     <p>Nuevo: estándar</p>
     <p>o</p>
     <p>Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación o edición de un estado personalizado

Puede agregar un estado personalizado para que lo utilice toda la organización o un solo grupo.

Al crear un estado personalizado para toda la organización, puede configurarlo para que todos los grupos del sistema puedan utilizarlo sin editarlo. O puede configurarlo para que los administradores de grupos puedan modificarlo para sus grupos, como se explica en [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).

1. En el panel izquierdo, haga clic en **Preferencias de proyecto** > **Estados**.

1. (Condicional) Si está creando o editando un estado para utilizarlo en todo el sistema, asegúrese de que **Estados del sistema** está seleccionado en el cuadro de la esquina superior derecha.

   ![](assets/system-statuses-in-upper-rt-corner-new.jpg)

   O

   Si el estado es para un grupo o subgrupo, empiece a escribir el nombre del grupo en la esquina superior derecha y, a continuación, selecciónelo cuando aparezca.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Seleccione la pestaña del tipo de objeto (**Proyecto**, **Tareas**, o **Problemas**) que desee asociar con el estado.

1. Si está creando un nuevo estado, haga clic en **Agregar nuevo estado**.

   O

   Si está editando un estado existente, pase el ratón sobre él y haga clic en el **Editar** que se muestra a la derecha.

   ![](assets/custom-status-edit.png)

1. Configure el estado con las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de estado</td> 
      <td> <p>Escriba un nombre para el estado. Este campo es obligatorio.</p> <p>Cuando cree un nombre de estado, tenga en cuenta que otros usuarios del sistema pueden crear un estado con el mismo nombre. Se recomienda utilizar un nombre único para evitar confusiones al seleccionar estados en Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>(Opcional) Escriba una descripción del estado. Esto comunica su propósito a quienes lo utilizan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Personalice el color del estado haciendo clic en el campo de color y seleccionando un color en el panel de muestras. También puede introducir un número hexadecimal en el campo.</p> <p>El color del estado se muestra en la esquina superior derecha de Workfront cuando un usuario ve el objeto.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Igual que</td> 
      <td> <p>Seleccione una de las opciones de la lista que mejor describa la función del estado. Por ejemplo, si el nombre del estado es Listo, la opción con la que se equipara debe ser Completo.</p> <p>Cada estado debe coincidir con una de estas opciones, ya que esto determina cómo funciona el estado.</p> <p>Esta opción no se puede modificar una vez creado el estado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clave</td> 
      <td> <p>Si está creando un nuevo estado, escriba un código o una abreviatura para el estado o utilice el que se ha generado. Esta clave debe ser única en Workfront, ya que puede utilizarse para la creación de informes. Si intenta especificar una clave que ya está en uso en el sistema, el campo se vuelve rojo.</p> <p>Podría resultar útil utilizar una abreviatura que sea reconocible para quienes la utilicen.</p> <p>Esta opción no se puede modificar una vez creado el estado.</p> <p>No se puede cambiar el código de clave para los estados Planificación, Actual y Finalizado. Esto es importante si está creando un informe en modo de texto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar estado</td> 
      <td> <p>(Solo estados de proyecto y tarea)</p> <p>Active esta opción si desea que el estado se oculte a los usuarios. Cuando esta opción está desactivada (la configuración predeterminada), todos los usuarios del sistema pueden utilizar el estado.</p> <p>Puede ocultar un estado de problema desactivando esta opción para los 4 tipos de problemas (Informe de errores, Orden de cambio, Problema, Solicitud).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear para todos los grupos</td> 
      <td>
       <p>Cuando un estado está bloqueado, los usuarios de todo el sistema pueden verlo y utilizarlo, y los administradores de grupos no pueden personalizarlo para sus grupos.</p> 
       <p>Cuando un estado está desbloqueado, los administradores de grupos pueden personalizarlo para sus grupos individuales.</p>

   <div>
       <p>Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación del sistema. Si crea un proceso de aprobación del sistema con un estado de sistema desbloqueado, los usuarios de todo el sistema pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema del sistema.</p>
       <p> En los casos siguientes, se muestran mensajes de advertencia para ayudarle a usted y a sus usuarios a comprender los resultados de desbloquear un estado:</p>
       <ul>
       <li>Un administrador desbloquea un estado de nivel de sistema que se utiliza en un proceso de aprobación. Un mensaje advierte que podrían eliminar el estado desbloqueado de sus grupos, lo que impediría que los miembros del grupo usaran correctamente ese proceso de aprobación para los objetos asignados a su grupo.</li>
       <li>Un usuario comienza a editar un proceso de aprobación que utiliza un estado desbloqueado. Un mensaje alerta al usuario sobre el estado de desbloqueado para que pueda evaluar si sería una buena idea volver a bloquearlo o reemplazarlo.</li>
       <li>Un proceso de aprobación de nivel de sistema con un estado desbloqueado está adjunto a un objeto y el estado se eliminó para el grupo asignado al objeto. Cuando un miembro del grupo va a la sección Approvals del objeto, un mensaje explica que no se puede iniciar el proceso de aprobación del objeto.</li>
       </ul>
       <p>Para obtener más información sobre los estados de bloqueo, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Estados bloqueados y desbloqueados en el nivel del sistema</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   Para obtener instrucciones sobre cómo convertir este estado en predeterminado, consulte [Usar estados personalizados como estados predeterminados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

Para obtener información sobre cómo reordenar los estados de grupo, consulte [Reordenar los estados de grupo y de nivel del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
