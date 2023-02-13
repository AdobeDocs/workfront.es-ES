---
title: Crear o editar un estado
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: Como administrador de Adobe Workfront, puede crear estados personalizados para proyectos, tareas y problemas.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 2%

---

# Crear o editar un estado

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

Como administrador de Adobe Workfront, puede crear estados personalizados para proyectos, tareas y problemas. Pueden ser para usuarios de todo el sistema de Workfront o para grupos o subgrupos específicos. Para obtener más información sobre los estados, consulte [Resumen de los estados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Los administradores del grupo también pueden crear sus propios estados de grupo, para que los utilicen únicamente sus grupos. Para obtener más información, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Requisitos de acceso

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Crear o editar un estado personalizado

Puede agregar un estado personalizado para su uso en toda la organización o en un solo grupo.

Cuando crea un estado personalizado para toda la organización, puede configurarlo para que todos los grupos del sistema puedan usarlo sin editarlo. O puede configurarlo para que los administradores de grupos puedan modificarlo para sus grupos, tal como se explica en [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Preferencias de proyecto** > **Estados**.

1. (Condicional) Si está creando o editando un estado para utilizarlo en todo el sistema, asegúrese de que **Estados del sistema** está seleccionado en el cuadro de la esquina superior derecha.

   ![](assets/system-statuses-in-upper-rt-corner.jpg)

   O

   Si el estado es para un grupo o subgrupo, empiece a escribir el nombre del grupo en la esquina superior derecha y, a continuación, selecciónelo cuando aparezca.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Seleccione la pestaña del tipo de objeto (**Proyecto**, **Tareas** o **Problemas**) que desea asociar al estado.

1. Si está creando un nuevo estado, haga clic en **Agregar un nuevo estado**.

   O

   Si está editando un estado existente, pase el ratón sobre él y haga clic en el botón **Editar** que se muestra al extremo derecho.

   ![](assets/custom-status-edit.png)

1. Configure el estado mediante las siguientes opciones:

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
      <td> <p>Personalice el color del estado haciendo clic en el campo de color y seleccionando un color en el panel de muestra. También puede introducir un número hexadecimal en el campo .</p> <p>El color del estado se muestra en la esquina superior derecha de Workfront cuando un usuario ve el objeto.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Igual que</td> 
      <td> <p>Seleccione una de las opciones de la lista que mejor describa la función del estado. Por ejemplo, si el nombre del estado es Listo, la opción con la que se equipara debe ser Completada.</p> <p>Cada estado debe coincidir con una de estas opciones porque esto determina cómo funciona el estado.</p> <p>Esta opción no se puede modificar una vez creado el estado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clave</td> 
      <td> <p>Si está creando un nuevo estado, escriba un código o abreviatura para el estado o use el que se ha generado para usted. Esta clave debe ser única en Workfront, ya que se puede utilizar para generar informes. Si intenta especificar una clave que ya se está utilizando en el sistema, el campo se vuelve rojo.</p> <p>Podría resultar útil utilizar una abreviatura reconocible para quienes la utilicen.</p> <p>Esta opción no se puede modificar una vez creado el estado.</p> <p>No se puede cambiar el código clave para los estados Planificación, Actual y Completado. Esto es importante si está creando un informe en modo de texto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar estado</td> 
      <td> <p>(Estados de proyecto y tarea únicamente)</p> <p>Active esta opción si desea que el estado esté oculto para los usuarios. Cuando está desactivado (la configuración predeterminada), todos los usuarios del sistema pueden utilizar el estado .</p> <p>Puede ocultar el estado de un problema desactivando los 4 tipos de problemas (informe de errores, orden de cambio, problema, solicitud).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear para todos los grupos</td> 
      <td>
       <p>Cuando un estado está bloqueado, los usuarios de todo el sistema pueden verlo y utilizarlo, y los administradores de grupos no pueden personalizarlo para sus grupos.</p> 
       <p>Cuando un estado está desbloqueado, los administradores de grupos pueden personalizarlo para sus grupos individuales.</p>

   <div>
       <p>Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación del sistema. Si crea un proceso de aprobación del sistema con un estado del sistema desbloqueado, los usuarios de todo el sistema pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema del sistema.</p>
       <p> En las siguientes situaciones, aparecen mensajes de advertencia para ayudarle a usted y a los usuarios a comprender los resultados de desbloquear un estado:</p>
       <ul>
       <li>Un administrador desbloquea un estado de nivel de sistema que se utiliza en un proceso de aprobación. Un mensaje advierte de que puede eliminar el estado desbloqueado de sus grupos, lo que impediría que los miembros del grupo usen correctamente ese proceso de aprobación para los objetos asignados a su grupo.</li>
       <li>Un usuario comienza a editar un proceso de aprobación que utiliza un estado desbloqueado. Un mensaje alerta al usuario sobre el estado de desbloqueo para que pueda evaluar si sería buena idea volver a bloquearlo o reemplazarlo.</li>
       <li>Un proceso de aprobación a nivel de sistema con un estado desbloqueado se adjunta en un objeto y el estado se eliminó para el grupo asignado al objeto. Cuando un miembro del grupo va a la sección Approvals del objeto, un mensaje explica que el proceso de aprobación no se puede iniciar para el objeto.</li>
       </ul>
       <p>Para obtener más información sobre los estados de bloqueo, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Estados de nivel de sistema bloqueados y desbloqueados</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   Para obtener instrucciones sobre cómo convertir este estado en un estado predeterminado, consulte [Usar estados personalizados como estados predeterminados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

Para obtener información sobre cómo reordenar los estados de los grupos, consulte [Reordenar los estados del sistema y del grupo](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
