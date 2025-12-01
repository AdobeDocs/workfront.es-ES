---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurar los días libres personales
description: Es importante indicar en Adobe Workfront cuándo tienen lugar los días libres aprobados, ya que esto afecta a la programación y repercute en las fechas de finalización previstas de las tareas que tiene asignadas.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 0e37a5a519770d3d48192f1799491aa53a871508
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 75%

---

# Configurar los días libres personales

<!-- Audited: 12/2025 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

[!DNL Adobe Workfront] no está diseñado para replicar o reemplazar los sistemas existentes de su organización para administrar, acumular o rastrear los días libres personales.

Sin embargo, es importante indicar cuándo tienen lugar los días libres aprobados, ya que esto afecta a la programación y repercute en las [!UICONTROL fechas de finalización previstas] de las tareas que tiene asignadas.

Por ejemplo, si se le asigna una tarea cuya duración prevista es de dos semanas y tiene previsto tomarse tres días libres durante ese tiempo, [!DNL Workfront] añade tres días a la línea de tiempo de la tarea para tener en cuenta los días libres.

Las herramientas de administración de recursos también utilizan sus días libres personales para indicar cuándo está disponible para ser programado para trabajar.

>[!NOTE]
>
>Para garantizar que no se produzcan incoherencias con las fechas en las que programa sus vacaciones, le recomendamos que la zona horaria de su perfil de usuario coincida con la de su programación. Para obtener más información, consulte los siguientes artículos:
>
>* [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td> Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td> <p>Para configurar su tiempo libre personal, debe tener:</p>
        <p>Estándar (para configurar su tiempo libre personal)</p>
        <p>Trabaje o superior (para configurar su tiempo libre personal)</p> </td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td><p>Para realizar cambios en el calendario de días libres de otro usuario, debe ser el administrador de ese usuario y tener acceso de Editar usuario.</p>
   <p><strong>NOTA:</strong> Si un administrador edita el calendario personal de días libres de otro usuario, todas las entradas se mostrarán en la zona horaria del usuario y no en la del administrador.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar los días libres personales en [!DNL Workfront]

{{step1-click-profile-pic}}

>[!NOTE]
>
>Si su organización está en la experiencia unificada de Adobe, haga clic en el menú de cuenta de **Adobe** (su imagen de perfil) en la esquina superior derecha del área de navegación superior y, a continuación, haga clic en **Perfil de Workfront**.
>
>![perfil de workfront](assets/aue-profile.png)

1. En el panel izquierdo, haga clic en **[!UICONTROL Días libres]**.
1. Seleccione la fecha que desee para sus días libres personales.

   ![Calendario personal de días libres](assets/personal-time-off-calendar-0925.png)

   <!--Sample image in the Production environment:
   ![Personal time off calendar](assets/personal-time-off-calendar.png)-->

1. Seleccione **[!UICONTROL Todo el día]**, si se toma un día libre completo.

   Deje desactivada la casilla de verificación si se toma menos de un día libre completo e indique las horas de inicio y finalización de los días libres.

1. Haga clic en **[!UICONTROL Guardar]**.

   Sus días libres son ahora visibles en todo el sistema de [!DNL Workfront] en las herramientas de administración de recursos como el Planificador de recursos y el Distribuidor de cargas de trabajo. Cuando se le asigna trabajo durante este tiempo, una herramienta de ayuda informa al usuario de que ha programado días libres.
