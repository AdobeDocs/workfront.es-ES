---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configurar el efecto en horas cuando se elimina y restaura un objeto
description: Puede configurar lo que sucede a las horas en las que alguien elimina un proyecto, tarea o problema con el que se registran las horas. La opción que elija también determina qué sucederá con las horas si el proyecto, la tarea o el problema se restauran más adelante. (Para obtener más información sobre la restauración de elementos en Workfront, consulte Restaurar elementos eliminados).
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Configurar el efecto en horas cuando se elimina y restaura un objeto

Puede configurar lo que sucede a las horas en las que alguien elimina un proyecto, tarea o problema con el que se registran las horas. La opción que elija también determina qué sucederá con las horas si el proyecto, la tarea o el problema se restauran más adelante. (Para obtener más información acerca de cómo restaurar elementos en Workfront, vea [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar cómo se administran las horas cuando se elimina y restaura un elemento

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Expanda **Hojas de horas y horas**, luego haga clic en **Preferencias**.

1. Busque la sección **Preferencias de eliminación de proyecto, tarea o problema**.
1. (Condicional) Para configurar cómo se administran las horas cuando se elimina un proyecto, seleccione una de las siguientes opciones en la sección **Al eliminar proyectos**:

   * Mantener las horas registradas que ya se hayan agregado a las hojas de horas como horas generales (si este proyecto se restaura posteriormente, las horas permanecen en la hoja de horas)\
     Esta opción está seleccionada de forma predeterminada.
   * Eliminar las horas registradas (si este proyecto se restaura más adelante, las horas registradas se restauran en el proyecto)

1. (Condicional) Para configurar cómo se administran las horas cuando se elimina una tarea o un problema, seleccione una de las siguientes opciones en la sección **Al eliminar tareas o problemas**:

   * Mover las horas registradas al proyecto donde resida la tarea o el problema (si esta tarea o este problema se restaura posteriormente, las horas permanecen en el proyecto)\
     Esta opción está seleccionada de forma predeterminada.
   * Eliminar las horas registradas (si esta tarea o este problema se restaura más adelante, las horas registradas se restauran en la tarea o el problema)

1. Haga clic en **Guardar**.
