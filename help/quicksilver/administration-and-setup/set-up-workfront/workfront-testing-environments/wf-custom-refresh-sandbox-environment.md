---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: El [!DNL Adobe Workfront] Entorno de espacio aislado de actualización personalizado
description: El espacio aislado de actualización personalizado es un entorno en el que puede realizar pruebas y trabajar con datos del entorno de producción. También es ideal para ejecutar cursos de formación y determinar la funcionalidad de la configuración.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 8ceb370df6ff6f3a7a4376d6086fbabe99609e29
workflow-type: tm+mt
source-wordcount: '1605'
ht-degree: 0%

---

# El [!DNL Adobe Workfront] Entorno de espacio aislado de actualización personalizado

El espacio aislado de actualización personalizado es un entorno en el que puede realizar pruebas y trabajar con datos del entorno de producción. También es ideal para ejecutar cursos de formación y determinar la funcionalidad de la configuración.

>[!NOTE]
>
>Esto es diferente a la Vista previa de espacio aislado, que también es un entorno de prueba que replica su [!DNL Workfront] entorno de producción.
>
>* Las nuevas funciones se introducen en la zona protegida de vista previa antes de que estén disponibles en producción.
>* Las nuevas funciones no se introducen en la zona protegida de actualización personalizada antes de que estén disponibles en el entorno de producción.
>
>  Además, hay un coste adicional para obtener la zona protegida de actualización personalizada que no es necesario para la vista previa de la zona protegida.
>
>  Para obtener más información sobre la vista previa de espacio aislado, consulte [El [!DNL Adobe Workfront] Previsualizar entorno de espacio aislado](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>[!UICONTROL Empresa] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licencia</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Debe ser un [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paquete de soporte</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL preferido] o [!UICONTROL Enterprise]</p> <p>El paquete de soporte estándar no tiene acceso a la zona protegida de actualización personalizada, pero sí tiene acceso a la de vista previa.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualización del espacio aislado de actualización personalizado

El espacio aislado de actualización personalizado contiene los datos de producción reales y no se actualiza hasta que se programa para ello. Puede programar una actualización en cualquier momento que le resulte conveniente, con la misma frecuencia que una vez a la semana.

>[!NOTE]
>
>* No se puede programar una actualización para el día actual. Por ejemplo, si hoy es 1 de junio, el primer día en que se puede programar una actualización es el 2 de junio.
>* La actualización programada se produce en algún momento durante la noche, según el clúster del usuario (los clústeres de EE. UU. se actualizan durante la noche en EE. UU.). La hora específica es impredecible debido a otros clientes en cola y a la cantidad de datos que se actualizan. Si la cola tiene muchos clientes grandes, es posible que la actualización no se ejecute hasta más tarde ese día o al día siguiente.
>* La zona protegida de actualización personalizada siempre tiene las mismas funciones de producto que el entorno de producción. Sin embargo, al actualizar la zona protegida de actualización personalizada, solo se conserva la marca para el color de fondo de la pantalla de inicio de sesión. La pantalla de inicio de sesión y los logotipos de la barra de navegación se restablecen a [!DNL Workfront] no se muestran los valores predeterminados ni las imágenes de personalización de marca que haya modificado antes de la actualización.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Acceda a la zona protegida de actualización personalizada desde el entorno de producción {#access-the-custom-refresh-sandbox-from-your-production-environment}

As a [!DNL Workfront] administrador, puede acceder a su zona protegida de actualización personalizada desde el entorno de producción.

>[!NOTE]
>
>Si su cuenta está en el clúster 4 (clúster de EMEA), no podrá acceder a su zona protegida de actualización personalizada desde el entorno de producción. Para obtener más información sobre cómo tener acceso a la zona protegida de actualización personalizada cuando tenga una cuenta en el clúster 4, consulte [Acceso a la zona protegida de actualización personalizada para cuentas en el clúster 4 (cuentas de EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Acceso a la zona protegida de actualización personalizada para cuentas en el clúster 4 (cuentas de EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Para acceder a su zona protegida de actualización personalizada:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Sistema]** >**[!UICONTROL Preferencias]**.

1. En el **[!UICONTROL Entorno de prueba]** , haga clic en **[!UICONTROL Espacio aislado 1]** o **[!UICONTROL Espacio aislado 2]**.

   El paquete de asistencia técnica especifica si tiene acceso a uno o dos entornos limitados de actualización personalizados.

1. Inicie sesión con sus credenciales de actualización personalizada de espacio aislado.

   Las credenciales de la zona protegida de actualización personalizada son las mismas que las credenciales de producción, a menos que haya cambiado las credenciales de producción desde la última vez que actualizó la zona protegida de actualización personalizada. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

   La zona protegida de actualización personalizada muestra la versión y la fecha de la última actualización en el banner en la parte superior de la pantalla. Toda la información de la producción está disponible y lista para trabajar con ella una vez completada la actualización.

## Acceso al espacio aislado de actualización personalizado mediante una dirección URL {#access-the-custom-refresh-sandbox-using-a-url}

Cualquier usuario puede acceder a la zona protegida de actualización personalizada mediante una dirección URL.

* [Acceso a la zona protegida de actualización personalizada para cuentas de los clústeres 1, 2, 3 y 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Acceso a la zona protegida de actualización personalizada para cuentas en el clúster 4 (cuentas de EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Acceso a la zona protegida de actualización personalizada para cuentas de los clústeres 1, 2, 3 y 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Según el paquete de soporte, debe tener acceso a uno o dos entornos limitados de actualización personalizados.

Para acceder al espacio aislado de actualización personalizado mediante una dirección URL:

1. Vaya a esta dirección URL si solo tiene una zona protegida de actualización personalizada:

   https://companyname.sb01.workfront.com (URL antigua):https://cr1.attasksandbox.com/.)

   O si tiene dos zonas protegidas de actualización personalizadas, además de las direcciones URL anteriores, también puede ir a la siguiente URL para acceder a su segunda zona protegida de actualización personalizada:

   https://companyname.sb02.workfront.com (URL antigua):https://cr2.attasksandbox.com/)

1. En la pantalla de inicio de sesión, inicie sesión con las credenciales de su zona protegida de actualización personalizada.
1. Las credenciales de la zona protegida de actualización personalizada son las mismas que las credenciales de producción, a menos que haya cambiado las credenciales de producción desde la última vez que se actualizó la zona protegida de actualización personalizada. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

### Acceso a la zona protegida de actualización personalizada para cuentas en el clúster 4 (cuentas de EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Si su [!DNL Workfront] está en el clúster 4 (clúster de EMEA), solo puede acceder a su zona protegida de actualización personalizada mediante una dirección URL. Para saber en qué clúster se encuentra su cuenta, póngase en contacto con nuestro equipo de asistencia al cliente.

Según el paquete de soporte, debe tener acceso a uno o dos entornos limitados de actualización personalizados.

Para acceder al espacio aislado de actualización personalizado mediante una dirección URL:

1. Vaya a esta dirección URL si solo tiene una zona protegida de actualización personalizada:

   https://companyname.sb01.workfront.com (URL antigua):https://cr3.attasksandbox.com)

   O

   Vaya a una de estas direcciones URL si tiene dos zonas protegidas de actualización personalizadas:

   https://companyname.sb01.workfront.com (URL antigua):https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (URL antigua):https://cr4.attasksandbox.com)

1. En la pantalla de inicio de sesión, inicie sesión con las credenciales de su zona protegida de actualización personalizada.

   Las credenciales de la zona protegida de actualización personalizada son las mismas que las credenciales de producción, a menos que haya cambiado las credenciales de producción desde la última vez que se actualizó la zona protegida de actualización personalizada. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

## Programe una actualización de su zona protegida de actualización personalizada

>[!IMPORTANT]
>
>La duración de la actualización depende del tamaño de los datos que se están actualizando. Durante el proceso de actualización, es fundamental que el entorno de la zona protegida de actualización personalizada no se utilice de ninguna manera (incluidas las llamadas y integraciones de la API), ya que esto evitará que la actualización de la zona protegida finalice correctamente. [!DNL Workfront] deshabilitará el entorno de zona protegida de actualización personalizada antes de que comience, pero debe finalizar cualquier sesión activa para asegurarse de que la actualización de la zona protegida se realice correctamente.

Después de programar una actualización del espacio aislado de actualización personalizado, puede cancelarla haciendo clic en [!UICONTROL Cancelar] en la parte superior de la página. También puede volver a programarla para más adelante.

>[!NOTE]
>
>No puede programar actualizaciones automáticas de zonas protegidas.

Para programar una actualización del espacio aislado de actualización del cliente:

1. Inicie sesión en su zona protegida de actualización personalizada.
1. Clic **[!UICONTROL Programación]** en el titular de la parte superior de la pantalla y seleccione una fecha del calendario.
1. Seleccione una fecha para el momento en que desea que se produzca la actualización y haga clic en **[!UICONTROL Programar actualización]**.

## Cambiar a producción desde la zona protegida de actualización personalizada

1. Inicie sesión en su zona protegida de actualización personalizada.

   Para obtener más información sobre el acceso a la zona protegida de actualización personalizada, consulte [Acceda a la zona protegida de actualización personalizada desde el entorno de producción](#access-the-custom-refresh-sandbox-from-your-production-environment) o [Acceso al espacio aislado de actualización personalizado mediante una dirección URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Clic **[!UICONTROL Ir a producción]** en el titular de la parte superior de la pantalla.

   Recuerde que el trabajo realizado en la zona protegida no será visible en la [!UICONTROL producción] , ya que la transferencia de datos es unidireccional, de producción a su zona protegida de actualización personalizada, y no a la inversa.

## Recibir correos electrónicos de la zona protegida de actualización personalizada

[!DNL Workfront] deshabilita toda la comunicación por correo electrónico desde el entorno de espacio aislado de actualización personalizado. Si desea recibir notificaciones por correo electrónico desde el entorno de espacio aislado de actualización personalizado, debe habilitar esta funcionalidad en la configuración de usuario. Para obtener más información sobre la activación de notificaciones por correo electrónico en el entorno de espacio aislado de actualización personalizado, consulte [Habilitar el envío de correos electrónicos desde el entorno de vista previa de espacio aislado](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Las notificaciones push y de envío de informes en la aplicación móvil siempre están desactivadas para el entorno de espacio aislado de actualización personalizado. Ni tú ni el [!DNL Workfront] El administrador de puede habilitar la entrega de informes o las notificaciones push para la aplicación móvil al acceder al entorno de espacio aislado de actualización personalizado.\
>Para obtener más información sobre los envíos de informes para el entorno de producción, consulte [Resumen de entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Para obtener más información sobre las notificaciones push en la aplicación móvil para el entorno de producción, consulte la sección en .

## Configurar el inicio de sesión único en la zona protegida de actualización personalizada

Si desea configurar la zona protegida de actualización personalizada para que funcione con una solución de inicio de sesión único, puede configurarla por separado desde el entorno de producción. La configuración de SSO de la zona protegida de actualización personalizada es independiente de la configuración de SSO del entorno de producción.\
Al actualizar el espacio aislado de actualización personalizado, la información de SSO no se copia del entorno de producción para sobrescribir la configuración del espacio aislado de actualización personalizado.

Los pasos para configurar el inicio de sesión único en la zona protegida de actualización personalizada son similares a los necesarios para configurarlo en el entorno de producción.\
Para obtener más información sobre la configuración [!DNL Workfront] con SSO, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Esta opción no está disponible si la organización [!DNL Workfront] está habilitada con Adobe IMS. Consulte al administrador de red o de TI si necesita más información.

## Uso y disponibilidad previstos

* [!DNL Workfront] Los entornos de la zona protegida de actualización personalizada no están pensados para pruebas de carga o rendimiento. En su lugar, utilice estos entornos para validar la funcionalidad de las funciones con los flujos de trabajo existentes de su organización.

* [!DNL Workfront] Los entornos de la zona protegida de actualización personalizada están pensados para estar siempre disponibles. Cualquier interrupción en un entorno de espacio aislado de actualización personalizado de Workfront durante el horario laboral normal será una prioridad inmediata después de resolver cualquier problema de producción, si existe. Cualquier interrupción en un entorno de espacio aislado de actualización personalizado de Workfront los fines de semana (sábados y domingos) se solucionará para que el entorno se ejecute en horario laboral los lunes.

* La revisión no está disponible en los entornos de la zona protegida de actualización personalizada.
