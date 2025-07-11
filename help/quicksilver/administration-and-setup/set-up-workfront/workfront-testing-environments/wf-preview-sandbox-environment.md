---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 'El entorno de vista previa de zona protegida de  [!DNL Adobe Workfront] '
description: La vista previa de la zona protegida es un entorno de prueba que sirve como réplica de su entorno en directo. Workfront lo actualiza todos los fines de semana. Los datos añadidos a su entorno en directo el viernes aparecerán en su zona protegida de vista previa el lunes que viene. Todos los paquetes de asistencia tienen acceso a esta zona protegida.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 7549c9699a86b6f87e5562efd7e586be282c5619
workflow-type: tm+mt
source-wordcount: '1302'
ht-degree: 93%

---

# El entorno de vista previa de zona protegida de [!DNL Adobe Workfront]

<!-- Audited: 12/2023 -->

Hay dos entornos de prueba para [!DNL Workfront] que son réplicas de su entorno de producción [!DNL Workfront]:

* La vista previa de zona protegida

  La vista previa de zona protegida es un entorno de prueba que sirve como réplica de su entorno activo y [!DNL Workfront] lo actualiza cada fin de semana. Los datos añadidos a su entorno en directo el viernes aparecerán en su zona protegida de vista previa el lunes que viene.

  Todos los paquetes de asistencia tienen acceso a la vista previa de zona protegida.

* La actualización personalizada de la zona protegida

  La zona protegida de actualización personalizada es un entorno de prueba independiente que se actualiza manualmente por usted. La zona protegida de actualización personalizada tiene un coste adicional. Para obtener más información sobre este entorno, consulte [El [!DNL Adobe Workfront] entorno de actualización personalizada de la zona protegida](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard] Paquete de soporte</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus], [!UICONTROL Preferred] y paquetes de soporte de [!UICONTROL Enterprise]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Vista previa de la zona protegida</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Actualización personalizada de la zona protegida</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vista previa de la zona protegida

La vista previa de la zona protegida sirve como entorno en el que los usuarios de su organización pueden probar y trabajar con seguridad con datos del entorno de producción sin que afecte al entorno de producción.

La vista previa de zona protegida contiene los datos de producción reales; sin embargo, se actualiza cada fin de semana para que los datos puedan retrasarse hasta una semana respecto al entorno de producción. Los elementos creados desde la última actualización se encuentran en el entorno de zona protegida de vista previa hasta la siguiente actualización.

Los datos fluyen unidireccionalmente, de Producción a Vista previa y no a la inversa. Una actualización del entorno de vista previa siempre la programa [!DNL Workfront] para cada fin de semana.

La vista previa de zona protegida también permite que [!DNL Workfront] implemente nuevas características en un entorno seguro antes de que estén listas para implementarse en el entorno de producción. Puede probar las nuevas características y proporcionar comentarios de [!DNL Workfront] sobre su funcionalidad accediendo a la vista previa de zona protegida. Por este motivo, el código de la vista previa de zona protegida siempre va por delante del código de producción, aunque los datos se actualicen semanalmente.

El entorno de vista previa es ideal para ejecutar cursos de formación, probar nuevas funciones y determinar la funcionalidad de la configuración.

>[!NOTE]
>
>Cuando acceda a la Vista previa de zona protegida, observe el banner azul en la parte superior de la pantalla. El banner no se puede quitar mientras esté trabajando en este entorno.
>
>El nombre del entorno al que accede (Vista previa) y la versión de lanzamiento del código se muestran en el banner. Haz clic en **[!UICONTROL Ver las novedades]** para obtener información sobre esa versión.
>
>![Vista previa del banner](assets/preview-banner-nwe-350x161.png)

## Acceso a la zona protegida de vista previa

De manera predeterminada, como administrador de [!DNL Workfront], tiene acceso al entorno de [!UICONTROL Vista previa] de zona protegida. Si no puede acceder al entorno de [!UICONTROL Vista previa] de zona protegida tal como se describe en esta sección, póngase en contacto con su administrador de [!DNL Workfront] o con nuestro equipo de atención al cliente.


### Acceder a la zona protegida de vista previa desde la interfaz [!DNL Workfront] {#accessing-the-preview-sandbox-from-the-workfront-interface}

Como administrador de [!DNL Workfront], puede acceder a la vista previa de zona protegida a través de la interfaz de [!DNL Workfront].

Para acceder a la vista previa de zona protegida:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Sistema]** > **[!UICONTROL Preferencias]**.

1. En la sección **[!UICONTROL Entornos de prueba]**, haga clic en **[!UICONTROL Vista previa de espacio aislado]**.

1. Inicie sesión con sus credenciales de vista previa.

   Deben ser las mismas credenciales que las de producción, a menos que las haya cambiado en Producción después de que se actualice la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

### Acceso a la zona protegida de vista previa mediante una URL {#accessing-the-preview-sandbox-using-a-url}

Puede acceder a la zona protegida de vista previa mediante una URL.

#### Acceder a la zona protegida de vista previa para cuentas en el clúster 1, 2, 3 y 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

