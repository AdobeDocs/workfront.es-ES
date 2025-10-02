---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurar los días libres personales
description: Es importante indicar en Adobe Workfront cuándo tienen lugar los días libres aprobados, ya que esto afecta a la programación y repercute en las fechas de finalización previstas de las tareas que tiene asignadas.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: ce2f1ebe7ea97f3c25ac6a7ef33fd3c066727220
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 88%

---

# Configurar los días libres personales

<!-- Audited: 12/2023 -->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado y se va a lanzar en un despliegue gradual en Producción.</span>

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
        <p>Actual: Trabajo o superior (para configurar sus días libres personales)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Manager] con acceso de [!UICONTROL Edit User] (para realizar cambios en el calendario de días libres de otros usuarios)<br>
 <strong>NOTA:</strong> si un administrador edita el calendario personal de días libres de otro usuario, todas las entradas se mostrarán en la zona horaria del usuario y no en la del administrador.</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Configurar los días libres personales en [!DNL Workfront]

{{step1-click-profile-pic}}

>[!NOTE]
>
>Si se encuentra en la experiencia unificada de Adobe, puede acceder a su perfil de Workfront haciendo clic en el menú de cuenta de Adobe (su imagen de perfil) en el área de navegación superior y, a continuación, seleccionando Perfil de Workfront.
>
>![perfil de workfront](assets/aue-profile.png)

1. En el panel izquierdo, haga clic en **[!UICONTROL Días libres]**.
1. Seleccione la fecha que desee para sus días libres personales.

   <span class="preview">Imagen de muestra en el entorno de vista previa:</span>
   ![Calendario personal de días libres](assets/personal-time-off-calendar-0925.png)

   Imagen de muestra en el entorno de producción:
   ![Calendario personal de días libres](assets/personal-time-off-calendar.png)

1. Seleccione **[!UICONTROL Todo el día]**, si se toma un día libre completo.

   Deje desactivada la casilla de verificación si se toma menos de un día libre completo e indique las horas de inicio y finalización de los días libres.

1. Haga clic en **[!UICONTROL Guardar]**.

   Sus días libres son ahora visibles en todo el sistema de [!DNL Workfront] en las herramientas de administración de recursos como el Planificador de recursos y el Distribuidor de cargas de trabajo. Cuando se le asigna trabajo durante este tiempo, una herramienta de ayuda informa al usuario de que ha programado días libres.
