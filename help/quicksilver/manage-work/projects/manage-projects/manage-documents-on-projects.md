---
product-area: projects
navigation-topic: manage-projects
title: Información general de administración de documentos para proyectos y objetos relacionados
description: Dependiendo de si el administrador de Workfront elige la opción predeterminada de almacenamiento, puede almacenar los documentos en el almacenamiento heredado de Workfront o en el almacenamiento en la nube de Adobe. En este artículo se describe cómo administrar documentos para proyectos, portafolios, programas, plantillas, tareas y problemas.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 9053a824ecec4feb35a612b26aebb91904ef2546
workflow-type: tm+mt
source-wordcount: '1961'
ht-degree: 0%

---

# Información general sobre la administración de documentos para proyectos y objetos relacionados

El administrador de Adobe Workfront puede definir el valor predeterminado de las preferencias de almacenamiento de su organización para indicar dónde se deben almacenar los documentos en Workfront.

El administrador de Workfront puede elegir una de las siguientes opciones:

* almacenamiento de Workfront
* Almacenamiento en la nube de Adobe

Esta preferencia permite almacenar automáticamente los documentos adjuntos a los objetos de Workfront en una de las ubicaciones de almacenamiento disponibles.

>[!IMPORTANT]
>
>Es posible que la instancia de Workfront no tenga acceso al almacenamiento de Workfront y Adobe. Algunas instancias de Workfront solo tienen acceso a Workfront, mientras que otras solo tienen acceso al almacenamiento en la nube de Adobe de forma predeterminada. No se necesita ninguna configuración para los clientes con acceso a un solo tipo de almacenamiento.

El administrador de Workfront puede realizar una de las siguientes acciones:

* Elija una de las dos opciones de almacenamiento como predeterminadas para su organización
* Permite elegir el almacenamiento que prefiere usar al crear uno de los siguientes objetos:

   * Proyectos
   * Portafolios
   * Plantillas

