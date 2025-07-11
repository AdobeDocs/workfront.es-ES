---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: El  [!DNL Adobe Workfront] Entorno De Espacio Aislado De Actualización Personalizado
description: La zona protegida de actualización personalizada es un entorno en el que puede realizar pruebas y trabajar usando datos del entorno de producción. También es ideal para ejecutar cursos de formación y determinar la funcionalidad de la configuración.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 7549c9699a86b6f87e5562efd7e586be282c5619
workflow-type: tm+mt
source-wordcount: '1763'
ht-degree: 92%

---

# El entorno de zona protegida de actualización personalizada de [!DNL Adobe Workfront]

La zona protegida de actualización personalizada es un entorno en el que puede realizar pruebas y trabajar usando datos del entorno de producción. También es ideal para ejecutar cursos de formación y determinar la funcionalidad de la configuración.

>[!NOTE]
>
>Es diferente de la zona protegida de vista previa, que también es un entorno de prueba que replica su entorno de producción de [!DNL Workfront].
>
>* Las nuevas funciones se introducen en la zona protegida de vista previa antes de que estén disponibles en producción.
>* Las nuevas funciones no se introducen en la zona protegida de actualización personalizada antes de que estén disponibles en el entorno de producción.
>
>  Además, hay un coste adicional para obtener la zona protegida de actualización personalizada que no es necesario para la vista previa de la zona protegida.
>
>  Para obtener más información sobre la zona protegida de vista previa, consulte [Entorno de zona protegida de vista previa [!DNL Adobe Workfront] .](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>[!UICONTROL Plan] </p> <p>Debe ser administrador de [!DNL Workfront]. Para obtener información sobre los administradores de [!DNL Workfront], consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paquete de soporte</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] o [!UICONTROL Enterprise]</p> <p>El paquete de soporte estándar no tiene acceso a la zona protegida de actualización personalizada, pero sí tiene acceso a la de vista previa.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Actualización de la zona protegida de actualización personalizada

La zona protegida de actualización personalizada contiene los datos de producción reales y no se actualiza hasta que la programe para ello. Puede programar una actualización en cualquier momento que le resulte conveniente, con una frecuencia de hasta una vez a la semana.

