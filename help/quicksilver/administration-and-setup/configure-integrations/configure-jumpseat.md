---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurar integración de JumpSeat
description: Puede integrar [!DNL JumpSeat] con [!DNL Workfront] para crear una guía personalizada en el producto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 91%

---

# Configurar integración de JumpSeat

Puede integrar [!DNL JumpSeat] con [!DNL Workfront] para crear una guía personalizada en el producto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table>
  <tr>
   <td>paquete de Adobe Workfront
   </td>
    <p>Workflow Ultimate</p>
   <td> <p>PRIME o ULTIMATE</p>
   </td>
  </tr>
    <tr>
   <td>Licencias de Adobe Workfront
   </td>
   <td>Estándar
   <p>Plan</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>Producto
   </td>
   <td>Debe tener un plan [!DNL JumpSeat] activo.
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de empezar, debe

* Añadir y activar [!DNL Workfront] como una aplicación en [!DNL JumpSeat]. Para obtener más información, consulte [Cómo añadir o eliminar una aplicación](https://support.jumpseat.io/article/how-to-add-an-application/).

>[!IMPORTANT]
>
>Si se encuentra en la experiencia unificada de Adobe, debe usar la siguiente URL de la aplicación: `.workfront.adobe.com`.



## Configurar integración de [!DNL JumpSeat]

Se recomienda configurar una integración de [!DNL JumpSeat] en los entornos de vista previa y producción.

>[!TIP]
>
>Debe añadir y activar dos aplicaciones [!DNL Workfront] independientes en [!DNL JumpSeat]: una para vista previa y otra para producción. Consulte [Cómo añadir o eliminar una aplicación](https://support.jumpseat.io/article/how-to-add-an-application/) para obtener más información.

Para configurar la integración de [!DNL JumpSeat]:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Sistema]** > Integración de **[!UICONTROL [!DNL JumpSeat]]**.
1. Introduzca la URL **de**&#x200B;[!DNL JumpSeat], que se encuentra en el icono de extensión en [!DNL JumpSeat].

>[!BEGINSHADEBOX]

**Ejemplo:**

https://{mycompanyname}.jumpseat.io

&#x200B;>>

>[!ENDSHADEBOX]

1. Introducir token **de integración de**&#x200B;[!DNL JumpSeat]. Lo puede encontrar en la página **[!UICONTROL Configuración]** en [!DNL JumpSeat].

   **Ejemplo:** $2y$10$BevsKeQ8...OYR.LurSg2U64O

1. Haga clic en **[!UICONTROL Probar configuración]**.
1. Elija si desea que la integración sea **[!UICONTROL Activa]** o **[!UICONTROL Inactiva]**.

   >[!IMPORTANT]
   >
   >La prueba de configuración realizada en el paso 5 debe ser satisfactoria para activar la integración.

   ![Página de integración de JumpSeat](assets/jumpseat-integration-page.png)

1. Haga clic en **[!UICONTROL Guardar]**.

>[!TIP]
>
>Para obtener más información sobre cómo configurar la integración de [!DNL JumpSeat], consulte la documentación de [!DNL JumpSeat] para [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
