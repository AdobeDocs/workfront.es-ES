---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configurar si se registra en horas o días
description: Como usuario con una licencia de planificación, puede configurar si registra tiempo en Adobe Workfront en horas o días. Los administradores del sistema pueden configurar esta opción para usuarios individuales o para varios usuarios de su organización. De forma predeterminada, los usuarios registran el tiempo en horas.
author: Lisa
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b0a3a11a3c04a0969bee99f8e1cea231911f0e6a
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 16%

---

# Configurar si se registra en horas o días

Como usuario con una licencia estándar o de planificación, puede configurar si inicia sesión en Adobe Workfront en horas o días. Los administradores del sistema pueden configurar esta opción para usuarios individuales o para varios usuarios de su organización. De forma predeterminada, los usuarios registran el tiempo en horas. Para obtener información acerca de cómo registrar tiempo en Workfront, consulte [Registrar tiempo](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Se recomienda registrar el tiempo del mismo modo, ya sea horas o días, en toda la organización para garantizar la precisión de la creación de informes.

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
   <td>
   <p>Estándar</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td><p>Los usuarios de Standard y Plan pueden configurar el tiempo ellos mismos. Solo un administrador de Workfront puede configurar el tiempo para otros usuarios.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

1. Realice una de las siguientes acciones, según el objetivo y el nivel de acceso del sistema:

   * **Usuario estándar o planificado que configura el registro de tiempo para usted:** Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en el nombre de usuario que aparece junto a la imagen de perfil. O (si está disponible), haz clic en tu imagen de perfil en el área de navegación superior y luego haz clic en **[!UICONTROL Perfil de Workfront]**. A continuación, haga clic en el icono **Más** junto a su nombre y seleccione **Editar**.

   * **Administrador del sistema configurando el registro de tiempo para otros:** Empiece a editar una o más cuentas de usuario, tal como se describe en [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. En el cuadro de diálogo resultante, en la sección **Planificación de recursos**, busque la opción **Registrar tiempo en**.

   ![Registrar tiempo en opciones](assets/user-profile-log-time-options.png)

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
