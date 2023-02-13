---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configuración de la integración de JumpSeat
description: Puede integrar [!DNL JumpSeat] con [!DNL Workfront] para crear directrices personalizadas internas del producto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# Configuración de la integración de JumpSeat

Puede integrar [!DNL JumpSeat] con [!DNL Workfront] para crear directrices personalizadas internas del producto.

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
   <td>Debe tener un [!DNL JumpSeat] plan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p> Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Antes de empezar, debe

* Agregar y activar [!DNL Workfront] como aplicación en [!DNL JumpSeat]. Para obtener más información, consulte [Cómo Agregar O Eliminar Una Aplicación](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configure las variables [!DNL JumpSeat] integración

Se recomienda configurar un [!DNL JumpSeat] integración en los entornos de producción y vista previa.

>[!TIP]
>
>Debe agregar y activar dos [!DNL Workfront] aplicaciones en [!DNL JumpSeat]: una para la vista previa y otra para la producción. Consulte [Cómo Agregar O Eliminar Una Aplicación](https://support.jumpseat.io/article/how-to-add-an-application/) para obtener más información.

Para configurar la variable [!DNL JumpSeat] integración:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]**.
1. En el panel izquierdo, haga clic en **[!UICONTROL Sistema]** > **[!UICONTROL [!DNL JumpSeat]Integración]**.
1. Escriba la **[!UICONTROL [!DNL JumpSeat]URL]**.

   **Ejemplo:** [!DNL https]://{mycompanyname}.jumpsit.io

1. Introduzca la variable **[!UICONTROL [!DNL JumpSeat]token de integración]**. Puede encontrarlo en el **[!UICONTROL Configuración]** en [!DNL JumpSeat].

   **Ejemplo:** $2 y$10$BevsKeQ8....OYR.LurSg2U64O

1. Haga clic en **[!UICONTROL Probar la configuración]**.
1. Seleccione si desea que se realice la integración **[!UICONTROL Activo]** o **[!UICONTROL Inactivo]**.

   >[!IMPORTANT]
   >
   >La prueba de configuración realizada en el paso 5 debe pasar para activar la integración.

   ![Página de integración de JumpSeat](assets/jumpseat-integration-page.png)

1. Haga clic en **[!UICONTROL Guardar]**.
