---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Actualizar usuarios para el inicio de sesión único
description: Puede actualizar los usuarios para el inicio de sesión único en Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 1%

---

# Actualizar usuarios para el inicio de sesión único

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

Cuando el inicio de sesión único (SSO) está habilitado en la instancia de Adobe Workfront, los usuarios pueden iniciar sesión en Workfront con sus credenciales de SSO.

Si tiene un sistema existente que ya se ha rellenado con usuarios asociados con credenciales de SSO, puede importar los ID de los usuarios en Workfront importando un archivo de valores separados por comas (CSV) en Workfront.

Para obtener más información sobre la integración de Workfront con un sistema SSO, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p><p>O</p><p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Nombres de usuario SSO

Según la solución de SSO que utilice, el nombre de usuario del entorno de SSO se puede llamar como cualquiera de las siguientes opciones:

* Nombre de usuario de SSO
* Identificador de federación
* Usuario de federación

Independientemente de cómo se llame el nombre de usuario en su entorno de SSO, el valor del campo se almacena en el campo Nombre de usuario de SSO, en el objeto Usuario.

Para que los usuarios puedan utilizar sus credenciales de SSO para iniciar sesión en Workfront, debe actualizar su perfil para incluir su nombre de usuario de SSO, además de su nombre de usuario de Workfront.

Como administrador de Workfront, puede actualizar de forma masiva el campo Nombre de usuario SSO para sus usuarios de Workfront importando una lista de nombres de usuario en Workfront. Esta lista debe:

* Contiene el ID de usuario de Workfront (GUID) así como el nombre de usuario de SSO correspondiente para cada usuario
* Se puede guardar como archivo CSV o TSV.

Este proceso actualiza los nombres de usuario de SSO existentes en Workfront o añade un nuevo nombre de usuario de SSO, en caso de que falte uno para los usuarios.

## Preparación del archivo de importación {#prepare-the-import-file}

Puede empezar a preparar el archivo de importación creando un informe de todos los usuarios de Workfront que deben tener actualizados sus campos de nombre de usuario SSO.

1. Cree un informe de usuario en Workfront.

   Para obtener instrucciones sobre la creación de informes de usuario en Workfront, consulte [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Seleccione los campos siguientes en el informe:

   | Campo | Explicación |
   |---|---|
   | Nombre | Nombre completo del usuario de Workfront. |
   | Identificador | El ID es el GUID alfanumérico de Workfront. |
   | Nombre de usuario de SSO | Añadir el campo Nombre de usuario SSO para garantizar que no haya nombres de usuario que sobrescriba con la importación. Este campo debe estar en blanco para todos los usuarios si estos aún no se han actualizado para SSO. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Guarde el informe.
1. Clic **Exportar** en la parte superior del informe y exporte el informe a Excel.
1. Abra el archivo de Excel exportado y añada los nombres de usuario de SSO para cada usuario en el informe, en la columna Nombre de usuario de SSO.

   >[!IMPORTANT]
   >
   >Los nombres de usuario de SSO distinguen entre mayúsculas y minúsculas.

1. Eliminar todas las columnas del archivo de Excel, excepto la **ID** y el **Nombre de usuario de SSO** columnas.

1. Elimine los encabezados de columna y asegúrese de que no haya filas en blanco en la parte superior del informe.

   El archivo que está utilizando para actualizar los usuarios de Workfront con los nombres de usuario SSO **debe** contener solo 2 columnas, en este orden:

   * La primera columna debe mostrar el ID de usuario de Workfront (el GUID de usuario encontrado en Workfront).
   * La segunda columna debe contener el nombre de usuario de SSO, tal como se muestra en el sistema de SSO.
   * Las columnas no deben tener encabezados y no debe haber ninguna fila vacía en la parte superior de la lista de nombres.

     ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Guarde el informe como archivo CSV o TSV en el equipo.

## Actualizar los usuarios para SSO {#update-your-users-for-sso}

El proceso de actualización de usuarios para SSO añade el campo Nombre de usuario de SSO a los usuarios de Workfront si no hay ninguno presente, o actualiza el valor de ese campo si hay un valor ya asociado a los usuarios.

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Haga clic en, **Sistema** luego seleccione **Actualizar usuarios para SSO**.

1. Clic **Elegir archivo** para buscar el archivo que ha preparado.

   Para obtener más información sobre cómo preparar este archivo, consulte [Preparación del archivo de importación](#prepare-the-import-file).

1. Seleccione el archivo desde el que está guardado en el equipo y haga clic en **Abrir**.

   Esto inserta las credenciales de SSO en Workfront, lo que permite a todos los usuarios iniciar sesión en Workfront con sus credenciales de SSO.

   El **Solamente permitir `<SSO Configuration>` Autenticación** Esta opción está habilitada para todos los usuarios incluidos en el CSV. Esto garantiza que los usuarios deben iniciar sesión mediante SSO.

## Comprobación del SSO con los nombres de usuario de Workfront de los usuarios

Para obtener instrucciones sobre la creación de un informe de usuario que contenga información sobre el nombre de usuario SSO, consulte [Preparación del archivo de importación](#prepare-the-import-file).

1. Ejecute un informe de usuario que contenga información sobre el nombre de usuario de SSO.

   Observe que la columna Nombre de usuario SSO se rellena para cada usuario.

1. Asegúrese de que los valores de la columna Nombre de usuario SSO coinciden con el Nombre de usuario SSO del servidor SSO.
1. Si la columna Nombre de usuario SSO está en blanco, actualice los nombres de usuario SSO de los usuarios.

   ![](assets/users-with-sso-field-updated.png)

   Para obtener instrucciones sobre cómo actualizar los usuarios para SSO, consulte [Actualizar los usuarios para SSO](#update-your-users-for-sso).
