---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: La variable [!DNL Adobe Workfront] Entorno de espacio aislado de vista previa
description: El espacio aislado de vista previa es un entorno de prueba que sirve como réplica del entorno en directo. Workfront lo actualiza todos los fines de semana. Los datos agregados a su entorno en directo el viernes aparecen en el Simulador para pruebas de vista previa el lunes siguiente. Todos los paquetes de soporte tienen acceso a este entorno limitado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 0%

---

# La variable [!DNL Adobe Workfront] Entorno de espacio aislado de vista previa

Hay dos entornos de prueba para [!DNL Workfront] que son réplicas de su [!DNL Workfront] entorno de producción:

* El Simulador para pruebas de vista previa

   El espacio aislado de vista previa es un entorno de prueba que sirve como réplica del entorno en directo y se actualiza cada fin de semana antes de [!DNL Workfront]. Los datos agregados a su entorno en directo el viernes aparecen en el Simulador para pruebas de vista previa el lunes siguiente.

   Todos los paquetes de soporte tienen acceso al Simulador para pruebas de vista previa.

* El Simulador para pruebas de actualización personalizado

   El Simulador para pruebas de actualización personalizado es un entorno de prueba independiente que usted actualiza manualmente. Hay un coste adicional para obtener el Simulador para pruebas de actualización personalizado. Para obtener más información sobre este entorno, consulte [La variable [!DNL Adobe Workfront] Entorno de espacio aislado de actualización personalizada](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Paquete de compatibilidad de [!UICONTROL Standard]</strong> </p> </th> 
   <th> <p><strong>Paquetes de compatibilidad con [!UICONTROL Plus], [!UICONTROL Preferido] y [!UICONTROL Enterprise]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Vista previa de Simulador para pruebas</p> </td> 
   <td scope="col"> <p>š</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Espacio aislado de actualización personalizado</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vista previa de Simulador para pruebas

El Simulador para pruebas de vista previa sirve como entorno en el que los usuarios de su organización pueden probar y trabajar de forma segura con los datos del entorno de producción sin afectar al entorno de producción.

El Simulador para pruebas de vista previa contiene los datos de producción reales; sin embargo, se actualiza cada fin de semana para que los datos puedan estar hasta una semana más atrás del entorno de producción. Los elementos creados desde la última actualización se encuentran en el entorno de espacio aislado de vista previa hasta la siguiente actualización.

Los datos fluyen de forma uni-direccional, de Producción a Vista previa, y no de forma inversa. Una actualización del entorno de Vista previa siempre está programada por [!DNL Workfront] cada fin de semana. Para obtener más información sobre el día y la hora específicos de la actualización, vaya a [status.adobe.com](https://status.adobe.com/es/).

El Simulador para pruebas de vista previa también permite [!DNL Workfront] para implementar nuevas funciones en un entorno seguro, antes de que estén listas para implementarse en Producción. Puede probar las nuevas funciones y proporcionar [!DNL Workfront] comentarios sobre su funcionalidad accediendo al Simulador para pruebas de vista previa. Por este motivo, el código del Simulador para pruebas de vista previa siempre va por delante del código de producción, aunque los datos se actualizan semanalmente.

El entorno de vista previa es ideal para ejecutar cursos de capacitación, probar nuevas funciones y determinar la funcionalidad de configuración.

>[!NOTE]
>
>Cuando acceda al Simulador para pruebas de vista previa, observe el aviso azul en la parte superior de la pantalla. El banner no se puede eliminar mientras esté trabajando en este entorno.
>
>El nombre del entorno al que accede (vista previa) y la versión del código se muestran en el banner. Haga clic en **[!UICONTROL Vea las novedades]** para obtener información sobre esa versión.
>
>![](assets/preview-banner-nwe-350x161.png)

## Acceso al Simulador para pruebas de vista previa

De forma predeterminada, como [!DNL Workfront] administrador, tiene acceso al [!UICONTROL Vista previa] Entorno de espacio aislado. Si no puede acceder a la variable [!UICONTROL Vista previa] Entorno de espacio aislado como se describe en esta sección, póngase en contacto con su [!DNL Workfront] o nuestro equipo de asistencia al cliente.

* [Acceder al Simulador para pruebas de vista previa desde el [!DNL Workfront] Interfaz](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [Acceso al Simulador para pruebas de vista previa mediante una dirección URL](#accessing-the-preview-sandbox-using-a-url)

### Acceder al Simulador para pruebas de vista previa desde el [!DNL Workfront] Interfaz {#accessing-the-preview-sandbox-from-the-workfront-interface}

Como [!DNL Workfront] administrador, puede acceder al Simulador para pruebas de vista previa a través del [!DNL Workfront] interfaz.

Para acceder al Simulador para pruebas de vista previa:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Sistema]** > **[!UICONTROL Preferencias]**.

1. En el **[!UICONTROL Entornos de prueba]** , haga clic en **[!UICONTROL Vista previa de Simulador para pruebas]**.

1. Inicie sesión con sus credenciales de vista previa.

   Estas deben ser las mismas que las credenciales de producción, a menos que las haya cambiado en Producción después de que se actualizara la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

### Acceso al Simulador para pruebas de vista previa mediante una dirección URL {#accessing-the-preview-sandbox-using-a-url}

* [Acceso al Simulador para pruebas de vista previa para cuentas en los clústeres 1, 2, 3 y 5](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [Acceso al Simulador para pruebas de vista previa para cuentas en el Cluster 4 (Cuentas EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### Acceso al Simulador para pruebas de vista previa para cuentas en los clústeres 1, 2, 3 y 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

Históricamente, accedió al Simulador para pruebas de vista previa accediendo a [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg).

Esta URL ya no es compatible y no se ha redirigido a la nueva URL para el entorno de espacio aislado de vista previa. La nueva dirección URL correcta para el Simulador para pruebas de vista previa es: [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ).

>[!NOTE]
>
>Si tiene marcadores vinculados a la dirección URL antigua del Simulador para pruebas de vista previa, tenga en cuenta este cambio y actualice la dirección URL en los marcadores.

Para iniciar sesión en el Simulador para pruebas de vista previa con una dirección URL:

1. Vaya a esta URL: [[!DNL https]://companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)

   Si es cliente de EMEA y su cuenta está en el Cluster 4, consulte la sección [Acceso al Simulador para pruebas de vista previa para cuentas en el Cluster 4 (Cuentas EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) en este artículo.

1. Inicie sesión con sus credenciales de vista previa.

   Las credenciales de vista previa deben ser las mismas que las credenciales de producción, a menos que las haya cambiado en Producción después de que se actualizara la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

#### Acceso al Simulador para pruebas de vista previa para cuentas en el Cluster 4 (Cuentas EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Para iniciar sesión en el Simulador para pruebas de vista previa con una dirección URL:

1. Vaya a esta URL: `https://companyname.preview.workfront.com/`.

   También puede acceder al Simulador para pruebas de vista previa accediendo a [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Inicie sesión con sus credenciales de vista previa.

   Las credenciales de vista previa deben ser las mismas que las credenciales de producción, a menos que las haya cambiado en Producción después de que se actualizara la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

## Recibir correos electrónicos del Simulador para pruebas de vista previa

Workfront deshabilita toda la comunicación por correo electrónico desde el entorno de la zona de pruebas de vista previa. Si desea recibir notificaciones por correo electrónico desde el entorno de espacio aislado de vista previa, debe habilitar esta funcionalidad en la configuración de usuario. Para obtener más información sobre la activación de notificaciones por correo electrónico en el entorno de la zona de pruebas de vista previa, consulte [Habilitar el envío de correos electrónicos desde el entorno de Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>El envío de informes y las notificaciones push en la aplicación móvil siempre están desactivadas para el entorno de espacio aislado de vista previa. Ni tú ni el [!DNL Workfront] el administrador puede activar el envío de informes o las notificaciones push para la aplicación móvil al acceder al entorno de espacio aislado de vista previa.
>
>Para obtener más información sobre los envíos de informes para el entorno de producción, consulte [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Inicio de sesión único (SSO)

Si utiliza SSO, trabaje con nuestro equipo de asistencia al cliente para asegurarse de que esté correctamente configurado de modo que pueda utilizar sus credenciales de SSO para iniciar sesión en [!UICONTROL Vista previa] Simulador para pruebas. Si su inicio de sesión inicial falla, póngase en contacto con su contacto de asistencia regular o [!DNL Workfront] administrador para obtener ayuda.

Para obtener más información sobre el inicio de sesión único, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configuración del inicio de sesión único en el simulador para pruebas de vista previa

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al [!DNL Adobe Admin Console]. Si su organización se ha incorporado a la variable [!DNL Adobe Admin Console], no es necesario realizar ninguna acción.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado al [!DNL Adobe Admin Console], consulte [Diferencias de administración basadas en plataformas ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Si desea configurar el Simulador para pruebas de vista previa para que funcione con una solución de Inicio de sesión único, puede hacerlo configurándolo de forma independiente del entorno de producción. La configuración de SSO del Simulador para pruebas de vista previa es independiente de la configuración de SSO del entorno de producción.

Cuando se actualiza el Simulador para pruebas de vista previa (todos los fines de semana), la información de SSO no se copia desde el entorno de producción para sobrescribir la configuración del Simulador para pruebas de vista previa.

Los pasos para configurar el inicio de sesión único en el Simulador para pruebas de vista previa son similares a los para configurarlo en el entorno de producción.

Para obtener más información sobre la configuración [!DNL Workfront] con SSO, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Previsualizar el rendimiento y la disponibilidad del entorno

[!DNL Workfront] Los entornos de vista previa no están pensados para pruebas de rendimiento o carga. En su lugar, utilice estos entornos para validar la funcionalidad de las funciones con los flujos de trabajo existentes de su organización.

[!DNL Workfront] Los entornos de vista previa están pensados para que estén siempre disponibles.

Cualquier interrupción en un [!DNL Workfront] El entorno de vista previa durante el horario laboral normal será una prioridad inmediata inmediatamente después de que se resuelvan los problemas de producción si existen.

Cualquier interrupción en un [!DNL Workfront] El entorno de vista previa los fines de semana (sábados y domingos) se solucionará para que el entorno se ejecute durante el horario laboral los lunes.
