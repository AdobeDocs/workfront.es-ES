---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurar las preferencias de Administración de recursos
description: Como [!DNL Adobe Workfront] administrador puede configurar las preferencias de administración de recursos para su sistema. Estas preferencias de Administración de recursos determinan cómo se calculan la disponibilidad o capacidad del usuario y el FTE para el [!DNL Workfront] herramientas de planificación y programación de recursos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Configurar [!UICONTROL Gestión de recursos] preferencias

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Como [!DNL Adobe Workfront] administrador puede configurar la variable [!UICONTROL Gestión de recursos] Preferencias para su sistema. Estas preferencias determinan cómo se calculan la disponibilidad del usuario o la capacidad y los FTE para el [!DNL Workfront] herramientas de planificación y programación de recursos.

Para obtener información sobre planificación y programación de recursos en [!DNL Workfront], consulte [Introducción a la administración de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Nivel de acceso del administrador del sistema</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar [!UICONTROL Gestión de recursos] preferencias

>[!NOTE]
>
>Debido a que esta es una configuración global, esta selección afecta a todos los cálculos para todo el sistema, para todos los usuarios, en todas las herramientas de administración de recursos y para todos los grupos de recursos.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).
1. Haga clic en **[!UICONTROL Gestión de recursos]**.
1. Seleccione uno de los siguientes métodos para calcular la disponibilidad de los usuarios en [!DNL Workfront]:

   * **La programación predeterminada**: [!DNL Workfront] utiliza la programación predeterminada del sistema y el editor de texto independiente del usuario para calcular las horas disponibles del usuario en las herramientas de administración de recursos.\

      Para obtener más información sobre las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obtener más información sobre el valor de FTE del usuario, consulte  [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront calcula las horas disponibles de un usuario mediante la fórmula siguiente cuando el administrador de Workfront elige La programación predeterminada:

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **Ejemplo:**\
      Por ejemplo, si la programación predeterminada es de 40 horas por semana y el FTE en el perfil del usuario es de 0,5, el usuario estará disponible para trabajar durante 20 horas por semana.

      Si el usuario tiene una hora de tiempo libre un día, sus horas disponibles se calcularán de la siguiente manera:

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

      <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
        <div class="example" data-mc-autonum="<b>Example: </b>">      
        <span class="autonumber"><span><b>Example: </b></span></span>      
        <div>      
        <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
        <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
        <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
        </div>      
        </div></li>      
        -->

   * **Programación del usuario**: [!DNL Workfront] utiliza la programación del usuario y la programación predeterminada del sistema para calcular el valor de FTE disponible del usuario en las herramientas de administración de recursos. Las horas disponibles se calculan según la programación del usuario. Se ignora el valor del FTE del usuario. Esta es la configuración predeterminada.

      >[!NOTE]
      >
      >Si el usuario no está asociado a una programación, las horas disponibles para el usuario se calculan mediante la programación predeterminada.

      El FTE disponible para el usuario se calcula mediante la fórmula siguiente:

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **Ejemplo:** Por ejemplo, si la programación predeterminada es de 40 horas por semana y la programación del usuario es de 30 horas por semana, el FTE del usuario es de 0,75.

      Si el usuario tiene 2 horas de tiempo libre un día, su tiempo disponible semanal se calculará de la siguiente manera:

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. Haga clic en **[!UICONTROL Guardar]**.
