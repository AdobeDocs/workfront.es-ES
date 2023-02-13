---
title: Acceda a la lista de estados de problemas del sistema
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Puede utilizar el estado de un problema para mostrar a los usuarios del sistema en qué fase de desarrollo se encuentra un problema en un momento determinado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# Acceda a la lista de estados de problemas del sistema

Puede utilizar el estado de un problema para mostrar a los usuarios del sistema en qué fase de desarrollo se encuentra un problema en un momento determinado.

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

## Acceso a estados de problemas

Puede acceder y modificar los estados de problemas a nivel de sistema. Puede editar información sobre los estados predeterminados del sistema o crear nuevos estados personalizados. Para obtener más información sobre la creación de estados personalizados o la edición de estados del sistema, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Para acceder a los estados de problemas a nivel de sistema:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Preferencias de proyecto** > **Estados**.

1. Haga clic en el **Problemas** para ver los estados de los problemas disponibles en Workfront.

   ![](assets/issue-status.png)

## Estados de problemas del sistema

Workfront incluye 10 estados de problemas originales. Los 4 primeros de la tabla siguiente son obligatorios, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos.

Puede agregar estados de problemas personalizados para que coincidan con las necesidades de su organización. Para obtener más información, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Para los usuarios, cambiar el estado de un problema suele ser un proceso manual. Sin embargo, hay situaciones que se describen en la siguiente lista, en las que el estado de un problema cambia automáticamente, según otros factores que estén ocurriendo en el sistema.

