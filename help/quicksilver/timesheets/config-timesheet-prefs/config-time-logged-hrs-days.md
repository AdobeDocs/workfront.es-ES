---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configure si la hora se registra en horas o días
description: Como usuario con una licencia de Plan, puede configurar si inicia sesión en Adobe Workfront en horas o días. Los administradores del sistema pueden configurar esta configuración para usuarios individuales o para varios usuarios de su organización. De forma predeterminada, los usuarios registran la hora en horas.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# Configure si la hora se registra en horas o días

Como usuario con una licencia de Planificador, puede configurar si inicia sesión en Adobe Workfront en horas o días. Los administradores del sistema pueden configurar esta configuración para usuarios individuales o para varios usuarios de su organización. De forma predeterminada, los usuarios registran la hora en horas. Para obtener información sobre cómo iniciar sesión en Workfront, consulte [Tiempo de registro](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Recomendamos registrar la hora del mismo modo, ya sea de horas o de días, en toda la organización para garantizar la precisión de los informes.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Los planificadores pueden configurar el tiempo por sí mismos. Solo los administradores de Workfront pueden configurar el tiempo para otros usuarios.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

1. Realice una de las siguientes acciones, según su objetivo y nivel de acceso en el sistema:

   * **Usuario planificador configurando el registro de tiempo por su cuenta:** Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en su nombre de usuario junto a su imagen de perfil. A continuación, haga clic en el **Más** junto a su nombre y seleccione **Editar**.

   * **Administrador del sistema configurando el registro de tiempo para otros usuarios:** Comience a editar una o varias cuentas de usuario, tal como se describe en [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. En el cuadro de diálogo resultante, en la **Planificación de recursos** , ubique la sección **Iniciar sesión** .

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (Condicional) Si es un administrador del sistema que edita varios usuarios simultáneamente, seleccione **Iniciar sesión**.
1. Seleccione entre las siguientes opciones para el tiempo de registro:

   | Opción | Descripción |
   |---|---|
   | **Horas** | Los usuarios especifican horas al iniciar sesión en Workfront. |
   | **Días** | Los usuarios especifican días al iniciar sesión en Workfront. |

1. (Condicional) Si seleccionó registrar la hora en días, en la variable **Horas equivalentes para Workday completo** , escriba el número de horas que sean iguales a un día completo. Un día en el parte de horas de un usuario es el equivalente al número de horas que escriba aquí.

   Tenga en cuenta lo siguiente al configurar esta configuración:

   * Esta opción no está disponible al configurar para registrar el tiempo en horas.
   * Esta opción solo se utiliza para registrar el tiempo. Esta opción no está relacionada con la variable **Programación** que también está disponible al editar un usuario. La variable **Programación** se utiliza para calcular líneas de tiempo y en otras áreas de Workfront. (Para obtener más información sobre el uso de la variable **Programación** , consulte [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Haga clic en **Guardar cambios**.