>[!NOTE]
>
>* No puede programar una actualización para el día actual. Por ejemplo, si hoy es 1 de junio, el primer día en que se puede programar una actualización es el 2 de junio.
>* La actualización programada se produce en algún momento durante la noche, según el clúster del usuario (los clústeres de EE. UU. se actualizan durante la noche en EE. UU.). La hora específica es impredecible debido a otros clientes que hay en la cola y a la cantidad de datos que se actualizan. Si la cola tiene muchos clientes grandes, es posible que su actualización no se ejecute hasta más tarde ese día o al día siguiente.
>* La zona protegida de actualización personalizada siempre ofrece las mismas características de producto que el entorno de producción. Sin embargo, al actualizar la zona protegida de actualización personalizada, solo se conserva la personalización de marca para el color de fondo de la pantalla de inicio de sesión. La pantalla de inicio de sesión y los logotipos de la barra de navegación se restablecen a los valores predeterminados de [!DNL Workfront], y no se muestran las imágenes de personalización de marca que haya modificado antes de la actualización.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Acceder a la zona protegida de actualización personalizada desde el entorno de producción {#access-the-custom-refresh-sandbox-from-your-production-environment}

Como administrador de [!DNL Workfront], puede acceder a su zona protegida de actualización personalizada desde el entorno de producción.

>[!NOTE]
>
>Si su cuenta está en el clúster 4 (clúster de EMEA), no podrá acceder a su zona protegida de actualización personalizada desde el entorno de producción. Para obtener más información sobre cómo puede acceder a la zona protegida de actualización personalizada cuando tenga una cuenta en el clúster 4, consulte [Acceder a la zona protegida de actualización personalizada para las cuentas del clúster 4 (cuentas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Acceder a la zona protegida de actualización personalizada para las cuentas del clúster 4 (cuentas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Para acceder a su zona protegida de actualización personalizada:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración de engranajes](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Sistema]** >**[!UICONTROL Preferencias]**.

1. En la sección **[!UICONTROL Entorno de prueba]**, haga clic en **[!UICONTROL Zona protegida 1]** o **[!UICONTROL Zona protegida 2]**.

   El paquete de soporte especifica si tiene acceso a una o dos zonas protegidas de actualización personalizadas.

1. Inicie sesión con las credenciales de la zona protegida de actualización personalizada.

   Las credenciales de la zona protegida de actualización personalizada son las mismas que las credenciales de producción, a menos que haya cambiado las credenciales de producción desde la última vez que actualizó la zona protegida de actualización personalizada. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

   La zona protegida de actualización personalizada muestra la versión y la fecha de la última actualización en el banner situado en la parte superior de la pantalla. Toda la información de producción está disponible y lista para trabajar con ella una vez completada la actualización.

## Acceder a la zona protegida de actualización personalizada mediante una dirección URL {#access-the-custom-refresh-sandbox-using-a-url}

Cualquier usuario puede acceder a la zona protegida de actualización personalizada mediante una dirección URL.

* [Acceso a la zona protegida de actualización personalizada para cuentas de los clústeres 1, 2, 3 y 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Acceso a la zona protegida de actualización personalizada para cuentas en el clúster 4 (cuentas de EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Acceso a la zona protegida de actualización personalizada para cuentas de los clústeres 1, 2, 3 y 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Según el paquete de soporte, debe tener acceso a una o dos zonas protegidas de actualización personalizadas.

Para acceder a la zona protegida de actualización personalizada mediante una dirección URL:

1. Vaya a esta dirección URL si solo tiene una zona protegida de actualización personalizada:

   `https://companyname.sb01.workfront.com` (URL anterior: `https://cr1.attasksandbox.com/`.)

   O si tiene dos zonas protegidas de actualización personalizadas, además de las direcciones URL anteriores, también puede ir a la siguiente URL para acceder a su segunda zona protegida de actualización personalizada:

   `https://companyname.sb02.workfront.com` (URL anterior: `https://cr2.attasksandbox.com/`)

1. En la pantalla de inicio de sesión, inicie sesión con las credenciales de su zona protegida de actualización personalizada.
1. Las credenciales de la zona protegida de actualización personalizada son las mismas que las credenciales de producción, a menos que haya cambiado las credenciales de producción desde la última vez que se actualizó la zona protegida de actualización personalizada. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

### Acceso a la zona protegida de actualización personalizada para cuentas en el clúster 4 (cuentas de EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Si su cuenta de [!DNL Workfront] está en el clúster 4 (clúster de EMEA), solo podrá acceder a su zona protegida de actualización personalizada mediante una dirección URL. Para saber en qué clúster se encuentra su cuenta, póngase en contacto con nuestro equipo de Asistencia al cliente.

Según el paquete de soporte, debe tener acceso a una o dos zonas protegidas de actualización personalizadas.

Para acceder a la zona protegida de actualización personalizada mediante una dirección URL:

1. Vaya a esta dirección URL si solo tiene una zona protegida de actualización personalizada:

   `https://companyname.sb01.workfront.com` (URL anterior: `https://cr3.attasksandbox.com`)

   O

   Vaya a una de estas direcciones URL si tiene dos zonas protegidas de actualización personalizadas:

   `https://companyname.sb01.workfront.com` (URL anterior: `https://cr3.attasksandbox.com`)

   `https://companyname.sb02.workfront.com` (URL anterior: `https://cr4.attasksandbox.com`)

1. En la pantalla de inicio de sesión, inicie sesión con las credenciales de su zona protegida de actualización personalizada.

   Las credenciales de la zona protegida de actualización personalizada son las mismas que las credenciales de producción, a menos que haya cambiado las credenciales de producción desde la última vez que se actualizó la zona protegida de actualización personalizada. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

## Programar una actualización de su zona protegida de actualización personalizada

>[!IMPORTANT]
>
>La duración de la actualización depende del tamaño de los datos que se están actualizando. Durante el proceso de actualización, es fundamental que el entorno de la zona protegida de actualización personalizada no se utilice de ninguna manera (incluidas las llamadas e integraciones de la API), ya que esto evitará que la actualización de la zona protegida finalice correctamente. [!DNL Workfront] deshabilitará el entorno de zona protegida de actualización personalizada antes de que comience, pero debe finalizar cualquier sesión activa para asegurarse de que la actualización de la zona protegida se realice correctamente.

Después de programar una actualización de la zona protegida de actualización personalizada, puede cancelarla haciendo clic en [!UICONTROL Cancelar] en la parte superior de la página. También puede volver a programarla para más adelante.

>[!NOTE]
>
>No puede programar actualizaciones automáticas de zonas protegidas.

Para programar una actualización de la zona protegida de actualización del cliente:

1. Inicie sesión en su zona protegida de actualización personalizada.
1. Haga clic en **[!UICONTROL Programar]** en el banner de la parte superior de la pantalla y seleccione una fecha del calendario.
1. Seleccione una fecha para cuando desee que se actualice y, a continuación, haga clic en **[!UICONTROL Programar actualización]**.

## Cambiar a producción desde la zona protegida de actualización personalizada

1. Inicie sesión en su zona protegida de actualización personalizada.

   Para obtener más información sobre el acceso a la zona protegida de actualización personalizada, consulte [Acceso a la zona protegida de actualización personalizada desde el entorno de producción](#access-the-custom-refresh-sandbox-from-your-production-environment) o [Acceso a la zona protegida de actualización personalizada mediante una dirección URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Haga clic en **[!UICONTROL Ir a producción]** en el banner de la parte superior de la pantalla.

   Recuerde que el trabajo realizado en la zona protegida no será visible en el entorno de [!UICONTROL producción], ya que la transferencia de datos es unidireccional, desde la producción a la zona protegida de actualización personalizada, y no a la inversa.

## Recibir correos electrónicos de la zona protegida de actualización personalizada

[!DNL Workfront] deshabilita toda la comunicación por correo electrónico desde el entorno de zona protegida de actualización personalizada. Si desea recibir notificaciones por correo electrónico desde el entorno de zona protegida de actualización personalizado, debe habilitar esta funcionalidad en la configuración de usuario. Para obtener más información sobre cómo habilitar las notificaciones por correo electrónico en el entorno de zona protegida de actualización personalizada, consulte [Habilitar el envío de correos electrónicos desde el entorno de zona protegida de vista previa](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Las notificaciones push y de envío de informes en la aplicación móvil siempre están desactivadas para el entorno de zona protegida de actualización personalizada. Ni usted ni el administrador de [!DNL Workfront] pueden habilitar la entrega de informes o las notificaciones push para la aplicación móvil al acceder al entorno de zona protegida de actualización personalizada.\
>Para obtener más información sobre los envíos de informes para el entorno de producción, consulte [Resumen de la entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Configuración del inicio de sesión único en la zona protegida de actualización personalizada

Si desea configurar la zona protegida de actualización personalizada para que funcione con una solución de inicio de sesión único, puede configurarla por separado desde el entorno de producción. La configuración de SSO de la zona protegida de actualización personalizada es independiente de la configuración de SSO del entorno de producción.\
Al actualizar la zona protegida de actualización personalizada, la información de SSO no se copia desde el entorno de producción para sobrescribir la configuración de la zona protegida de actualización personalizada.

Los pasos para configurar el inicio de sesión único en la zona protegida de actualización personalizada son similares a los necesarios para configurarlo en el entorno de producción.\
Para obtener más información sobre la configuración de [!DNL Workfront] con SSO, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Esto no está disponible si la instancia de [!DNL Workfront] de su organización está habilitada con Adobe IMS. Consulte al administrador de red o de TI si necesita más información.

## Recálculo automático de escalas de tiempo de proyectos

Recalcular las cronologías permite a los administradores ver cómo las fuerzas de fuera del proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas del proyecto.

Como administrador de Workfront, puede configurar cuándo Workfront recalcula automáticamente las escalas de tiempo de los proyectos. Workfront puede recalcular las escalas de tiempo del proyecto cada noche, cuando cambia el ámbito del proyecto o ambas cosas.

Para obtener más información, vea [Configurar cálculos de escala de tiempo para proyectos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Para el entorno de espacio aislado de actualización personalizado, el cálculo nocturno está deshabilitado y las escalas de tiempo del proyecto no se recalculan automáticamente. Debe recalcular manualmente la cronología del proyecto para el entorno de espacio aislado de actualización personalizado. Para obtener más información, consulte [Recalcular líneas de tiempo de proyecto](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Uso y disponibilidad previstos

* Los entornos de zona protegida de actualización personalizada de [!DNL Workfront] no están pensados para pruebas de carga o rendimiento. En su lugar, utilice estos entornos para validar la funcionalidad de las funciones con los flujos de trabajo existentes de su organización.

* Los flujos de trabajo que implican documentos deben centrarse en procesos y no en pruebas de carga. Los archivos grandes no son compatibles con los entornos de espacio aislado.

* Los entornos de zona protegida de actualización personalizada de [!DNL Workfront] están pensados para estar siempre disponibles. Cualquier interrupción en un entorno de zona protegida de actualización personalizada de Workfront durante el horario laboral normal será una prioridad inmediata después de resolver cualquier problema de producción, si existe. Cualquier interrupción en un entorno de zona protegida de actualización personalizada de Workfront los fines de semana (sábados y domingos) se solucionará para que el entorno se ejecute en horario laboral los lunes.

* La revisión no está disponible en los entornos de la zona protegida de actualización personalizada.
