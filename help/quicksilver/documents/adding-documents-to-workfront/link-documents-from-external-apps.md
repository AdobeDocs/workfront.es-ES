---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Vincular documentos de aplicaciones externas
description: 'Puede vincular documentos y carpetas a Adobe Workfront desde las siguientes fuentes: EDIT ME.'
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: 0ecee45183f5bc77a1c4a489013e486d8c26094c
workflow-type: tm+mt
source-wordcount: '2586'
ht-degree: 0%

---

# Vincular documentos de aplicaciones externas

Puede vincular documentos y carpetas a Adobe Workfront desde las siguientes fuentes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Proveedores de documentos de nube de terceros existentes</td> 
   <td>Entre ellas se incluyen las siguientes: 
    <ul> 
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Empresa Dropbox</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Revisión de Workfront </td> 
   <td>Puede hacer que las pruebas que se crearon originalmente en Workfront Proof estén disponibles en Workfront. Para utilizar esta función se necesita un plan Pro Workfront o superior. Para obtener más información sobre los distintos planes disponibles, consulte <a href="https://www.workfront.com/plans">Planes de Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>Puede vincular documentos a Workfront desde Experience Manager Assets Essentials. Para obtener más información, consulte <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> Adobe Workfront para Experience Manager Assets Essentials</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront DAM </td> 
   <td>Esto requiere una compra adicional. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Otros proveedores de documentos (a través de integraciones de documentos personalizadas)</td> 
   <td> <p class="workfront_plans">Para utilizar esta función se necesita un plan Pro Workfront o superior. Para obtener más información sobre los distintos planes disponibles, consulte <a href="https://www.workfront.com/plans">Planes de Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Antes de vincular documentos o carpetas, el administrador de Workfront debe habilitar esta funcionalidad para cada proveedor de documentos o para una integración de documentos personalizada, tal como se describe en [Configurar integraciones de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

Puede probar y aprobar documentos vinculados a un proveedor de nube externo del mismo modo que lo hace con documentos cargados directamente en Workfront. 

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Almacenamiento de documentos

Los documentos vinculados a Workfront desde una aplicación externa se almacenan con el proveedor de nube externo, no dentro de Workfront.

Se aplican las siguientes excepciones:

* Cuando el servicio de documentos lo proporciona, las miniaturas y las imágenes de vista previa pueden almacenarse en servidores de Workfront.
* Cuando se utilizan pruebas en Workfront, el documento se copia y se agrega a los servidores de pruebas. 

## Vinculación de un documento desde una aplicación externa a Workfront

Puede vincular documentos existentes con un proveedor de nube externo. Esto incluye cualquier documento compartido.

* [Requisitos previos](#prerequisites)
* [Vinculación de un documento externo a Workfront](#link-an-external-document-to-workfront)
* [Añadir una nueva versión de un documento vinculado](#add-a-new-version-of-a-linked-document)
* [Vincular documentos de prueba de Workfront](#link-workfront-proof-documents)
* [Crear un documento de Google desde Workfront](#create-a-google-document-from-within-workfront)

### Requisitos previos {#prerequisites}

Antes de vincular documentos o carpetas, el administrador de Workfront debe habilitar esta funcionalidad para cada proveedor de documentos o para una integración de documentos personalizada, tal como se describe en [Configurar integraciones de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### Vinculación de un documento externo a Workfront {#link-an-external-document-to-workfront}

Puede vincular documentos a Workfront desde una aplicación externa como Google y Microsoft OneDrive.

>[!IMPORTANT]
>
>El Dropbox almacena los documentos en función de la ruta del archivo. Por este motivo, si un archivo vinculado desde un Dropbox se mueve, se cambia el nombre o se elimina, se vuelve inaccesible en Workfront.

1. Vaya a la **Documentos** en Workfront donde desee el documento.
1. Haga clic en **Agregar nuevo** y, a continuación, haga clic en el proveedor de documentos externo donde desea vincular documentos a Workfront.

   Por ejemplo, para vincular documentos del Dropbox, haga clic en **De Dropbox**.

   Los proveedores externos que ya ha autorizado aparecen en la parte superior de la lista.

1. (Condicional) Si se le solicita que inicie sesión en el servicio externo, escriba sus credenciales de inicio de sesión para el servicio en el cuadro que aparece y haga clic en **Iniciar sesión**.
1. (Condicional) Si se le solicita que autorice la aplicación externa, haga clic en el botón **Autorizar** botón.

   Solo tiene que hacerlo una vez.

1. En el cuadro de búsqueda de la variable **Vincular archivos y carpetas externos** que aparece, escriba el nombre del elemento que desea buscar y presione **Entrar** para ver todos los resultados de la aplicación externa, independientemente de la carpeta en la que se almacenen.

   O

   Busque y seleccione los documentos que desea vincular.

   Aunque puede seleccionar varios documentos, solo los documentos seleccionados en la vista actual están vinculados. Por ejemplo, si selecciona un documento y luego entra en una carpeta, el documento que seleccionó originalmente no está vinculado.

1. (Condicional) Si es cliente de Workfront DAM, haga clic en el **Miniatura** para mostrar los archivos como imágenes en miniatura.

   >[!NOTE]
   Los clientes de Workfront DAM pueden ver miniaturas al vincular documentos desde Workfront DAM. También se pueden mostrar miniaturas para clientes de Workfront DAM para otros servicios como Dropbox y Caja. Sin embargo, no se admite la visualización de miniaturas de servicios que no sean Workfront DAM en Workfront, y las miniaturas nunca se muestran al vincular documentos desde SharePoint o Google Drive.

1. Haga clic en **Vínculo**.

   En Workfront, el icono del proveedor de la nube aparece junto a los documentos.

   >[!NOTE]
   Para los documentos vinculados a Cuadro, el vínculo al documento en Cuadro no se muestra hasta que se actualiza la página.

### Añadir una nueva versión de un documento vinculado {#add-a-new-version-of-a-linked-document}

Puede añadir una nueva versión de un documento vinculado a Workfront desde una aplicación externa.

1. Vaya a la **Documentos** área en la que está vinculado el documento, seleccione el documento vinculado.

   >[!IMPORTANT]
   El documento debe estar fuera de una carpeta vinculada para crear una nueva versión.

1. Haga clic en **Agregar nuevo** > **Versión** y, a continuación, haga clic en el proveedor de documentos externo.

   Por ejemplo, para vincular una nueva versión de un documento desde el Dropbox, haga clic en **De Dropbox**.

   Los proveedores externos que ya ha autorizado aparecen en la parte superior de la lista.

1. (Condicional) Si se le solicita que inicie sesión en el servicio externo, escriba sus credenciales de inicio de sesión para el servicio en el cuadro que aparece y haga clic en **Iniciar sesión**.
1. (Condicional) Si se le solicita que autorice la aplicación externa, haga clic en **Autorizar**.

   Solo tiene que hacerlo una vez.

1. En el cuadro de búsqueda de la variable **Vincular archivos y carpetas externos** que aparece, escriba el nombre del elemento que desea buscar y presione **Entrar** para ver todos los resultados de la aplicación externa, independientemente de la carpeta en la que se almacenen.

   O

   Busque y seleccione los documentos que desea vincular.

   Puede seleccionar varios documentos; sin embargo, solo los documentos seleccionados en la vista actual están vinculados. Por ejemplo, si selecciona un documento y luego entra en una carpeta, el documento que seleccionó originalmente no está vinculado.

1. (Condicional) Si es cliente de Workfront DAM, haga clic en el **Miniatura** para mostrar los archivos como imágenes en miniatura.

   >[!NOTE]
   Los clientes de Workfront DAM pueden ver miniaturas al vincular documentos desde Workfront DAM. También se pueden mostrar miniaturas para clientes de Workfront DAM para otros servicios como Dropbox y Caja. Sin embargo, no se admite la visualización de miniaturas de servicios que no sean Workfront DAM en Workfront, y las miniaturas nunca se muestran al vincular documentos desde SharePoint o Google Drive.

1. Haga clic en **Vínculo**.

   En Workfront, el icono del proveedor de la nube aparece junto a los documentos, indicando que están vinculados al proveedor de la nube externa.

   >[!NOTE]
   Para los documentos vinculados a Cuadro, el vínculo al documento en Cuadro no se muestra hasta que se actualiza la página.

Para obtener información sobre cómo agregar una nueva versión de un documento que ha cargado en Workfront desde el sistema de archivos, consulte [Agregar documentos a Adobe Workfront desde el sistema de archivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#adding-new-versions-of-documents) en [Agregar documentos a Adobe Workfront desde el sistema de archivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Vincular documentos de prueba de Workfront {#link-workfront-proof-documents}

Puede vincular pruebas a Workfront que existían originalmente en Workfront Proof. Al vincular una prueba desde Workfront Proof, todos los comentarios y otros metadatos asociados con la prueba están disponibles en Workfront. 

Solo puede vincular las pruebas para las que tiene acceso a Vista en Workfront Proof.

1. Vaya a la **Documentos** en Workfront donde desee el documento.
1. Haga clic en **Agregar nuevo** y haga clic en **De la prueba de Workfront**.

   >[!NOTE]
   Las opciones de este menú pueden variar en función de los proveedores de terceros configurados en su entorno.

1. En el **Vínculo** pruebas **from** Workfront Proof que aparece, empiece a escribir el nombre de la prueba que desea poner a disposición en Workfront.

   La lista se filtra a medida que escribe.

1. Seleccione hasta 10 pruebas para vincular.

   Cualquier nombre de prueba atenuado no está disponible para vincularse, ya que la prueba ya está asociada a un documento en Workfront.

1. Haga clic en **Vínculo**.

   La versión más actual de la prueba está vinculada a Workfront. Al abrir la prueba, todas las versiones están disponibles en el visor de pruebas.

### Crear un documento de Google desde Workfront {#create-a-google-document-from-within-workfront}

Puede crear un nuevo documento de Google desde Workfront. No puede crear nuevos documentos desde Workfront para otros proveedores de la nube.

1. Vaya a la **Documentos** en Workfront donde desee el documento.
1. Haga clic en **Agregar nuevo** > **Archivo Google** y, a continuación, seleccione el tipo de documento de Google que desea crear.

1. Seleccione el tipo de documento de Google que desea crear.
1. Si la variable **Agregar cuenta de unidad de Google** , haga clic en **Autorizar la unidad de Google**.

   Se agrega un documento de Google al **Documentos** pestaña .

   >[!NOTE]
    My Drive y Shared with Me muestran dos resultados diferentes. Si no puede encontrar un archivo en Mi unidad, marque la carpeta Compartido conmigo .

## Actualizar y vincular un documento de Workfront a un proveedor de nube externo

Puede cargar y vincular un documento de Workfront a un proveedor de nube externo. Esto mueve el almacenamiento del documento de Workfront al proveedor de nube externo. Cuando el documento se cambia en la aplicación externa, se actualiza automáticamente en Workfront.

Los usuarios sin acceso a Workfront pueden ver el documento en la aplicación externa si tienen acceso a la aplicación.

1. Seleccione un documento que se haya cargado en Workfront.
1. Haga clic en **Más** >**Enviar a** y, a continuación, seleccione el proveedor de nube que desea almacenar en el documento vinculado.

   También puede utilizar el menú Más ![](assets/more-icon.png) en la página Detalles del documento para hacerlo.

1. Seleccione la carpeta en la aplicación del proveedor donde desea almacenar el documento.

   Puede ser cualquier carpeta de la aplicación del proveedor, incluida una carpeta compartida.

1. Haga clic en **Guardar**.

   El logotipo del proveedor externo aparece junto al nombre del documento para indicar que el documento está ahora vinculado a Workfront y almacenado por el proveedor externo de la nube.

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## Vincular carpetas

Al vincular una carpeta entre Workfront y un proveedor de nube externo, la carpeta y todo su contenido se vinculan. Si los usuarios sin acceso a Workfront agregan, eliminan y modifican archivos de la aplicación de documentos externa, sus cambios se sincronizan con Workfront. Las secciones siguientes describen cómo vincular carpetas y subcarpetas:

* [Derechos de acceso a carpetas](#folder-access-rights)
* [Vincular una o más carpetas externas](#link-one-or-more-external-folders)
* [Añadir subcarpetas a una carpeta vinculada](#add-subfolders-to-a-linked-folder)

### Derechos de acceso a carpetas {#folder-access-rights}

Al sincronizar el contenido de una carpeta desde una aplicación de documento externa, Workfront utiliza las credenciales del usuario que vinculó originalmente la carpeta. Esto resulta en la siguiente experiencia de usuario:

* Si los usuarios no tienen acceso para ver archivos y carpetas en la aplicación externa, pero sí tienen acceso para ver la carpeta vinculada a través de Workfront, solo pueden ver los nombres de los archivos y carpetas en Workfront, no su contenido.
* Cuando alguien accede al contenido de una carpeta vinculada de Workfront (como una subcarpeta de una carpeta vinculada) vinculada a Workfront por otro usuario, el contenido se sincroniza con Workfront mediante las credenciales de inicio de sesión de Workfront del usuario que vinculó originalmente la carpeta, no las credenciales del usuario que accede al contenido.

>[!IMPORTANT]
* Si el usuario que vinculó originalmente la carpeta se elimina del sistema Workfront, los usuarios ya no podrán acceder al contenido de la carpeta vinculada a través de Workfront. En este caso, la carpeta debe volver a vincularla un usuario de Workfront activo que tenga derechos sobre la carpeta en la aplicación externa.
* Si el usuario que vinculó una carpeta ya no tiene acceso a la aplicación externa, Workfront ya no puede acceder al contenido de la carpeta. Esto puede suceder, por ejemplo, si el usuario que vinculó originalmente la carpeta abandona la empresa. Para garantizar un acceso continuado, un usuario con acceso a la carpeta debe volver a vincular la carpeta.


### Vincular una o más carpetas externas {#link-one-or-more-external-folders}

1. Vaya al área de Workfront donde desee la carpeta y haga clic en  **Documentos** ![](assets/document-icon.png) en el panel izquierdo .

1. Haga clic en **Agregar nuevo** y, a continuación, haga clic en el proveedor de documentos externo desde el que desea vincular una carpeta a Workfront.
1. (Condicional) Si aún no ha autorizado el servicio externo, especifique sus credenciales de inicio de sesión para el proveedor externo y haga clic en **Iniciar sesión**.

   Los proveedores externos que ya ha autorizado aparecen en la parte superior de la lista.

1. En el **Vincular archivos y carpetas externos** que aparece, busque y seleccione las carpetas que desee vincular.

   O

   Escriba el nombre de la carpeta que desea buscar y presione **Entrar**.

   Puede seleccionar varias carpetas; sin embargo, solo las carpetas seleccionadas en la vista actual están vinculadas. Por ejemplo, si selecciona una carpeta y, a continuación, entra en una carpeta, la carpeta seleccionada originalmente no está vinculada.

   >[!NOTE]
   Al vincular carpetas desde Google Drive, solo puede vincular carpetas que estén dentro de su unidad personal (My Drive) y Team Drive. No puede vincular carpetas desde el área Compartido conmigo .

1. Haga clic en **Vínculo**.

   En Workfront, el logotipo del proveedor de la nube aparece junto a la carpeta, lo que indica que está vinculado al proveedor de la nube externa.

1. (Opcional) Para cambiar el nombre de la carpeta de forma que el nombre de la carpeta en Workfront sea diferente del nombre de la carpeta en la aplicación de documento externa, seleccione la carpeta en la **Carpetas** , haga clic en el menú Más ![](assets/more-icon.png)  que aparece junto al nombre de la carpeta y, a continuación, haga clic en **Cambiar nombre**.

   ![](assets/documents-folderlink-rename-nwe-350x154.png)

Esto no cambia el nombre de la carpeta en la aplicación externa.

### Añadir subcarpetas a una carpeta vinculada  {#add-subfolders-to-a-linked-folder}

Puede crear una carpeta nueva dentro de una carpeta vinculada existente. También puede arrastrar otra carpeta a una carpeta vinculada existente.

1. Para crear una nueva carpeta dentro de una carpeta vinculada existente, vaya a la carpeta existente y, a continuación, cree la nueva carpeta tal como se describe en [Crear carpetas de documentos](../../documents/organizing-documents/create-documents-folder.md).

   O

   Para arrastrar una carpeta existente a una carpeta vinculada existente, vaya al área Documentos donde desee la subcarpeta y arrástrela a la carpeta vinculada.

   ![](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   Las siguientes limitaciones se aplican al arrastrar una carpeta de Workfront existente a una carpeta vinculada:
   * La carpeta que está arrastrando no se puede vincular y no puede contener ningún contenido que ya esté vinculado.
   * La carpeta (incluido su contenido) que está arrastrando no puede superar los 50 MB.


## Añadir un documento a una carpeta vinculada

Al añadir un documento a una carpeta vinculada a través de Workfront, se añade automáticamente como documento vinculado.

1. En el **Documentos** área donde desee el documento, arrástrelo a una carpeta vinculada.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode"> <img src="assets/documents-linked-document-move-nwe-350x126.png" style="width: 350;height: 126;">Selection box is wonky on the left<br></p>
   -->

   O

   Seleccione la carpeta vinculada en la que desea el documento y haga clic en **Agregar nuevo > Documento** y, a continuación, busque el documento y agréguelo a la carpeta .

   Se crea automáticamente una nueva versión del documento en la aplicación externa y se vincula a Workfront.

## Eliminar un documento o una carpeta vinculados

Cuando se elimina un documento o carpeta vinculado de la aplicación externa, el documento o la carpeta permanecen en el sistema Workfront hasta que también se elimina de Workfront.

1. Seleccione el documento o la carpeta vinculados y haga clic en **Eliminar**.
1. En el cuadro de confirmación que aparece, haga clic en **Sí, desvincúlelo**.

   El documento se desvincula del sitio de Workfront. No se ve afectado en la aplicación externa.

## Acerca del cambio del nombre de documentos y carpetas vinculados

Al cambiar el nombre de un documento o carpeta vinculado, el cambio solo está visible en la aplicación en la que lo hace. Por ejemplo, si cambia el nombre de un documento vinculado en Workfront, el nuevo nombre solo será visible en Workfront.

Si desea que el nombre coincida en Workfront y en la aplicación externa, debe cambiarlo de nombre en ambos lugares.

>[!IMPORTANT]
No cambie el nombre de un documento en Workfront vinculado a un Dropbox; al hacerlo, el archivo en Workfront es inaccesible. En su lugar, cambie el nombre del archivo en el Dropbox y vuelva a sincronizar el archivo, tal como se describe en [Vincular documentos de aplicaciones externas](#synchronizing-changes-made-on-a-linked-document).
