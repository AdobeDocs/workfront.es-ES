---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Instalación de Desktop Proofing Viewer para su organización
description: El Visor de prueba de escritorio, que está diseñado principalmente para probar contenido interactivo, es una aplicación que debe instalarse en el equipo local de cada usuario. Como administrador de Adobe Workfront o de Workfront Proof, puede realizar esta instalación.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 58f976d9f4245e528a4ddf23d39b92d9fa405311
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Instalación de Desktop Proofing Viewer para su organización

El Visor de prueba de escritorio, que está diseñado principalmente para probar contenido interactivo, es una aplicación que debe instalarse en el equipo local de cada usuario. Como administrador de Adobe Workfront o de Workfront Proof, puede realizar esta instalación.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Premium o Select</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o plan</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe tener el administrador seleccionado en el perfil de permisos de prueba. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configuración del acceso de prueba de un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos del sistema

El Visor de prueba de escritorio es compatible con los siguientes sistemas operativos:

* Windows 7 y versiones posteriores, de 32 y 64 bits
* Mac OS X 10.9 y posteriores de 64 bits

## Requisitos previos

Para permitir que los usuarios utilicen el Visor de prueba de escritorio, debe

* Configure el sistema para que inicie Desktop Proofing Viewer como vista predeterminada para pruebas interactivas antes de la instalación.

## Configure el Visor de prueba de escritorio como predeterminado para pruebas interactivas

Después de instalar el Visor de pruebas de escritorio para su organización, puede establecerlo como visor predeterminado para pruebas interactivas.

1. En Workfront, haga clic en el menú principal ![](assets/main-menu-icon.png)y, a continuación, haga clic en Prueba ![](assets/proofing-in-main-menu.png) para acceder a Workfront Proof.

1. Haga clic en **Configuración de la cuenta** cerca de la esquina superior derecha de la prueba de Workfront y, a continuación, haga clic en la **Configuración** pestaña .

1. En **Valores predeterminados de prueba**, al final del **Visor de pruebas de escritorio para pruebas interactivas** fila, haga clic en **Configuración**.

   ![](assets/proof-defaults-350x265.png)

1. Haga clic en **Habilitado y predeterminado** y haga clic en **Guardar**.

## Instalación del visualizador de pruebas de escritorio para los usuarios

* [Instalación de Desktop Proofing Viewer en Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Instalación de Desktop Proofing Viewer en Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Instalación de Desktop Proofing Viewer en Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. En el equipo del usuario, realice una de las siguientes acciones para descargar la aplicación:

   * Si está utilizando el entorno Producción, haga clic en  [Descarga de producción de Mac para el visualizador de pruebas de escritorio.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg)
   * Si está utilizando el entorno de vista previa, haga clic en  [Descarga de vista previa de Mac para el visualizador de pruebas de escritorio.](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg)
)

1. Abra el archivo que acaba de descargar para iniciar la instalación.
1. En el cuadro de instalación que aparece, haga clic en **Continuar** y haga clic en **Instalar**.

   ![0000776.png](assets/00000776-350x244.png)

1. Asegúrese de que cada usuario completa la instalación abriendo una prueba interactiva desde el área Documentos de Workfront.

### Instalación de Desktop Proofing Viewer en Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. En el equipo del usuario, realice una de las siguientes acciones para descargar la aplicación:

   * En el entorno Producción, haga clic en [Descarga de producción de Windows para Desktop Proofing Viewer.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe)
   * En el entorno de vista previa, haga clic en [Descarga de Windows Preview para el Visor de pruebas de escritorio](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Abra el archivo que acaba de descargar para iniciar la instalación.
1. En el cuadro de advertencia de seguridad que aparece, haga clic en **Ejecutar**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   El Visor de prueba de escritorio instala y ejecuta.

1. (Condicional) Si instala la aplicación mediante Internet Explorer, actualice la página de inicio en el explorador después de que la aplicación se instale.
1. Asegúrese de que cada usuario completa la instalación abriendo una prueba interactiva desde el área Documentos de Workfront.