Los siguientes estados de problemas se proporcionan con la instancia de Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Estado del problema del sistema</th> 
   <th>Cómo se puede utilizar el estado</th> 
   <th>Qué sucede en el estado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nuevo (estado requerido)</td> 
   <td>Este es el estado predeterminado de cada problema recién creado.</td> 
   <td>Si el problema está en un proyecto con el estado Actual, el problema aparece en la pestaña Solicitudes de trabajo de los usuarios asignados al problema. Los usuarios ahora pueden empezar a trabajar en el problema.</td> 
  </tr> 
  <tr> 
   <td>In Progress (estado requerido)</td> 
   <td> <p>Puede colocar un problema en este estado para indicar que se ha iniciado el trabajo en ese problema.</p> <p>Si la resolución del problema está conectada a otro objeto (una tarea, un proyecto u otro problema), el estado del problema se cambia automáticamente a In Progress cuando se cambia el estado del objeto de resolución a In Progress. </p> <p>Para obtener más información sobre la resolución de objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y resolución de objetos </a>.</p> </td> 
   <td> <p>Si el problema está en un proyecto con el estado Actual, el problema se muestra en la pestaña Trabajar en de los usuarios asignados al problema.</p> <p>Cuando un problema está en curso, el problema muestra un valor para la fecha de inicio real.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Cerrado (estado requerido)</td> 
   <td> <p>Puede marcar manualmente un problema como Cerrado cuando se complete el trabajo en él. </p> <p>Si la resolución del problema está conectada a otro objeto (una tarea, un proyecto u otro problema), el estado del problema se cambia a Cerrado automáticamente al cambiar el estado del objeto resuelto a Cerrado.</p> <p>Para obtener más información sobre la resolución de objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y resolución de objetos </a>.</p> </td> 
   <td> <p>Cuando se cierra un problema, el problema se elimina de la lista de trabajo activado del usuario asignado. En este caso, el problema muestra un valor para la fecha de finalización real. </p> <p>Cuando se completan todas las tareas y se cierran los problemas de un proyecto, este se puede completar.</p> </td> 
  </tr> 
  <tr> 
   <td>En espera (estado requerido)</td> 
   <td> <p>Puede marcar manualmente un problema como En espera para indicar que se ha producido un retraso al completar el problema. </p> </td> 
   <td> <p>Si el problema está en un proyecto con el estado Actual, el problema se muestra en la pestaña Trabajar en de los usuarios asignados al problema. </p> <p>Cuando se completan todas las tareas de un proyecto, pero hay al menos un problema en espera en el proyecto, este no se puede completar. </p> </td> 
  </tr> 
  <tr> 
   <td>Reabierto (coincide con en curso)</td> 
   <td> <p>Es posible que coloque un problema en este estado para indicar que el trabajo sobre ese tema no se completó cuando el problema se cerró anteriormente, y que fue necesario reabrirlo para completar el trabajo.</p> </td> 
   <td> <p>Si el problema está en un proyecto con el estado Actual, el problema aparece en la pestaña Solicitudes de trabajo de los usuarios asignados al problema. Los usuarios ahora pueden empezar a trabajar en el problema.</p> <p>Este estado es importante en los informes para diferenciar entre problemas que están abiertos por primera vez (normalmente en el estado Nuevo) y problemas que se abren después de haberse cerrado antes (normalmente en el estado Reabierto). </p> </td> 
  </tr> 
  <tr> 
   <td>Esperando comentarios (coincide con en espera)</td> 
   <td>Puede colocar un problema en este estado para indicar que está esperando comentarios (normalmente del Contacto principal) antes de continuar trabajando en el problema. </td> 
   <td> <p>Si el problema está en un proyecto con el estado Actual, el problema se muestra en la pestaña Trabajar en de los usuarios asignados al problema.</p> <p>Si hay un problema en espera de comentarios, no se puede completar un proyecto.</p> <p>Este estado es importante en los informes, para diferenciar entre los problemas que están abiertos actualmente pero que están en proceso de solución (normalmente en el estado En curso) y los que están abiertos actualmente pero no se está trabajando en ellos porque se necesitan más comentarios para completarlos (normalmente en el estado Esperando comentarios ).</p> </td> 
  </tr> 
  <tr> 
   <td>No se puede duplicar (es igual a cerrado)</td> 
   <td>Puede colocar un problema en este estado para indicar que está cerrando el problema, pero no puede ver el problema que activó la apertura del problema. El problema puede seguir existiendo, pero no puede repetirse en un momento determinado. </td> 
   <td> <p>Este estado es importante en los informes, para diferenciar entre los problemas que se completan y cuyo problema se ha solucionado (normalmente en el estado Cerrado) y los problemas cuyo problema no es visible en un momento determinado (normalmente en el estado No se puede duplicar).</p> <p>Cuando un problema está marcado como No se puede duplicar, el problema se elimina de la lista de trabajo activado del usuario asignado. En este caso, el problema muestra un valor para la Fecha de Finalización Real.</p> <p>Si se completan todas las tareas de un proyecto y algunos problemas están en estado No se puede duplicar, se puede completar el proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Resuelto (coincide con cerrado)</td> 
   <td>Puede colocar un problema en este estado para indicar que está cerrando el problema y que el problema que lo creó se ha resuelto.</td> 
   <td> <p>Este estado es importante en los informes, para diferenciar entre problemas que se cierran con o sin una resolución (normalmente en el estado Cerrado) y problemas que se cierran con una resolución real (normalmente en el estado Resuelto).</p> <p>Cuando un problema se marca como Resuelto, se elimina de la lista de trabajo activado del usuario asignado. En este caso, el problema muestra un valor para la fecha de finalización real.</p> <p>Si se completan todas las tareas de un proyecto y al menos un problema está en estado Resuelto, se puede completar el proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>Finalización verificada (equivale a cerrado)</td> 
   <td>Puede colocar un problema en este estado para indicar que está cerrando el problema y que ha verificado que el problema que generó el problema se ha resuelto.</td> 
   <td> <p>Cuando un problema se marca como Verified Complete, el problema se elimina de la lista de Trabajo en. En este caso, el problema muestra un valor para la fecha de finalización real.</p> <p>Si se completan todas las tareas de un proyecto y algunos problemas están en estado Verified Complete , se puede completar el proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>No se resuelve (coincide con cerrado)</td> 
   <td>Puede colocar un problema en este estado para indicar que está cerrando el problema, pero el problema que lo ha generado no se puede resolver.</td> 
   <td> <p>Este estado es importante en los informes, para diferenciar entre problemas que se cierran con o sin una resolución (normalmente en el estado Cerrado) y problemas que se cierran sin una resolución real (normalmente en el estado No Resolver).</p> <p>Cuando un problema está marcado como No se resuelve, el problema se elimina de la lista de trabajo activado del usuario asignado. En este caso, el problema muestra un valor para la fecha de finalización real.</p> <p>Si se completan todas las tareas de un proyecto y al menos un problema está en estado No se resuelve, se puede completar el proyecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalización de los estados de problemas

Un administrador de Workfront puede agregar a Workfront estados de problemas a nivel de sistema y de grupo y cambiar el orden en que los usuarios los ven. Para obtener más información, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Un administrador de grupos puede agregar un estado personalizado específico de un grupo. Para obtener más información, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
