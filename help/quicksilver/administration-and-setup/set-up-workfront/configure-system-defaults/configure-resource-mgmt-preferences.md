---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurar preferencias de administración de recursos
description: Como administrador de  [!DNL Adobe Workfront] puede configurar las Preferencias de administración de recursos para su sistema. Estas preferencias de Administración de recursos determinan cómo se calculan la disponibilidad o capacidad del usuario y el valor de FTE para las herramientas de planificación y programación de recursos  [!DNL Workfront] e.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# Configurar las preferencias de [!UICONTROL Administración de recursos]

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Como administrador de [!DNL Adobe Workfront], puede configurar las preferencias de [!UICONTROL Administración de recursos] para su sistema. Estas preferencias determinan cómo se calcula la disponibilidad o capacidad de horas de usuario o FTE para las herramientas de planificación y programación de recursos de [!DNL Workfront].

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

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>Nivel de acceso del administrador del sistema</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>.</p> <p><b>NOTA</b>:

Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

+++

## Información que se tiene en cuenta al calcular la capacidad de un usuario

Al calcular la capacidad de un usuario, Workfront tiene en cuenta la siguiente información:

* La cantidad de horas programadas, tal como se define en el Horario del usuario o en el [!UICONTROL Horario predeterminado] del sistema Workfront
* [!UICONTROL Horario] [!UICONTROL Excepciones] (dependiendo de qué [!UICONTROL Horario] se use, pueden ser las excepciones de la programación del usuario o las asociadas con el [!DNL Workfront] [!UICONTROL Horario predeterminado])
* Tiempo libre del usuario
* El valor del equivalente a tiempo completo ([!UICONTROL FTE]) del usuario o del sistema [!DNL Workfront]. El [!UICONTROL ETC] es igual a 1 cuando el usuario trabaja a tiempo completo, tal como se define en la programación.
* El valor de [!UICONTROL Tiempo de trabajo] para el usuario que hace referencia al tiempo que el usuario dedica al trabajo relacionado con el proyecto. Esto no incluye el tiempo de espera, como reuniones y formación. El [!UICONTROL Tiempo de trabajo] es igual a 1 cuando el usuario está disponible para trabajar todo el tiempo, tal como se indica en el [!UICONTROL ETC] o en el horario, lo que significa que no invierte ningún tiempo en trabajo no relacionado con el proyecto, como reuniones o capacitaciones.


Para obtener información acerca de la planificación y programación de recursos en [!DNL Workfront], vea [Introducción a la administración de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configurar las preferencias de [!UICONTROL Administración de recursos]

>[!NOTE]
>
>Como se trata de una configuración global, esta selección afecta a todos los cálculos del sistema completo, para todos los usuarios, en todas las herramientas de administración de recursos.

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Administración de recursos]**.
1. Seleccione uno de los siguientes métodos para calcular la disponibilidad de los usuarios en [!DNL Workfront]:

   * **El horario predeterminado**: [!DNL Workfront] utiliza el horario predeterminado del sistema y el valor de FTE individual del usuario para calcular las horas disponibles del usuario en las herramientas de administración de recursos.

     Para obtener más información acerca de las programaciones, vea [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Para obtener más información sobre cómo encontrar el valor del [!UICONTROL ETC] del usuario, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     Workfront calcula las horas disponibles de un usuario mediante la fórmula siguiente cuando el administrador de Workfront elige el [!UICONTROL horario predeterminado]:


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Por ejemplo, si el Horario predeterminado es de 40 horas a la semana, el valor de FTE en el perfil del usuario es 0,5, el usuario tiene 1 hora libre un día y el valor de [!UICONTROL Tiempo de trabajo] en el perfil del usuario es 0,5, el usuario está disponible para trabajar realmente en el proyecto durante 9,5 horas a la semana.
     >
     >Si el usuario tiene 1 hora de tiempo libre un día, las horas disponibles se calcularán de la siguiente manera:
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
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

   * **El horario del usuario**: [!DNL Workfront] utiliza el horario del usuario así como el [!UICONTROL Horario predeterminado] del sistema para calcular el valor de [!UICONTROL FTE] disponible del usuario en las herramientas de administración de recursos. Las horas disponibles se calculan según la programación del usuario. Se ignora el valor de [!UICONTROL FTE] del usuario. Esta es la configuración predeterminada.

     Para obtener más información acerca de las programaciones, vea [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Para obtener más información sobre el [!UICONTROL horario] de un usuario, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     >[!NOTE]
     >
     >Si el usuario no está asociado a una programación, las horas disponibles para el usuario se calculan usando solamente el [!UICONTROL horario predeterminado].

     Las horas disponibles para el usuario se calculan mediante la siguiente fórmula:


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     El [!UICONTROL ETC] disponible para el usuario se calcula mediante la siguiente fórmula:


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Por ejemplo, si el [!UICONTROL horario predeterminado] es de 40 horas a la semana, el horario del usuario es de 30 horas a la semana y el [!UICONTROL tiempo de trabajo] del usuario es de 0,5, mientras que el [!UICONTROL ETC] del usuario es de 0,35.
     >
     >Si el usuario tiene 2 horas de tiempo libre un día, su [!UICONTROL ETC] disponible semanalmente se calculará de la siguiente manera:
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. Haga clic en **[!UICONTROL Guardar]**.
