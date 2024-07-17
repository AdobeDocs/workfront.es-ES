---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configuración de la integración de JumpSeat
description: Puede integrar [!DNL JumpSeat] con [!DNL Workfront] para crear orientación personalizada en el producto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Configuración de la integración de JumpSeat

Puede integrar [!DNL JumpSeat] con [!DNL Workfront] para crear orientación personalizada en el producto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Product</strong></td> 
   <td>Debe tener un plan [!DNL JumpSeat] activo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p> Debe ser administrador de [!DNL Workfront]. Para obtener información sobre los administradores de [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

Antes de empezar, debe

* Agregar y activar [!DNL Workfront] como una aplicación en [!DNL JumpSeat]. Para obtener más información, vea [Cómo agregar o eliminar una aplicación](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configurar la integración de [!DNL JumpSeat]

Se recomienda configurar una integración de [!DNL JumpSeat] en los entornos de vista previa y producción.

>[!TIP]
>
>Debe agregar y activar dos aplicaciones [!DNL Workfront] independientes en [!DNL JumpSeat]: una para vista previa y otra para producción. Consulte [Cómo Agregar O Eliminar Una Aplicación](https://support.jumpseat.io/article/how-to-add-an-application/) para obtener más información.

Para configurar la integración de [!DNL JumpSeat]:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]**.
1. En el panel izquierdo, haga clic en **[!UICONTROL Sistema]** > Integración de **[!UICONTROL [!DNL JumpSeat]]**.
1. Escriba la dirección URL **[!UICONTROL [!DNL JumpSeat]]**, que se encuentra en el icono de extensión en [!DNL JumpSeat].

   **Ejemplo:** [!DNL https]://{mycompanyname}.jumpseat.io

1. Escriba el token de integración **[!UICONTROL [!DNL JumpSeat]]**. Puede encontrar esto en la página **[!UICONTROL Configuración]** en [!DNL JumpSeat].

   **Ejemplo:** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Haga clic en **[!UICONTROL Probar configuración]**.
1. Elija si desea que la integración sea **[!UICONTROL Activa]** o **[!UICONTROL Inactiva]**.

   >[!IMPORTANT]
   >
   >La prueba de configuración realizada en el paso 5 debe pasar para activar la integración.

   ![Página de integración de JumpSeat](assets/jumpseat-integration-page.png)

1. Haga clic en **[!UICONTROL Guardar]**.

>[!TIP]
>
>Para obtener más información sobre cómo configurar la integración de [!DNL JumpSeat], consulte la documentación de [!DNL JumpSeat] para [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
