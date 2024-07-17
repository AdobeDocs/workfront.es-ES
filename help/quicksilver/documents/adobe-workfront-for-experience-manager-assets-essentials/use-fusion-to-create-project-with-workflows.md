---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilice Workfront Fusion para crear un proyecto de Workfront que tenga flujos de trabajo de Adobe Experience Manager
description: Si está creando un proyecto a través de Workfront Fusion y desea incluir flujos de trabajo de Adobe Experience Manager en el proyecto, debe utilizar una configuración de módulo de Fusion específica, que se describe en este artículo.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 012aa4c15bcdb26a3e30f8c143599a7e90c9a0f3
workflow-type: tm+mt
source-wordcount: '883'
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
    <td><strong>plan Adobe Workfront*</strong></td>
    <td>Cualquiera</td>
  </tr>
  <tr>
   <td><strong>Licencias de Adobe Workfront*</strong></td>
   <td>Solicitud o superior</td>
  </tr>
  <tr>
   <td><strong>Product</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>Debe tener Assets Essentials as a Cloud Service de Experience Manager Assets y se le debe agregar al producto como usuario en el Admin Console.</p>
       </li>
       <li>
        <p>Debe tener acceso de escritura al repositorio en Adobe Experience Manager.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <p>Nuevo:</p>
     <ul>
       <li>
         <p>Plan Select or Prime Workfront: su organización debe adquirir Adobe Workfront Fusion.</p>
       </li>
       <li> 
         <p>Plan Workfront definitivo: Workfront Fusion está incluido.</p>
       </li>
     </ul>
     <p>O</p>
     <p>Actual: Su organización debe adquirir Adobe Workfront Fusion.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso*</strong>
   </td>
   <td>Editar acceso a documentos
     <p>
       <strong>Nota: </strong>Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <strong>Crear o modificar niveles de acceso personalizados</strong>.
     </p>
   </td>
  </tr>
</table>

## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar los flujos de trabajo en una integración de Adobe Experience Manager. Para obtener más información, consulte [Configuración de la as a Cloud Service de Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Debe tener una plantilla de proyecto configurada con un flujo de trabajo de carpetas vinculadas de integración de Adobe Experience Manager.
* Debe haber creado una aplicación OAuth en Workfront para configurar la conexión de este módulo.

  Para obtener instrucciones, consulte [Crear una aplicación de OAuth](#create-an-oauth-application) en este artículo.

## Configuración del módulo

En Workfront Fusion, si desea crear un proyecto que incluya flujos de trabajo de Adobe Experience Manager, debe utilizar el módulo Workfront > Varias acciones.

1. Agregue el módulo **Workfront** > **Misc Action** a su escenario.
1. En el campo **Conexión**, seleccione la conexión de Workfront que se conecta a la cuenta que utilizará este módulo.

   Para obtener instrucciones sobre cómo crear una conexión, consulte [Conectar [!DNL Workfront] a [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) en el artículo Módulos de Workfront.

   Para obtener instrucciones sobre cómo crear el ID de cliente y el Secreto de cliente, deberá crear una conexión, consulte [Crear una aplicación de OAuth](#create-an-oauth-application) en este artículo.

1. En el campo **Tipo de registro**, seleccione `Issue`.
1. En el campo **Acción**, seleccione `convertToProject`.
1. En el campo **ID**, escriba o asigne el ID del problema que está convirtiendo en un proyecto.
1. Habilitar **Mostrar configuración avanzada**.
1. Desplácese hasta la parte inferior del módulo y busque el campo **Proyecto (colección avanzada)**.
1. Pegue el siguiente texto en el campo **Proyecto (colección avanzada)**.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Reemplazar `Folder tree ID here` por los identificadores de carpeta.

   Para localizar los identificadores del árbol de carpetas, consulte [Buscar identificadores del árbol de carpetas](#locate-folder-tree-ids) en este artículo.

   Para utilizar más de un árbol de carpetas, separe los ID con una coma:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Reemplazar `New project name here` con el nombre que tendrá el nuevo proyecto.
1. Reemplace `Template ID here` por el identificador de la plantilla que está usando para el nuevo proyecto.

   Puede asignar el ID de plantilla de un módulo anterior (como un módulo de Workfront > Buscar ) o localizarlo en la dirección URL de la página de la plantilla en Workfront.

1. Haga clic en **Aceptar** para guardar la configuración del módulo.

## Buscar ID de árbol de carpetas

Para localizar los ID del árbol de carpetas:

>[!NOTE]
>
>Estas instrucciones utilizan el explorador Chrome.

1. En Workfront, abra la plantilla que desee utilizar para este proyecto. Esta plantilla debe incluir la configuración de Adobe Experience Manager que desee utilizar para el proyecto.
1. Abra las herramientas para desarrolladores del explorador.
1. Abra la ficha **Red** en las herramientas para desarrolladores.
1. En el cuadro **Filtro**, escriba `object-workflow`.
1. En la columna Nombre, haga clic en el ID alfanumérico que aparece.

   ![Localizando ID de carpeta 1](assets/finding-folder-id-1.png)

1. Haga clic en la ficha **Vista previa** a la derecha del identificador alfanumérico.
1. Abra las siguientes secciones contraídas:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Cada árbol de carpetas está representado por un número. 0 (cero) representa la primera carpeta de la lista, 1 representa la segunda, y así sucesivamente. Si la plantilla incluye solo un árbol de carpetas, es el número 0.

1. Abra el árbol de carpetas que desee utilizar para el nuevo proyecto. Tome nota del valor del campo `_id`. Si desea usar más de un árbol de carpetas, anote todos los valores de campo de `_id` para los árboles de carpetas que desee usar.

   ![Localizando ID de carpeta 2](assets/finding-folder-id-2.png)

   Estos son los valores de `aemNativeFolderTreeIDs` que especificará en el campo **Proyecto (colección avanzada)** del módulo **Workfront** > **Acciones diversas** de Fusion.

## Creación de una aplicación de OAuth

Debe configurar una aplicación OAuth en Workfront para la conexión de este módulo. Solo debe hacerlo una vez para una conexión Workfront determinada en Fusion.

1. En Workfront, empiece a crear una aplicación OAuth, tal como se describe en [Crear una aplicación OAuth2 con credenciales de usuario (Flujo de código de autorización)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) en el artículo Crear aplicaciones OAuth2 para integraciones de [!DNL Workfront].
1. Copie el ID de cliente y el Secreto del cliente a una ubicación segura.
1. En el campo **URI de redireccionamiento**, escriba lo siguiente:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Haga clic en **Guardar**.

Utilizará este ID de cliente y este secreto de cliente al configurar la conexión del módulo en Fusion.

Para obtener instrucciones sobre cómo crear una conexión, consulte [Conectar [!DNL Workfront] a [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) en el artículo Módulos de Workfront.
