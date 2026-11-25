---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Usar Adobe Cloud Drive
description: Trabaje con sus proyectos de almacenamiento en la nube de Adobe directamente desde el Finder o el Explorador de archivos mediante Adobe Cloud Drive. Abra y edite archivos en cualquier aplicación, trabaje sin conexión y resuelva conflictos.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 19e1a78a32429ddba173583bf56af8acc5d72eb0
workflow-type: tm+mt
source-wordcount: '3955'
ht-degree: 1%
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

### Sincronizar lista de exclusión

Adobe Cloud Drive excluye de la sincronización ciertos archivos temporales, de bloqueo y generados por el sistema. Se excluyen los siguientes tipos de archivo y patrones:

| Categoría | Tipos/patrones de archivo | Descripción |
|---|---|---|
| Archivos de sistema | `.DS_Store`, `Thumbs.db` | Metadatos del sistema operativo y archivos de caché de miniaturas. |
| Archivos de sistema y de memoria virtual | `*.sys` (por ejemplo, `hiberfil.sys`, `pagefile.sys`, `swapfile.sys`) | Archivos de sistema grandes utilizados para la memoria virtual, la hibernación u otras funciones del sistema operativo. |
| Archivos de indexación de macOS | `.Spotlight-V100`, `.fseventsd` | Indexación de macOS Spotlight y archivos de seguimiento de eventos del sistema de archivos. |
| Archivos temporales y de copia de seguridad | `*.tmp`, `*.swp`, `*~`, `*.bak` | Archivos temporales, transitorios o de copia de seguridad generados por las aplicaciones. |

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

<!-- Courtney check me: New sections below (Upload to Cloud through Open in Workfront) added for Adobe Cloud Drive v1.2.0, per helpxNewFeature.pdf from Pulkit Goel. Verify content, placement, and heading order. -->

## Carga de archivos en la nube (carga directa) {#direct-upload}

<!-- Courtney check me: Source PDF calls this "Upload to Cloud (Direct Upload)". Confirm heading wording. -->

La carga directa envía archivos desde el equipo directamente al almacenamiento en la nube de Adobe, sin copiarlos primero en la carpeta Adobe Cloud Drive.

<!-- Courtney check me: Removed folder mentions from the Direct Upload section (intro, heading, step 1, 500-file bullet, hidden files bullet, and the Sync Activity link text), per Pulkit: folder support isn't available yet. Confirm nothing else should change. -->

### Cargar archivos

1. Haga clic con el botón secundario en un archivo de Finder (Mac) o Explorador de archivos (Windows).
1. Seleccione **Cargar a la nube**.
1. En el selector de destino, seleccione una ubicación dentro de uno de los proyectos de Adobe Cloud Drive y, a continuación, haga clic en **Cargar aquí**.
1. Monitorice el progreso en la sección **Carga directa** de la ventana Actividad de sincronización.

### Aspectos que debe saber sobre la carga directa

* La carga directa copia el artículo en la nube. El elemento original permanece en su ubicación actual.
* Puede seleccionar varios elementos para cargarlos a la vez.
* La sección Carga directa solo enumera archivos individuales, hasta un máximo de 500.
* Puede cargar elementos desde el directorio de inicio del usuario o desde cualquier unidad externa conectada. No se admiten otras ubicaciones de almacenamiento en la nube, como iCloud Drive o `~/Library/CloudStorage`.
* Debe haber iniciado sesión con una cuenta de Adobe con derecho a. No necesita una conexión a Internet para iniciar una carga. Sin una conexión, las cargas permanecen en cola.
* Pausar la sincronización cancela las cargas que están en curso. Las cargas en cola se reanudan automáticamente al reanudar la sincronización.
* Si sale de Adobe Cloud Drive durante una carga, las cargas en curso se marcan como canceladas. Las cargas en cola se reanudan automáticamente al reiniciar la aplicación.
* Los archivos ocultos, los vínculos simbólicos y los alias no son compatibles.
* Adobe Cloud Drive controla cuántas cargas se ejecutan al mismo tiempo. Las cargas restantes permanecen en cola hasta que haya una ranura disponible.
* Se muestra un recuento activo de las cargas, incluidas las cargas fallidas, por ejemplo &quot;Carga de 3 archivos&quot;. Cuando todas las cargas se completan correctamente, el recuento cambia a un resumen como &quot;3 archivos cargados&quot;. Seleccione **Descartar** para eliminarlo.

