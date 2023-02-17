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
source-git-commit: 95c999a72020ce825f3a8377662c71e35a194d80
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Configurar [!UICONTROL Gestión de recursos] preferencias

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa.</span>

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

## Información que se tiene en cuenta al calcular la capacidad de un usuario

Al calcular la capacidad de un usuario, Workfront tiene en cuenta la siguiente información:

* El número de horas programadas, tal como se define en la programación del usuario o en la [!UICONTROL Programación predeterminada]
* [!UICONTROL Programación] [!UICONTROL Excepciones] (dependiendo de qué [!UICONTROL Programación] se utiliza, puede ser las excepciones de la programación del usuario o las asociadas con la variable [!DNL Workfront] [!UICONTROL Programación predeterminada])
* Tiempo de espera del usuario
* El valor del equivalente de tiempo completo ([!UICONTROL FTE]) del usuario o del del [!DNL Workfront] sistema. La variable [!UICONTROL FTE] es igual a 1 cuando el usuario trabaja a tiempo completo, tal como se define en la programación.
* <span class="preview">El valor de [!UICONTROL Tiempo de trabajo] para el usuario que hace referencia al tiempo que el usuario emplea en el trabajo relacionado con el proyecto. Esto no incluye el tiempo invertido, como las reuniones y la formación. La variable [!UICONTROL Tiempo de trabajo] es igual a 1 cuando el usuario está disponible para trabajar todo el tiempo indicado por la variable [!UICONTROL FTE] o el programa, lo que significa que no pasan tiempo en trabajos no relacionados con proyectos como reuniones o capacitación.</span>

Para obtener información sobre planificación y programación de recursos en [!DNL Workfront], consulte [Introducción a la administración de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configurar [!UICONTROL Gestión de recursos] preferencias

>[!NOTE]
>
>Debido a que esta es una configuración global, esta selección afecta a todos los cálculos para todo el sistema, para todos los usuarios, en todas las herramientas de administración de recursos.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).
1. Haga clic en **[!UICONTROL Gestión de recursos]**.
1. Seleccione uno de los siguientes métodos para calcular la disponibilidad de los usuarios en [!DNL Workfront]:

   * **La programación predeterminada**: [!DNL Workfront] utiliza la programación predeterminada del sistema y el FTE individual del usuario para calcular las horas disponibles del usuario en las herramientas de administración de recursos.

      Para obtener más información sobre las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obtener más información sobre cómo localizar el valor de la variable [!UICONTROL FTE], consulte  [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront calcula las horas disponibles de un usuario mediante la fórmula siguiente cuando el administrador de Workfront elige [!UICONTROL Programación predeterminada]:


      En el entorno Producción:

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

      <div class="preview">

      En el entorno de vista previa:

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >Por ejemplo, si el Programa predeterminado es de 40 horas por semana, el FTE en el perfil del usuario es de 0,5, el usuario tiene 1 hora de Tiempo libre un día y el valor de [!UICONTROL Tiempo de trabajo] en el perfil del usuario es 0,5, el usuario está disponible para el trabajo real del proyecto durante 9,5 horas a la semana.
      >
      >Si el usuario tiene una hora de tiempo libre un día, sus horas disponibles se calcularán de la siguiente manera:
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>


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
      >Si el usuario no está asociado a una programación, las horas disponibles para el usuario se calculan usando solo la variable [!UICONTROL Programación predeterminada].

      En el entorno Producción:


      Las horas disponibles para el usuario se calculan mediante la fórmula siguiente:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```

      Los [!UICONTROL FTE] para el usuario se calcula mediante la fórmula siguiente:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
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

      <div class="preview">

      En el entorno de vista previa:

      Las horas disponibles para el usuario se calculan mediante la fórmula siguiente:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```

      Los [!UICONTROL FTE] para el usuario se calcula mediante la fórmula siguiente:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Por ejemplo, si la variable [!UICONTROL Programación predeterminada] es de 40 horas por semana, la programación del usuario es de 30 horas por semana y la del usuario [!UICONTROL Tiempo de trabajo] es 0,5 la variable [!UICONTROL FTE] del usuario es 0.35.
      >
      >Si el usuario tiene 2 horas de tiempo libre un día, su disponibilidad semanal [!UICONTROL FTE] se calcularán de la siguiente manera:
      >
      >
      ```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```

      </div>

1. Haga clic en **[!UICONTROL Guardar]**.
