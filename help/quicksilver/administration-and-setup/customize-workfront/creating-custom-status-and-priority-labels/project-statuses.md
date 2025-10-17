---
title: Acceso a la lista de estados de proyectos del sistema
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Los usuarios pueden especificar el estado de un proyecto para que otros usuarios puedan ver su fase actual de desarrollo en un momento determinado.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 96%

---

# Acceder a la lista de estados de proyectos del sistema

Los usuarios pueden especificar el estado de un proyecto para que otros usuarios puedan ver su fase actual de desarrollo en un momento determinado.

Workfront viene con 9 estados de proyectos del sistema. Se puede cambiar el nombre de estos estados, pero no eliminarlos.

También se pueden añadir estados de proyectos personalizados para que coincidan con las necesidades de su organización.

Como persona con la función de administrador de Workfront, puede configurar el estado predeterminado de todos los proyectos nuevos del sistema. Para obtener instrucciones, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

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

## Acceder a los estados de proyectos

Como persona con la función de administrador de Workfront, puede acceder a la lista de estados de proyectos del nivel de sistema.

Para obtener información sobre cómo editar el estado de un sistema y crear estados personalizados, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** > **Estados**.

1. Haga clic en la pestaña **Proyecto**.

   Los estados de proyectos disponibles en Workfront se enumeran en esta pestaña.

   ![Estado del proyecto](assets/project-status.png)

   Para obtener detalles acerca de cada uno de los estados de proyectos integrados del sistema, consulte [Información general sobre los estados de los proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## Creación de estados de proyectos personalizados y personalización de estados del sistema

Como persona con la función de administrador de Workfront, puede añadir estados de proyectos del sistema a Workfront. Como propietario de un grupo, puede añadir un estado personalizado específico a un grupo. Para obtener más información sobre cómo crear estados personalizados o editar los del sistema, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Al crear un estado de proyecto personalizado, siempre debe equiparar el nuevo estado con un estado del sistema existente. Debe comprender el comportamiento de los estados del sistema para saber con qué estado es adecuado equiparar su estado personalizado. Después de seleccionar la equiparación de estado, esta selección no se puede cambiar. Para obtener más información sobre los estados de los proyectos del sistema, consulte [Información general sobre los estados de los proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