<!-- Courtney check me: "Pausing sync cancels uploads in progress" and the quit behavior are from the PDF. Confirm with dev that both are intended. -->

### Estado de carga

<!-- Courtney check me: Icons extracted from the PDF (48x48 px, low resolution) and named by table order. Verify each icon matches its status and ask Pulkit's team for higher-resolution originals. Add alt text review too. -->

| Icono | Estado | Descripción | Acciones disponibles |
| --- | --- | --- | --- |
| ![Icono en cola](assets/acd-upload-status-queued.png) | En cola | La carga está esperando para iniciarse. | **Cancelar** cancela este elemento. |
| ![Icono de carga](assets/acd-upload-status-uploading.png) | Cargando... | La carga está en curso. | **Cancelar** cancela este elemento. |
| ![Icono completado](assets/acd-upload-status-completed.png) | Finalizado | La carga ha finalizado correctamente. | **Abrir en Workfront** abre el recurso en la interfaz web de Workfront. |
| ![Icono con error](assets/acd-upload-status-failed.png) | Error | No se ha podido completar la carga. | **Mostrar archivo de origen** revela el archivo original. **Reintentar** reintenta la carga. Reintentar solo está disponible para determinados errores. |
| ![Icono cancelado](assets/acd-upload-status-cancelled.png) | Cancelado | La carga se ha detenido, tanto por su parte como por el sistema. | Ninguno. Las cargas canceladas no se vuelven a intentar. Debe iniciar una nueva carga. |

Para ver el motivo de un error, pase el ratón sobre el elemento con error.

### Administrar la lista de carga

Cada acción solo está disponible cuando se aplica.

* **Cancelar todas las cargas:** Disponible cuando las cargas están en cola o en curso. Cancela todos ellos.
* **Reintentar cargas con errores:** disponible cuando existen cargas con errores que se pueden reintentar. Reintenta todos ellos. Las cargas que no se pueden reintentar permanecen sin cambios.
* **Borrar:** Disponible cuando no hay cargas en cola o en curso. Quita todos los elementos completados, fallidos y cancelados. Los archivos locales y el contenido ya cargado no se ven afectados.
* **Borrado automático:** los elementos completados, erróneos y cancelados se quitan automáticamente 24 horas después de su última actualización. Los elementos en cola y en curso nunca se quitan automáticamente.

## Pausar y reanudar la sincronización {#pause-resume-sync}

Puede pausar Adobe Cloud Drive cuando no desee que cargue o descargue archivos, por ejemplo, con una conexión a Internet lenta o con contador. Mientras la sincronización está en pausa, los cambios no se envían a la nube y no se descargan en el equipo. La sincronización permanece en pausa hasta que la reanuda.

### Pausar sincronización

1. Haga clic en el icono de Adobe Cloud Drive en la bandeja del sistema (Windows) o en la barra de menús (Mac).
1. Haga clic en el icono **Menú** (≡) en la esquina superior derecha de la ventana Adobe Cloud Drive.
1. Seleccionar **Pausar sincronización**.

   >[!TIP]
   >
   >Con la ventana Adobe Cloud Drive abierta, también puede presionar Ctrl+P (Windows) o Comando+P (Mac).

   La ventana de Adobe Cloud Drive muestra **La sincronización está en pausa** y el mensaje **Los archivos no se sincronizarán hasta que reanudes**. Cuando pasa el ratón sobre el icono de Adobe Cloud Drive, se muestra **Adobe Cloud Drive (en pausa)**.

>[!NOTE]
>
>La sincronización en pausa solo está disponible cuando ha iniciado sesión y Adobe Cloud Drive está conectado.

### Reanudar sincronización

