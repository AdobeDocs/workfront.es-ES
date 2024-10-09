---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Crear una cuenta de Reader (servicio) para Snowflake
description: Para acceder a los datos de Data Connect, primero debe crear una cuenta de Snowflake reader.
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Crear una cuenta de Reader (servicio) para Snowflake

Para acceder a los datos de Data Connect, primero debe crear una cuenta de Snowflake reader (o servicio) para cada nueva conexión. Después de crear una conexión, puede encontrar su URL y nombre de usuario asociados haciendo clic en ella en la página **Acceso a datos** (**Menú principal** > **Configuración** > **Sistema** > **Acceso a datos**) en la pestaña **Conexiones existentes**.

Para obtener información sobre cómo usar una conexión recién creada con un producto externo, consulte [Establecer una conexión con Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td><p>Incluido en los siguientes planes:</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <p>Se puede comprar como complemento de los siguientes planes:</p> 
    <ul>
        <li>Seleccionar</li> 
        <li>Prime</li>
    </ul> 
    <p>Workfront Data Connect no está disponible para los planes Workfront heredados.</p> 
   </td> </td> 
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

+++

## Crear una cuenta de lector

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haga clic en **Crear nueva conexión**

1. En la ventana que aparece, escriba un nombre para la conexión en **Descripción de referencia de la conexión** y un nombre de usuario en **Usuario de conexión**, y después haga clic en **Generar conexión**.

   ![Crear cuenta de lector](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Se generará una **contraseña predeterminada**, así como una dirección URL donde los datos se podrán ver a través del Snowflake. Deberá utilizar la contraseña junto con el nombre de usuario que eligió para iniciar sesión en Snowflake por primera vez, así que asegúrese de mantener un registro de ella y de la dirección URL. Marque la casilla que indica que lo ha hecho y luego haga clic en **Cerrar**.

   ![Contraseña de cuenta predeterminada](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Abra el Snowflake con un explorador para ir a la dirección URL del paso anterior, escriba el nombre de usuario que seleccionó y la contraseña predeterminada del paso anterior y luego haga clic en **Iniciar sesión**.

1. Después de iniciar sesión correctamente por primera vez, se le pedirá que elija una nueva contraseña. Escriba una contraseña de su elección en los campos **Nueva contraseña** y **Confirmar contraseña** y luego haga clic en **Enviar**.

   ![Restablecer contraseña de Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Ahora puede utilizar su nombre de usuario y la nueva contraseña para acceder a su repositorio de datos de Data Connect en Snowflake o a la herramienta de visualización empresarial de su elección.

## Revocar una cuenta de lector

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haga clic en el icono de la papelera ![Eliminar icono](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a la derecha de la cuenta que desee revocar.

1. En la ventana que aparece, marque la casilla para confirmar y luego haga clic en **Eliminar**.
