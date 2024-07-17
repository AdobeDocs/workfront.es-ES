---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Eliminar vínculos entre Adobe Workfront y proveedores de almacenamiento de documentos externos
description: Al cargar un documento desde cualquier servicio por primera vez, Adobe Workfront solicita permiso al usuario para acceder a su servicio de documentos. Cuando el usuario proporciona sus credenciales de servicio de documentos para iniciar sesión, el servicio de documentos se vincula a sí mismo a Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Eliminar vínculos entre Adobe Workfront y proveedores de almacenamiento de documentos externos

Al cargar un documento desde cualquier servicio por primera vez, Adobe Workfront solicita permiso al usuario para acceder a su servicio de documentos. Cuando el usuario proporciona sus credenciales de servicio de documentos para iniciar sesión, el servicio de documentos se vincula a sí mismo a Workfront.

Para obtener información sobre cómo vincular servicios de documentos externos a Workfront, consulte [Vinculación de documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Dado que el servicio de documentos es el que permite vincular permisos a Workfront, Workfront no puede eliminar el permiso concedido por el servicio de documentos. Debe quitar el permiso desde la aplicación del servicio de documentos o llamar a nuestro Equipo de soporte para quitar este vínculo de nuestros servidores.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Eliminar el vínculo entre Workfront y Dropbox

1. Inicie sesión en el Dropbox.
1. Haz clic en la imagen de perfil en la esquina superior derecha y, a continuación, haz clic en **Configuración**.
1. Haga clic en la ficha **Aplicaciones conectadas** y desplácese hacia abajo hasta **Aplicaciones vinculadas**.

1. Haz clic en **X** junto a Workfront.

## Eliminar el vínculo entre Workfront y Box

1. Inicie sesión en su cuenta de Box.
1. Haga clic en la imagen de perfil en la esquina superior derecha.
1. Haga clic en **Configuración de la cuenta** y luego en la ficha **Seguridad**.

1. Busque **MyWorkfront** y haga clic en **X** en Olvidar aplicación.

## Quitar el vínculo entre Workfront y Google Drive

1. Inicie sesión en la unidad de Google.
1. Haga clic en el icono de engranaje en la esquina superior derecha y, a continuación, haga clic en **Configuración**.
1. Haz clic en **Administrar aplicaciones** en el lado izquierdo y encuentra **Workfront** en la lista.

1. En el menú desplegable Opciones, haga clic en **Desconectar de la unidad**.

## Eliminar los vínculos entre Workfront y otros proveedores de almacenamiento de documentos

Debe llamar a nuestro Equipo de soporte para desconectar Microsoft One Drive o WebDAM de Workfront.

Para obtener información sobre cómo comunicarse con nuestro Equipo de soporte, consulte [Comuníquese con Atención al cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