1. Haga clic en el icono de Adobe Cloud Drive en la bandeja del sistema (Windows) o en la barra de menús (Mac).
1. Realice una de las siguientes acciones:

   * Haga clic en **Reanudar**.
   * Haga clic en el icono **Menú** (≡) y, a continuación, seleccione **Reanudar sincronización**. Con la ventana abierta, también puede presionar Ctrl+R (Windows) o Comando+R (Mac).

   Adobe Cloud Drive comienza a sincronizar de nuevo, incluidos los cambios realizados mientras la sincronización se detuvo.

## Ver y administrar el historial de versiones {#version-history}

Puede usar el Historial de versiones en Adobe Cloud Drive para examinar las versiones guardadas en la nube de un archivo compatible, ver los detalles de la versión y las miniaturas, y volver a una versión anterior. También puede editar el nombre y la descripción de una versión si dispone de los permisos necesarios.

### Ver historial de versiones

1. Navegue hasta la carpeta Adobe Cloud Drive en el Finder o el Explorador de archivos.
1. Seleccione un archivo compatible.
1. Haga clic con el botón derecho en el archivo y seleccione **Historial de versiones**.
1. Seleccione una versión para ver los detalles y las miniaturas disponibles.

   Si el archivo no tiene versiones anteriores, se muestra **No hay versiones anteriores**. Es posible que las miniaturas no estén disponibles para cada archivo o versión.

### Editar información de versión

1. Abra el Historial de versiones del archivo.
1. Seleccione la versión que desee actualizar.
1. Abra el menú de opciones de la versión y seleccione **Editar información de versión**.
1. Escriba un **nombre de versión** o **descripción**.
1. Seleccione **Guardar**.

   La información actualizada se guarda y aparece cuando se vuelve a abrir el Historial de versiones.

### Revertir a una versión anterior

1. Abra el Historial de versiones del archivo.
1. Seleccione la versión que desea restaurar.
1. Seleccione **Revertir a esta versión**, si está disponible.
1. Espere a que se complete la sincronización.
1. Vuelva a abrir el archivo para comprobar que el contenido de la versión seleccionada está actualizado.

## Administración del almacenamiento local {#manage-local-storage}

Puede usar Administrar almacenamiento local en Adobe Cloud Drive para supervisar el uso del disco local, establecer un límite de almacenamiento y ver los archivos marcados como **Siempre en este dispositivo**.

<!-- Courtney check me: PDF says "Always on this device" here but this article uses "Always Keep On This Device" for the right-click option. Confirm which label the UI shows in each place. -->

### Ver uso del almacenamiento local

1. Seleccione el icono Adobe Cloud Drive y abra su menú de opciones.
1. Seleccione **Administrar almacenamiento local**.
1. Revise el uso actual del almacenamiento y la lista de archivos marcados como **Siempre en este dispositivo**.
1. Ordene la lista de archivos por **Nombre** o **Tamaño** para encontrar archivos específicos.

### Cambio del límite de almacenamiento local

1. Abra **Administrar almacenamiento local** desde el menú de opciones de Adobe Cloud Drive.
1. Introduzca el límite de almacenamiento deseado.
1. Seleccione **Guardar** para aplicar el cambio.

>[!NOTE]
>
>Asegúrese de que haya suficiente espacio libre en disco disponible en el dispositivo cuando establezca el límite de almacenamiento.

## Ver actividad de sincronización {#sync-activity}

La actividad de sincronización muestra la actividad reciente entre la carpeta Adobe Cloud Drive del equipo y el almacenamiento en la nube de Adobe. Utilícelo para supervisar las cargas y descargas, revisar los cambios completados e identificar los elementos que no se pudieron sincronizar.

### Ver actividad de sincronización

1. Seleccione el icono Adobe Cloud Drive en la barra de menús (Mac) o en la bandeja del sistema (Windows).
1. Expanda la sección de actividad de sincronización mediante la flecha situada junto al resumen de estado.
1. Revise los elementos enumerados y sus indicadores de estado. Pase el ratón sobre un indicador de estado para ver el progreso de la transferencia, la operación completada o un mensaje de error.
1. Seleccione el menú más acciones situado junto a un elemento para ver las acciones disponibles para dicho elemento.

### Cosas que hay que saber sobre Sync Activity

