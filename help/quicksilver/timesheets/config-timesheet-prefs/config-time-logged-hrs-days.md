---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configurar si se registra en horas o días
description: Como usuario con una licencia de planificación, puede configurar si registra tiempo en Adobe Workfront en horas o días. Los administradores del sistema pueden configurar esta opción para usuarios individuales o para varios usuarios de su organización. De forma predeterminada, los usuarios registran el tiempo en horas.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: 106ef838bfee5e496cae864eca5c19fd12fdd18e
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 16%

---

# Configurar si se registra en horas o días

Como usuario con una licencia de Planner, puede configurar si registra tiempo en Adobe Workfront en horas o días. Los administradores del sistema pueden configurar esta opción para usuarios individuales o para varios usuarios de su organización. De forma predeterminada, los usuarios registran el tiempo en horas. Para obtener información acerca de cómo registrar tiempo en Workfront, vea [Registrar tiempo](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Se recomienda registrar el tiempo del mismo modo, ya sea horas o días, en toda la organización para garantizar la precisión de la creación de informes.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Los planificadores pueden configurar el tiempo por sí mismos. Solo un administrador de Workfront puede configurar el tiempo para otros usuarios.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

1. Realice una de las siguientes acciones, según el objetivo y el nivel de acceso del sistema:

   * **Usuario del planificador que configura el registro de tiempo para usted mismo:** Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en su nombre de usuario junto a la imagen de perfil. A continuación, haga clic en el icono **Más** junto a su nombre y seleccione **Editar**.

   * **Administrador del sistema configurando el registro de tiempo para otros:** Empiece a editar una o más cuentas de usuario, tal como se describe en [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. En el cuadro de diálogo resultante, en la sección **Planificación de recursos**, busque la opción **Registrar tiempo en**.

   ![Registrar tiempo en opciones](assets/user-profile-log-time-options.png)

1. (Condicional) Si es administrador del sistema y edita varios usuarios simultáneamente, seleccione **Registrar tiempo en**.
1. Seleccione entre las siguientes opciones para registrar el tiempo:

   | Opción | Descripción |
   |---|---|
   | **Horas** | Los usuarios especifican horas al registrar el tiempo en Workfront. |
   | **Días** | Los usuarios especifican días al registrar la hora en Workfront. |

1. (Condicional) Si seleccionó registrar el tiempo en días, en el campo **Horas equivalentes a Workday completo**, escriba el número de horas que equivale a un día completo. Un día en la plantilla de horas de un usuario equivale al número de horas que se introduce aquí.

   Tenga en cuenta lo siguiente al configurar esta opción:

   * Esta opción no está disponible al configurar para registrar el tiempo en horas.
   * Esta opción solo se utiliza para registrar el tiempo. Esta opción no está relacionada con la opción **Programar** que también está disponible al editar un usuario. La opción **Schedule** se usa al calcular escalas de tiempo y en otras áreas de Workfront. (Para obtener más información sobre el uso de la opción **Programar**, consulte [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Haga clic en **Guardar cambios**.
