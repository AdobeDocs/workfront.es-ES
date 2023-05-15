---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Agregar documentos a Adobe Workfront desde el sistema de archivos
description: Puede añadir documentos a proyectos, tareas o problemas en las siguientes áreas de Adobe Workfront - EDIT ME.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
source-git-commit: fe9f1da23f1196dac468ec33aae776950ce49f2c
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 1%

---

# Agregar documentos a Adobe Workfront desde el sistema de archivos

Puede agregar documentos a proyectos, tareas o problemas en las siguientes áreas de Adobe Workfront:

* Área de documentos globales
* Área Documentos de un objeto Workfront

También puede cargar nuevas versiones de documentos y agregar vínculos a documentos de proveedores de la nube de terceros, como Google Drive, Dropbox y Microsoft OneDrive. Para obtener información sobre cómo agregar nuevas versiones de documentos, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md). Para obtener información sobre cómo agregar documentos de proveedores de nube de terceros, consulte [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

No hay restricciones en los tipos y tamaños de archivos que puede cargar en Workfront. Sin embargo, para que la carga sea correcta, debe completarse en un plazo de cinco minutos y debe disponer de espacio de almacenamiento adecuado.

Si necesita información sobre cómo cargar nuevas versiones de un documento a Workfront, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

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

## Añadir documentos a Workfront

Puede agregar nuevos documentos a Workfront desde el sistema de archivos de su estación de trabajo. También puede vincular documentos de aplicaciones de terceros como Google Drive y SharePoint.

>[!NOTE]
>
>Aunque no hay límite de tamaño para las cargas de documentos, las descargas de documentos están limitadas a 4 GB.

Para agregar un documento:

1. Vaya al proyecto, la tarea o el problema en el que desea agregar un nuevo documento.
1. Haga clic en el **Documentos** y, a continuación, haga clic en la pestaña **Agregar nuevo** menú desplegable.

   ![](assets/add-new-350x138.png)

1. En función del tipo de documento que desee agregar, realice una de las acciones siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Cargar documentos desde el sistema de archivos en la estación de trabajo</td> 
      <td> 
       <ol> 
        <li value="1">En el <strong>Agregar nuevo</strong> menú desplegable, seleccione <strong>Documento.</strong></li> 
        <li value="2"> <p>Busque y seleccione el documento que desea agregar desde el sistema de archivos de la estación de trabajo.<br></p> <p>Para seleccionar varios documentos, pulse la tecla Mayús mientras selecciona archivos adicionales.</p> </li> 
        <li value="3">Haga clic en <strong>Apertura</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cargar documentos desde una aplicación de terceros como Google Drive o SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>En el <strong>Agregar nuevo</strong> menú desplegable, seleccione <strong>De &lt;name_of_third-party_application&gt;</strong>.</p> <p>Por ejemplo, para cargar un documento desde Google Drive, haga clic en <strong>Desde Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Siga las indicaciones para seleccionar el documento en la aplicación de terceros.<br></p> <p>Para obtener más información sobre los documentos vinculados, consulte <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Vincular documentos de aplicaciones externas</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solicitar un documento de otro usuario de Workfront</td> 
      <td> 
       <ol> 
        <li value="1">En el <strong>Agregar nuevo</strong> menú desplegable, seleccione <strong>Solicitar un documento</strong>.</li> 
        <li value="2">En el <strong>De quién lo solicita</strong> , escriba el nombre del usuario desde el que solicita el documento.</li> 
        <li value="3">En el <strong>Dígales lo que estás solicitando</strong> , escriba el nombre del documento.</li> 
        <li value="4"> <p>Haga clic en <strong>Enviar solicitud</strong>.</p> <p>La solicitud se muestra en la ficha Documentos .</p> <p> <img src="assets/request-a-document-350x110.png" style="width: 350;height: 110;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>Para obtener más información sobre la solicitud de documentos, consulte <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Solicitar un documento</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

## Seguridad de los documentos

El sitio de Workfront evita que los virus y otro contenido malicioso entren al sitio a través de documentos de las siguientes maneras:

* [Cómo detecta Workfront los archivos dañados](#how-workfront-detects-corrupted-files)
* [Restricciones de nombre de archivo](#file-name-restrictions)

### Cómo detecta Workfront los archivos dañados {#how-workfront-detects-corrupted-files}

El análisis de documentos solo está habilitado para su organización si se solicita.

Si la digitalización de documentos está habilitada, los archivos menores de 25 MB se analizan cuando se cargan. Los archivos de más de 25 MB no se analizan.

Si Workfront detecta un documento dañado, Workfront interrumpe el proceso de carga y aparece un mensaje que indica que el archivo está dañado. También recibirá una notificación por correo electrónico cuando Workfront detecte contenido potencialmente malintencionado y el archivo esté programado para su eliminación.

Los archivos dañados se eliminan en un plazo de 24 horas tras la detección, a menos que los elimine manualmente. Si elimina un archivo dañado, Workfront rastrea esta acción como una actualización. Si permite que Workfront lo elimine, no se registrarán actualizaciones.

### Restricciones de nombre de archivo {#file-name-restrictions}

Los archivos cargados en Workfront no pueden contener ciertos caracteres en los nombres de archivo. Si un archivo contiene cualquiera de los siguientes caracteres en el nombre del archivo, los caracteres se eliminan del nombre del archivo cuando se carga: `< > { }`.
