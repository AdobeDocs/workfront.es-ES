---
title: Adjuntar una tarjeta de tarifas a un proyecto
description: Al adjuntar una tarjeta de tarifas a un proyecto, se añaden al proyecto todas las funciones por ubicación y sus tarifas de facturación asociadas.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 97%

---

# Adjuntar una tarjeta de tarifas a un proyecto

{{highlighted-preview-article-level}}

Las tarjetas de tarifas almacenan varias tarifas de facturación por función, según la ubicación. Podría tener una función de diseñador con sede en París y un segundo diseñador con sede en Nueva York, cada uno con diferentes tarifas de facturación. Sin embargo, no se requiere una ubicación para las funciones en una tarjeta de tarifas. Una tarifa de facturación para una función (y posiblemente una ubicación) en una tarjeta de tarifas también puede incluir fechas efectivas.

Al adjuntar una tarjeta de tarifas a un proyecto, se añaden al proyecto todas las funciones por ubicación y sus tarifas de facturación asociadas.

>[!NOTE]
>
>Al adjuntar una tarjeta de tarifas, se anulan las tarifas de facturación existentes en el proyecto.

Puede editar las tarifas de facturación desde la tarjeta de tarifas directamente en el proyecto. Esto no afecta a las tarifas guardadas en la tarjeta de tarifas predeterminadas.

Para obtener información sobre cómo crear tarjetas de tarifas, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Para obtener información general acerca de cómo anular las tarifas de facturación de funciones para los proyectos y calcular los ingresos del proyecto, consulte [Información general sobre cómo anular las tarifas de facturación de funciones y calcular los ingresos en un proyecto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos y datos financieros</p> <p>Acceso administrativo para funciones del puesto</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Permisos de administración para el proyecto con permisos para administrar finanzas </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adjuntar una tarjeta de tarifas a un proyecto

1. Vaya al proyecto. 
1. Haga clic en **Tarifas de facturación** en el panel izquierdo. Es posible que primero tenga que hacer clic en **Mostrar más**.
1. Haga clic en **Añadir tarifa de facturación > Adjuntar una tarjeta de tarifas**.

   Se abre la página Adjuntar una tarjeta de tarifas. Para obtener más información, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Seleccione la tarjeta de tarifas que se añadirá al proyecto y haga clic en **Adjuntar**.

   La tarjeta de tarifas y todas las tarifas de su función se añaden a la lista de tarifas de facturación.

   ![Tarjeta de tarifas añadida al proyecto](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >En la lista de tarifas de facturación, puede eliminar una o varias funciones que provengan de una tarjeta de tarifas. Al quitar una tarifa de facturación de función del proyecto, no se elimina de la tarjeta de tarifas predeterminada.