La dirección URL de la zona protegida de vista previa es: `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Si tenía marcadores que se vinculaban a la dirección URL antigua para la zona protegida de vista previa, tome nota de este cambio y actualice la dirección URL en sus marcadores.

Para iniciar sesión en la zona protegida de vista previa con una dirección URL:

1. Vaya a esta dirección URL: `https://companyname.preview.workfront.com/`.

   Si es cliente de EMEA y su cuenta está en el clúster 4, consulte la sección Acceso a la zona protegida de vista previa para cuentas en el clúster 4 (cuentas de EMEA) a continuación.

1. Inicie sesión con sus credenciales de vista previa.

   >[!TIP]
   >
   >Las credenciales de vista previa deben ser las mismas que las de producción, a menos que las haya cambiado en Producción después de la actualización de la Vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.


#### Acceso a la zona protegida de vista previa para cuentas en el clúster 4 (Cuentas EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Para iniciar sesión en la zona protegida de vista previa con una dirección URL:

1. Vaya a esta dirección URL: `https://companyname.preview.workfront.com/`.

   También puede obtener acceso a la zona protegida de vista previa accediendo a [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Inicie sesión con sus credenciales de vista previa.

   Las credenciales de vista previa deben ser las mismas que las de producción, a menos que las haya cambiado en Producción después de la actualización de la Vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.

## Recepción de correos electrónicos desde la zona protegida de vista previa

Workfront deshabilita toda la comunicación por correo electrónico desde el entorno de zona protegida de vista previa. Si desea recibir notificaciones por correo electrónico desde el entorno zona protegida de de vista previa, debe habilitar esta funcionalidad en la configuración de usuario. Para obtener más información sobre la habilitación de las notificaciones por correo electrónico en el entorno de zona protegida de vista previa, consulte [Habilitación del envío de correos electrónicos desde el entorno de zona protegida de vista previa](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Las notificaciones push y de envío de informes en la aplicación móvil siempre están desactivadas para el entorno de zona protegida de vista previa. Ni usted ni el administrador de [!DNL Workfront] pueden habilitar la entrega de informes ni las notificaciones push para la aplicación móvil al acceder al entorno de zona protegida de vista previa.
>
>Para obtener más información sobre las entregas de informes para el entorno de producción, consulte [Información general sobre la entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Inicio de sesión único (SSO)

Si usa SSO, colabore con nuestro equipo de atención al cliente para asegurarse de que esté configurado correctamente para que pueda utilizar sus credenciales de SSO para iniciar sesión en la zona protegida de [!UICONTROL Vista previa]. Si falla el inicio de sesión, comuníquese con el servicio de atención al cliente habitual o con el administrador de [!DNL Workfront] para obtener ayuda.

Para obtener más información sobre el inicio de sesión único, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configuración del inicio de sesión único en la zona protegida de vista previa

>[!IMPORTANT]
>
>El procedimiento que se describe en esta página solo se aplica a las organizaciones que aún no se han incorporado a [!DNL Adobe Admin Console]. Si su organización se ha incorporado a [!DNL Adobe Admin Console], no es necesario realizar ninguna acción.
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a [!DNL Adobe Admin Console], consulte [Diferencias de administración basadas en la plataforma ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Si desea configurar la zona protegida de vista previa para que funcione con una solución de inicio de sesión único, puede configurarla por separado desde el entorno de producción. La configuración de SSO en la zona protegida de vista previa es independiente de la configuración de SSO en el entorno de producción.

Cuando se actualiza la zona protegida de vista previa (todos los fines de semana), la información de SSO no se copia desde el entorno de producción para sobrescribir la configuración de la zona protegida de vista previa.

Los pasos para configurar el inicio de sesión único en la zona protegida de vista previa son similares a los necesarios para configurarlo en el entorno de producción.

Para obtener más información sobre la configuración de [!DNL Workfront] con SSO, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Recálculo automático de escalas de tiempo de proyectos

Recalcular las cronologías permite a los administradores ver cómo las fuerzas de fuera del proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas del proyecto.

Como administrador de Workfront, puede configurar cuándo Workfront recalcula automáticamente las escalas de tiempo de los proyectos. Workfront puede recalcular las escalas de tiempo del proyecto cada noche, cuando cambia el ámbito del proyecto o ambas cosas.

Para obtener más información, vea [Configurar cálculos de escala de tiempo para proyectos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Para el entorno de vista previa, el cálculo nocturno está deshabilitado y las escalas de tiempo del proyecto no se recalculan automáticamente. Debe recalcular manualmente la cronología del proyecto para el entorno de vista previa. Para obtener más información, consulte [Recalcular líneas de tiempo de proyecto](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Rendimiento y disponibilidad del entorno de vista previa

* [!DNL Workfront] Los entornos de vista previa no están pensados para pruebas de carga o rendimiento. En su lugar, utilice estos entornos para validar la funcionalidad de las funciones con los flujos de trabajo existentes de su organización.

* Los flujos de trabajo que implican documentos deben centrarse en procesos y no en pruebas de carga. Los archivos grandes no son compatibles con los entornos de espacio aislado.

* [!DNL Workfront] Los entornos de vista previa están pensados para estar siempre disponibles.

* Cualquier interrupción en un entorno de vista previa de [!DNL Workfront] durante el horario laboral normal será una primera prioridad inmediatamente después de que se resuelva cualquier problema de producción, si existe.

* Cualquier interrupción en un entorno de vista previa de [!DNL Workfront] los fines de semana (sábados y domingos) se solucionará para que el entorno funcione durante el horario laboral los lunes.