* La sincronización normal realiza un seguimiento de los cambios realizados a través de la carpeta Adobe Cloud Drive, incluidas las cargas, las descargas, las creaciones, los cambios de nombre, los movimientos y las eliminaciones.
* La lista de sincronización normal contiene hasta 500 entradas recientes. Las entradas nuevas o actualizadas aparecen en la parte superior. Las entradas más antiguas pueden eliminarse a medida que la lista alcanza su límite.
* Una entrada puede mostrar inicialmente **Preparando...** mientras se resuelve su nombre o metadatos.
* El resumen muestra el número de elementos que se están sincronizando actualmente. **Sincronización completa** significa que no hay elementos activos en este momento. Inspeccione la lista en busca de elementos fallidos o excluidos, en lugar de tratar este resumen como una confirmación de que cada elemento se ha realizado correctamente.
* Los archivos y carpetas excluidos de la sincronización pueden aparecer con un error que explica el nombre no admitido, el tipo no admitido u otro motivo de exclusión.
* La actividad se borra al cerrar la sesión. La lista es una vista de actividad, no un historial de auditoría permanente.

### Estado de sincronización

<!-- Courtney check me: The PDF has two sync status tables (page 7 with 4 statuses, page 8 with 3 statuses and icons). I used the page 8 icons with the page 7 descriptions where they overlap. Confirm and decide whether to keep both tables. -->

| Icono | Estado | Descripción | Acciones disponibles |
| --- | --- | --- | --- |
| Indicador de espera | Esperando a sincronizarse | El elemento está esperando a que comience su operación. | **Mostrar en Finder** (Mac) o **Mostrar en Explorer** (Windows), donde corresponda. |
| ![Icono de carga](assets/acd-sync-status-uploading.png) | Carga/Descarga | Se está transfiriendo el contenido del archivo. Pase el ratón sobre el indicador para ver la dirección de transferencia y el porcentaje cuando estén disponibles. Al 100%, la información sobre herramientas podría mostrar **Finalizando...** hasta que finalice el procesamiento. | **Mostrar en Finder** o **Mostrar en Explorer**, donde corresponda. |
| ![Icono completado](assets/acd-sync-status-completed.png) | Operación sincronizada/completada | Se completó la operación. La información del objeto puede identificar Cargado, Descargado, Creado, Cambiado de nombre, Cambiado de nombre en la nube, Movido, Eliminado o Eliminado en la nube. | **Mostrar en Finder** o **Mostrar en Explorer** para elementos no eliminados. **Abrir en Workfront** para elementos calificados, completados y no eliminados. |
| ![Icono con error](assets/acd-sync-status-failed.png) | Error/exclusión de sincronización | El elemento no se pudo sincronizar o se ha excluido de la sincronización. Pase el ratón sobre el indicador del motivo. | **Mostrar en Finder** o **Mostrar en Explorer**, donde corresponda. Resuelva el problema del que se ha informado antes de esperar que se sincronice el elemento. |

Los elementos eliminados no se pueden mostrar localmente ni abrir en Workfront desde la entrada de su actividad.

### Administración de la lista de actividades

| Acción | Descripción |
| --- | --- |
| Expandir o contraer | Utilice la flecha situada junto al resumen de sincronización para mostrar u ocultar entradas individuales. |
| Mostrar en el buscador / Mostrar en el explorador | Busque un elemento no eliminado en la carpeta Adobe Cloud Drive. |
| Abrir en Workfront | Abre un artículo completado que cumpla los requisitos en Workfront en tu navegador. Esta acción no está disponible para entradas de sincronización normal activas, con errores o eliminadas. |
| Borrar | Disponible cuando no hay elementos de sincronización normales activos. Borra las entradas finalizadas, incluidas las entradas con errores, de la vista de actividad. Borrar el historial no elimina los archivos locales ni el contenido de la nube y no resuelve un error de sincronización. |
| Descartar | Después de borrar un lote completado, es posible que se muestre un resumen de elementos sincronizados. Seleccione el botón Cerrar para cerrar el resumen. |

