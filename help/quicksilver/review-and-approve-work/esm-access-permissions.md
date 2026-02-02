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
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 1%

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


## Proyectos

Los usuarios con permisos de nivel de proyecto pueden ver y administrar documentos para proyectos en otros productos de Adobe como Frame.io y Adobe Creative Cloud.

Los nombres de proyecto también son visibles fuera de Workfront para proyectos de ESM.

Los datos financieros no son visibles fuera de Workfront para proyectos de ESM.

## Tareas y problemas

Los documentos se almacenan en el nivel de proyecto, pero se pueden compartir con tareas y problemas individuales según sea necesario. Los usuarios con acceso a tareas y problemas heredan automáticamente el acceso a documentos del proyecto. No puede modificar su nivel de acceso. Tienen acceso de administración o no tienen acceso.