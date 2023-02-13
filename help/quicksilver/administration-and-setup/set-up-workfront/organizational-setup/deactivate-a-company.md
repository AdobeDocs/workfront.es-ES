---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desactivar o reactivar una empresa
description: Puede desactivar una empresa que ya no utilice conservando todos los datos históricos asociados. Si desactiva una empresa que ya está en uso en algún lugar del sistema, seguirá funcionando como siempre. No se elimina ni se bloquea.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Desactivar o reactivar una empresa

Puede desactivar una empresa que ya no utilice conservando todos los datos históricos asociados. Si desactiva una empresa que ya está en uso en algún lugar del sistema, seguirá funcionando como siempre. No se elimina ni se bloquea.

## Requisitos de acceso

Debe tener lo siguiente para administrar empresas en [!DNL Workfront]:

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
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator], que permite editar cualquier empresa del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p>Acceso administrativo para administrar empresas, que le permite editar cualquier empresa del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>También puede administrar empresas asociadas con cualquier grupo al que tenga asignado como administrador de grupo.</p> </li> 
      <li> <p>Para agregar y eliminar usuarios de la [!DNL Workfront] sistema, debe tener una de las siguientes opciones:</p> 
       <ul> 
        <li> <p>Nivel de acceso de [!UICONTROL System Administrator]. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
        <li> <p>En el nivel de acceso, debe seleccionar [!UICONTROL Edit] para la configuración [!UICONTROL Users]. Además, para la configuración [!UICONTROL Usuarios], en [!UICONTROL Ajuste la configuración] <img src="assets/gear-icon-in-access-levels.png"> , la opción [!UICONTROL Crear] y al menos una de las dos opciones [!UICONTROL User Admin] deben estar activadas. </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>Si utiliza la opción [!UICONTROL User Admin (Group Users)], debe ser administrador de grupo de un grupo del que sea miembro el usuario.</p> </li> 
       </ul> <p>Para obtener información sobre la configuración Usuarios en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Desactivar o reactivar una empresa

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Compañías]** ![](assets/companies-icon-left-panel.png).

1. Seleccione una o varias empresas para desactivarlas o reactivarlas.
1. Haga clic en **[!UICONTROL Editar]**.
1. Para una sola empresa, deshabilite el **[!UICONTROL Está activo]** para desactivarla o activar la opción.

   O

   Para varias empresas, seleccione **[!UICONTROL No]** de la variable **[!UICONTROL Está activo]** menú desplegable para desactivarlos, o **[!UICONTROL Sí]** para activarlos.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
