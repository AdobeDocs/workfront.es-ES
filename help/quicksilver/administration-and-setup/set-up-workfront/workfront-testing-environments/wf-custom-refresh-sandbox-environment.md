---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: La variable [!DNL Adobe Workfront] Entorno de espacio aislado de actualización personalizada
description: El Simulador para pruebas de actualización personalizado es un entorno en el que puede probar y trabajar con datos del entorno de producción. También es ideal para ejecutar entrenamientos y determinar la funcionalidad de configuración.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 0%

---

# La variable [!DNL Adobe Workfront] Entorno de espacio aislado de actualización personalizada

El Simulador para pruebas de actualización personalizado es un entorno en el que puede probar y trabajar con datos del entorno de producción. También es ideal para ejecutar entrenamientos y determinar la funcionalidad de configuración.

>[!NOTE]
>
>Esto es diferente al espacio aislado de vista previa, que también es un entorno de prueba que duplica su [!DNL Workfront] entorno de producción.
>
>* Las nuevas funciones se introducen en el Simulador para pruebas de vista previa antes de que estén disponibles en Producción.
>* Las nuevas funciones no se introducen en el Simulador para pruebas de actualización personalizado antes de que estén disponibles en Producción.
>
>  Además, existe un coste adicional para obtener el Simulador para pruebas de actualización personalizado que no es necesario para el Simulador para pruebas de vista previa.
>
>  Para obtener más información sobre el Simulador para pruebas de vista previa, consulte [La variable [!DNL Adobe Workfront] Entorno de espacio aislado de vista previa](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>[!UICONTROL Business] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licencia</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paquete de soporte</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferido] o [!UICONTROL Enterprise]</p> <p>El paquete de soporte estándar no tiene acceso al Simulador para pruebas de actualización personalizado, pero sí al Simulador para pruebas de vista previa.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualización del Simulador para pruebas de actualización personalizado

El Simulador para pruebas de actualización personalizado contiene los datos de producción reales y no se actualiza hasta que se programe para hacerlo. Puede programar una actualización en cualquier momento que le convenga, con tanta frecuencia como una vez a la semana.

>[!NOTE]
>
>* No se puede programar una actualización para el día actual. Por ejemplo, si hoy es el 1 de junio, el día más temprano en el que se puede programar una actualización es el 2 de junio.
>* El Simulador para pruebas de actualización personalizado siempre tiene las mismas características de producto que el entorno de producción. Sin embargo, cuando actualiza el Simulador para pruebas de actualización personalizado, conserva la marca únicamente para el color de fondo de la pantalla de inicio de sesión. La pantalla de inicio de sesión y los logotipos de la barra de navegación se restablecen a [!DNL Workfront] no se muestran los valores predeterminados ni las imágenes de marca que haya modificado antes de la actualización.
>




