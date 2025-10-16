---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desactivar o reactivar una compañía
description: Puede desactivar una compañía que ya no utilice y conservar a la vez todos sus datos históricos asociados. Si desactiva una compañía que ya está en uso en algún lugar del sistema, seguirá funcionando como siempre lo ha hecho. No se elimina ni se bloquea.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 8fb17d1008b00bc0701ce6e2f06c59d020510e90
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 57%

---

# Desactivación o reactivación de una compañía

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

Puede desactivar una compañía que ya no utilice y conservar a la vez todos sus datos históricos asociados. Si desactiva una compañía que ya está en uso en algún lugar del sistema, seguirá funcionando como siempre lo ha hecho. No se elimina ni se bloquea.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] paquete</p> </td> 
   <td><p>Cualquiera</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
  <td> <p>Debe tener uno de los siguientes elementos:</p> 
    <ul> 
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator], que permite editar cualquier compañía del sistema.</p> </li> 
     <li> <p>Acceso administrativo para gestionar empresas, que permite editar cualquier empresa del sistema.</p> </li> 
    </ul> <p><b>NOTA</b>:
     <ul> 
      <li> <p>También puede administrar compañías asociadas a cualquier grupo en el que esté asignado como administrador de grupos.</p> </li> 
      <li> <p>Para agregar y quitar usuarios del sistema [!DNL Workfront], debe tener uno de los siguientes elementos:</p> 
       <ul> 
        <li> <p>Nivel de acceso de [!UICONTROL System Administrator]. </p> </li> 
        <li> <p>Configuración de <b>[!UICONTROL Usuarios]</b> en su nivel de acceso configurado a <b>[!UICONTROL Editar]</b> acceso, con <b>[!UICONTROL Crear]</b> y al menos una de las dos opciones de <b>[!UICONTROL Administrador de usuario]</b> habilitadas en <b>[!UICONTROL Ajustar la configuración]</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>De estas dos opciones, si <b>[!UICONTROL User Admin (Usuarios del grupo)]</b> está habilitado, debe ser administrador de un grupo del que sea miembro el usuario.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desactivación o reactivación de una compañía

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Compañías]** ![Icono de Compañías](assets/companies-icon-left-panel.png).

1. Seleccione una o varias compañías que desea desactivar o reactivar.
1. Haga clic en **[!UICONTROL Editar]**.<!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>-->
1. Para una sola compañía, deshabilite la opción **[!UICONTROL Está activo]** para desactivarla o habilite la opción para activarla. <!--ADD TO THE FRONT OF THIS SENTENCE In the Production environment, -->

   O

   Para varias compañías, seleccione **[!UICONTROL No]** en el menú desplegable **[!UICONTROL Está activo]** para desactivarlas o **[!UICONTROL Sí]** para activarlas.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
