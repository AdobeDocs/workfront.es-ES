---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilice Workfront Fusion para crear un proyecto de Workfront que tenga flujos de trabajo de Adobe Experience Manager
description: Si está creando un proyecto a través de Workfront Fusion y desea incluir flujos de trabajo de Adobe Experience Manager en el proyecto, debe utilizar una configuración de módulo de Fusion específica, que se describe en este artículo.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
source-git-commit: df8f99da107f50eb1302188aa544f45b7b451966
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Utilice Workfront Fusion para convertir un problema de Workfront en un proyecto que incluya flujos de trabajo de Adobe Experience Manager

Si está creando un proyecto a través de Workfront Fusion y desea incluir flujos de trabajo de Adobe Experience Manager en el proyecto, debe utilizar una configuración de módulo de Fusion específica, que se describe en este artículo.

>[!NOTE]
>
>Los flujos de trabajo solo están disponibles en una integración de Adobe Experience Manager as a Cloud Service. No están disponibles en integraciones con Adobe Experience Manager Assets Essentials.


## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>plan Adobe Workfront*</strong>
   </td>
   <td>Cualquiera
   </td>
  </tr>
  <tr>
   <td><strong>Licencias de Adobe Workfront*</strong>
   </td>
   <td>Solicitud o superior
   </td>
  </tr>
  <tr>
   <td><strong>Product</strong>
   </td>
   <td><b>Adobe Experience Manager<b>:<ul><li><p>Debe tener Experience Manager Assets as a Cloud Service o Assets Essentials, y se le debe añadir al producto como usuario en el Admin Console.</p></li><li><p>Debe tener acceso de escritura al repositorio en Adobe Experience Manager.</p></li></ul>
  <b>Workfront Fusion</b>:<p>Nuevo:</p> <ul><li>[!UICONTROL Seleccionar] o [!UICONTROL Prime] [!DNL Workfront] Plan: su organización debe comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] está incluido.</li></ul>   <p>O</p>
   <p>Actual: Su organización debe comprar [!DNL Adobe Workfront Fusion].</p>
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso*</strong>
   </td>
   <td>Editar acceso a documentos
<p>
<strong>Nota: </strong>Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <strong>Crear o modificar niveles de acceso personalizados</strong>.
   </td>
  </tr>
</table>

## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar los flujos de trabajo en una integración de Adobe Experience Manager. Para obtener más información, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Debe tener una plantilla de proyecto configurada con un flujo de trabajo de carpetas vinculadas de integración de Adobe Experience Manager.
* Debe haber creado una aplicación OAuth en Workfront para configurar la conexión de este módulo.

  Para obtener instrucciones, consulte [Creación de una aplicación de OAuth](#create-an-oauth-application) en este artículo.

## Configuración del módulo

En Workfront Fusion, si desea crear un proyecto que incluya flujos de trabajo de Adobe Experience Manager, debe utilizar el módulo Workfront > Varias acciones.

1. Añada el **Workfront** > **Misc Action** a su escenario.
1. En el **Conexión** , seleccione la conexión de Workfront que se conecta a la cuenta que utilizará este módulo.

   Para obtener instrucciones sobre cómo crear una conexión, consulte [Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) en el artículo Módulos de Workfront.

   Para obtener instrucciones sobre cómo crear el ID de cliente y el Secreto de cliente, deberá crear una conexión, consulte [Creación de una aplicación de OAuth](#create-an-oauth-application) en este artículo.

1. En el **Tipo de registro** , seleccione `Issue`.
1. En el **Acción** , seleccione `convertToProject`.
1. En el **ID** , introduzca o asigne el ID del problema que está convirtiendo en un proyecto.
1. Activar **Mostrar configuración avanzada**.
1. Desplácese hasta la parte inferior del módulo y busque **Proyecto (colección avanzada)** field.
1. Pegue el siguiente texto en la **Proyecto (colección avanzada)** field.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Reemplazar `Folder tree ID here` con los ID de carpeta.

   Para localizar los ID del árbol de carpetas, consulte [Buscar ID de árbol de carpetas](#locate-folder-tree-ids) en este artículo.

   Para utilizar más de un árbol de carpetas, separe los ID con una coma:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Reemplazar `New project name here` con el nombre que tendrá el nuevo proyecto.
1. Reemplazar `Template ID here` con el ID de la plantilla que está utilizando para el nuevo proyecto.

   Puede asignar el ID de plantilla de un módulo anterior (como un módulo de Workfront > Buscar ) o localizarlo en la dirección URL de la página de la plantilla en Workfront.

1. Clic **OK** para guardar la configuración del módulo.

## Buscar ID de árbol de carpetas

Para localizar los ID del árbol de carpetas:

>[!NOTE]
>
>Estas instrucciones utilizan el explorador Chrome.

1. En Workfront, abra la plantilla que desee utilizar para este proyecto. Esta plantilla debe incluir la configuración de Adobe Experience Manager que desee utilizar para el proyecto.
1. Abra las herramientas para desarrolladores del explorador.
1. Abra el **Red** en las herramientas para desarrolladores.
1. En el **Filtrar** , escriba `object-workflow`.
1. En la columna Nombre, haga clic en el ID alfanumérico que aparece.

   ![Localizando ID de carpeta 1](assets/finding-folder-id-1.png)

1. Haga clic en **Previsualizar** a la derecha del ID alfanumérico.
1. Abra las siguientes secciones contraídas:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Cada árbol de carpetas está representado por un número. 0 (cero) representa la primera carpeta de la lista, 1 representa la segunda, y así sucesivamente. Si la plantilla incluye solo un árbol de carpetas, es el número 0.

1. Abra el árbol de carpetas que desee utilizar para el nuevo proyecto. Tome nota de la `_id` valor de campo. Si desea utilizar más de un árbol de carpetas, anote todos los `_id` valores de campo para los árboles de carpetas que desea utilizar.

   ![Localizando ID de carpeta 2](assets/finding-folder-id-2.png)

   Estas son las `aemNativeFolderTreeIDs`  valores que introducirá en la variable **Proyecto (colección avanzada)** en el campo **Workfront** > **Acciones diversas** Módulo Fusion.

## Creación de una aplicación de OAuth

Debe configurar una aplicación OAuth en Workfront para la conexión de este módulo. Solo debe hacerlo una vez para una conexión Workfront determinada en Fusion.

1. En Workfront, empiece a crear una aplicación OAuth como se describe en [Crear una aplicación OAuth2 con credenciales de usuario (flujo de código de autorización)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) en el artículo Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones.
1. Copie el ID de cliente y el Secreto del cliente a una ubicación segura.
1. En el **URI de redireccionamiento** , introduzca lo siguiente:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Haga clic en **Guardar**.

Utilizará este ID de cliente y este secreto de cliente al configurar la conexión del módulo en Fusion.

Para obtener instrucciones sobre cómo crear una conexión, consulte [Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) en el artículo Módulos de Workfront.

