---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Compartir una carpeta de documentos
description: Puede compartir una carpeta y su contenido desde el área Documentos.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Compartir una carpeta de documentos

Puede compartir una carpeta y su contenido desde el área Documentos.

>[!NOTE]
>
>* La carpeta debe estar en los cinco niveles superiores de una jerarquía de carpetas en un objeto. Cada carpeta del sexto nivel o inferior hereda sus configuraciones de uso compartido de la carpeta directamente superior a ella.
>
>  Para obtener información acerca de cómo agregar subcarpetas para crear una jerarquía de carpetas, vea la sección [Crear carpetas y subcarpetas](../../documents/organizing-documents/create-documents-folder.md#creating-folders) en el artículo [Crear carpetas de documentos](../../documents/organizing-documents/create-documents-folder.md).
>
>* Las carpetas inteligentes no se pueden compartir.
>* Si configura opciones de uso compartido para una carpeta de documentos dentro de una plantilla y alguien crea un proyecto a partir de esa plantilla, las configuraciones de uso compartido no se transfieren a la carpeta de documentos del nuevo proyecto.
>* Si configura opciones de uso compartido para una carpeta de documentos dentro de un elemento de trabajo y, a continuación, copia el elemento de trabajo, las configuraciones de uso compartido no se transfieren a la carpeta de documentos del nuevo elemento de trabajo.
>

## Requisitos de acceso

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver el acceso a un objeto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Compartir una carpeta

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y luego haga clic en **Documentos**.

   O

   Con un objeto de Workfront abierto, haga clic en **Documentos** en el panel izquierdo.

1. Seleccione la carpeta y, a continuación, haga clic en el icono Compartir ![](assets/share-icon.png) de la barra de herramientas.

   La carpeta debe estar en los cinco niveles superiores de una jerarquía de carpetas en un objeto y no puede ser una carpeta inteligente.

1. En el cuadro que se muestra, en **Dar acceso a la carpeta a**, empiece a escribir el nombre del usuario, equipo, rol, grupo o compañía con el que desea compartir la carpeta y, a continuación, presione **Entrar** cuando se muestre el nombre.
1. Para ajustar el acceso del usuario, equipo, función del trabajo, grupo o compañía que acaba de agregar, haga clic en el menú desplegable situado a la derecha del nombre y, a continuación, configure una de las siguientes opciones disponibles y cualquiera de sus opciones avanzadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Verlo</td> 
      <td> <p>Capacidad para ver la carpeta y su contenido.</p> <p>Haga clic en <strong>Configuración avanzada</strong> para especificar si desea permitir lo siguiente:</p> 
       <ul> 
        <li><strong>Descargar</strong>: Capacidad para descargar la carpeta y su contenido como archivo ZIP</li> 
        <li> <p><strong>Compartir</strong>: capacidad para compartir la carpeta con otros usuarios del sistema</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administrarlo</td> 
      <td> <p>Capacidad para ver y editar la carpeta y su contenido</p> <p>Haga clic en <strong>Configuración avanzada</strong> para especificar si desea permitir que los usuarios hagan lo siguiente:</p> 
       <ul> 
        <li><strong>Eliminar</strong>: elimine la carpeta y su contenido del sistema</li> 
        <li><b>Descargar</b>: Descargue la carpeta y su contenido como archivo ZIP</li> 
        <li><strong>Compartir</strong>: comparte la carpeta y su contenido con otros usuarios del sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita los pasos 3-4 para añadir otros nombres a la lista y configurar sus opciones.
1. (Opcional) Si desea que todos los usuarios del sistema puedan ver la carpeta y su contenido, haga clic en el icono de engranaje ![](assets/gear-icon-settings-with-dn-arrow.jpg) en la esquina superior derecha del cuadro para compartir y, a continuación, haga clic en **Hacer esto visible en todo el sistema.**

   Si cambia de opinión, puede hacer clic en **Quitar el acceso en todo el sistema** (la opción predeterminada).

## Cómo acceden los usuarios al contenido de una carpeta compartida con ellos

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

Actualmente, cuando comparte una carpeta, los destinatarios no ven la carpeta en su área de Documentos. Sin embargo, pueden acceder a sus documentos ejecutando un informe de documento.

Para obtener información acerca de cómo ejecutar un informe, vea la sección [Informe sobre objetos](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) en el artículo [Comprender los objetos en Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Vea también [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## Permisos heredados al compartir un objeto que contiene una carpeta

Cuando comparte un objeto que tiene una carpeta de documentos, los destinatarios también obtienen acceso a la carpeta:

* Si concede a los destinatarios acceso de Vista al objeto principal, tendrán acceso de Vista a la carpeta.
* Si concede a los destinatarios acceso de Contribute o de Administración al objeto principal, tendrán acceso de Administración a la carpeta.
* Si concede un tipo de acceso (Ver, Contribute o Administrar) al objeto principal y otro tipo a la carpeta, los destinatarios tendrán el mayor de esos dos tipos de acceso a los documentos de la carpeta

  Por ejemplo, si comparte el objeto principal con acceso de visualización y la carpeta con acceso de administración, los destinatarios tendrán acceso de administración a los documentos de la carpeta.

  >[!NOTE]
  >
  >Un documento adjunto hereda permisos únicamente del objeto en el que se adjuntó. Si crea una carpeta en el objeto y mueve el documento a la carpeta, heredará los permisos de la carpeta. Sin embargo, si crea una carpeta en un objeto principal o abuelo y mueve el documento a esa carpeta, no heredará los permisos de esa carpeta.

* Si la opción &quot;Nunca heredar el acceso a documentos de proyectos, tareas, problemas, etc.&quot; está habilitada en el nivel de acceso del destinatario, no heredarán los permisos de los documentos de una carpeta que comparta con ellos. Para que tengan acceso a un documento de la carpeta, debe compartir el documento.

  Para obtener información acerca de la opción &quot;No heredar nunca&quot;, vea [Configurar el acceso a Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  Para obtener información acerca de cómo compartir un documento, vea [Compartir un documento](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
