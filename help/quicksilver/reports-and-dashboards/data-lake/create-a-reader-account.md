---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Crear una cuenta de lector para Snowflake
description: Para acceder a los datos de Data Connect, primero debe crear una cuenta de Snowflake Reader.
author: Courtney
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: b6267718fd76a643395c850b97352095a0fe12fc
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 17%

---

# Crear una cuenta de lector o una conexión para Snowflake

Para acceder a los datos de Data Connect, primero debe crear una cuenta de Snowflake Reader (o servicio) para su organización y, a continuación, crear una nueva conexión para cada usuario o herramienta que desee que tenga acceso a Data Connect.

Después de crear una conexión, puede encontrar su URL y nombre de usuario asociados haciendo clic en ella en la página Data Connect (menú principal > Configuración > Sistema > Data Connect) en la pestaña Existing Connections.

Para obtener información sobre cómo usar una conexión recién creada con un producto externo, consulte [Establecer una conexión con Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una cuenta de lector

Debe crear una nueva cuenta de Snowflake Reader para su organización antes de empezar a crear conexiones.

>[!IMPORTANT]
>
>Este proceso debe completarse solo una vez por organización. Si el botón **Crear cuenta de Reader** no está presente en la ubicación que se describe a continuación, ya se ha creado la cuenta de Reader.

Para crear una cuenta de lector:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront (si está disponible), o haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Conexión de datos**.

1. Haga clic en el botón **Crear cuenta de Reader** para empezar a crear la cuenta de Reader de su organización. El proceso es automático, pero puede tardar hasta 24 horas en completarse.

1. Una vez finalizado, aparecerá una ventana de diálogo en la que se explica que la cuenta de Reader ya está activa. Actualice la página del explorador para obtener acceso al botón **Crear nueva conexión**.

![Cuadro de diálogo creado en la cuenta de Reader](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## Crear una conexión

>[!IMPORTANT]
>
>En junio de 2026, se requerirán credenciales de nombre de usuario y contraseña para utilizar la autenticación de varios factores (MFA). Se recomienda realizar la transición a la autenticación RSA o basada en PAT para cuentas de usuario de servicio utilizadas para cargar datos de Data Connect en herramientas de visualización de terceros, procesadores de datos y scripts que no funcionarán con MFA en el proceso de autenticación.


1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configuración**.

1. En el panel izquierdo, haga clic en **Sistema** > **Conexión de datos**.

1. Haga clic en **Crear nueva conexión**.

1. En la ventana que aparece, escriba un nombre para la conexión en **Descripción de referencia de la conexión** y un nombre de usuario en **Usuario de conexión**, y después haga clic en **Generar conexión**.

   ![Crear nueva conexión](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Elija un método de autenticación para la conexión:
   * [Autenticación de contraseña](#password-authentication)
   * [Autenticación de token de acceso mediante programación](#programmatic-access-token-authentication)
   * [Autenticación de clave RSA](#rsa-key-authentication)

### Autenticación de contraseña

1. Haga clic en **Contraseña** y luego en **Generar conexión**.

1. Se genera una **contraseña predeterminada**, así como una dirección URL donde los datos se pueden ver a través de Snowflake. Debe utilizar la contraseña con el nombre de usuario que eligió para iniciar sesión en Snowflake por primera vez, así que asegúrese de mantener un registro de ella y de la dirección URL. Marque la casilla que indica que lo ha hecho y luego haga clic en **Cerrar**.

   ![Contraseña de cuenta predeterminada](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Abra Snowflake con un explorador para ir a la dirección URL del paso anterior, escriba el nombre de usuario que seleccionó y la contraseña predeterminada del paso anterior y luego haga clic en **Iniciar sesión**.

1. Después de iniciar sesión correctamente por primera vez, se le pedirá que elija una nueva contraseña. Escriba una contraseña de su elección en los campos **Nueva contraseña** y **Confirmar contraseña** y luego haga clic en **Enviar**.

   ![Restablecer contraseña de Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Ahora puede utilizar su nombre de usuario y la nueva contraseña para acceder a su repositorio de datos de Data Connect en Snowflake o a la herramienta de visualización empresarial de su elección.

### Autenticación de token de acceso mediante programación

1. Haga clic en **Token de acceso mediante programación**.

1. Escriba una fecha de caducidad para su token en el campo **Fecha de caducidad**. Puede elegir una fecha de caducidad de hasta 365 días en el futuro.

1. Haga clic en **Generar conexión**.

1. Se genera un token PAT que puede utilizarse para autenticarse y se proporciona la URL de entorno de Snowflake. Puede utilizar la PAT y el nombre de usuario que ha proporcionado para conectarse a Snowflake desde su herramienta de visualización o procesador de datos de terceros. Asegúrese de mantener un registro de este y de la dirección URL. Marque la casilla que indica que lo ha hecho y luego haga clic en **Cerrar**.

   ![diálogo de token de acceso programático](/help/quicksilver/reports-and-dashboards/data-lake/assets/pat-test.png)


### Autenticación de clave RSA

1. Haga clic en **Clave RSA**.

1. Escriba una clave pública RSA en el campo **Clave pública RSA**.

1. Haga clic en **Generar conexión**.

1. Se genera una conexión y se proporciona la dirección URL del entorno de Snowflake. Puede utilizar la clave RSA y el nombre de usuario que proporcionó para conectarse a Snowflake desde la herramienta de visualización o el procesador de datos de terceros.



Debe utilizar la clave RSA con el nombre de usuario que eligió para iniciar sesión en Snowflake, así que asegúrese de mantener un registro de ella y de la dirección URL. Marque la casilla que indica que lo ha hecho y luego haga clic en **Cerrar**.

¡    ![Cuadro de diálogo de clave RSA](Assets/rsa-test.png)

## Revocar una cuenta de lector

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront (si está disponible), o haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haga clic en el icono de la papelera ![Eliminar icono](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a la derecha de la cuenta que desee revocar.

1. En la ventana que aparece, marque la casilla para confirmar y luego haga clic en **Eliminar**.
