---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Crear una cuenta de Reader (servicio) para Snowflake
description: Para acceder a los datos del lago de datos de Workfront, primero debe crear una cuenta de Reader para Snowflake.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 912f46c87170d6b678d885ccc1fb0170526578df
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Crear una cuenta de Reader (servicio) para Snowflake

Para acceder a los datos del lago de datos de Workfront, primero debe crear una cuenta de Reader para Snowflake. Además, debe agregar direcciones IP a la lista de permitidos para cualquier herramienta externa que planee conectar con los datos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Por determinar</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Crear una cuenta de lector

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Clic **Crear nueva conexión**

1. En la ventana que aparece, introduzca un nombre para la conexión en **Descripción de referencia de conexión** y un nombre de usuario en **Usuario de conexión**, luego haga clic en **Generar conexión**.

   ![Crear cuenta de lector](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Contraseña predeterminada** , así como una dirección URL donde los datos pueden verse a través del Snowflake. Deberá utilizar la contraseña junto con el nombre de usuario que eligió para iniciar sesión en Snowflake por primera vez, así que asegúrese de mantener un registro de ella y de la dirección URL. Marque la casilla que indica que lo ha hecho y haga clic en **Cerrar**.

   ![Contraseña de cuenta predeterminada](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Abra Snowflake con un explorador para ir a la dirección URL del paso anterior, introduzca el nombre de usuario seleccionado y la contraseña predeterminada del paso anterior y, a continuación, haga clic en **Iniciar sesión**.

1. Después de iniciar sesión correctamente por primera vez, se le pedirá que elija una nueva contraseña. Introduzca una contraseña de su elección en **Nueva contraseña** y **Confirmar contraseña** campos y haga clic en **Enviar**.

   ![Restablecer contraseña de Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Ahora puede utilizar su nombre de usuario y la nueva contraseña para acceder a su repositorio de datos de Workfront en Snowflake o a la herramienta de visualización empresarial de su elección.

## Añadir direcciones IP a la lista de permitidos

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haga clic en **IP permitidas** y, a continuación, haga clic en **Añadir una dirección IP a la Lista de permitidos** botón.

1. Introduzca un nombre para la dirección IP en **Descripción de dirección IP** e introduzca la dirección IP de la herramienta que desea utilizar en **Dirección IP**, luego haga clic en **Añadir IP a la Lista de permitidos**.

   ![Añadir dirección IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Revocar una cuenta de Reader o quitar una dirección IP de la lista de permitidos

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haga clic en el icono de la papelera ![Icono Eliminar](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a la derecha de la cuenta que desea revocar.

   O

   Haga clic en **IP permitidas** pestaña, luego haga clic en el icono de la papelera ![Icono Eliminar](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a la derecha de la dirección IP que desea eliminar.

1. En la ventana que aparece, marque la casilla para confirmar y luego haga clic en **Eliminar**.
