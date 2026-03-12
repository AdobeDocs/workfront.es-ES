---
product-area: documents
navigation-topic: approvals
title: Permisos de objeto e información general del nivel de acceso para el modelo de almacenamiento empresarial de Adobe
description: Información general sobre permisos y acceso al almacenamiento empresarial de Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
source-git-commit: 522175549d1a2b19c9e6a47a7e4b0d63ac08e3a3
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 2%

---

# Permisos de objeto e información general del nivel de acceso para el modelo de almacenamiento empresarial de Adobe

<!--linked in UI -->

El almacenamiento empresarial de Adobe es una solución de almacenamiento basada en la nube que sirve como repositorio de almacenamiento central para los recursos de los productos empresariales de Adobe. Los entornos de Workfront que utilizan el almacenamiento empresarial de Adobe tienen permisos de objeto y comportamientos de nivel de acceso ligeramente diferentes a los que utilizan el almacenamiento de documentos de Workfront heredado.

## Niveles de acceso

Los niveles de acceso de Workfront solo se aplican en Workfront. Las restricciones de proyectos y documentos dentro de Workfront no siempre se aplican a otras aplicaciones de Adobe.

### Entornos que utilizan almacenamiento empresarial de Adobe y almacenamiento heredado de Workfront

El acceso a los documentos se comporta de forma diferente en función de si el proyecto se encuentra en el almacenamiento empresarial de Adobe o en el almacenamiento de Workfront heredado:

* **Almacenamiento heredado de Workfront**: Los proyectos, programas, portafolios y plantillas que usan almacenamiento heredado de Workfront siguen la lógica estándar de nivel de acceso de Workfront para el acceso a documentos. Cuando un nivel de acceso tiene **Sin acceso** seleccionado para documentos, no puede ver documentos en Workfront u otros productos de Adobe como Frame.io o Creative Cloud.
* **almacenamiento empresarial de Adobe**: Los proyectos, programas, portafolios y plantillas que usan el almacenamiento empresarial de Adobe siguen la lógica de nivel de acceso al almacenamiento empresarial de Adobe para otros productos de Adobe.


   * **Permisos de objetos de proyectos, programas, portafolios y plantillas**: cuando un nivel de acceso tiene **Sin acceso** seleccionado para proyectos, programas, portafolios y plantillas, pero el objeto se comparte con ellos, los usuarios no pueden ver el objeto en Workfront, pero pueden ver el nombre del objeto y cualquier documento asociado en otras herramientas de Adobe, como Frame.io y Adobe Creative Cloud.
   * **Permisos de documentos**: cuando se selecciona un nivel de acceso de **Sin acceso** para los documentos, los usuarios no pueden ver los documentos de los proyectos de Workfront, pero sí pueden ver y administrar los documentos de los proyectos compartidos con ellos en otras herramientas de Adobe, como Frame.io y Adobe Creative Cloud. Esto se debe a que el acceso a los documentos está determinado por los permisos de nivel de proyecto en el almacenamiento empresarial de Adobe, en lugar de hacerlo solo por los niveles de acceso de Workfront.

Si tiene habilitado el almacenamiento empresarial de Adobe en su entorno de Workfront, puede crear proyectos de almacenamiento empresarial de Adobe y proyectos de almacenamiento de Workfront heredados. Los proyectos de almacenamiento de Workfront heredados muestran un icono junto al nombre del proyecto siempre que se muestre en Workfront. Los proyectos de almacenamiento empresarial de Adobe no muestran ningún icono.

![icono de almacenamiento de workfront heredado junto al nombre del proyecto](assets/legacy-project-icon.png)


### Entornos que solo utilizan almacenamiento empresarial de Adobe

No puede modificar los permisos de documento en el nivel de acceso para proyectos, programas y portafolios que utilizan Adobe Enterprise Storage.

Todos los niveles de acceso tienen acceso de edición a los documentos. Los permisos de nivel de proyecto determinan el acceso a documentos en otras herramientas de Adobe.

No puede restringir el acceso a la herencia de documentos.


### Entornos que solo utilizan almacenamiento heredado de Workfront

No hay cambios en los niveles de acceso a documentos ni en el comportamiento.

## Permisos de objeto

Los permisos de objetos determinan lo que se puede ver y hacer con proyectos, tareas, problemas y documentos en Workfront. Los permisos se asignan cuando alguien comparte un objeto con usted.

>[!IMPORTANT]
>
>En el almacenamiento empresarial de Adobe, los permisos de documento funcionan de forma diferente que en el almacenamiento heredado de Workfront. Los documentos heredan los permisos del proyecto, la tarea o el problema al que están vinculados.


### Funcionamiento de los permisos de documento

Los permisos de documento los controla el objeto al que está vinculado el documento. No puede establecer permisos en documentos individuales.

Al cargar un documento en una tarea o un problema, se crea una carpeta generada por el sistema con el nombre de la tarea o el problema. Esta carpeta está vinculada a la tarea o al problema y hereda sus permisos.

Puede crear subcarpetas dentro de la carpeta generada por el sistema para organizar aún más los documentos. Todas las subcarpetas heredan los permisos de la carpeta principal. En el nivel de proyecto, puede cargar documentos fuera de una carpeta, pero solo los usuarios con acceso en el nivel de proyecto pueden verlos.

En el nivel de proyecto, las carpetas generadas por el sistema muestran un objeto vinculado. Normalmente, es el nombre de la tarea o del problema y así es como el sistema sabe en qué tarea o problema debe verse la carpeta.

### Permisos de proyecto

Cuando tenga permisos en el nivel de proyecto, podrá ver y administrar los documentos de ese proyecto en Workfront y en otros productos de Adobe como Frame.io y Adobe Creative Cloud. El nombre del proyecto también es visible en esas herramientas. Otros datos del proyecto no son visibles fuera de Workfront.

### Permisos de tareas y problemas

Las tareas y los problemas heredan los permisos del proyecto. Cuando tenga permisos de nivel de tarea o problema, puede ver y administrar documentos vinculados a esa tarea o problema en Workfront y otros productos de Adobe como Frame.io y Adobe Creative Cloud.

**Carpetas generadas por el sistema**

* Al eliminar usuarios de una tarea o un problema, no se elimina automáticamente el acceso a sus carpetas. Todavía pueden tener acceso a través de permisos de nivel de proyecto.
* Las subtareas no heredan los permisos de carpeta generados por el sistema de las tareas principales. Debe ser agregado directamente a una subtarea para acceder a su carpeta generada por el sistema.
* Al agregar usuarios a una tarea o un problema, se comparte con ellos la carpeta generada por el sistema del objeto.

**Mover y cambiar el nombre de las carpetas generadas por el sistema:**

* Las carpetas generadas por el sistema se pueden mover y cambiar de nombre.
* Si una carpeta generada por el sistema se mueve a otra ubicación, su objeto vinculado se actualiza al nuevo objeto. A continuación, los permisos se heredan del nuevo objeto principal.

Las solicitudes siguen el mismo comportamiento que las tareas y los problemas.

### Aprobaciones

Cuando se le agrega a un flujo de trabajo de aprobación de documentos, puede ver lo siguiente independientemente de los permisos del proyecto:

* Nombre del proyecto
* Nombre de documento
* Miniatura del documento










