---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Vinculación de documentos desde aplicaciones externas
description: Puede vincular documentos y carpetas a Adobe Workfront desde fuentes externas.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: fde2ad9a8ef1b7f659f8f52c157726d0562b972a
workflow-type: tm+mt
source-wordcount: '2608'
ht-degree: 0%

---

# Vinculación de documentos desde aplicaciones externas

<!-- Audited: 01/2024 -->

Puede vincular documentos y carpetas a Adobe Workfront desde las siguientes fuentes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Proveedores de documentos de nube de terceros existentes</td> 
   <td>Entre ellos se incluyen los siguientes: 
    <ul> 
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Dropbox Empresa</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
     <li>Quip</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Revisión de Workfront </td> 
   <td>Puede hacer que las pruebas creadas originalmente en Workfront Proof estén disponibles en Workfront. Para las licencias actuales, se requiere un plan Pro Workfront o superior para utilizar esta función. Para las nuevas licencias, todos los planes incluyen esta función. Para obtener más información sobre los diversos planes disponibles, consulte <a href="https://www.workfront.com/plans">Planes de Workfront</a>.</td> 
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
   <td role="rowheader">Otros proveedores de documentos (mediante integraciones de documentos personalizadas)</td> 
   <td> <p class="workfront_plans">Para las licencias actuales, se requiere un plan Pro Workfront o superior para utilizar esta función. Para las nuevas licencias, todos los planes incluyen esta función. Para obtener más información sobre los diversos planes disponibles, consulte <a href="https://www.workfront.com/plans">Planes de Workfront</a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Antes de vincular documentos o carpetas, el administrador de Workfront debe habilitar esta funcionalidad para cada proveedor de documentos o para una integración de documentos personalizada, tal como se describe en [Configurar integraciones de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

Puede probar y aprobar documentos vinculados a un proveedor de nube externo del mismo modo que lo hace con documentos cargados directamente en Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td>
   <td> <p> Cualquiera</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td>
   <td><p>Nuevo: Colaborador o superior</p>
    <p>o</p>
    <p>Actual: Solicitud o superior</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Almacenamiento de documentos

Los documentos vinculados a Workfront desde una aplicación externa se almacenan con el proveedor de la nube externo, no en Workfront.

Se aplican las siguientes excepciones:

* Cuando lo proporciona el servicio de documentos, las miniaturas y las imágenes de vista previa se pueden almacenar en servidores de Workfront.
* Al utilizar la revisión en Workfront, el documento se copia y se agrega a los servidores de revisión.

## Vinculación de un documento de una aplicación externa a Workfront

Puede vincular documentos existentes con un proveedor de nube externo. Esto incluye cualquier documento compartido.

### Requisitos previos {#prerequisites}

Antes de vincular documentos o carpetas, el administrador de Workfront debe habilitar esta funcionalidad para cada proveedor de documentos o para una integración de documentos personalizada, tal como se describe en [Configurar integraciones de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### Vinculación de un documento externo a Workfront {#link-an-external-document-to-workfront}

Puede vincular documentos a Workfront desde una aplicación externa como Google y Microsoft OneDrive.

>[!IMPORTANT]
>
>El Dropbox almacena los documentos en función de la ruta de acceso del archivo. Debido a esto, si se mueve, se cambia el nombre o se elimina un archivo vinculado desde el Dropbox, no se puede acceder a él en Workfront.

1. Vaya al área de **Documentos** de Workfront donde desee colocar el documento.
1. Haga clic en **Agregar nuevo** y, a continuación, haga clic en el proveedor de documentos externo donde desee vincular documentos a Workfront.

   Por ejemplo, para vincular documentos desde el Dropbox, haga clic en **Desde el Dropbox**.

   Los proveedores externos que ya ha autorizado aparecen en la parte superior de la lista.

1. (Condicional) Si se le pide que inicie sesión en el servicio externo, escriba sus credenciales de inicio de sesión para el servicio en el cuadro que aparece y, a continuación, haga clic en **Iniciar sesión**.
1. (Condicional) Si se le pide que autorice la aplicación externa, haga clic en el botón **Autorizar**.

   Tienes que hacer esto solo una vez.

1. En el cuadro de búsqueda del cuadro **Vincular archivos y carpetas externos** que aparece, escriba el nombre del elemento que desea buscar y, a continuación, presione **Entrar** para ver todos los resultados de la aplicación externa, independientemente de la carpeta en la que se almacenen.

   O

   Busque y seleccione los documentos que desea vincular.

   Aunque puede seleccionar varios documentos, sólo se vinculan los documentos seleccionados en la vista actual. Por ejemplo, si selecciona un documento y luego va a una carpeta, el documento seleccionado originalmente no está vinculado.

1. (Condicional) Si es cliente de Workfront DAM, haga clic en el icono **Miniatura** para mostrar los archivos como imágenes en miniatura.

   >[!NOTE]
   >
   >Los clientes de Workfront DAM pueden ver miniaturas al vincular documentos desde Workfront DAM. Las miniaturas también se pueden mostrar para los clientes de Workfront DAM para otros servicios como Dropbox y Box. Sin embargo, no se admite la visualización de miniaturas para servicios que no sean Workfront DAM en Workfront, y las miniaturas nunca se muestran al vincular documentos desde SharePoint o Google Drive.

1. Haga clic en **Vínculo**.

   En Workfront, el icono del proveedor de la nube aparece junto a los documentos.

   >[!NOTE]
   >
   >* Si la dirección URL de descarga utilizada para vincular el documento supera los 2048 caracteres, el archivo no se puede vincular.
   >* En el caso de los documentos vinculados a Box, el vínculo al documento en Box no se muestra hasta que se actualiza la página.

### Agregar una nueva versión de un documento vinculado {#add-a-new-version-of-a-linked-document}

Puede añadir una nueva versión de un documento vinculado a Workfront desde una aplicación externa.

1. Vaya al área de **Documentos** donde está vinculado el documento y, a continuación, seleccione el documento vinculado.

   >[!IMPORTANT]
   >
   >El documento debe estar fuera de una carpeta vinculada para crear una nueva versión.

1. Haga clic en **Agregar nuevo** > **Versión** y, a continuación, haga clic en el proveedor de documentos externo.

   Por ejemplo, para vincular una nueva versión de un documento desde el Dropbox, haga clic en **Desde el Dropbox**.

   Los proveedores externos que ya ha autorizado aparecen en la parte superior de la lista.

1. (Condicional) Si se le pide que inicie sesión en el servicio externo, escriba sus credenciales de inicio de sesión para el servicio en el cuadro que aparece y, a continuación, haga clic en **Iniciar sesión**.
1. (Condicional) Si se le pide que autorice la aplicación externa, haga clic en **Autorizar**.

   Tienes que hacer esto solo una vez.

1. En el cuadro de búsqueda del cuadro **Vincular archivos y carpetas externos** que aparece, escriba el nombre del elemento que desea buscar y, a continuación, presione **Entrar** para ver todos los resultados de la aplicación externa, independientemente de la carpeta en la que estén almacenados.

   O

   Busque y seleccione los documentos que desea vincular.

   Puede seleccionar varios documentos; sin embargo, sólo se vinculan los documentos seleccionados en la vista actual. Por ejemplo, si selecciona un documento y luego va a una carpeta, el documento seleccionado originalmente no está vinculado.

1. (Condicional) Si es cliente de Workfront DAM, haga clic en el icono **Miniatura** para mostrar los archivos como imágenes en miniatura.

   >[!NOTE]
   >
   >Los clientes de Workfront DAM pueden ver miniaturas al vincular documentos desde Workfront DAM. Las miniaturas también se pueden mostrar para los clientes de Workfront DAM para otros servicios como Dropbox y Box. Sin embargo, no se admite la visualización de miniaturas para servicios que no sean Workfront DAM en Workfront, y las miniaturas nunca se muestran al vincular documentos desde SharePoint o Google Drive.

1. Haga clic en **Vínculo**.

   En Workfront, el icono del proveedor de la nube aparece junto a los documentos, lo que indica que están vinculados al proveedor de la nube externo.

   >[!NOTE]
   >
   >En el caso de los documentos vinculados a Box, el vínculo al documento en Box no se muestra hasta que se actualiza la página.

Para obtener información sobre cómo agregar una nueva versión de un documento que ha subido a Workfront desde su sistema de archivos, consulte [Agregar documentos a Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#add-documents-to-workfront) en [Agregar documentos a Adobe Workfront desde su sistema de archivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Vincular documentos de Workfront Proof {#link-workfront-proof-documents}

Puede vincular pruebas a Workfront que existían originalmente en Workfront Proof. Al vincular una prueba desde Workfront Proof, todos los comentarios y demás metadatos asociados a la prueba están disponibles en Workfront.

Solo puede vincular las pruebas para las que tenga acceso de visualización en Workfront Proof.

1. Vaya al área de **Documentos** de Workfront donde desee colocar el documento.
1. Haz clic en **Agregar nuevo** y luego haz clic en **Desde Workfront Proof**.

   >[!NOTE]
   >
   >Las opciones de este menú pueden variar según los proveedores de terceros que estén configurados en su entorno.

1. En el cuadro **Enlazar revisiones desde Workfront Proof** que aparece, empiece a escribir el nombre de la revisión que desea que esté disponible en Workfront.

   La lista se filtra a medida que escribe.

1. Seleccione hasta 10 pruebas para vincular.

   No es posible vincular ningún nombre de revisión atenuado porque la revisión ya está asociada a un documento en Workfront.

1. Haga clic en **Vínculo**.

   La versión más actual de la revisión está vinculada a Workfront. Al abrir la prueba, todas las versiones están disponibles en el visualizador de pruebas.

### Creación de un documento de Google desde Workfront {#create-a-google-document-from-within-workfront}

Puede crear un nuevo documento de Google desde Workfront. No puede crear nuevos documentos desde Workfront para otros proveedores de la nube.

1. Vaya al área de **Documentos** de Workfront donde desee colocar el documento.
1. Haga clic en **Agregar nuevo** > **Archivo de Google** y, a continuación, seleccione el tipo de documento de Google que desea crear.
1. Si aparece el cuadro **Agregar cuenta de Google Drive**, haga clic en **Autorizar Google Drive**.

   Se agregó un documento de Google a la ficha **Documentos**.

   >[!NOTE]
   >
   > Mi unidad y Compartido conmigo muestran dos resultados diferentes. Si no puede encontrar un archivo en Mi unidad, marque en la carpeta Compartido conmigo.

## Cargar y vincular un documento de Workfront a un proveedor de nube externo

Puede cargar y vincular un documento de Workfront a un proveedor de nube externo. Esto mueve el almacenamiento del documento de Workfront al proveedor de nube externo. Cuando se cambia el documento en la aplicación externa, se actualiza automáticamente en Workfront.

>[!NOTE]
>
>Al enviar un recurso a un proveedor de documentos externo, se crea una nueva versión del recurso.

Los usuarios sin acceso a Workfront pueden ver el documento en la aplicación externa si tienen acceso a la aplicación.

1. Seleccione un documento que se haya cargado en Workfront.
1. Haga clic en **Más** >**Enviar a** y, a continuación, seleccione el proveedor de la nube que desea que almacene el documento vinculado.

   También puede usar el menú Más ![](assets/more-icon.png) de la página Detalles del documento para hacerlo.

1. Seleccione la carpeta de la aplicación del proveedor en la que desea almacenar el documento.

   Puede ser cualquier carpeta de la aplicación del proveedor, incluida una carpeta compartida.

1. Haga clic en **Guardar**.

   El logotipo del proveedor externo aparece junto al nombre del documento para indicar que el documento ahora está vinculado a Workfront y el proveedor de nube externo lo almacena.

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## Vincular carpetas

Al vincular una carpeta entre Workfront y un proveedor de nube externo, la carpeta y todo su contenido se vinculan. Si los usuarios sin acceso a Workfront agregan, quitan y modifican archivos desde la aplicación de documento externa, sus cambios se sincronizan con Workfront.

### Derechos de acceso a carpetas {#folder-access-rights}

Al sincronizar el contenido de la carpeta desde una aplicación de documento externa, Workfront utiliza las credenciales del usuario que originalmente vinculó la carpeta. Esto resulta en la siguiente experiencia de usuario:

* Si los usuarios no tienen acceso para ver archivos y carpetas en la aplicación externa, pero sí para ver la carpeta vinculada mediante Workfront, pueden ver únicamente los nombres de los archivos y carpetas en Workfront, no su contenido.
* Cuando alguien accede al contenido de una carpeta vinculada en Workfront (como una subcarpeta de una carpeta vinculada) vinculada a Workfront por otro usuario, el contenido se sincroniza con Workfront mediante las credenciales de inicio de sesión de Workfront del usuario que originalmente vinculó la carpeta, no las del usuario que accede al contenido.

>[!IMPORTANT]
>
>* Si el usuario que originalmente vinculó la carpeta se elimina del sistema de Workfront, los usuarios ya no podrán acceder al contenido de la carpeta vinculada a través de Workfront. En este caso, la carpeta debe volver a vincularse con un usuario activo de Workfront que tenga derechos sobre la carpeta en la aplicación externa.
>* Si el usuario que ha vinculado una carpeta ya no tiene acceso a la aplicación externa, Workfront ya no puede acceder al contenido de la carpeta. Esto puede suceder, por ejemplo, si el usuario que vinculó originalmente la carpeta abandona la compañía. Para garantizar el acceso continuo, un usuario con acceso a la carpeta debe volver a vincular la carpeta.

### Vincular una o más carpetas externas {#link-one-or-more-external-folders}

1. Vaya al área de Workfront donde desee la carpeta y haga clic en **Documentos** ![](assets/document-icon.png) en el panel izquierdo

1. Haga clic en **Agregar nuevo** y, a continuación, haga clic en el proveedor de documentos externo desde el que desea vincular una carpeta a Workfront.
1. (Condicional) Si aún no ha autorizado el servicio externo, especifique sus credenciales de inicio de sesión para el proveedor externo y haga clic en **Iniciar sesión**.

   Los proveedores externos que ya ha autorizado aparecen en la parte superior de la lista.

1. En el cuadro **Vincular archivos y carpetas externos** que aparece, busque y seleccione las carpetas que desee vincular.

   O

   Escriba el nombre de la carpeta que desea buscar y, a continuación, presione **Entrar**.

   Puede seleccionar varias carpetas; sin embargo, solo las carpetas seleccionadas en la vista actual están vinculadas. Por ejemplo, si selecciona una carpeta y luego entra en una carpeta, la carpeta que seleccionó originalmente no está vinculada.

   >[!NOTE]
   >
   >Al vincular carpetas desde Google Drive, sólo puede vincular carpetas que se encuentren en su unidad personal (Mi unidad) y en Team Drive. No puede vincular carpetas desde el área Compartida conmigo.

1. Haga clic en **Vínculo**.

   En Workfront, el logotipo del proveedor de la nube se muestra junto a la carpeta, lo que indica que está vinculado al proveedor de la nube externo.

1. (Opcional) Para cambiar el nombre de la carpeta de modo que el nombre de la carpeta en Workfront sea diferente del nombre de la carpeta en la aplicación de documento externa, seleccione la carpeta en la sección **Carpetas**, haga clic en el menú Más ![](assets/more-icon.png) que aparece junto al nombre de la carpeta y, a continuación, haga clic en **Cambiar nombre**.

   ![](assets/documents-folderlink-rename-nwe-350x154.png)

Esto no cambia el nombre de la carpeta en la aplicación externa.

### Agregar subcarpetas a una carpeta vinculada  {#add-subfolders-to-a-linked-folder}

Puede crear una carpeta nueva dentro de una carpeta vinculada existente. También puede arrastrar otra carpeta a una carpeta vinculada existente.

1. Para crear una carpeta nueva dentro de una carpeta vinculada existente, vaya a la carpeta existente y, a continuación, cree la carpeta nueva tal como se describe en [Crear carpetas de documentos](../../documents/organizing-documents/create-documents-folder.md).

   O

   Para arrastrar una carpeta existente a una carpeta vinculada existente, vaya al área Documentos donde desee colocar la subcarpeta y arrástrela a la carpeta vinculada.

   ![](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   >
   >Al arrastrar una carpeta de Workfront existente a una carpeta vinculada, se aplican las siguientes limitaciones:
   >
   >* La carpeta que está arrastrando no se puede vincular y no puede contener ningún contenido que ya esté vinculado.
   >* La carpeta (incluido su contenido) que está arrastrando no puede superar los 50 MB.

## Agregar un documento a una carpeta vinculada

Cuando se agrega un documento a una carpeta vinculada mediante Workfront, se agrega automáticamente como documento vinculado.

1. Seleccione la carpeta vinculada en la que desea el documento, haga clic en **Agregar nuevo > Documento**, desplácese hasta el documento y agréguelo a la carpeta.

   O

   En el área **Documentos** donde desee colocar el documento, arrástrelo a una carpeta vinculada.

   Se crea automáticamente una nueva versión del documento en la aplicación externa y se vincula a Workfront.

>[!NOTE]
>
> * Las opciones de documento no están disponibles mientras el documento se está moviendo.
>
> * Cuando un documento se mueve a Experience Manager Assets, ya no está visible en la lista de documentos de Workfront.
>
> * Las acciones o ediciones que realice en un documento mientras se mueve no aparecerán en el documento en Experience Manager Assets y, por lo tanto, se perderán.

## Eliminar un documento o una carpeta vinculados

Cuando se elimina un documento o una carpeta vinculados de la aplicación externa, el documento o la carpeta permanece en el sistema de Workfront hasta que también se elimina de Workfront.

1. Seleccione el documento o la carpeta vinculados y luego haga clic en **Eliminar**.
1. En el cuadro de confirmación que aparece, haga clic en **Sí, desvincularlo**.

   El documento se desenlazará del sitio de Workfront. No se ve afectado en la aplicación externa.

## Cambiar el nombre de documentos y carpetas vinculados

Al cambiar el nombre de un documento o carpeta vinculados, el cambio solo es visible en la aplicación en la que lo realiza. Por ejemplo, si cambia el nombre de un documento vinculado en Workfront, el nuevo nombre solo será visible en Workfront.

Si desea que el nombre coincida en Workfront y en la aplicación externa, debe cambiarle el nombre en ambos lugares.

>[!IMPORTANT]
>
>No cambie el nombre de un documento en Workfront que esté vinculado a Dropbox; si lo hace, el archivo en Workfront será inaccesible. En su lugar, cambie el nombre del archivo en Dropbox y vuelva a sincronizar el archivo.
