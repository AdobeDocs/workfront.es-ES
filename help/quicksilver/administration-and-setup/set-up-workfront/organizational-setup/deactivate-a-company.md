---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desactivar o reactivar una compañía
description: Puede desactivar una compañía que ya no utilice y conservar todos sus datos históricos asociados. Si desactiva una compañía que ya está en uso en algún lugar del sistema, seguirá funcionando como siempre. No se ha eliminado ni bloqueado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Desactivar o reactivar una compañía

Puede desactivar una compañía que ya no utilice y conservar todos sus datos históricos asociados. Si desactiva una compañía que ya está en uso en algún lugar del sistema, seguirá funcionando como siempre. No se ha eliminado ni bloqueado.

## Requisitos de acceso

Debe tener lo siguiente para administrar compañías en [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan*</p> </td> 
   <td>[!UICONTROL Team] o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Uno de los siguientes:</p> 
    <ul> 
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator], que permite editar cualquier compañía del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>. </p> </li> 
     <li> <p>Acceso administrativo para gestionar empresas, que permite editar cualquier empresa del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a ciertas áreas</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>También puede administrar empresas asociadas a cualquier grupo al que esté asignado como administrador del grupo.</p> </li> 
      <li> <p>Para agregar y quitar usuarios del sistema [!DNL Workfront], debe tener uno de los siguientes elementos:</p> 
       <ul> 
        <li> <p>Nivel de acceso de [!UICONTROL System Administrator]. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>. </p> </li> 
        <li> <p>En su nivel de acceso, [!UICONTROL Edit] debe estar seleccionado para la opción [!UICONTROL Users]. Además, para la configuración de [!UICONTROL Usuarios], en [!UICONTROL Ajustar la configuración] <img src="assets/gear-icon-in-access-levels.png"> , la opción [!UICONTROL Crear] y al menos una de las dos opciones de [!UICONTROL Administración de usuarios] deben estar habilitadas. </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>Si utiliza la opción [!UICONTROL User Admin (Usuarios del grupo)], debe ser administrador de un grupo del que sea miembro el usuario.</p> </li> 
       </ul> <p>Para obtener información sobre la configuración Usuarios en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Desactivar o reactivar una compañía

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Compañías]** ![](assets/companies-icon-left-panel.png).

1. Seleccione una o varias empresas para desactivar o reactivar.
1. Haga clic en **[!UICONTROL Editar]**.
1. Para una sola compañía, deshabilite la opción **[!UICONTROL Está activo]** para desactivarla o habilite la opción para activarla.

   O

   Para varias empresas, selecciona **[!UICONTROL No]** en el menú desplegable **[!UICONTROL Está activo]** para desactivarlas o **[!UICONTROL Sí]** para activarlas.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