<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Acceda al Simulador para pruebas de actualización personalizado desde el entorno de producción. {#access-the-custom-refresh-sandbox-from-your-production-environment}

Como [!DNL Workfront] administrador, puede acceder al Simulador para pruebas de actualización personalizado desde el entorno de producción.

>[!NOTE]
>
>Si su cuenta está en el clúster 4 (clúster de EMEA), no puede acceder al Simulador para pruebas de actualización personalizado desde el entorno de producción. Para obtener más información sobre cómo acceder al Simulador para pruebas de actualización personalizado cuando tiene una cuenta en el Clúster 4, consulte [Acceso al Simulador para pruebas de actualización personalizado para cuentas en el Cluster 4 (Cuentas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Acceso al Simulador para pruebas de actualización personalizado para cuentas en el Cluster 4 (Cuentas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Para acceder al Simulador para pruebas de actualización personalizado:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Sistema]** >**[!UICONTROL Preferencias]**.

1. En el **[!UICONTROL Entorno de prueba]** , haga clic en **[!UICONTROL Espacio aislado 1]** o **[!UICONTROL Espacio aislado 2]**.

   El paquete de soporte especifica si tiene acceso a uno o dos entornos limitados de actualización personalizados.

1. Inicie sesión con las credenciales del Simulador para pruebas de actualización personalizado.

   Las credenciales del Simulador para pruebas de actualización personalizado son las mismas que las de producción, a menos que haya cambiado las credenciales de producción desde la última vez que actualizó el Simulador para pruebas de actualización personalizado. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

   El Simulador para pruebas de actualización personalizado muestra la versión y la fecha de la última actualización en el banner de la parte superior de la pantalla. Toda la información de producción está disponible y lista para funcionar después de que se complete una actualización.

## Acceso al Simulador para pruebas de actualización personalizado mediante una dirección URL {#access-the-custom-refresh-sandbox-using-a-url}

Cualquier usuario puede acceder al Simulador para pruebas de actualización personalizado utilizando una dirección URL.

* [Acceso al Simulador para pruebas personalizado para cuentas de los clústeres 1, 2, 3 y 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Acceso al Simulador para pruebas de actualización personalizado para cuentas en el Cluster 4 (Cuentas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Acceso al Simulador para pruebas personalizado para cuentas de los clústeres 1, 2, 3 y 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Según el paquete de soporte, debe tener acceso a uno o dos entornos limitados de actualización personalizados.

Para acceder al Simulador para pruebas de actualización personalizado con una dirección URL:

1. Vaya a esta URL si solo tiene un Simulador para pruebas de actualización personalizado:

   https://companyname.sb01.workfront.com (URL antigua):https://cr1.attasksandbox.com/.)

   O si tiene dos entornos limitados de actualización personalizados, además de las direcciones URL anteriores, también puede ir a la siguiente URL para acceder al segundo espacio aislado de actualización personalizada:

   https://companyname.sb02.workfront.com (URL antigua):https://cr2.attasksandbox.com/)

1. En la pantalla de inicio de sesión, inicie sesión con las credenciales del Simulador para pruebas de actualización personalizado.
1. Las credenciales del Simulador para pruebas de actualización personalizado son las mismas que las de producción, a menos que haya cambiado las credenciales de producción desde la última actualización del Simulador para pruebas personalizado. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

### Acceso al Simulador para pruebas de actualización personalizado para cuentas en el Cluster 4 (Cuentas EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Si su [!DNL Workfront] La cuenta está en el clúster 4 (clúster EMEA), solo puede acceder al Simulador para pruebas de actualización personalizado mediante una URL. Para averiguar en qué clúster se encuentra su cuenta, póngase en contacto con nuestro equipo de asistencia al cliente.

Según el paquete de soporte, debe tener acceso a uno o dos entornos limitados de actualización personalizados.

Para acceder al Simulador para pruebas de actualización personalizado con una dirección URL:

1. Vaya a esta URL si solo tiene un Simulador para pruebas de actualización personalizado:

   https://companyname.sb01.workfront.com (URL antigua):https://cr3.attasksandbox.com)

   O

   Vaya a cualquiera de estas direcciones URL si tiene dos entornos limitados de actualización personalizados:

   https://companyname.sb01.workfront.com (URL antigua):https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (URL antigua):https://cr4.attasksandbox.com)

1. En la pantalla de inicio de sesión, inicie sesión con las credenciales del Simulador para pruebas de actualización personalizado.

   Las credenciales del Simulador para pruebas de actualización personalizado son las mismas que las de producción, a menos que haya cambiado las credenciales de producción desde la última actualización del Simulador para pruebas personalizado. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

## Programar una actualización del Simulador para pruebas de actualización personalizado

>[!IMPORTANT]
>
>La duración de la actualización depende del tamaño de los datos que se actualizan. Durante el proceso de actualización, es fundamental que el entorno limitado de actualización personalizado no se esté utilizando de ninguna manera (incluidas las llamadas a la API y las integraciones), ya que esto evitará que la actualización del entorno limitado termine correctamente. [!DNL Workfront] deshabilitará el entorno de entorno limitado de actualización personalizado antes de que comience, pero deberá finalizar las sesiones activas para garantizar que la actualización del entorno limitado se realice correctamente.

Después de programar una actualización del Simulador para pruebas de actualización personalizado, puede cancelarla haciendo clic en [!UICONTROL Cancelar] en la parte superior de la página. También puede volver a programarlo para más adelante.

>[!NOTE]
>
>No se pueden programar actualizaciones automáticas de entornos limitados.

Para programar una actualización del Simulador para pruebas de actualización del cliente:

1. Inicie sesión en el Simulador para pruebas de actualización personalizado.
1. Haga clic en **[!UICONTROL Programación]** en el banner de la parte superior de la pantalla y seleccione una fecha del calendario.
1. Seleccione una fecha para cuándo desea que se produzca la actualización y haga clic en **[!UICONTROL Programar actualización]**.

## Cambie a Producción desde el Simulador para pruebas de actualización personalizado

1. Inicie sesión en el Simulador para pruebas de actualización personalizado.

   Para obtener más información sobre el acceso al Simulador para pruebas de actualización personalizado, consulte [Acceda al Simulador para pruebas de actualización personalizado desde el entorno de producción.](#access-the-custom-refresh-sandbox-from-your-production-environment) o [Acceso al Simulador para pruebas de actualización personalizado mediante una dirección URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Haga clic en **[!UICONTROL Ir a producción]** en el banner de la parte superior de la pantalla.

   Recuerde que el trabajo realizado en el entorno limitado no será visible en la [!UICONTROL producción] , ya que la transferencia de datos es unidireccional, desde la producción hasta el Simulador para pruebas de actualización personalizado, y no al revés.

## Recibir correos electrónicos del Simulador para pruebas de actualización personalizado

[!DNL Workfront] deshabilita toda la comunicación por correo electrónico desde el entorno de espacio aislado de actualización personalizado. Si desea recibir notificaciones por correo electrónico del entorno limitado de actualización personalizada, debe habilitar esta funcionalidad en la configuración de usuario. Para obtener más información sobre la activación de notificaciones por correo electrónico en el entorno de espacio aislado de actualización personalizada, consulte [Habilitar el envío de correos electrónicos desde el entorno de Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>El envío de informes y las notificaciones push en la aplicación móvil siempre están desactivadas para el entorno limitado de actualización personalizada . Ni tú ni el [!DNL Workfront] el administrador puede activar el envío de informes o las notificaciones push para la aplicación móvil al acceder al entorno limitado de actualización personalizada.\
>Para obtener más información sobre los envíos de informes para el entorno de producción, consulte [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Para obtener más información sobre las notificaciones push en la aplicación móvil para el entorno de producción, consulte la sección en .

## Configuración del inicio de sesión único en el simulador para pruebas de actualización personalizado

Si desea configurar el Simulador para pruebas de actualización personalizado para que funcione con una solución de Inicio de sesión único, puede hacerlo configurándolo de forma independiente del entorno de producción. La configuración de SSO del Simulador para pruebas de actualización personalizada es independiente de la configuración de SSO del entorno de producción.\
Al actualizar el Simulador para pruebas de actualización personalizado, la información de SSO no se copia desde el entorno de producción para sobrescribir la configuración del Simulador para pruebas de actualización personalizada.

Los pasos para configurar el inicio de sesión único en el Simulador para pruebas de actualización personalizado son similares a los para configurarlo en el entorno de producción.\
Para obtener más información sobre la configuración [!DNL Workfront] con SSO, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Esto no está disponible si la [!DNL Workfront] está habilitada con Adobe IMS. Si necesita más información, consulte con su administrador de red o TI.

## Uso y disponibilidad previstos

[!DNL Workfront] Los entornos del Simulador para pruebas de actualización personalizado no están pensados para pruebas de rendimiento o carga. En su lugar, utilice estos entornos para validar la funcionalidad de las funciones con los flujos de trabajo existentes de su organización.

[!DNL Workfront] Los entornos del Simulador para pruebas de actualización personalizado están pensados para que estén siempre disponibles. Cualquier interrupción en un entorno limitado de actualización personalizada de Workfront durante el horario laboral normal será una prioridad inmediata inmediatamente después de que se resuelvan los problemas de producción si existen. Cualquier interrupción en un entorno limitado de actualización personalizada de Workfront los fines de semana (sábados y domingos) se solucionará para que el entorno se ejecute durante el horario laboral los lunes.
