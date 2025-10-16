---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Eliminar vínculos entre Adobe Workfront y proveedores externos de almacenamiento de documentos
description: Al cargar un documento desde cualquier servicio por primera vez, Adobe Workfront solicita permiso al usuario para acceder a su servicio de documentos. Cuando el usuario proporciona sus credenciales de servicio de documentos para iniciar sesión, el servicio de documentos se vincula a sí mismo a Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 98%

---

# Eliminar vínculos entre Adobe Workfront y proveedores externos de almacenamiento de documentos

Al cargar un documento desde cualquier servicio por primera vez, Adobe Workfront solicita permiso al usuario para acceder a su servicio de documentos. Cuando el usuario proporciona sus credenciales de servicio de documentos para iniciar sesión, el servicio de documentos se vincula a sí mismo a Workfront.

Para obtener información sobre cómo vincular servicios de documentos externos a Workfront, consulte [Vinculación de documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Dado que el servicio de documentos es el que permite vincular permisos a Workfront, Workfront no puede eliminar el permiso concedido por el servicio de documentos. Debe quitar el permiso desde la aplicación del servicio de documentos o llamar a nuestro equipo de soporte para quitar este vínculo de nuestros servidores.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> 
   <p>Colaborador o superior</p>
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminar el vínculo entre Workfront y Dropbox

1. Inicie sesión en Dropbox.
1. Haga clic en la imagen de perfil en la esquina superior derecha y, a continuación, haga clic en **Configuración**.
1. Haga clic en la ficha **Aplicaciones conectadas** y desplácese hacia abajo hasta **Aplicaciones vinculadas**.

1. Haga clic en **X** junto a Workfront.

## Eliminar el vínculo entre Workfront y Box

1. Inicie sesión en su cuenta de Box.
1. Haga clic en la imagen de perfil en la esquina superior derecha.
1. Haga clic en **Configuración de la cuenta** y luego en la ficha **Seguridad**.

1. Busque **MyWorkfront** y haga clic en **X** en Olvidar aplicación.

## Eliminar el vínculo entre Workfront y Google Drive

1. Inicie sesión en Google Drive.
1. Haga clic en el icono de engranaje en la esquina superior derecha y, a continuación, haga clic en **Configuración**.
1. Haga clic en **Administrar aplicaciones** en el lado izquierdo y encuentre **Workfront** en la lista.

1. En el menú desplegable Opciones, haga clic en **Desconectar de la unidad**.

## Eliminar los vínculos entre Workfront y otros proveedores de almacenamiento de documentos

Debe llamar a nuestro Equipo de soporte para desconectar Microsoft One Drive o WebDAM de Workfront.

Para obtener información sobre cómo comunicarse con nuestro Equipo de soporte, consulte [Póngase en contacto con el servicio de atención al cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
