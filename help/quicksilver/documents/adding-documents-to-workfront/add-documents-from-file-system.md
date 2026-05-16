---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Añadir documentos a Adobe Workfront desde su sistema de archivos
description: Puede agregar documentos a proyectos, tareas o problemas en varias áreas en Adobe Workfront.
author: Courtney, Alina
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 8%

---

# Añadir documentos a Adobe Workfront desde su sistema de archivos

Adobe Workfront tiene actualmente los dos tipos siguientes de almacenamiento de documentos:

* Almacenamiento de Workfront heredado
* almacenamiento en la nube de Adobe

Para obtener más información acerca de estos tipos de almacenamiento, vea [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

>[!NOTE]
>
>Algunos clientes tienen ambos tipos de almacenamiento de documentos y algunos solo tienen almacenamiento de Workfront o Adobe.

La adición de documentos a Workfront difiere según la versión del área de documentos que utilice su organización.

* [Agregar documentos del sistema de archivos en el área Documentos heredados](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [Agregar documentos a Workfront en el área de nuevos documentos](#add-documents-to-workfront-in-the-new-documents-area)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de Workfront para administrar documentos mediante el almacenamiento heredado de Workfront</p>
<p>Cualquier paquete de flujo de trabajo para administrar documentos mediante Adobe Cloud Storage.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Almacenamiento de Workfront heredado: Editar acceso a documentos</p> 
   <p>Almacenamiento en la nube de Adobe: Editar acceso a documentos está habilitado de forma predeterminada y no se puede cambiar</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agregar documentos del sistema de archivos en el área Documentos heredados

Si su organización utiliza almacenamiento heredado de Workfront, verá el área Documentos heredados al acceder a documentos en Workfront.

Para obtener más información sobre el almacenamiento de Workfront, consulte [Diferencias entre el almacenamiento en la nube de Adobe y el almacenamiento de Workfront heredado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Puede agregar documentos a las siguientes áreas de Workfront:

* El área Documentos del menú principal
* El área Documentos de un objeto Workfront (proyecto, tarea, problema, plantilla, tarea de plantilla, portafolio, programa)
* Tarjeta conectada en una placa Workfront

También puede cargar nuevas versiones de documentos y agregar vínculos a documentos de proveedores de la nube de terceros, como Google Drive, Dropbox y Microsoft OneDrive.

Para obtener información acerca de cómo agregar nuevas versiones de documentos, vea [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

Para obtener información sobre cómo agregar documentos de proveedores de la nube de terceros, consulte [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

No hay restricciones en cuanto a los tipos y tamaños de archivos que se pueden cargar en Workfront. Sin embargo, para que la carga se realice correctamente, debe completarse en un plazo de cinco minutos y tener disponible un espacio de almacenamiento adecuado.

Si necesita información sobre cómo cargar nuevas versiones de un documento en Workfront, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).


### Agregar documentos a Workfront en el área de Documentos heredados

Puede añadir nuevos documentos a Workfront desde el sistema de archivos de su estación de trabajo. También puede vincular documentos desde aplicaciones de terceros, como Google Drive y SharePoint.

>[!IMPORTANT]
>
>* Puede cargar hasta 150 documentos al mismo tiempo.
>* No hay límite en el tamaño del archivo.
>* Las descargas de documentos están limitadas a 4 GB.

Para agregar un documento:

1. Vaya al objeto de Workfront donde desee agregar un documento nuevo.
1. Haga clic en la ficha **Documentos** y, a continuación, haga clic en el menú desplegable **Agregar nuevo**.

   ![Agregar nuevo documento](assets/add-new-doc.png)

1. Según el tipo de documento que desee agregar, realice una de las acciones siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Cargar documentos desde el sistema de archivos en la estación de trabajo</td> 
      <td> 
       <ol> 
        <li value="1">En el menú desplegable <strong>Agregar nuevo</strong>, seleccione <strong>Documento.</strong></li> 
        <li value="2"> <p>Busque y seleccione el documento que desea añadir del sistema de archivos de la estación de trabajo.<br></p> <p>Para seleccionar varios documentos, pulse la tecla Mayús mientras selecciona otros archivos.</p> </li> 
        <li value="3">Haga clic en <strong>Abrir</strong>.</li> 
       </ol> 
       <p><b>NOTA</b>: También puede arrastrar y soltar archivos directamente desde el administrador de archivos a la lista de documentos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cargar documentos desde una aplicación de terceros, como Google Drive o SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>En el menú desplegable <strong>Agregar nuevo</strong>, seleccione <strong>De &lt;name_of_third-party_application&gt;</strong>.</p> <p>Por ejemplo, para cargar un documento desde Google Drive, haz clic en <strong>Desde Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Siga las indicaciones para seleccionar el documento en la aplicación de terceros.<br></p> <p>Para obtener más información acerca de los documentos vinculados, vea <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Vincular documentos de aplicaciones externas</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solicitar un documento a otro usuario de Workfront</td> 
      <td> 
       <ol> 
        <li value="1">En el menú desplegable <strong>Agregar nuevo</strong>, seleccione <strong>Solicitar un documento</strong>.</li> 
        <li value="2">En el cuadro <strong>Quién se lo solicita a</strong>, escriba el nombre del usuario al que desea solicitar el documento.</li> 
        <li value="3">En el cuadro <strong>Dígales lo que solicita</strong>, escriba el nombre del documento.</li> 
        <li value="4"> <p>Haga clic en <strong>Enviar solicitud</strong>.</p> <p>La solicitud se mostrará en la ficha Documentos.</p> <p>Para obtener más información sobre cómo solicitar documentos, consulte <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Solicitar un documento</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

   El documento se agrega a la sección Documentos del objeto seleccionado.

## Agregar documentos a Workfront en el área de nuevos documentos

Puede agregar documentos a objetos mediante el modelo de almacenamiento en la nube de Adobe. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Funcionalidad no admitida actualmente en el área de nuevos documentos:

* Carga de documentos en el área Documentos del menú Principal
* Agregar vínculos a documentos de proveedores de nube de terceros, como Google Drive, Dropbox y Microsoft OneDrive.
* Solicitud de documentos
* Copia de un vínculo a una carpeta
* Retirada de documentos
* Pegar imágenes desde el portapapeles
* Adición de carpetas inteligentes

### Agregar documentos a Workfront en el área de nuevos documentos

Si su organización utiliza el almacenamiento en la nube de Adobe, verá la nueva área Documentos al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para agregar un documento:

1. Vaya al objeto de Workfront donde desee agregar un documento nuevo.
1. Haga clic en la sección **Documentos** del panel izquierdo.
1. Haga clic en **Nuevo** en el lado derecho de la página o arrastre y suelte el archivo en la zona de colocación que aparece. Puede agregar varios documentos al mismo tiempo.

   ![Agregar nuevo documento](assets/add-new-doc-new-doc.png)

Si necesita información sobre cómo cargar nuevas versiones de un documento en Workfront, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

En la sección Documentos se crea automáticamente una carpeta con el mismo nombre que el objeto en el que está cargando el documento y el documento se agrega a la carpeta.

## Seguridad de documentos para el almacenamiento en la nube de Adobe

Workfront evita que virus y otro contenido malicioso entren en el sitio a través de documentos de las siguientes maneras:

**Cómo detecta Workfront los archivos dañados**

La digitalización de documentos se habilita automáticamente para los objetos que utilizan el modelo de almacenamiento en la nube de Adobe.

Todos los archivos de menos de 500 MB se analizan cuando se cargan. Los archivos de más de 500 MB no se analizan. Si Workfront detecta un documento dañado, se eliminará automáticamente.

**Restricciones de nombre de archivo**

Dado que esta integración se crea mediante el almacenamiento en la nube de Adobe, existen algunas convenciones de estructura y nomenclatura obligatorias que se deben tener en cuenta al administrar proyectos y documentos.

* Los nombres de objeto deben ser únicos y no se pueden duplicar
* El almacenamiento en la nube de Adobe requiere nombres únicos para objetos de igual a igual con el mismo elemento principal en el árbol de jerarquías
* Los documentos no pueden tener el mismo nombre si pertenecen al mismo proyecto
* Los nombres de documento no pueden contener ninguno de los siguientes caracteres especiales: `\ / : * ? " | < >`
* Los nombres de documento están limitados a un máximo de 255 caracteres

Teniendo en cuenta estas limitaciones, Workfront cambia automáticamente el nombre de los objetos o documentos según sea necesario para evitar conflictos.


## Seguridad de documentos para el almacenamiento heredado de Workfront

Workfront evita que virus y otro contenido malicioso entren en el sitio a través de documentos de las siguientes maneras:

**Cómo detecta Workfront los archivos dañados**

La digitalización de documentos solo está habilitada para su organización si se solicita.

Si la digitalización de documentos está habilitada, los archivos de menos de 25 MB se analizan cuando se cargan. Los archivos de más de 25 MB no se analizan.

Si Workfront detecta un documento dañado, aparecerá un mensaje que indica que el archivo está dañado. También recibe una notificación por correo electrónico cuando Workfront detecta contenido potencialmente malicioso y el archivo está programado para su eliminación.

Los archivos dañados se eliminan en un plazo de 24 horas tras la detección, a menos que los elimine manualmente. Si elimina un archivo dañado, Workfront realiza el seguimiento de esta acción como una actualización. Si permite que Workfront lo elimine, no se registrará ninguna actualización.

**Restricciones de nombre de archivo**

Los archivos cargados en Workfront no pueden contener ciertos caracteres en los nombres de archivo. Si un archivo contiene cualquiera de los siguientes caracteres en el nombre de archivo, los caracteres se eliminan del nombre de archivo cuando se carga el archivo: `! # % * \ | ' " / ? < > { } [ ]`.
