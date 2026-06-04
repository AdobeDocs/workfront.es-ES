---
product-area: documents
navigation-topic: approvals
title: Permisos de objetos e información general del nivel de acceso para el modelo de almacenamiento en la nube de Adobe
description: 'permisos de almacenamiento en la nube Adobe y acceso: información general'
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ckHEVC5iDp8A8xidvA16L0csKu0ey8LZHVlA2-QlCgQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 944
ht-degree: 1%

---

# Permisos de objetos e información general del nivel de acceso para el modelo de almacenamiento en la nube de Adobe

<!--linked in UI -->

El almacenamiento en la nube de Adobe es una solución de almacenamiento basada en la nube que sirve como repositorio de almacenamiento central para los recursos de los productos empresariales de Adobe. Los entornos de Workfront que utilizan el almacenamiento en la nube de Adobe tienen permisos de objeto y comportamientos de nivel de acceso ligeramente diferentes a los que utilizan el almacenamiento de documentos de Workfront heredado.

## Niveles de acceso

Los niveles de acceso de Workfront solo se aplican en Workfront. Las restricciones de proyectos y documentos dentro de Workfront no siempre se aplican a otras aplicaciones de Adobe.

### Entornos que utilizan el almacenamiento en la nube de Adobe y el almacenamiento heredado de Workfront

El acceso a los documentos se comporta de forma diferente en función de si el proyecto se encuentra en el almacenamiento en la nube de Adobe o en el almacenamiento de Workfront heredado:

* **Almacenamiento heredado de Workfront**: Los proyectos, programas, portafolios y plantillas que usan almacenamiento heredado de Workfront siguen la lógica estándar de nivel de acceso de Workfront para el acceso a documentos. Cuando un nivel de acceso tiene **Sin acceso** seleccionado para documentos, no puede ver documentos en Workfront u otros productos de Adobe como Frame.io o Creative Cloud.
* **Almacenamiento en la nube de Adobe**: Los proyectos, programas, portafolios y plantillas que usan el almacenamiento en la nube de Adobe siguen la lógica de nivel de acceso del almacenamiento en la nube de Adobe para otros productos de Adobe.


   * **Permisos de objetos de proyectos, programas, portafolios y plantillas**: cuando un nivel de acceso tiene **Sin acceso** seleccionado para proyectos, programas, portafolios y plantillas, pero el objeto se comparte con ellos, los usuarios no pueden ver el objeto en Workfront, pero pueden ver el nombre del objeto y cualquier documento asociado en otras herramientas de Adobe, como Frame.io y Adobe Creative Cloud.
   * **Permisos de documentos**: cuando se selecciona un nivel de acceso de **Sin acceso** para los documentos, los usuarios no pueden ver los documentos de los proyectos de Workfront, pero sí pueden ver y administrar los documentos de los proyectos compartidos con ellos en otras herramientas de Adobe, como Frame.io y Adobe Creative Cloud. Esto se debe a que el acceso a los documentos está determinado por los permisos de nivel de proyecto en el almacenamiento en la nube de Adobe, en lugar de hacerlo solo por los niveles de acceso de Workfront.

Si tiene habilitado el almacenamiento en la nube de Adobe en su entorno de Workfront, puede crear proyectos de almacenamiento en la nube de Adobe y proyectos de almacenamiento de Workfront heredados. Los proyectos de almacenamiento de Workfront heredados muestran un icono junto al nombre del proyecto siempre que se muestre en Workfront. Los proyectos de almacenamiento en la nube de Adobe no muestran ningún icono.

![icono de almacenamiento de workfront heredado junto al nombre del proyecto](assets/legacy-project-icon.png)


### Entornos que solo utilizan el almacenamiento en la nube de Adobe

No puede modificar los permisos de documento en el nivel de acceso para proyectos, programas y portafolios que utilicen el almacenamiento en la nube de Adobe.

Todos los niveles de acceso tienen acceso de edición a los documentos. Los permisos de nivel de proyecto determinan el acceso a documentos en otras herramientas de Adobe.

No puede restringir el acceso a la herencia de documentos.


### Entornos que solo utilizan almacenamiento heredado de Workfront

No hay cambios en los niveles de acceso a documentos ni en el comportamiento.

## Permisos de objeto

Los permisos de objetos determinan lo que se puede ver y hacer con proyectos, tareas, problemas y documentos en Workfront. Los permisos se asignan cuando alguien comparte un objeto con usted.

>[!IMPORTANT]
>
>En Adobe Cloud Storage, los permisos de documento funcionan de forma diferente que en el almacenamiento heredado de Workfront. Los documentos heredan los permisos del proyecto, la tarea o el problema al que están vinculados.


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


## Asignación de permisos a Frame.io

Como parte de la integración, los permisos de usuario se controlan en Workfront y fluyen a Frame.io. Esto significa que no puede invitar a un usuario a un proyecto en Frame.io ni modificar los permisos de usuario en Frame.io. Estas acciones deben realizarse mediante el modal Uso compartido de proyectos en Workfront.

En la tabla siguiente se muestra cómo se asignan los permisos de Workfront a los permisos de Frame.io:

<table>
<tr>
<th>Permiso de usuario de Workfront</th>
<th>Permiso de usuario de Frame.io</th>
</tr>
<tr>
<td>Administrar</td>
<td>Editar y compartir</td>
</tr>
<tr>
<td>Aportar</td>
<td>Editar y compartir</td>
</tr>
<tr>
<td>Ver</td>
<td>Solo comentario</td>
</tr>
</table>






