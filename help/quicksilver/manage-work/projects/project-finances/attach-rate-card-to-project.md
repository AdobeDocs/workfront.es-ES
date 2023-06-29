---
title: Adjuntar una tarjeta de tarifa a un proyecto
description: Al adjuntar una tarjeta de tarifas a un proyecto, se agregan al proyecto todas las funciones por ubicación y sus tarifas de facturación asociadas.
author: Lisa
feature: Work Management
role: User
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Adjuntar una tarjeta de tarifa a un proyecto

{{highlighted-preview-article-level}}

Las tarjetas de tarifas almacenan varias tarifas de facturación por rol, según la ubicación. Podría tener una función de Designer con sede en París y una segunda función de Designer con sede en Nueva York, cada una con diferentes tarifas de facturación. Sin embargo, no se requiere una ubicación para los roles en una tarjeta de tarifas. Una tarifa de facturación para un rol (y posiblemente una ubicación) en una tarjeta de tarifas también puede incluir fechas efectivas.

Al adjuntar una tarjeta de tarifas a un proyecto, se agregan al proyecto todas las funciones por ubicación y sus tarifas de facturación asociadas.

>[!NOTE]
>
>Al adjuntar una tarjeta de tarifas, se anulan las tarifas de facturación existentes en el proyecto.

Puede editar las tarifas de facturación desde la tarjeta de tarifas directamente en el proyecto. Esto no afecta a las tarifas almacenadas en la tarjeta de tarifas predeterminadas.

Para obtener información sobre la creación de tarjetas de tarifa, consulte [Administrar tarjetas de tarifa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Para obtener información general sobre la anulación de tarifas de facturación de roles de trabajo para proyectos y el cálculo de ingresos de proyectos, consulte [Resumen de anulación de Tarifas de facturación de rol y cálculo de ingresos en un proyecto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Estándar</p><p>O</p><p>Plan heredado: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y datos financieros</p> <p>Acceso administrativo para funciones del puesto</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto con permisos para Administrar finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Adjuntar una tarjeta de tarifa a un proyecto

1. Vaya al proyecto.
1. Clic **Tarifas de facturación** en el panel izquierdo. Es posible que primero tenga que hacer clic en **Mostrar más**.
1. Clic **Agregar tarifa de facturación > Adjuntar una tarjeta de tarifa**.

   Se abrirá la página Adjuntar una tarjeta de tarifa. Para obtener más información, consulte [Administrar tarjetas de tarifa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Seleccione la tarjeta de tarifas que desea añadir al proyecto y haga clic en **Adjuntar**.

   La tarjeta de tarifas y todas las tarifas de su rol se agregan a la lista de tarifas de facturación.

   ![Tarjeta de tarifas agregada al proyecto](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >En la lista de tarifas de facturación, puede eliminar uno o más roles de trabajo que provengan de una tarjeta de tarifas. Al eliminar una tarifa de facturación de rol del proyecto, no se elimina de la tarjeta de tarifas predeterminada.

