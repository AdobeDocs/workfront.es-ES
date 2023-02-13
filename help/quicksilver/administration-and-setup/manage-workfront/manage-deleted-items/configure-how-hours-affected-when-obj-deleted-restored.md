---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configurar el efecto en horas en las que se elimina y se restaura un objeto
description: Puede configurar lo que sucede a las horas en que alguien elimina un proyecto, una tarea o un problema con el que se han registrado las horas. La opción que elija también determina qué sucede con las horas si el proyecto, la tarea o el problema se restauran más adelante. (Para obtener más información sobre la restauración de elementos en Workfront, consulte Restaurar elementos eliminados).
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Configurar el efecto en horas en las que se elimina y se restaura un objeto

Puede configurar lo que sucede a las horas en que alguien elimina un proyecto, una tarea o un problema con el que se han registrado las horas. La opción que elija también determina qué sucede con las horas si el proyecto, la tarea o el problema se restauran más adelante. (Para obtener más información sobre la restauración de elementos en Workfront, consulte [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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

## Configurar cómo se administran las horas cuando se elimina y se restaura un elemento

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Expandir **Hojas de hora y horas** y haga clic en **Preferencias**.

1. Busque la variable **Preferencias de eliminación de proyectos, tareas o problemas** para obtener más información.
1. (Condicional) Para configurar cómo se administran las horas cuando se elimina un proyecto, seleccione una de las siguientes opciones en la sección **Al eliminar proyectos** sección:

   * Mantener las horas registradas ya agregadas a las hojas de horas como horas generales (si este proyecto se restaura más adelante, las horas permanecerán en el parte de horas)\
      Esta opción está seleccionada de forma predeterminada.
   * Eliminar las horas registradas (si este proyecto se restaura más adelante, las horas registradas se restauran al proyecto)

1. (Condicional) Para configurar cómo se administran las horas cuando se elimina una tarea o problema, seleccione una de las siguientes opciones en la **Al eliminar tareas o problemas** sección:

   * Mover las horas registradas al proyecto en el que reside la tarea o el problema (si esta tarea o problema se restaura más adelante, las horas permanecen en el proyecto)\
      Esta opción está seleccionada de forma predeterminada.
   * Elimine las horas registradas (si esta tarea o problema se restaura más tarde, las horas registradas se restauran a la tarea o problema)

1. Haga clic en **Guardar**.
