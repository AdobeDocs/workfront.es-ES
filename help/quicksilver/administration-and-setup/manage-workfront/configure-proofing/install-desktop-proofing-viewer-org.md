---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Instalación del Visor de corrección de escritorio para su organización
description: Desktop Proofing Viewer, diseñado principalmente para revisar contenido interactivo, es una aplicación que debe instalarse en el equipo local de cada usuario. Como administrador de Adobe Workfront o de Workfront Proof, puede realizar esta instalación.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 5cc1acffff12d78e48228f3ae223514c0ff379ef
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Instalación del Visor de corrección de escritorio para su organización

<!--Audited: 05/2024-->

Desktop Proofing Viewer, diseñado principalmente para revisar contenido interactivo, es una aplicación que debe instalarse en el equipo local de cada usuario. Como administrador de Adobe Workfront o de Workfront Proof, puede realizar esta instalación.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Premium o Select</p> <p>Para obtener más información sobre la revisión del acceso con los diferentes planes, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Plan actual: Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe haber seleccionado Administrador en el perfil de permisos de revisión. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configuración del acceso de revisión de un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos del sistema

El Visor de corrección de escritorio es compatible con los siguientes sistemas operativos:

* Windows 7 y versiones posteriores, 32 y 64 bits
* Mac OS X 10.9 y posterior, 64 bits

## Requisitos previos

Para permitir que los usuarios usen el Visor de corrección de escritorio, debe configurar el sistema para iniciar el Visor de corrección de escritorio como la vista predeterminada para las pruebas interactivas antes de la instalación.

## Configure el Visor de corrección de escritorio como predeterminado para las pruebas interactivas

Después de instalar el Visor de corrección de escritorio para su organización, puede establecerlo como el visor predeterminado para las pruebas interactivas.

{{step1-to-proofing}}

1. Clic **Configuración de cuenta** situado cerca de la esquina superior derecha de Workfront Proof y, a continuación, haga clic en **Configuración** pestaña.

1. En **Valores predeterminados de revisión**, al final del **Visor de corrección de escritorio para revisión interactiva** fila, haga clic en **Configurar**.

   ![Valores predeterminados de revisión](assets/proof-defaults.png)

1. Clic **Habilitado y predeterminado**, luego haga clic en **Guardar**.

## Instalación del Visor de corrección de escritorio para los usuarios

* [Instalación del Visor de corrección de escritorio en Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Instalación del Visor de corrección de escritorio en Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Instalación del Visor de corrección de escritorio en Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. En el equipo del usuario, realice una de las siguientes acciones para descargar la aplicación:

   * Si está utilizando el entorno Producción, haga clic en [Descarga de producción de Mac para el visor de corrección de escritorio](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg).
   * Si está utilizando el entorno de vista previa, haga clic en [Descarga de vista previa de Mac para el visor de corrección de escritorio](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg).

1. Abra el archivo que acaba de descargar para iniciar la instalación.
1. Haga clic en el cuadro de instalación que aparece **Continuar**, luego haga clic en **Instalar**.

   ![Cuadro de instalación](assets/install-wf-proof-box.png)

1. Asegúrese de que cada usuario complete la instalación abriendo una prueba interactiva desde el área Documentos en Workfront.

### Instalación del Visor de corrección de escritorio en Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. En el equipo del usuario, realice una de las siguientes acciones para descargar la aplicación:

   * En el entorno Producción, haga clic en [Descarga de producción de Windows para el Visor de corrección de escritorio](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe).
   * En el entorno de vista previa, haga clic en [Descarga de Vista previa de Windows para el Visor de corrección de escritorio](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Abra el archivo que acaba de descargar para iniciar la instalación.
1. En el cuadro que aparece, haga clic en **Ejecutar**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   Se instala y ejecuta el Visor de corrección de escritorio.

1. (Condicional) Si instala la aplicación mediante Internet Explorer, actualice la página de inicio en el explorador después de que se instale la aplicación.
1. Asegúrese de que cada usuario complete la instalación abriendo una prueba interactiva desde el área Documentos en Workfront.
