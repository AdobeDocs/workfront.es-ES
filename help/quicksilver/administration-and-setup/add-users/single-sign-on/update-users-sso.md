---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Actualización de usuarios para el inicio de sesión único
description: Puede actualizar usuarios para el inicio de sesión único en Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# Actualización de usuarios para el inicio de sesión único

{{important-admin-console-onboard}}

Cuando el inicio de sesión único (SSO) está habilitado en su instancia de Adobe Workfront, puede iniciar sesión en Workfront con sus credenciales de SSO.

Si tiene un sistema existente que ya está completado con usuarios asociados con credenciales de SSO, puede importar los ID de los usuarios en Workfront importando un archivo de valores separados por comas (CSV) en Workfront.

Para obtener más información sobre la integración de Workfront con un sistema SSO, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


## Requisitos de acceso

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Nombres de usuario de SSO

Según la solución de SSO que utilice, se puede llamar al nombre de usuario de su entorno de SSO a cualquiera de las siguientes opciones:

* Nombre de usuario de SSO
* Identificador de federación
* Nombre de usuario de federación

En Workfront, todos estos nombres se almacenan en el campo Nombre de usuario de SSO, en el objeto de usuario.

Para que los usuarios puedan utilizar sus credenciales de SSO para iniciar sesión en Workfront, debe actualizar su perfil para incluir su nombre de usuario de SSO, además de su nombre de usuario de Workfront.

Como administrador de Workfront, puede actualizar de forma masiva el campo Nombre de usuario de SSO para los usuarios de Workfront mediante una lista de nombres de usuario e importarlo en Workfront. Esta lista debe contener el ID de usuario de Workfront (GUID) así como el nombre de usuario de SSO correspondiente para cada usuario y debe guardarse como archivo CSV o TSV. Este proceso actualiza los nombres de usuario de SSO existentes en Workfront o añade un nuevo nombre de usuario de SSO si falta uno para los usuarios.

## Preparación del archivo de importación {#prepare-the-import-file}

Puede empezar a preparar el archivo de importación creando un informe de todos los usuarios de Workfront que deben actualizar sus campos de nombre de usuario de SSO.

1. Genere un informe de usuario en Workfront.

   Para obtener instrucciones sobre la creación de informes de usuario en Workfront, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Seleccione los campos siguientes en el informe:

   | Nombre | El nombre completo del usuario de Workfront. |
   |---|---|
   | Identificador | El ID es el GUID alfanumérico de Workfront. |
   | Nombre de usuario de SSO | Seleccione el campo Nombre de usuario de SSO para asegurarse de que no hay nombres de usuario que esté sobrescribiendo con la importación. Este campo debe estar en blanco para todos los usuarios si estos aún no se han actualizado para SSO. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Guarde el informe.
1. Haga clic en **Exportar** en la parte superior del informe y exporte el informe a Excel.
1. Abra el archivo de Excel exportado y empiece a agregar los nombres de usuario de SSO para cada usuario en el informe de la columna Nombre de usuario de SSO .

   >[!IMPORTANT]
   >
   >Los nombres de usuario de SSO distinguen entre mayúsculas y minúsculas.

1. Elimine todas las columnas del archivo de Excel, excepto la **ID** y **Nombre de usuario de SSO** columnas.

1. Elimine los encabezados de columna y asegúrese de que no haya filas en blanco en la parte superior del informe.

   El archivo que utiliza para actualizar los usuarios de Workfront con los nombres de usuario de SSO debe contener solo 2 columnas, en este orden:

   * La primera columna debe mostrar el ID de usuario de Workfront (el GUID de usuario que se encuentra en Workfront).
   * La segunda columna debe contener el nombre de usuario de SSO, tal como se muestra en el sistema SSO.
   * Las columnas no deben tener encabezados y no debe haber filas vacías en la parte superior de la lista de nombres.

      ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Guarde el informe como archivo CSV o TSV en el equipo.

## Actualizar los usuarios para SSO {#update-your-users-for-sso}

El proceso de actualización de usuarios para SSO añade el campo Nombre de usuario de SSO a los usuarios de Workfront si no está presente, o actualiza el valor de ese campo si ya hay un valor asociado a los usuarios.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** then **Actualizar usuarios para SSO**.

1. Haga clic en **Elegir archivo** para buscar el archivo que ha preparado.

   Para obtener más información sobre cómo preparar este archivo, consulte [Preparación del archivo de importación](#prepare-the-import-file).

1. Seleccione el archivo donde está guardado en el equipo y haga clic en **Apertura**.

   Esto permite a todos los usuarios iniciar sesión en Workfront con sus credenciales de SSO.

   La variable **Permitir sólo `<SSO Configuration>` Autenticación** está habilitado para todos los usuarios incluidos en el CSV.

## Verificar SSO de los nombres de usuario de Workfront de los usuarios

Para obtener instrucciones sobre la creación de un informe de usuario que contenga información sobre el nombre de usuario de SSO, consulte [Preparación del archivo de importación](#prepare-the-import-file).

1. Ejecute un informe de usuario que contenga información sobre el nombre de usuario de SSO.

   Observe que la columna Nombre de usuario de SSO se rellena para cada usuario.

1. Asegúrese de que los valores de la columna Nombre de usuario de SSO coinciden con el nombre de usuario de SSO de su servidor SSO.
1. Si la columna Nombre de usuario de SSO está en blanco, actualice los nombres de usuario de SSO de los usuarios.

   ![](assets/users-with-sso-field-updated.png)

   Para obtener instrucciones sobre cómo actualizar los usuarios para SSO, consulte [Actualizar los usuarios para SSO](#update-your-users-for-sso).
