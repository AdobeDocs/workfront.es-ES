---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: El [!DNL Adobe Workfront] Previsualizar entorno de espacio aislado
description: La zona protegida de vista previa es un entorno de prueba que sirve como réplica del entorno en directo. Workfront lo actualiza todos los fines de semana. Los datos agregados a su entorno en directo el viernes aparecerán en su zona protegida de vista previa el lunes que viene. Todos los paquetes de asistencia tienen acceso a esta zona protegida.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 0%

---

# El [!DNL Adobe Workfront] Previsualizar entorno de espacio aislado

Existen dos entornos de prueba para [!DNL Workfront] que son réplicas de su [!DNL Workfront] entorno de producción:

* La zona protegida de previsualización

   La zona protegida de vista previa es un entorno de prueba que sirve como réplica del entorno en directo y se actualiza cada fin de semana con [!DNL Workfront]. Los datos agregados a su entorno en directo el viernes aparecerán en su zona protegida de vista previa el lunes que viene.

   Todos los paquetes de asistencia tienen acceso a la zona protegida de vista previa.

* La zona protegida de actualización personalizada

   La zona protegida de actualización personalizada es un entorno de prueba independiente que actualiza manualmente. Hay un coste adicional para obtener la zona protegida de actualización personalizada. Para obtener más información sobre este entorno, consulte [El [!DNL Adobe Workfront] Entorno de espacio aislado de actualización personalizado](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Paquete de soporte de [!UICONTROL Standard]</strong> </p> </th> 
   <th> <p><strong>Paquetes de soporte de [!UICONTROL Plus], [!UICONTROL preferido] y [!UICONTROL Enterprise]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Previsualizar zona protegida</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Actualizar espacio aislado personalizado</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Previsualizar zona protegida

La vista previa de espacio aislado sirve como entorno en el que los usuarios de su organización pueden probar y trabajar con seguridad con datos del entorno de producción sin afectar al entorno de producción.

La zona protegida de vista previa contiene los datos de producción reales; sin embargo, se actualiza cada fin de semana para que los datos puedan retrasarse hasta una semana respecto al entorno de producción. Los elementos creados desde la última actualización se encuentran en el entorno de vista previa de espacio aislado hasta la siguiente actualización.

Los datos fluyen unidireccionalmente, de Producción a Vista previa y no a la inversa. siempre programa una actualización del entorno de vista previa [!DNL Workfront] cada fin de semana.

La zona protegida de previsualización también permite [!DNL Workfront] para implementar nuevas funciones en un entorno seguro, antes de que estén listas para implementarse en el entorno de producción. Puede probar las nuevas funciones y proporcionar [!DNL Workfront] comentarios sobre su funcionalidad accediendo a la zona protegida de vista previa. Por este motivo, el código de la zona protegida de vista previa siempre va por delante del código de producción, aunque los datos se actualicen semanalmente.

El entorno de vista previa es ideal para ejecutar cursos de formación, probar nuevas funciones y determinar la funcionalidad de la configuración.

>[!NOTE]
>
>Cuando acceda a la Vista previa de espacio aislado, observe el banner azul en la parte superior de la pantalla. El titular no se puede quitar mientras esté trabajando en este entorno.
>
>El nombre del entorno al que accede (Vista previa) y la versión de lanzamiento del código se muestran en el banner. Clic **[!UICONTROL Ver las novedades]** para obtener más información sobre esa versión.
>
>![](assets/preview-banner-nwe-350x161.png)

## Acceso a la zona protegida de previsualización

De forma predeterminada, como [!DNL Workfront] administrador, tiene acceso a la [!UICONTROL Previsualizar] Entorno de zona protegida. Si no puede acceder a [!UICONTROL Previsualizar] Entorno de zona protegida como se describe en esta sección, póngase en contacto con su [!DNL Workfront] o nuestro equipo de asistencia al cliente.

* [Acceder a la vista previa de espacio aislado desde [!DNL Workfront] Interfaz](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [Acceso a la vista previa de zona protegida mediante una URL](#accessing-the-preview-sandbox-using-a-url)

### Acceder a la vista previa de espacio aislado desde [!DNL Workfront] Interfaz {#accessing-the-preview-sandbox-from-the-workfront-interface}

As a [!DNL Workfront] administrador, puede acceder a la vista previa de la zona protegida mediante el [!DNL Workfront] interfaz.

Para acceder a la zona protegida de vista previa:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Sistema]** > **[!UICONTROL Preferencias]**.

1. En el **[!UICONTROL Entornos de prueba]** , haga clic en **[!UICONTROL Previsualización de zona protegida]**.

1. Inicie sesión con sus credenciales de vista previa.

   Deben ser las mismas que sus credenciales de producción, a menos que las haya cambiado en Producción después de que se actualice la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

### Acceso a la vista previa de zona protegida mediante una URL {#accessing-the-preview-sandbox-using-a-url}

* [Acceder a la vista previa de espacio aislado para cuentas en el clúster 1, 2, 3 y 5](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [Acceso a la Vista Previa de la Zona Protegida para Cuentas en el Cluster 4 (Cuentas EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### Acceder a la vista previa de espacio aislado para cuentas en el clúster 1, 2, 3 y 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

La URL de la zona protegida de vista previa es: `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Si tenía marcadores que se vinculaban a la dirección URL antigua para la zona protegida de vista previa, tome nota de este cambio y actualice la dirección URL en sus marcadores.

Para iniciar sesión en la zona protegida de vista previa con una dirección URL:

1. Vaya a esta dirección URL: `https://companyname.preview.workfront.com/`.

   Si es cliente de EMEA y su cuenta se encuentra en el clúster 4, consulte la sección [Acceso a la Vista Previa de la Zona Protegida para Cuentas en el Cluster 4 (Cuentas EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) en este artículo.

1. Inicie sesión con sus credenciales de vista previa.

   Las credenciales de vista previa deben ser las mismas que las de producción, a menos que las haya cambiado en Producción después de la actualización de la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

#### Acceso a la Vista Previa de la Zona Protegida para Cuentas en el Cluster 4 (Cuentas EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Para iniciar sesión en la zona protegida de vista previa con una dirección URL:

1. Vaya a esta dirección URL: `https://companyname.preview.workfront.com/`.

   También puede acceder a la Vista previa de espacio aislado accediendo a [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Inicie sesión con sus credenciales de vista previa.

   Las credenciales de vista previa deben ser las mismas que las de producción, a menos que las haya cambiado en Producción después de la actualización de la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

## Recepción de correos electrónicos desde la zona protegida de previsualización

Workfront deshabilita toda la comunicación por correo electrónico desde el entorno de vista previa de espacio aislado. Si desea recibir notificaciones por correo electrónico desde el entorno de vista previa de espacio aislado, debe habilitar esta funcionalidad en la configuración de usuario. Para obtener más información sobre la activación de notificaciones por correo electrónico en el entorno de vista previa de espacio aislado, consulte [Habilitar el envío de correos electrónicos desde el entorno de vista previa de espacio aislado](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Las notificaciones push y de envío de informes en la aplicación móvil siempre están desactivadas para el entorno de vista previa de espacio aislado. Ni tú ni el [!DNL Workfront] El administrador de puede activar la entrega de informes o las notificaciones push para la aplicación móvil al acceder al entorno de vista previa de espacio aislado.
>
>Para obtener más información sobre los envíos de informes para el entorno de producción, consulte [Resumen de entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Inicio de sesión único (SSO)

Si utiliza SSO, colabore con nuestro equipo de asistencia al cliente para asegurarse de que está configurado correctamente y de que puede utilizar sus credenciales de SSO para iniciar sesión en [!UICONTROL Previsualizar] Zona protegida. Si falla su inicio de sesión, póngase en contacto con su contacto de asistencia habitual o [!DNL Workfront] administrador para obtener ayuda.

Para obtener más información sobre el inicio de sesión único, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configuración del inicio de sesión único en la zona protegida de vista previa

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica sólo a las organizaciones que aún no se han incorporado al [!DNL Adobe Admin Console]. Si su organización se ha incorporado al [!DNL Adobe Admin Console]No es necesario realizar ninguna acción.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado al [!DNL Adobe Admin Console], consulte [Diferencias de administración basadas en la plataforma ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Si desea configurar la zona protegida de vista previa para que funcione con una solución de inicio de sesión único, puede configurarla por separado desde el entorno de producción. La configuración de SSO de la zona protegida de vista previa es independiente de la configuración de SSO del entorno de producción.

Cuando se actualiza la zona protegida de vista previa (todos los fines de semana), la información de SSO no se copia del entorno de producción para sobrescribir la configuración de la zona protegida de vista previa.

Los pasos para configurar el inicio de sesión único en la zona protegida de vista previa son similares a los necesarios para configurarlo en el entorno de producción.

Para obtener más información sobre la configuración [!DNL Workfront] con SSO, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Previsualizar rendimiento y disponibilidad del entorno

[!DNL Workfront] Los entornos de vista previa no están pensados para pruebas de carga o rendimiento. En su lugar, utilice estos entornos para validar la funcionalidad de las funciones con los flujos de trabajo existentes de su organización.

[!DNL Workfront] Los entornos de vista previa están pensados para estar siempre disponibles.

Cualquier interrupción en un [!DNL Workfront] El entorno de vista previa durante el horario laboral normal será una primera prioridad inmediatamente después de que se resuelvan los problemas de producción, si los hay.

Cualquier interrupción en un [!DNL Workfront] Se abordará el entorno de vista previa los fines de semana (sábados y domingos) para que el entorno funcione durante el horario laboral los lunes.
