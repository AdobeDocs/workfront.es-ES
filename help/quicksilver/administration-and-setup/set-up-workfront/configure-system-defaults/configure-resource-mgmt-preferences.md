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
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Configurar [!UICONTROL Gestión de recursos] preferencias

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<!--drafted for Work time field: <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Como [!DNL Adobe Workfront] administrador puede configurar la variable [!UICONTROL Gestión de recursos] Preferencias para su sistema. Estas preferencias determinan cómo se calculan las horas del usuario o la disponibilidad o capacidad de los FTE para la variable [!DNL Workfront] herramientas de planificación y programación de recursos.

## Requisitos de acceso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Nivel de acceso del administrador del sistema</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>:

Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

<!--drafted for Work time field: 

## Information taken into account when calculating user's capacity

When calculating a user's capacity, Workfront takes into account the following information:

* The number of scheduled hours, as defined in either the Schedule of the user or the Workfront system's [!UICONTROL Default Schedule]
* [!UICONTROL Schedule] [!UICONTROL Exceptions] (depending on which [!UICONTROL Schedule] is used, it can be the exceptions of the user's schedule, or those associated with the [!DNL Workfront] [!UICONTROL Default Schedule])
* User's time off
* The value of the Full Time Equivalent ([!UICONTROL FTE]) of the user or that of the [!DNL Workfront] system. The [!UICONTROL FTE] equals 1 when the user works full time, as defined in the schedule. 

<!-drafted for Work Time field  

* <span class="preview">The value of [!UICONTROL Work Time] for the user which refers to time that the user spends on project-related work. This does not include overhead time, like meetings and training. The [!UICONTROL Work Time] equals 1 when the user is available for work the entire time as indicated by the [!UICONTROL FTE] or the schedule, which means they don't spend any time in non-project-related work like meetings or trainings.</span>

-->

Para obtener información sobre planificación y programación de recursos en [!DNL Workfront], consulte [Introducción a la administración de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

—>

## Configurar [!UICONTROL Gestión de recursos] preferencias

>[!NOTE]
>
>Debido a que esta es una configuración global, esta selección afecta a todos los cálculos para todo el sistema, para todos los usuarios, en todas las herramientas de administración de recursos y para todos los grupos de recursos.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).
1. Haga clic en **[!UICONTROL Gestión de recursos]**.
1. Seleccione uno de los siguientes métodos para calcular la disponibilidad de los usuarios en [!DNL Workfront]:

   * **La programación predeterminada**: [!DNL Workfront] utiliza la programación predeterminada del sistema y el FTE individual del usuario para calcular las horas disponibles del usuario en las herramientas de administración de recursos.

      Para obtener más información sobre las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obtener más información sobre el valor del usuario [!UICONTROL FTE], consulte  [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront calcula las horas disponibles de un usuario mediante la fórmula siguiente cuando el administrador de Workfront elige [!UICONTROL Programación predeterminada]:

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > Por ejemplo, si la variable [!UICONTROL Programación predeterminada] es de 40 horas semanales y [!UICONTROL FTE] en el perfil del usuario es 0,5, el usuario está disponible para trabajar durante 20 horas a la semana.
      >Si el usuario tiene una hora de tiempo libre un día, sus horas disponibles se calcularán de la siguiente manera:
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
   <!--drafted for Work Time field

      <div class="preview">
      
      In the Preview environment: 

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >For example, if the Default Schedule is 40 hours a week,  the FTE in the profile of the user is 0.5, the user has 1 hour of Time off one day, and the [!UICONTROL Work Time] in the profile of the user is 0.5, the user is available for actual project work for 9.5 hours a week.
      >
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>

   -->

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

   * **Programación del usuario**: [!DNL Workfront] utiliza la programación del usuario, así como el [!UICONTROL Programación predeterminada] del sistema para calcular el [!UICONTROL FTE] valor del usuario en las herramientas de administración de recursos. Las horas disponibles se calculan según la programación del usuario. El valor de la variable [!UICONTROL FTE] del usuario se ignora. Esta es la configuración predeterminada.

      Para obtener más información sobre las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obtener más información sobre el [!UICONTROL Programación], consulte  [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >Si el usuario no está asociado a una programación, las horas disponibles para el usuario se calculan usando la variable [!UICONTROL Programación predeterminada].

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      Los [!UICONTROL FTE] para el usuario se calcula mediante la fórmula siguiente:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Por ejemplo, si la variable [!UICONTROL Programación predeterminada] es de 40 horas semanales y la programación del usuario es de 30 horas semanales, la variable [!UICONTROL FTE] del usuario es 0.70.
      >  
      >Si el usuario tiene 2 horas de tiempo libre un día, su disponibilidad semanal [!UICONTROL FTE] se calcularán de la siguiente manera:
      > 
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```

      <!--drafted for Work Time field:

      <div class="preview">

      In the Preview environment: 
      
      The Available hours for the user is calculated by the following formula:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```    

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week, the schedule of the user is 30 hours a week, and the user's [!UICONTROL Work Time] is 0.5 the [!UICONTROL FTE] of the user is 0.35.
      >
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      >
      >```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```
      (************ checking this second other with Dev/ Artur - not sure where Exceptions fit in **********)

      </div>
      -->
1. Haga clic en **[!UICONTROL Guardar]**.
