---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desactivar o reactivar una compañía
description: Puede desactivar una compañía que ya no utilice y conservar todos sus datos históricos asociados. Si desactiva una compañía que ya está en uso en algún lugar del sistema, seguirá funcionando como siempre. No se ha eliminado ni bloqueado.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 1%

---

# Desactivar o reactivar una compañía

Puede desactivar una compañía que ya no utilice y conservar todos sus datos históricos asociados. Si desactiva una compañía que ya está en uso en algún lugar del sistema, seguirá funcionando como siempre. No se ha eliminado ni bloqueado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td><p>Actual: [!UICONTROL Equipo] o superior</p>
   <p>O</p>
   <p>Nuevo: Cualquiera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licencia</p> </td> 
   <td><p>Actual: [!UICONTROL plan]</p>
   <p>O</p>
   <p>Nuevo: [!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong> </td> 
   <td> <p>Uno de los siguientes:</p> 
    <ul> 
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator], que permite editar cualquier compañía del sistema.</p> </li> 
     <li> <p>Acceso administrativo para gestionar empresas, que permite editar cualquier empresa del sistema.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>También puede administrar empresas asociadas a cualquier grupo al que esté asignado como administrador del grupo.</p> </li> 
      <li> <p>Para agregar y quitar usuarios del sistema [!DNL Workfront], debe tener uno de los siguientes elementos:</p> 
       <ul> 
        <li> <p>Nivel de acceso de [!UICONTROL System Administrator].</p> </li> 
        <li> <p>En su nivel de acceso, [!UICONTROL Edit] debe estar seleccionado para la opción [!UICONTROL Users]. Además, para la configuración de [!UICONTROL Usuarios], en [!UICONTROL Ajustar la configuración] <img src="assets/gear-icon-in-access-levels.png"> , la opción [!UICONTROL Crear] y al menos una de las dos opciones de [!UICONTROL Administración de usuarios] deben estar habilitadas. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si utiliza la opción [!UICONTROL User Admin (Usuarios del grupo)], debe ser administrador de un grupo del que sea miembro el usuario.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desactivar o reactivar una compañía

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Compañías]** ![](assets/companies-icon-left-panel.png).

1. Seleccione una o varias empresas para desactivar o reactivar.
1. Haga clic en **[!UICONTROL Editar]**.
1. Para una sola compañía, deshabilite la opción **[!UICONTROL Está activo]** para desactivarla o habilite la opción para activarla.

   O

   Para varias empresas, selecciona **[!UICONTROL No]** en el menú desplegable **[!UICONTROL Está activo]** para desactivarlas o **[!UICONTROL Sí]** para activarlas.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
