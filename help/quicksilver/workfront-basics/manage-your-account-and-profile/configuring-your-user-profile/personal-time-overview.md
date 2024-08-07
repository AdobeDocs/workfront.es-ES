---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configuración del tiempo libre personal
description: Es importante indicar en Adobe Workfront cuándo se produce el tiempo libre aprobado, ya que esto afecta a la programación y afecta a las fechas de finalización planificadas de las tareas a las que está asignado.
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 1%

---

# Configuración del tiempo libre personal

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] no está diseñado para replicar o reemplazar los sistemas existentes para administrar, acumular y rastrear los días libres personales.

Sin embargo, es importante indicar cuándo se producen los días libres aprobados, ya que esto afecta tanto a la programación como a las [!UICONTROL Fechas planificadas de finalización] de las tareas a las que está asignado.

Por ejemplo, si se le asigna una tarea que está programada para tomar dos semanas y planea tomarse tres días libres durante ese tiempo, [!DNL Workfront] agrega tres días a la escala de tiempo de la tarea para tener en cuenta el tiempo libre.

Las herramientas de administración de recursos también utilizan su tiempo libre personal para indicar cuándo está disponible para que se le programe trabajar.

>[!NOTE]
>
>Para garantizar que no se produzcan incoherencias con las fechas en las que programa sus vacaciones, le recomendamos que la zona horaria de su perfil de usuario coincida con la de su programación. Para obtener más información, consulte los siguientes artículos:
>
>* [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: Estándar (para configurar sus días libres personales)</p>
        <p>o</p>
        <p>Actual: Trabaje o superior (para configurar sus días libres personales)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Manager] con acceso de [!UICONTROL Editar usuario] (para realizar cambios en el calendario de días libres de otros usuarios)<br>
   <strong>NOTA:</strong> Si un administrador edita el calendario personal de días libres de otro usuario, todas las entradas se mostrarán en la zona horaria del usuario y no en la del administrador.</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Configurar tiempo libre personal en [!DNL Workfront]

{{step1-click-profile-pic}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Tiempo libre]**.
1. Seleccione la fecha que desee para sus vacaciones personales.

   ![Tiempo libre personal](assets/personal-time-off-calendar.png)

1. Seleccione **[!UICONTROL Todo el día]**, si se toma un día libre completo.

   Deje desactivada la casilla de verificación si se toma menos de un día libre completo e indique las horas de inicio y finalización del tiempo libre.

1. Haga clic en **[!UICONTROL Guardar]**.

   Su tiempo libre ahora es visible en todo el sistema [!DNL Workfront] en las herramientas de administración de recursos como el Planificador de recursos y el Distribuidor de cargas de trabajo. Cuando se le asigna trabajo durante este tiempo, la información del objeto informa al usuario de que ha programado tiempo libre.
