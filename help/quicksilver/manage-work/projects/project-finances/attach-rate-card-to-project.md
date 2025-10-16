---
title: Adjuntar una tarjeta de tarifas a un proyecto
description: Al adjuntar una tarjeta de tarifas a un proyecto, se añaden al proyecto todas las funciones por ubicación y sus tarifas de facturación asociadas.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 93%

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos y datos financieros</p> <p>Acceso administrativo para funciones del puesto</p></td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administrar permisos para el proyecto que incluye Editar datos financieros </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adjuntar una tarjeta de tarifas a un proyecto

1. Vaya al proyecto. 
1. Haga clic en **Tarifas de facturación** en el panel de la izquierda.
1. Haga clic en **Añadir tarifa de facturación > Adjuntar una tarjeta de tarifas**.

   Se abre la página Adjuntar una tarjeta de tarifas. Para obtener más información, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Seleccione la tarjeta de tarifas que se añadirá al proyecto y haga clic en **Adjuntar**.

   La tarjeta de tarifas y todas las tarifas de su función se añaden a la lista de tarifas de facturación.

   ![Tarjeta de tarifas añadida al proyecto](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >En la lista de tarifas de facturación, puede eliminar una o varias funciones que provengan de una tarjeta de tarifas. Al quitar una tarifa de facturación de función del proyecto, no se elimina de la tarjeta de tarifas predeterminada.
