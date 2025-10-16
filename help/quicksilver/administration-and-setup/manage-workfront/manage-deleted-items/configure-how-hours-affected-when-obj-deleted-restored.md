---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configurar el efecto en horas cuando se elimina y restaura un objeto
description: Puede configurar lo que ocurre con las horas cuando alguien elimina un proyecto, tarea o problema con el que se registran las horas. La opción que elija también determina qué sucederá con las horas si el proyecto, la tarea o el problema se restauran más adelante. (Para obtener más información sobre la restauración de elementos en Workfront, consulte Restaurar elementos eliminados).
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 93%

---

# Configurar el efecto en horas cuando se elimina y restaura un objeto

Puede configurar lo que ocurre con las horas cuando alguien elimina un proyecto, tarea o problema con el que se registran las horas. La opción que elija también determina qué sucederá con las horas si el proyecto, la tarea o el problema se restauran más adelante. (Para obtener más información acerca de cómo restaurar elementos en Workfront, consulte [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuración de la gestión de las horas cuando se elimina y restaura un elemento

{{step-1-to-setup}}

1. Expanda **Hojas de horas y horas** y luego, haga clic en **Preferencias**.

1. Busque la sección **Preferencias de eliminación del proyecto, tarea o problema**.
1. (Condicional) Para configurar cómo se administran las horas cuando se elimina un proyecto, seleccione una de las siguientes opciones en la sección **Al eliminar proyectos**:

   * Mantenga las horas registradas ya añadidas a las hojas de horas como horas generales (si se restaura este proyecto posteriormente, las horas permanecerán en la plantilla de horas).\
     Esta opción está desactivada de forma predeterminada.
   * Eliminar las horas registradas (si este proyecto se restaura más adelante, las horas registradas se restaurarán en el proyecto)

1. (Condicional) Para configurar cómo se administran las horas cuando se elimina una tarea o un problema, seleccione una de las siguientes opciones en la sección **Al eliminar tareas o problemas**:

   * Mueva las horas registradas al proyecto donde reside la tarea o el problema (si esta tarea o problema se restaura más adelante, las horas permanecerán en el proyecto).\
     Esta opción está desactivada de forma predeterminada.
   * Elimine las horas registradas (si se restaura esta tarea o este problema posteriormente, las horas registradas se restaurarán en la tarea o el problema)

1. Haga clic en **Guardar**.
