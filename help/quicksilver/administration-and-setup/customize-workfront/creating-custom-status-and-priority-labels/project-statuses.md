---
title: Acceso a la lista de estados de proyectos del sistema
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Los usuarios pueden especificar el estado de un proyecto para que otros usuarios puedan ver su fase actual de desarrollo en un momento determinado.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Acceso a la lista de estados de proyectos del sistema

Los usuarios pueden especificar el estado de un proyecto para que otros usuarios puedan ver su fase actual de desarrollo en un momento determinado.

Workfront viene con 9 estados de proyecto del sistema. Puede cambiar el nombre de estos estados, pero no puede eliminarlos.

También puede agregar estados de proyecto personalizados para que coincidan con las necesidades de su organización.

Como administrador de Workfront, puede configurar el estado predeterminado de todos los proyectos nuevos del sistema. Para obtener instrucciones, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Acceso a los estados del proyecto

Como administrador de Workfront, puede acceder a la lista de estados de proyectos de nivel del sistema.

Para obtener información sobre cómo editar el estado de un sistema y crear estados personalizados, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** > **Estados**.

1. Haga clic en la ficha **Proyecto**.

   Los estados de proyecto disponibles en Workfront se enumeran en esta pestaña.

   ![](assets/project-status.png)

   Para obtener detalles acerca de cada uno de los estados de proyectos de sistema integrados, vea [Información general sobre los estados de proyectos de sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## Creación de estados de proyecto personalizados y personalización de estados del sistema

Como administrador de Workfront, puede agregar estados de proyectos del sistema a Workfront. Como propietario de un grupo, puede agregar un estado personalizado específico a un grupo. Para obtener más información sobre cómo crear estados personalizados o editar los del sistema, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Al crear un estado de proyecto personalizado, siempre debe equiparar el nuevo estado con un estado de sistema existente. Debe comprender el comportamiento de los estados del sistema para saber con qué estado es adecuado equiparar su estado personalizado. Después de seleccionar la igualdad de estado, esta selección no se puede cambiar. Para obtener más información sobre los estados de los proyectos del sistema, vea [Información general sobre los estados de los proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