Para obtener información sobre cómo establecer las preferencias de almacenamiento para Workfront, consulte [Habilitar el almacenamiento en la nube de Adobe para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

En este artículo se describe cómo administrar documentos para proyectos, portafolios, programas, tareas, problemas, plantillas y tareas de plantilla.

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## Resumen de almacenamiento de documentos

Los clientes pueden tener acceso a una de las siguientes funciones de almacenamiento de documentos:

* Solo almacenamiento de Workfront. El área Preferencias de almacenamiento de Preferencias del sistema no existe.
* Solo almacenamiento en la nube de Adobe. El área Preferencias de almacenamiento de Preferencias del sistema no existe.
* Almacenamiento en la nube de Workfront y Adobe. El administrador de Workfront puede elegir entre lo siguiente:

   * Selecciona un entorno de almacenamiento predeterminado para la gestión futura de documentos.
   * Permite a los usuarios elegir el almacenamiento que desean cuando crean los objetos siguientes:

      * Proyectos
      * Portafolios
      * Plantillas

  >[!NOTE]
  >
  >* Las tareas y los problemas heredan el tipo de almacenamiento del proyecto.
  >* Las tareas de plantilla heredan el tipo de almacenamiento de la plantilla
  >* Los programas heredan el tipo de almacenamiento del portafolio.


Los documentos almacenados en objetos en Workfront Storage se administran de forma diferente a los almacenados en Adobe Cloud Storage.

Para obtener más información, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Las siguientes secciones documentan cómo funciona el almacenamiento de documentos para objetos de Workfront cuando existen opciones de Workfront y de almacenamiento en la nube de Adobe en el mismo entorno.

### Administración de documentos para proyectos

Tenga en cuenta lo siguiente al trabajar con proyectos:

* Cuando crea un proyecto de almacenamiento en la nube de Adobe, Workfront crea una carpeta en la sección Documentos del proyecto en la que se guardan los documentos. El nombre de la carpeta es el mismo nombre que el proyecto. No puede eliminar la carpeta ni cambiarle el nombre manualmente. Se cambiará el nombre de la carpeta si cambia el nombre del proyecto para que coincida con el nuevo nombre del proyecto.
* Al crear o mover un proyecto de almacenamiento en la nube de Adobe a un portafolio o programa de almacenamiento en la nube de Workfront heredado, el portafolio o programa se convierte automáticamente en un objeto de almacenamiento en la nube de Adobe, si el portafolio o programa no tiene documentos adjuntos antes de que se agregue el proyecto.
* No puede crear un proyecto de almacenamiento de Workfront heredado para un portafolio o programa de almacenamiento en la nube de Adobe.
* Al importar un proyecto desde MS Project, Workfront crea un proyecto de almacenamiento de Workfront heredado, incluso cuando el administrador de Workfront establece el almacenamiento en la nube de Adobe como predeterminado para el sistema.
* Al crear proyectos mediante una automatización de Workfront Planning, Workfront utiliza la preferencia de almacenamiento predeterminada del sistema para el proyecto. Debe adquirir el paquete de Planning para acceder a Workfront Planning.

### Administración de documentos para portafolios

Tenga en cuenta lo siguiente al trabajar con portafolios:

* Cuando crea un portafolio de almacenamiento en la nube de Adobe, Workfront crea una carpeta en la sección Documentos del portafolio en la que se guardan los documentos. El nombre de la carpeta es el mismo nombre que el portafolio. No puede eliminar la carpeta ni cambiarle el nombre manualmente. Se cambiará el nombre de la carpeta si cambia el nombre del portafolio de modo que coincida con el nuevo nombre del portafolio.

* Cuando agrega un proyecto de almacenamiento en la nube de Adobe a una cartera de productos de almacenamiento de Workfront heredados y esta no tiene documentos adjuntos, la cartera se convierte en una cartera de productos de almacenamiento en la nube de Adobe.
* Cuando agrega un proyecto de almacenamiento en la nube de Adobe a una cartera de productos de almacenamiento de Workfront heredados y esta tiene documentos adjuntos a él, el almacenamiento de documentos de la cartera permanece en el almacenamiento de Workfront. Sin embargo, el icono de almacenamiento de Workfront heredado del portafolio ![Icono de almacenamiento de portafolio heredado](assets/legacy-storage-project-icon.png) se eliminará del portafolio.
* No puede agregar un proyecto de almacenamiento de Workfront heredado a un catálogo de productos de Adobe Cloud Storage.

* Al crear portafolios mediante una automatización de Workfront Planning, Workfront utiliza la preferencia de almacenamiento predeterminada del sistema para el portafolio. Debe adquirir el paquete de Planning para acceder a Workfront Planning.

### Administración de documentos para programas

Tenga en cuenta lo siguiente al trabajar con programas:

* Cuando crea un programa de almacenamiento en la nube de Adobe, Workfront crea una carpeta en la sección Documentos del programa en la que se guardan los documentos. El nombre de la carpeta es el mismo que el nombre del programa. No puede eliminar la carpeta ni cambiarle el nombre manualmente. Si cambia el nombre del programa, se cambiará el nombre de la carpeta para que coincida con el nuevo nombre del programa.

* Cuando se agrega un proyecto de almacenamiento en la nube de Adobe a un programa de almacenamiento heredado de Workfront y el programa no tiene documentos adjuntos a él, el programa se convierte en un programa de almacenamiento en la nube de Adobe. La cartera del programa también se convierte.
* Cuando se agrega un proyecto de almacenamiento en la nube de Adobe a un programa de almacenamiento de Workfront heredado y el programa tiene documentos adjuntos a él, el almacenamiento de documentos del programa permanece en el almacenamiento de Workfront. Si el portafolio también tiene documentos, su almacenamiento de documentos también permanece en el almacenamiento de Workfront; de lo contrario, el portafolio se convierte al almacenamiento en la nube de Adobe.

  El icono de almacenamiento de Workfront heredado del programa ![Icono de almacenamiento de portafolios heredado](assets/legacy-storage-project-icon.png) se ha eliminado del programa.
* No puede agregar un proyecto de almacenamiento de Workfront heredado a un programa de almacenamiento en la nube de Adobe.

* Al crear programas mediante una automatización de Workfront Planning, Workfront utiliza la preferencia de almacenamiento predeterminada del sistema para el programa. Debe adquirir el paquete de Planning para acceder a Workfront Planning.

### Administración de documentos para tareas

Tenga en cuenta lo siguiente al trabajar con tareas:

* Las tareas heredan el tipo de almacenamiento de los proyectos.
* Al cargar un documento en una tarea de un proyecto de almacenamiento en la nube de Adobe, Workfront crea automáticamente una carpeta en la sección Documentos de la tarea. El nombre de la carpeta es el mismo que la tarea.
* Puede cambiar el nombre de la carpeta de documentos y eliminarla desde la tarea de almacenamiento en la nube de Adobe, que también elimina los documentos de la carpeta. Después de agregar nuevos documentos a la tarea, la carpeta se vuelve a crear automáticamente. Los documentos eliminados no vuelven a colocarse en la carpeta.
* En los proyectos de almacenamiento en la nube de Adobe, la carpeta de documentos de una tarea se muestra como una subcarpeta en la carpeta de documentos creada automáticamente para el proyecto.
* No puede copiar ni mover una tarea de un proyecto de almacenamiento de Workfront heredado a uno de almacenamiento en la nube de Adobe. Lo contrario tampoco es posible.
* Existen los siguientes escenarios al convertir una tarea en un proyecto: <!--this info also duplicated in Convert tasks to projects-->
   * Una tarea de almacenamiento de Workfront heredado crea un proyecto de almacenamiento de Workfront heredado.
   * Una tarea de almacenamiento en la nube de Adobe crea un proyecto de almacenamiento en la nube de Adobe.
   * Al usar una plantilla de almacenamiento de Workfront heredada para convertir una tarea de almacenamiento de nube de Adobe, se crea un proyecto de almacenamiento de nube de Adobe.
   * El uso de una plantilla de almacenamiento en la nube de Adobe para convertir una tarea de almacenamiento de Workfront heredada crea un proyecto de almacenamiento de Workfront heredado.
* No puede agregar documentos a tareas de almacenamiento en la nube de Adobe en el Panel de resumen.

### Administración de documentos para problemas

Tenga en cuenta lo siguiente al trabajar con problemas:

* Los problemas heredan el tipo de almacenamiento de los proyectos.
* Cuando se carga un documento en un problema de un proyecto de almacenamiento en la nube de Adobe, Workfront crea automáticamente una carpeta en la sección Documentos del problema. El nombre de la carpeta es el mismo que el problema.
* Puede cambiar el nombre de la carpeta de documentos y eliminarla del problema de almacenamiento en la nube de Adobe, que también elimina los documentos de la carpeta. Después de agregar nuevos documentos al problema, la carpeta se vuelve a crear automáticamente. Los documentos eliminados no vuelven a colocarse en la carpeta.
* En los proyectos de almacenamiento en la nube de Adobe, la carpeta de documentos de un problema se muestra como una subcarpeta en la carpeta de documentos creada automáticamente para el proyecto.
* No puede copiar ni mover un problema de un proyecto de almacenamiento de Workfront heredado a uno de Adobe Cloud Storage. Lo contrario tampoco es posible.
* Existen los siguientes escenarios al convertir un problema en un proyecto: <!--this info also duplicated in Convert an issue to a project-->
   * Un problema de almacenamiento de Workfront heredado crea un proyecto de almacenamiento de Workfront heredado.
   * Un problema de almacenamiento en la nube de Adobe crea un proyecto de almacenamiento en la nube de Adobe.
   * El uso de una plantilla de almacenamiento de Workfront heredada para convertir un problema de almacenamiento en la nube de Adobe crea un proyecto de almacenamiento en la nube de Adobe.
   * El uso de una plantilla de almacenamiento en la nube de Adobe para convertir un problema de almacenamiento de Workfront heredado crea un proyecto de almacenamiento de Workfront heredado.
* No puede agregar documentos a problemas de almacenamiento en la nube de Adobe en el Panel de resumen.

### Administración de documentos para solicitudes de

* Cuando envía una solicitud de Workfront que tiene un documento adjunto a un proyecto de almacenamiento de Workfront heredado que funciona como cola de solicitudes, el área Documentos de la solicitud muestra el documento utilizando el tipo de almacenamiento del proyecto, incluso cuando la preferencia predeterminada de almacenamiento del sistema es el almacenamiento en la nube de Adobe.
* Cuando adjunta un documento a un problema enviado a una cola de solicitudes asociada al almacenamiento de Adobe, se crea una carpeta para cada problema enviado en el que se almacenan los documentos. La carpeta también se agrega como subcarpeta a la carpeta de proyecto creada automáticamente en el proyecto de cola de solicitudes.

### Administración de documentos para plantillas de proyecto

Tenga en cuenta lo siguiente al trabajar con plantillas:

* Cuando crea una plantilla de almacenamiento en la nube de Adobe, Workfront crea una carpeta en la sección Documentos de la plantilla en la que se guardan los documentos. El nombre de la carpeta es el mismo nombre que el programa. No puede eliminar la carpeta ni cambiarle el nombre manualmente. Si cambia el nombre de la plantilla, se cambiará el nombre de la carpeta para que coincida con el nuevo nombre de la plantilla.
* Puede utilizar una plantilla de almacenamiento de Workfront heredada para crear proyectos de almacenamiento de Workfront heredados; puede utilizar una plantilla de almacenamiento de nube de Adobe para crear un proyecto de almacenamiento de nube de Adobe.
* Puede adjuntar una plantilla de almacenamiento de Workfront heredada a un proyecto de almacenamiento en la nube de Adobe, lo cual no cambia la ubicación de almacenamiento de los documentos del proyecto.
* Puede adjuntar una plantilla de almacenamiento en la nube de Adobe a un proyecto de almacenamiento de Workfront heredado, lo que no cambia la ubicación de almacenamiento de los documentos del proyecto. Los documentos de la carpeta de almacenamiento en la nube de Adobe para la plantilla se agregan directamente al proyecto, sin la carpeta, mientras que los documentos de las carpetas de tareas de plantilla se agregan a carpetas adjuntas a las tareas del proyecto en la sección Documentos de las tareas.
* Al guardar un proyecto como plantilla, el tipo de almacenamiento del proyecto se transfiere a la plantilla, independientemente de lo que haya configurado el administrador de Workfront para las preferencias de almacenamiento del sistema.


### Administración de documentos para tareas de plantilla

Tenga en cuenta lo siguiente al trabajar con tareas de plantilla:

* Las tareas de plantilla heredan el tipo de almacenamiento de las plantillas.
* Al cargar un documento en una tarea de plantilla en una plantilla de almacenamiento de la nube de Adobe, Workfront crea automáticamente una carpeta en la sección Documentos de la tarea de plantilla. El nombre de la carpeta es el mismo que el de la tarea de plantilla.
* Puede cambiar el nombre de la carpeta de documentos y eliminarla desde la tarea de plantilla de Adobe Cloud Storage, que también elimina los documentos de la carpeta. Después de agregar nuevos documentos a la tarea de plantilla, la carpeta se vuelve a crear automáticamente. Los documentos eliminados no vuelven a colocarse en la carpeta.
* Para las plantillas de almacenamiento en la nube de Adobe, la carpeta de documentos de una tarea de plantilla se muestra como una subcarpeta en la carpeta de documentos creada automáticamente para la plantilla.
* No puede copiar ni mover una tarea de plantilla de una plantilla de almacenamiento de Workfront heredada a una plantilla de almacenamiento en la nube de Adobe. Lo contrario tampoco es posible.

