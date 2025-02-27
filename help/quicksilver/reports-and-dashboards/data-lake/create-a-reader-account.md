---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Crear una cuenta de lector para Snowflake
description: Para acceder a los datos de Data Connect, primero debe crear una cuenta de Snowflake Reader.
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 25%

---

# Crear una cuenta de lector o una conexión para Snowflake

Para acceder a los datos de Data Connect, primero debe crear una cuenta de Snowflake Reader (o servicio) para su organización y, a continuación, crear una nueva conexión para cada usuario o herramienta que desee que tenga acceso a Data Connect.

Después de crear una conexión, puede encontrar su URL y nombre de usuario asociados haciendo clic en ella en la página **Conexión de datos** (**Menú principal** > **Configuración** > **Sistema** > **Conexión de datos**) en la pestaña **Conexiones existentes**.

Para obtener información sobre cómo usar una conexión recién creada con un producto externo, consulte [Establecer una conexión con Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td><p>Incluido en los siguientes planes:</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect no está disponible para los planes Workfront heredados.</p> 
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
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

1. Haga clic en el botón **Crear cuenta de Reader** para empezar a crear la cuenta de Reader de su organización. El proceso es automático, pero puede tardar unos minutos en completarse.

1. Una vez finalizado, aparecerá una ventana de diálogo en la que se explica que la cuenta de Reader ya está activa. Actualice la página del explorador para obtener acceso al botón **Crear nueva conexión**.

![Cuadro de diálogo creado en la cuenta de Reader](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## Crear una conexión

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront (si está disponible), o haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Conexión de datos**.

1. Haga clic en **Crear nueva conexión**

1. En la ventana que aparece, escriba un nombre para la conexión en **Descripción de referencia de la conexión** y un nombre de usuario en **Usuario de conexión**, y después haga clic en **Generar conexión**.

   ![Crear nueva conexión](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Se generará **una contraseña predeterminada**, así como una dirección URL donde los datos se podrán ver a través de Snowflake. Deberá utilizar la contraseña junto con el nombre de usuario que eligió para iniciar sesión en Snowflake por primera vez, por lo que debe asegurarse de mantener un registro de ella y de la dirección URL. Marque la casilla que indica que lo ha hecho y luego haga clic en **Cerrar**.

   ![Contraseña de cuenta predeterminada](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Abra Snowflake con un explorador para ir a la dirección URL del paso anterior, escriba el nombre de usuario que seleccionó y la contraseña predeterminada del paso anterior y luego haga clic en **Iniciar sesión**.

1. Después de iniciar sesión correctamente por primera vez, se le pedirá que elija una nueva contraseña. Escriba una contraseña de su elección en los campos **Nueva contraseña** y **Confirmar contraseña** y luego haga clic en **Enviar**.

   ![Restablecer contraseña de Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Ahora puede utilizar su nombre de usuario y la nueva contraseña para acceder a su repositorio de datos de Data Connect en Snowflake o a la herramienta de visualización empresarial de su elección.

## Revocar una cuenta de lector

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront (si está disponible), o haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haga clic en el icono de la papelera ![Eliminar icono](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a la derecha de la cuenta que desee revocar.

1. En la ventana que aparece, marque la casilla para confirmar y luego haga clic en **Eliminar**.
