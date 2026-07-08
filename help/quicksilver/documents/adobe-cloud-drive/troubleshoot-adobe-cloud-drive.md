---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Solucionar problemas de Adobe Cloud Drive
description: Revise las limitaciones, consideraciones de rendimiento y soluciones a problemas comunes con Adobe Cloud Drive en Mac y Windows.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 6ad89f8d00dd3a06eb160863c3213a9f80b1a44b
workflow-type: tm+mt
source-wordcount: 928
ht-degree: 0%

---

# Solucionar problemas de Adobe Cloud Drive

Este artículo describe las limitaciones de Adobe Cloud Drive, las consideraciones de rendimiento que se deben tener en cuenta y las soluciones a los problemas comunes que puede encontrar.

Para obtener información sobre cómo trabajar con Adobe Cloud Drive, consulte [Usar Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Limitaciones

### Operaciones de archivo y carpeta

* Las carpetas de proyecto son de sólo lectura en el nivel superior. No puede cambiarles el nombre, eliminarlos ni moverlos desde Adobe Cloud Drive. Para crear, cambiar el nombre o eliminar un proyecto, utilice la interfaz web de Workfront.
* Las operaciones de archivo y carpeta dentro de una carpeta de proyecto son totalmente compatibles.

### Límites de archivos y rutas

* Los nombres de archivo no pueden superar los 255 caracteres en ninguna plataforma.
* La ruta completa del archivo (todos los nombres de carpeta más el nombre de archivo) no puede superar los 1024 caracteres. Los archivos con rutas superiores a este límite no aparecen en Adobe Cloud Drive, aunque estén visibles en la interfaz web de Workfront.
* Si observa un error **Ruta de acceso completa demasiado larga** en un archivo, acorte los nombres de las carpetas o reduzca la profundidad de anidamiento de las carpetas para que la ruta se encuentre dentro del límite.

### Almacenamiento

* Los archivos guardados en Adobe Cloud Drive utilizan localmente el espacio en disco del dispositivo.
* Los archivos solo de nube no utilizan almacenamiento local.
* Elimine el acceso sin conexión a los archivos que ya no necesite. Para obtener más información, consulte [Quitar el acceso sin conexión para liberar espacio](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#remove-offline-access-to-free-up-space) en [Usar Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Consideraciones de rendimiento

* **Tamaño de archivo:** El tiempo necesario para la sincronización depende del tamaño del archivo. Los archivos más grandes suelen tardar más.
* **Velocidad de la red:** Las conexiones más rápidas proporcionan un mejor rendimiento de sincronización. La sincronización se reanuda automáticamente tras una interrupción.
* **Acceso por primera vez:** Los archivos se descargan bajo demanda la primera vez que se obtiene acceso a ellos. El acceso posterior es más rápido porque el archivo se almacena en caché localmente.

## Problemas comunes

### Adobe Cloud Drive no aparece.

**Causas posibles:**

* Adobe Cloud Drive no está instalado.
* La instalación no se completó correctamente.
* Su organización no tiene una versión de Workfront que admita el almacenamiento en la nube de Adobe.

**Soluciones:**

* Compruebe que Adobe Cloud Drive está instalado. Compruebe **Aplicaciones** (Mac) o **Programas** (Windows).
* Inicie Adobe Cloud Drive manualmente.
* Póngase en contacto con su administrador de Workfront para confirmar que su organización dispone de una versión de Workfront compatible con el almacenamiento en la nube de Adobe.
* Vuelva a instalar Adobe Cloud Drive si es necesario. Para obtener más información, consulte [Instalar Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

### El icono de Adobe Cloud Drive no está visible en la barra de menús o en la barra de tareas

**Causas posibles:**

* La barra de menús (Mac) o la bandeja del sistema (Windows) no tienen espacio suficiente para mostrar el icono.

**Soluciones:**

* **Mac:** Mantenga presionado Cmd y arrastre los iconos existentes de la barra de menús para reorganizarlos o quitarlos, creando espacio para el icono de Adobe Cloud Drive.
* **Windows:** Haz clic en la flecha hacia arriba (**Mostrar iconos ocultos**) en la barra de tareas para buscar el icono de Adobe Cloud Drive y, a continuación, arrástralo al área visible.

### Los proyectos no se muestran o faltan algunos proyectos

**Causas posibles:**

* No tiene acceso a ningún proyecto.
* La sincronización no se ha completado.
* Tiene un problema de conectividad de red.

**Soluciones:**

* Compruebe el acceso al proyecto en la interfaz web de Workfront.
* Compruebe la conexión de red.
* Cierre la sesión de Adobe Cloud Drive y vuelva a iniciarla.

### Los archivos no se están sincronizando

**Causas posibles:**

* Tiene un problema de conectividad de red.
* Hay un error de sincronización en el archivo o la carpeta.
* No tiene suficiente espacio en disco.

**Soluciones:**

* Compruebe la conexión a Internet.
* Compruebe que dispone de suficiente espacio en disco.
* Compruebe los indicadores de estado del archivo para ver si hay errores de sincronización. Para obtener más información, consulte [Indicadores de estado de archivos](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#file-status-indicators) en [Usar Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).
* Reinicie Adobe Cloud Drive.
* Compruebe el estado de Adobe Cloud Drive en la bandeja del sistema (Windows) o en la barra de menús (Mac).

### No puede abrir un archivo

**Causas posibles:**

* El archivo es solo de nube y se produjo un error en la descarga.
* La aplicación necesaria para abrir el archivo no está instalada.
* El archivo está dañado.

**Soluciones:**

* Compruebe el indicador de estado del archivo.
* Asegúrese de que está instalada la aplicación requerida.
* Haga clic con el botón derecho en el archivo, seleccione **Mantener siempre activado este dispositivo** e intente abrirlo de nuevo.
* Compruebe que el archivo no esté dañado en la interfaz web de Workfront.

### La sincronización es lenta

**Causas posibles:**

* El archivo es grande.
* La conexión de red es lenta.
* Se están sincronizando muchos archivos al mismo tiempo.

**Soluciones:**

* Tenga paciencia con los archivos grandes. La sincronización se puede reanudar, por lo que se reanuda desde el punto en el que se detuvo después de una interrupción.
* Compruebe la velocidad de la red.
* Limite el número de operaciones de archivo simultáneas.
* Mantenga los archivos grandes solo en la nube a menos que necesite acceso sin conexión.

### Los archivos sin conexión ocupan demasiado espacio

**Soluciones:**

* Haga clic con el botón derecho en los archivos sin conexión y seleccione **Espacio disponible**.
* Compruebe el espacio en disco regularmente.
* Mantenga los archivos grandes a los que raramente accede en el modo de solo nube.

### No puede crear, editar ni eliminar archivos o carpetas

**Causas posibles:**

* Está intentando crear, cambiar el nombre o eliminar una carpeta de proyecto. Las carpetas de proyecto son de sólo lectura en el nivel superior.
* El proyecto es de solo lectura, por lo que no puede crear, editar ni eliminar archivos o carpetas dentro de él.

**Soluciones:**

* Para crear, cambiar el nombre o eliminar un proyecto, utilice la interfaz web de Workfront.
* Pida al propietario del proyecto que comparta el proyecto con usted con acceso de edición.

## Obtener ayuda

Si tiene preguntas sobre la licencia, problemas de acceso al proyecto o una configuración específica de la organización, póngase en contacto con el administrador de Workfront.

Para compartir registros con la asistencia de Adobe, siga los pasos de [Ejecutar la herramienta de recopilación de registros de Adobe](https://helpx.adobe.com/creative-cloud/apps/troubleshoot/diagnostics-repair-tools/run-log-collector-tool.html).

## Prácticas recomendadas

* **Planificar trabajo sin conexión.** Descargue archivos antes de viajar o trabajar en áreas con mala conectividad.
* **Supervisar estado de sincronización.** Compruebe los indicadores de archivo antes de cerrar las aplicaciones.
* **Seguir la estructura de carpetas del proyecto.** Organice los archivos de las carpetas del proyecto como desee el propietario del proyecto.
* **Usar nombres de archivo descriptivos.** Ayude a los integrantes del equipo a encontrar lo que necesitan.
* **Evite crear duplicados.** No realice copias innecesarias de los archivos.
