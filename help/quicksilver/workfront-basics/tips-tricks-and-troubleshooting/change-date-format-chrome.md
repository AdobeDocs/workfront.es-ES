---
filename: change-date-format-chrome
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Cambiar el formato de las fechas en  [!DNL Adobe Workfront]
description: Para cambiar el formato de fecha de las fechas en  [!DNL Adobe Workfront] debe cambiar la configuración de idioma en el explorador.
feature: Get Started with Workfront
exl-id: 9fac92fb-e3d1-4537-b324-4b35447cef28
source-git-commit: 7ad3fbcfa5be5074016f399560cca509d81f4714
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Cambiar el formato de las fechas de [!DNL Adobe Workfront]

<!--this article used to be called "Change the date format in Adobe Workfront when using Chrome". The team decieded to make it more generic and hide the steps. Also see drafted content below-->

>[!IMPORTANT]
>
> La información de este artículo se aplica solo a las organizaciones que aún no se han incorporado a la experiencia unificada de Adobe.
> Si su organización se ha incorporado a la experiencia unificada de Adobe, su preferencia de fecha está controlada por la preferencia de idioma establecida en Unified Shell de Adobe. La configuración de idioma predeterminada y, por lo tanto, la configuración de fecha predeterminada, es `en-US`.

Puede cambiar el formato de fecha de las fechas de [!DNL Adobe Workfront], como [!UICONTROL Fecha planificada de finalización], [!UICONTROL Fecha real de finalización] o [!UICONTROL Fecha proyectada de finalización].

Por ejemplo, puede cambiar un formato de fecha de _DD/MM/AAAA_ a _MM/DD/AAAA_ o viceversa.
O bien, puede cambiar el formato de fecha de _MM/DD/AA_ a _Lun DD, AAAA_.

Puede cambiar los formatos de fecha en Workfront de las siguientes maneras, según los cambios que desee ver y dónde desee ver los cambios.

* Para cambiar todos los formatos de fecha de todas las páginas de [!DNL Workfront] según su ubicación e idioma, debe cambiar la configuración de idioma en el explorador.

  Por ejemplo, si el idioma predeterminado en su explorador está establecido en *[!UICONTROL Inglés (Estados Unidos)]*, las fechas se mostrarán en los siguientes formatos:

   * DD/MM/AAAA
   * Lun DD, AAAA

  Para cambiar la configuración de idioma en [!DNL Chrome] o en cualquier otro explorador, debe modificar la configuración de ese explorador. Los pasos para modificar la configuración de un explorador varían de un explorador a otro. Consulta las áreas de [!UICONTROL Ayuda], [!UICONTROL Preferencias] o [!UICONTROL Configuración] de tu explorador para saber cómo modificar su configuración.

* Para cambiar el formato de las fechas solamente en informes y vistas, debe actualizar la configuración de [!UICONTROL Formato de campo] en el área de [!UICONTROL Opciones avanzadas] de una columna al crear el informe o la vista. Esto no modifica el formato de fecha según la ubicación o el idioma. Modifica el formato de las fechas en el contexto de la misma ubicación o idioma.

  ![](assets/field-format-in-advanced-options-of-a-view-highlighted.png)

  Para obtener más información, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Para cambiar el formato de las fechas en todas las notificaciones salientes por correo electrónico para toda la organización, debe actualizar la configuración de [!UICONTROL Configuración regional de correo electrónico predeterminada] en el área de [!UICONTROL Información del cliente] en [!UICONTROL Configuración].

  ![](assets/default-email-locale-field.png)

  Para obtener más información, vea [Configurar información básica para el sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Para cambiar el formato de todas las fechas en todas las notificaciones salientes por correo electrónico de un solo usuario, debe actualizar la configuración de [!UICONTROL Configuración regional de correo electrónico] en el cuadro [!UICONTROL Editar persona] al editar el perfil de un usuario.

  ![](assets/email-locale-for-user-profile-highlighted.png)

  Para obtener más información, consulte [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--drafted because we should not document steps for a third-party application

To change your language settings in Chrome:

1. Click the 3-dots in the top right corner of your Chrome interface, then click **Settings**.
1. On the left area of the Settings page, expand **Advanced**, then click **Languages**.  
   Or  
   Search for *language*&nbsp;at the top of the Settings page, then click **Languages**.

1. In the **Language** list, locate the language and region that use your preferred date format.

   **Example:** If you speak English and you want the date format to be MM/DD/YYYY, you would select **English (United States)**. If you speak English and you want the date format to be DD/MM/YYY, you would select **English (United Kingdom)**.

1. (Conditional) If the language and region you want to use are not visible in the list, click **Add languages** to add it to the list.
1. Click the 3-dot menu next to the language and region you want to use, then click **Move to the top**.
1. Return to the Workfront interface, then refresh the page.  
   The date format is now updated in projects and other areas of Workfront that use MM/DD/YYYY or DD/MM/YYYY format when displaying dates.

   -->
