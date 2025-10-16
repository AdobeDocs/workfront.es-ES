---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilice Workfront Fusion para crear un proyecto de Workfront que tenga flujos de trabajo de Adobe Experience Manager
description: Si está creando un proyecto a través de Workfront Fusion y desea incluir flujos de trabajo de Adobe Experience Manager en el proyecto, debe utilizar una configuración de módulo de Fusion específica, que se describe en este artículo.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 6a21465ab8c92888c83344f33574302c5cc446e8
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 89%

---

# Utilizar Workfront Fusion para convertir un problema de Workfront en un proyecto que incluya flujos de trabajo de Adobe Experience Manager

Si está creando un proyecto a través de Workfront Fusion y desea incluir flujos de trabajo de Adobe Experience Manager en el proyecto, debe utilizar una configuración de módulo de Fusion específica, que se describe en este artículo.

>[!NOTE]
>
>Los flujos de trabajo solo están disponibles en una integración de Adobe Experience Manager as a Cloud Service. No están disponibles en integraciones con Adobe Experience Manager Assets Essentials.


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table>
  <tr>
    <td><strong>paquete de Adobe Workfront</strong></td>
   <td> <p>Cualquier paquete de flujo de trabajo de Adobe Workfront y cualquier paquete de integración y automatización de Adobe Workfront</p><p>Workfront Ultimate</p><p>Paquetes Workfront Prime y Select, con una compra adicional de Workfront Fusion.</p> </td> 
  </tr>
  <tr>
   <td><strong>Licencias de Adobe Workfront</strong></td>
   <td><p>Colaborador o superior</p><p>Solicitud o superior</p></td>
  </tr>
  <tr>
   <td><strong>Producto</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>Debe tener Experience Manager Assets as a Cloud Service o Assets Essentials, y debe estar añadido al producto como usuario en la Admin Console.</p>
       </li>
       <li>
        <p>Debe tener acceso de escritura al repositorio en Adobe Experience Manager.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <ul>
       <li>
        <p>Si su organización tiene un paquete Select o Prime Workfront que no incluye la automatización y la integración de Workfront, su organización debe adquirir Adobe Workfront Fusion.</li></ul>
       </li>
     </ul>
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso</strong>
   </td>
   <td><p>Acceso de edición a documentos</p>
   </td>
  </tr>
</table>

+++

## Requisitos previos

Antes de comenzar,

* El administrador de Workfront debe configurar los flujos de trabajo en una integración de Adobe Experience Manager. Para obtener más información, consulte [Configuración de la integración de Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Debe tener una plantilla de proyecto configurada con un flujo de trabajo de carpetas vinculadas de integración de Adobe Experience Manager.
* Debe haber creado una aplicación OAuth en Workfront para configurar la conexión de este módulo.

  Para obtener instrucciones, consulte [Crear una aplicación de OAuth](#create-an-oauth-application) en este artículo.

## Configuración del módulo

En Workfront Fusion, si desea crear un proyecto que incluya flujos de trabajo de Adobe Experience Manager, debe utilizar el módulo Workfront > Acciones diversas.

1. Añada el módulo **Workfront** > **Acciones diversas** a su escenario.
1. En el campo **Conexión**, seleccione la conexión de Workfront que se conecta a la cuenta que utilizará este módulo.

   Para obtener instrucciones sobre cómo crear una conexión, consulte [Conectar [!DNL Workfront] con [!DNL Workfront Fusion]](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) en el artículo Módulos de Workfront.

   Para obtener instrucciones sobre cómo crear el ID de cliente y el Secreto de cliente, deberá crear una conexión; consulte [Crear una aplicación de OAuth](#create-an-oauth-application) en este artículo.

1. En el campo **Tipo de registro**, seleccione `Issue`.
1. En el campo **Acción**, seleccione `convertToProject`.
1. En el campo **ID**, escriba o asigne el ID del problema que está convirtiendo en un proyecto.
1. Habilite **Mostrar ajustes avanzados**.
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

1. Reemplace `Folder tree ID here` por los identificadores de carpeta.

   Para localizar los identificadores del árbol de carpetas, consulte [Localizar los ID de árbol de carpetas](#locate-folder-tree-ids) en este artículo.

   Para utilizar más de un árbol de carpetas, separe los ID con una coma:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Reemplace `New project name here` por el nombre que tendrá el nuevo proyecto.
1. Reemplace `Template ID here` por el ID de la plantilla que usará para el nuevo proyecto.

   Puede asignar el ID de plantilla de un módulo anterior (como un módulo de Workfront > Buscar) o localizarlo en la dirección URL de la página de la plantilla de Workfront.

1. Haga clic en **Aceptar** para guardar la configuración del módulo.

## Localizar los ID de árbol de carpetas

Para localizar los ID de árbol de carpetas:

>[!NOTE]
>
>Estas instrucciones utilizan el explorador Chrome.

1. En Workfront, abra la plantilla que desee utilizar para este proyecto. Esta plantilla debe incluir la configuración de Adobe Experience Manager que desee utilizar para el proyecto.
1. Abra las herramientas para desarrolladores del explorador.
1. Abra la pestaña **Red** en las herramientas para desarrolladores.
1. En el cuadro **Filtro**, introduzca `object-workflow`.
1. En la columna Nombre, haga clic en el ID alfanumérico que aparece.

   ![Locating folder ID 1](assets/finding-folder-id-1.png)

1. Haga clic en la pestaña **Vista previa** a la derecha del ID alfanumérico.
1. Abra las siguientes secciones contraídas:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Cada árbol de carpetas está representado por un número. 0 (cero) representa la primera carpeta de la lista, 1 representa la segunda, y así sucesivamente. Si la plantilla incluye solo un árbol de carpetas, es el número 0.

1. Abra el árbol de carpetas que desee utilizar para el nuevo proyecto. Tome nota del valor del campo `_id`. Si desea usar más de un árbol de carpetas, anote todos los valores de campo `_id` para los árboles de carpetas que desee usar.

   ![Locating folder ID 2](assets/finding-folder-id-2.png)

   Estos son los valores de `aemNativeFolderTreeIDs` que introducirá en el campo **Proyecto (colección avanzada)** del módulo de Fusion **Workfront** > **Acciones diversas**.

## Crear una aplicación de OAuth

Debe configurar una aplicación de OAuth en Workfront para la conexión de este módulo. Solo debe hacerlo una vez para una conexión Workfront determinada en Fusion.

1. En Workfront, empiece a crear una aplicación de OAuth, tal como se describe en [Crear una aplicación de OAuth2 con credenciales de usuario (flujo de código de autorización)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) en el artículo Crear aplicaciones de OAuth2 para integraciones de [!DNL Workfront].
1. Copie el ID de cliente y el secreto de cliente en una ubicación segura.
1. En el campo **URI de redireccionamiento**, introduzca lo siguiente:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Haga clic en **Guardar**.

Utilizará este ID de cliente y este secreto de cliente al configurar la conexión del módulo en Fusion.

Para obtener instrucciones sobre cómo crear una conexión, consulte [Conectar [!DNL Workfront] con [!DNL Workfront Fusion]](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) en el artículo Módulos de Workfront.