>[!NOTE]
>
>Las filas de sincronización normal no proporcionan las acciones **Reintentar** o **Cancelar** por elemento que usa la carga directa. Para obtener información sobre la carga directa, consulte [Cargar archivos a la nube (carga directa)](#direct-upload).

## Abrir un elemento en Workfront {#open-in-workfront}

Abrir en Workfront le lleva desde un elemento de Adobe Cloud Drive a su ubicación correspondiente en Workfront en el explorador. Utilícelo para seguir trabajando con el elemento de nube en Workfront sin buscarlo manualmente.

### Abrir un elemento desde Finder o el Explorador de archivos

1. Abra la carpeta Adobe Cloud Drive en Finder (Mac) o el Explorador de archivos (Windows).
1. Seleccione un solo archivo o carpeta asociado a un elemento de Workfront.
1. Haga clic con el botón derecho en el elemento y seleccione **Abrir en Workfront**.

   El explorador abre la ubicación de Workfront correspondiente. Si se le solicita, inicie sesión con una cuenta que tenga acceso a ese elemento.

### Abrir un elemento desde Actividad de sincronización

1. Seleccione el icono Adobe Cloud Drive en la barra de menús (Mac) o en la bandeja del sistema (Windows).
1. Expanda la sección de actividad de sincronización.
1. Para un elemento elegible completado y no eliminado, abre el menú de más acciones y selecciona **Abrir en Workfront**.
1. Para un archivo cargado mediante carga directa, use la misma acción en la entrada completada en la sección **Carga directa**.

### Cosas que hay que saber sobre Open en Workfront

* Seleccionar solo un elemento a la vez. No se admite la apertura de varios elementos seleccionados en Workfront.
* En el Explorador de archivos, el comando está oculto para los elementos que no están en la carpeta de Adobe Cloud Drive y para la propia raíz de la unidad. Se desactiva cuando se seleccionan varios elementos.
* Un elemento debe tener una ubicación de Workfront correspondiente. Es posible que algunas carpetas u otros elementos no tengan una asignación de Workfront, aunque estén visibles en Adobe Cloud Drive.
* Es posible que un nuevo elemento local que no haya terminado de cargarse aún no tenga un vínculo de Workfront. Espere a que se complete la carga antes de intentarlo de nuevo.
* En la actividad de sincronización normal, la acción se ofrece solo para las entradas completadas aptas. No se ofrece para entradas activas, fallidas o eliminadas.
* En la carga directa, la acción se ofrece para cargas completadas, no para entradas en cola, de carga, fallidas o canceladas.
* Debe iniciar sesión en Adobe Cloud Drive. Workfront también puede pedirle que inicie sesión por separado en el explorador, y los permisos de Workfront seguirán aplicándose.
* Necesita una conexión a Internet para recuperar un vínculo no almacenado en caché y acceder a Workfront. Un vínculo resuelto anteriormente no proporciona acceso sin conexión a Workfront.
* Esta acción abre Workfront en un explorador. No abre el archivo en su aplicación de escritorio, no carga otra copia ni cambia su disponibilidad local sin conexión.

### Abrir en Disponibilidad de Workfront

| Elemento o estado | Comportamiento de Abrir en Workfront | Qué hacer |
| --- | --- | --- |
| Un solo artículo apto en Adobe Cloud Drive | Abre la ubicación de Workfront correspondiente. | Seleccione **Abrir en Workfront**. |
| Varios elementos seleccionados | No se admite la apertura de varios elementos. El Explorador de archivos desactiva el comando. | Seleccione un solo elemento. |
| El nuevo elemento se sigue cargando | Es posible que el vínculo de Workfront aún no esté disponible. | Espere a que se complete la carga e inténtelo de nuevo. |
| Entrada de sincronización normal finalizada | Disponible cuando el artículo cumple los requisitos y no se ha eliminado. | Utilice el menú de más acciones de la entrada. |
| Entrada de carga directa completada | Disponible una vez finalizada la carga. | Utilice el menú de más acciones de la entrada. |
| Elemento sin asignación de Workfront | Un mensaje indica que el elemento no está disponible en Workfront. | Compruebe el elemento directamente en Workfront o elija otro elemento compatible. |
| Entrada de sincronización normal eliminada | La acción no está disponible. | Utilice Workfront directamente si necesita investigar el elemento eliminado. |

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

