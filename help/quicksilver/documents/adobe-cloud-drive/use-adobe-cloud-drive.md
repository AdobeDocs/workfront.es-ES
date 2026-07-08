---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Usar Adobe Cloud Drive
description: Trabaje con sus proyectos de almacenamiento en la nube de Adobe directamente desde el Finder o el Explorador de archivos mediante Adobe Cloud Drive. Abra y edite archivos en cualquier aplicación, trabaje sin conexión y resuelva conflictos.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: d5dd769447e81d5d95b4907f8a01016b118f2322
workflow-type: tm+mt
source-wordcount: 1723
ht-degree: 2%

---

# Usar Adobe Cloud Drive

Después de instalar Adobe Cloud Drive, puede trabajar con sus proyectos de almacenamiento en la nube de Adobe directamente desde el Finder o el Explorador de archivos. Puede abrir y editar archivos en cualquier aplicación, trabajar sin conexión y permitir que Adobe Cloud Drive sincronice sus cambios con la nube.

Para obtener información acerca de la instalación de Adobe Cloud Drive, consulte [Instalar Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versión de Adobe Workfront</td> 
   <td>Flujo de trabajo de Ultimate, con Adobe Cloud Storage habilitado</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>
      <p>Ver el acceso a un proyecto para verlo en Adobe Cloud Drive</p>
      <p>Editar el acceso a un proyecto para agregar, editar o eliminar archivos</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acceso a sus proyectos

1. Abra Finder (Mac) o el Explorador de archivos (Windows).
1. Vaya a **Adobe Cloud Drive**.
1. Examine la lista de proyectos a los que tiene acceso en Workfront. Abra cualquier carpeta del proyecto para ver sus archivos y subcarpetas.

   >[!NOTE]
   >
   >* Las carpetas de proyecto son de sólo lectura en el nivel superior. No puede cambiar el nombre, eliminar ni mover las carpetas del proyecto por sí mismas.
   >* Puede trabajar con archivos y carpetas dentro de una carpeta de proyecto: abrir, editar, crear, eliminar, etc.
   >* Los proyectos de Workfront heredados no aparecen en Adobe Cloud Drive. Solo están disponibles los proyectos almacenados en Adobe Cloud Storage.

## Indicadores de estado de archivo

Adobe Cloud Drive utiliza indicadores visuales para mostrar el estado de sincronización de archivos. Los iconos difieren entre Windows y Mac.

### Indicadores de estado de archivos en Windows

| Icono | Estado | Significado del archivo | Significado de carpeta |
| --- | --- | --- | --- |
| ![Icono de solo conexión](assets/acd-windows-online-only.png) | Solo en línea | El archivo está sincronizado, pero solo está disponible en línea. | Todos los archivos que contiene están disponibles en línea. |
| ![Icono de sincronización](assets/acd-windows-syncing.png) | Sincronizando | Las últimas actualizaciones del archivo se están sincronizando con la caché local o con el almacenamiento en la nube de Adobe. | Al menos un archivo de la carpeta se está sincronizando. |
| ![Icono sin conexión disponible](assets/acd-windows-available-offline.png) | Disponible sin conexión | El archivo está sincronizado y disponible sin conexión. | Al menos un archivo de la carpeta está disponible sin conexión. |
| ![Icono anclado](assets/acd-windows-pinned.png) | Anclado (mantener siempre en el dispositivo) | El archivo se sincroniza y siempre se mantiene sin conexión. Adobe Cloud Drive no purga el contenido anclado automáticamente. | Todos los archivos de la carpeta están en la caché local y disponibles sin conexión. |
| ![Icono de solo lectura](assets/acd-windows-read-only.png) | Solo lectura | El archivo es de solo lectura. | La carpeta es de solo lectura. |
| ![Icono de error de sincronización](assets/acd-windows-sync-error.png) | Error de sincronización | El archivo no se puede sincronizar. Pase el ratón sobre el icono para obtener más información. | La carpeta no se puede sincronizar. Pase el ratón sobre el icono para obtener más información. |
| ![Icono de sincronización excluida](assets/acd-windows-sync-excluded.png) | Sincronización excluida | El archivo no se puede sincronizar debido a un tipo o nombre no compatible. | La carpeta no se puede sincronizar debido a un nombre no compatible. |

### Indicadores de estado de archivos en Mac

| Icono | Estado | Significado del archivo | Significado de carpeta |
| --- | --- | --- | --- |
| (Sin icono) | Disponible sin conexión | El archivo está sincronizado y disponible sin conexión. | Todos los archivos están disponibles sin conexión. |
| ![Icono de solo conexión](assets/acd-mac-online-only.png) | Solo en línea | El archivo está sincronizado y solo está disponible en línea. | Al menos un archivo de la carpeta está en línea. |
| ![Icono de sincronización](assets/acd-mac-syncing.png) | Sincronizando | Las últimas actualizaciones del archivo se están sincronizando con la caché local o con el almacenamiento en la nube de Adobe. | Se está sincronizando el contenido de la carpeta. |
| ![Icono de error de sincronización](assets/acd-windows-sync-error.png) | Error de sincronización | El archivo no se puede actualizar ni sincronizar. Pase el ratón sobre el icono para obtener más información. | La carpeta no se puede actualizar ni sincronizar. Pase el ratón sobre el icono para obtener más información. |
| ![Icono de sincronización excluida](assets/acd-windows-sync-excluded.png) | Sincronización excluida | El archivo no se puede sincronizar. | La carpeta se excluye de la sincronización. |
| ![Icono de solo lectura](assets/acd-mac-read-only.png) | Solo lectura | El archivo es de solo lectura. | La carpeta es de solo lectura. |
| ![Icono anclado](assets/acd-windows-pinned.png) | Anclado (mantener siempre en el dispositivo) | El archivo está anclado para estar disponible sin conexión. Adobe Cloud Drive no purga el contenido anclado automáticamente. | La carpeta está anclada para estar disponible sin conexión. |

### Información sobre herramientas de error

Cuando se produzca un error de sincronización o un problema, pase el ratón sobre el icono del archivo o la carpeta para ver información sobre herramientas que describa el problema.

| Categoría de error | Ventana de ayuda contextual | Significado |
|---|---|---|
| Sincronización excluida | Tipo de archivo no compatible | Adobe Cloud Drive no admite el tipo de archivo. |
| Sincronización excluida | Nombre de archivo no compatible | Adobe Cloud Drive no admite el nombre de archivo. |
| Sincronización excluida | Proyecto principal eliminado | Se ha eliminado el proyecto principal de Workfront. |
| Sincronización suspendida | Contenido de archivo no admitido | No se puede sincronizar el contenido del archivo (por ejemplo, se detectó un problema de seguridad). |
| Sincronización suspendida | Caracteres no válidos en el nombre de archivo | El nombre de archivo contiene caracteres no válidos. |
| Sincronización suspendida | Ruta de acceso completa demasiado larga | La ruta del archivo supera la longitud máxima permitida. |
| Sincronización suspendida | Sin permiso de escritura | Se ha revocado su acceso de escritura a este archivo o proyecto. |
| Error de sincronización | Problema de autenticación | Hay un problema con sus credenciales de inicio de sesión. |
| Error de sincronización | Almacenamiento en la nube no disponible | Los servicios en la nube de Adobe no están disponibles temporalmente. |
| Error de sincronización | Almacenamiento en la nube completo | La cuota de almacenamiento en la nube está llena. |
| Error de sincronización | Disco local lleno | El disco local no tiene suficiente espacio libre. |
| Error de sincronización | Sin conexión a Internet | El dispositivo no está conectado a Internet. |
| Error de sincronización | Error inesperado | Error inesperado durante la sincronización. |
| Error de sincronización | Cuenta bloqueada | El servicio ha bloqueado su cuenta. |

>[!NOTE]
>
>Los errores de nivel de sistema, como desconectado, error de autenticación, red no disponible, disco local lleno o almacenamiento en la nube lleno, se muestran en la bandeja del sistema (Windows) o en la barra de menús (Mac), no en archivos individuales.

## Abrir un archivo

1. En Adobe Cloud Drive, vaya al archivo.
1. Haga doble clic en el archivo.

   El archivo se abre en su aplicación predeterminada.

Adobe Cloud Drive admite cualquier tipo de archivo que pueda abrir una aplicación instalada en el equipo, como:

* Formatos de Adobe Creative Cloud (PSD, AI, INDD, PROJ, AEP, etc.)
* Documentos de Microsoft Office (DOCX, XLSX, PPTX)
* Imágenes (JPG, PNG, GIF, etc.)
* Archivos de vídeo (MP4, MOV, etc.)

>[!NOTE]
>
>Los formatos de documentos de la nube (PSDC, AIDC, etc.) se abren como sus equivalentes estándar (PSD, AI, etc.) al acceder a ellos a través de Adobe Cloud Drive.

## Edición y guardado de un archivo

1. Abra un archivo desde Adobe Cloud Drive.
1. Realice los cambios en la aplicación.
1. Guarde el archivo seleccionando **Archivo** > **Guardar** o presionando Ctrl+S (Windows) o Cmd+S (Mac).

   Los cambios se sincronizan automáticamente con el almacenamiento en la nube de Adobe.

>[!IMPORTANT]
>
>Guardar archivos usando **Archivo** > **Guardar** o el método abreviado de teclado. Evite usar **Guardar como** para crear copias, ya que genera archivos duplicados en la unidad.

## Crear o agregar un nuevo archivo

Puede crear un nuevo archivo directamente en un proyecto o agregar un archivo existente del almacenamiento local.

### Crear un nuevo archivo desde una aplicación

1. Abra la aplicación que desee utilizar para crear el archivo.
1. Cree el archivo como lo haría normalmente.
1. Cuando guarde, elija una ubicación dentro de una carpeta de proyecto de Adobe Cloud Drive.

   El archivo aparece en Adobe Cloud Drive y se sincroniza con el almacenamiento en la nube de Adobe.

### Agregar un archivo existente a un proyecto

1. En Finder (Mac) o el Explorador de archivos (Windows), abra la carpeta del proyecto en Adobe Cloud Drive.
1. Arrastre o copie archivos del almacenamiento local a la carpeta del proyecto.

   Los archivos se sincronizan automáticamente con el almacenamiento en la nube de Adobe.

## Hacer que los archivos y carpetas estén disponibles sin conexión

Cuando un archivo o carpeta está disponible sin conexión, puede abrirlo y editarlo sin conexión a Internet. Los archivos sin conexión utilizan espacio en disco local.

### Mantener un archivo o una carpeta en el dispositivo

1. Haga clic con el botón derecho en el archivo o la carpeta en Adobe Cloud Drive.
1. Seleccione **Mantener siempre en este dispositivo**.

   El archivo o la carpeta se descarga en la caché local y puede trabajar con él incluso cuando esté sin conexión.

### Eliminar el acceso sin conexión para liberar espacio

1. Haga clic con el botón secundario en el archivo o carpeta sin conexión.
1. Seleccione **Espacio Libre**.

   El archivo o la carpeta permanece en el almacenamiento de la nube, pero se elimina de la caché local.

>[!NOTE]
>
>Los archivos y carpetas sin conexión utilizan el espacio en disco local. Elimine el acceso sin conexión a los archivos y carpetas que ya no necesita para liberar espacio.

## Copiar un archivo en el almacenamiento local

Puede copiar un archivo de Adobe Cloud Drive en la unidad local. El original permanece en Adobe Cloud Drive y la copia se convierte en un archivo local independiente.

1. Haga clic con el botón derecho en el archivo en Adobe Cloud Drive.
1. Seleccione **Copiar** y pegue el archivo en la ubicación de la unidad local donde lo desee.

   El archivo se copia en el destino. El original permanece en Adobe Cloud Drive.

>[!NOTE]
>
>Los archivos copiados en el almacenamiento local son copias independientes. Los cambios que realice en una copia local no se sincronizan con el almacenamiento en la nube de Adobe.

## Cerrar sesión en Adobe Cloud Drive

Si cierra sesión en Adobe Cloud Drive, la unidad permanecerá visible en Finder o en el Explorador de archivos. Sin embargo, los cambios que realice dentro de la unidad mientras esté cerrada la sesión y los que no se hayan sincronizado antes de cerrarla no se sincronizarán con la nube.

Lo que sucede a continuación depende de la cuenta con la que vuelva a iniciar sesión.

### Volver a iniciar sesión con la misma cuenta

Adobe Cloud Drive conserva la carpeta montada local cuando cierra la sesión. Si vuelve a iniciar sesión con las mismas credenciales:

* Adobe Cloud Drive reutiliza el montaje existente automáticamente.
* Se conservarán los cambios no sincronizados que haya realizado antes de cerrar la sesión y se sincronizarán una vez restaurada la conexión.
* No es necesario que realice ninguna acción.

### Iniciar sesión con una cuenta diferente

Si inicia sesión con una cuenta de Adobe diferente después de cerrar la sesión:

* Se cambiará automáticamente el nombre de la carpeta montada actual y se hará una copia de seguridad de ella. El nombre de la carpeta de copia de seguridad utiliza este formato: `Adobe Cloud Drive <usermail>_<short_guid> (backup yyyy-MM-dd HH-mm-ss)`.
* La unidad de nube de Adobe asignada a la nueva cuenta está disponible en el Finder o en el Explorador de archivos como de costumbre.
* Puede recuperar manualmente cualquier trabajo no sincronizado de la carpeta de copia de seguridad antes de quitarla.

>[!NOTE]
>
>Las carpetas de copia de seguridad se guardaron en `~/Library/CloudStorage` en Mac y en `C:\Users\<user>\` en Windows. Si cambia de cuenta varias veces, se crearán varias carpetas de copia de seguridad con marca de hora. Revise y limpie copias de seguridad periódicamente para liberar espacio en disco.

## Resolver conflictos de archivos

Los conflictos pueden producirse en cualquiera de las siguientes situaciones:

* Varios usuarios editan o eliminan el mismo archivo al mismo tiempo.
* Se modifica un archivo mientras otro usuario lo tiene abierto.
* Las interrupciones de red causan problemas de sincronización.

### Solución de conflictos con Adobe Cloud Drive

Adobe Cloud Drive utiliza una estrategia de duplicación para los conflictos:

* **Sin bloqueo de archivos.** Varios usuarios pueden editar archivos al mismo tiempo.
* **Duplicación automática.** Cuando Adobe Cloud Drive detecta un conflicto, conserva ambas versiones.
* **Borrar nombre.** Los archivos de conflicto incluyen el nombre de usuario y la marca de tiempo en este formato: `filename (Conflicted copy from username on date_time).extension`. Por ejemplo, `hero-banner (Conflicted copy from John on 2026-02-10_16-06-44).psd`

### Resolución manual de un conflicto

1. Identifique el archivo en conflicto. Los archivos de conflicto tienen &quot;copia en conflicto&quot; en el nombre del archivo.
1. Revise ambas versiones para determinar cuál es la correcta.
1. Conserve la versión correcta y elimine la otra versión.
1. Asigne un nombre adecuado al archivo retenido.

>[!TIP]
>
>Para minimizar los conflictos:
>
>* Compruebe el estado de sincronización antes de editar los archivos.
>* Comuníquese con los integrantes del equipo para saber quién está editando qué archivos.
>* Guardar con frecuencia para que los cambios se sincronicen rápidamente.
>* Cierre los archivos cuando termine de editar.
