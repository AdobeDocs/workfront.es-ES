---
product-area: projects
navigation-topic: manage-projects
title: Información general de administración de documentos para proyectos y objetos relacionados
description: Dependiendo de si el administrador de Workfront elige la opción predeterminada de almacenamiento, puede almacenar los documentos en el almacenamiento heredado de Workfront o en el almacenamiento empresarial de Adobe. En este artículo se describe cómo administrar documentos para proyectos, portafolios, programas, plantillas, tareas y problemas.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 2b0fdb3c74882b566a397872e1cc8007728b770c
workflow-type: tm+mt
source-wordcount: '1755'
ht-degree: 0%

---

# Información general sobre la administración de documentos para proyectos y objetos relacionados

El administrador de Adobe Workfront puede definir el valor predeterminado de las preferencias de almacenamiento de su organización para indicar dónde se deben almacenar los documentos en Workfront.

El administrador de Workfront puede elegir una de las siguientes opciones:

* almacenamiento de Workfront
* Almacenamiento empresarial de Adobe

Esta preferencia permite almacenar automáticamente los documentos adjuntos a los objetos de Workfront en una de las ubicaciones de almacenamiento disponibles.

>[!IMPORTANT]
>
>Es posible que la instancia de Workfront no tenga acceso al almacenamiento de Workfront y Adobe. Algunas instancias de Workfront solo tienen acceso a Workfront, mientras que otras solo tienen acceso al almacenamiento de Adobe Enterprise de forma predeterminada. No se necesita ninguna configuración para los clientes con acceso a un solo tipo de almacenamiento.

El administrador de Workfront puede realizar una de las siguientes acciones:

* Elija una de las dos opciones de almacenamiento como predeterminadas para su organización
* Permite elegir el almacenamiento que prefiere usar al crear uno de los siguientes objetos:

   * Proyectos
   * Portafolios
   * Plantillas

Para obtener información sobre cómo establecer las preferencias de almacenamiento para Workfront, consulte [Habilitar el almacenamiento empresarial de Adobe para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

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
* Solo almacenamiento de Adobe Enterprise. El área Preferencias de almacenamiento de Preferencias del sistema no existe.
* Almacenamiento de Workfront y almacenamiento de Adobe Enterprise. El administrador de Workfront puede elegir entre lo siguiente:

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


Los documentos almacenados en objetos en el almacenamiento de Workfront se administran de forma diferente a los almacenados en el almacenamiento empresarial de Adobe.

Para obtener más información, consulte [Información general sobre el almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Las siguientes secciones documentan cómo funciona el almacenamiento de documentos para objetos de Workfront cuando las opciones de Workfront y Adobe Enterprise Storage existen en el mismo entorno.

### Administración de documentos para proyectos

Tenga en cuenta lo siguiente al trabajar con proyectos:

* Al crear un proyecto de almacenamiento empresarial de Adobe, Workfront crea una carpeta en la sección Documentos del proyecto donde se guardan los documentos. El nombre de la carpeta es el mismo nombre que el proyecto. No puede eliminar la carpeta ni cambiarle el nombre manualmente. Se cambiará el nombre de la carpeta si cambia el nombre del proyecto para que coincida con el nuevo nombre del proyecto.
* Al crear o mover un proyecto de almacenamiento empresarial de Adobe a un programa o portafolio de almacenamiento de Workfront heredado, el portafolio o programa se convierte automáticamente en un objeto de almacenamiento empresarial de Adobe.
* No puede crear un proyecto de almacenamiento de Workfront para un portafolio o programa de almacenamiento empresarial de Adobe.
* Al importar un proyecto desde MS Project, Workfront crea un proyecto de almacenamiento de Workfront, incluso cuando el administrador de Workfront ha establecido el almacenamiento empresarial de Adobe como predeterminado para el sistema.
* Al crear proyectos mediante una automatización de Workfront Planning, Workfront utiliza la preferencia de almacenamiento predeterminada del sistema para el proyecto. Debe adquirir el paquete de Planning para acceder a Workfront Planning.

### Administración de documentos para portafolios

Tenga en cuenta lo siguiente al trabajar con portafolios:

* Al crear un portafolio de almacenamiento empresarial de Adobe, Workfront crea una carpeta en la sección Documentos del portafolio en la que se guardan los documentos. El nombre de la carpeta es el mismo nombre que el portafolio. No puede eliminar la carpeta ni cambiarle el nombre manualmente. Se cambiará el nombre de la carpeta si cambia el nombre del portafolio de modo que coincida con el nuevo nombre del portafolio.
* Al crear o mover un proyecto de almacenamiento empresarial de Adobe a una cartera de productos de almacenamiento de Workfront heredados, la cartera se convierte automáticamente en un objeto de almacenamiento empresarial de Adobe.
* Si el portafolio convertido tenía documentos adjuntos anteriormente, estos permanecen almacenados en el almacenamiento de Workfront. Los nuevos documentos también se almacenan en el almacenamiento de Workfront.
* Si el portafolio convertido no tenía documentos adjuntos en el almacenamiento de Workfront, los nuevos documentos se almacenan en el almacenamiento empresarial de Adobe.
* Al crear portafolios mediante una automatización de Workfront Planning, Workfront utiliza la preferencia de almacenamiento predeterminada del sistema para el portafolio. Debe adquirir el paquete de Planning para acceder a Workfront Planning.

### Administración de documentos para programas

Tenga en cuenta lo siguiente al trabajar con programas:

* Al crear un programa de almacenamiento empresarial de Adobe, Workfront crea una carpeta en la sección Documentos del programa en la que se guardan los documentos. El nombre de la carpeta es el mismo que el nombre del programa. No puede eliminar la carpeta ni cambiarle el nombre manualmente. Si cambia el nombre del programa, se cambiará el nombre de la carpeta para que coincida con el nuevo nombre del programa.
* Al crear o mover un proyecto de almacenamiento empresarial de Adobe a una cartera de productos de almacenamiento de Workfront heredados, la cartera se convierte automáticamente en un objeto de almacenamiento empresarial de Adobe.
* Si el programa convertido tenía documentos adjuntos anteriormente, estos siguen almacenados en el almacenamiento de Workfront. Los nuevos documentos también se almacenan en el almacenamiento de Workfront.
* Si el programa convertido no tenía documentos adjuntos en el almacenamiento de Workfront, los nuevos documentos se almacenan en el almacenamiento empresarial de Adobe.
* Al crear programas mediante una automatización de Workfront Planning, Workfront utiliza la preferencia de almacenamiento predeterminada del sistema para el programa. Debe adquirir el paquete de Planning para acceder a Workfront Planning.

### Administración de documentos para tareas

Tenga en cuenta lo siguiente al trabajar con tareas:

* Las tareas heredan el tipo de almacenamiento de los proyectos.
* Cuando se carga un documento en una tarea de un proyecto de almacenamiento de Adobe, Workfront crea automáticamente una carpeta en la sección Documentos de la tarea. El nombre de la carpeta es el mismo que la tarea.
* Puede cambiar el nombre de la carpeta de documentos y eliminarla desde la tarea de almacenamiento empresarial de Adobe, que también elimina los documentos de la carpeta. Después de agregar nuevos documentos a la tarea, la carpeta se vuelve a crear automáticamente. Los documentos eliminados no vuelven a colocarse en la carpeta.
* En los proyectos de almacenamiento empresarial de Adobe, la carpeta de documentos de una tarea se muestra como una subcarpeta en la carpeta de documentos creada automáticamente para el proyecto.
* No puede copiar ni mover una tarea de un proyecto de almacenamiento de Workfront a uno de almacenamiento de Adobe. Lo contrario tampoco es posible.
* Existen los siguientes escenarios al convertir una tarea en un proyecto: <!--this info also duplicated in Convert tasks to projects-->
   * Una tarea de almacenamiento de Workfront crea un proyecto de almacenamiento de Workfront.
   * Una tarea de almacenamiento empresarial de Adobe crea un proyecto de almacenamiento de Adobe.
   * Si se utiliza una plantilla de almacenamiento de Workfront para convertir una tarea de almacenamiento de Adobe, se crea un proyecto de almacenamiento de Adobe.
   * El uso de una plantilla de almacenamiento de Adobe para convertir una tarea de almacenamiento de Workfront crea un proyecto de almacenamiento de Workfront.

### Administración de documentos para problemas

Tenga en cuenta lo siguiente al trabajar con problemas:

* Los problemas heredan el tipo de almacenamiento de los proyectos.
* Cuando se carga un documento en un problema de un proyecto de almacenamiento de Adobe, Workfront crea automáticamente una carpeta en la sección Documentos del problema. El nombre de la carpeta es el mismo que el problema.
* Puede cambiar el nombre de la carpeta de documentos y eliminarla del problema de almacenamiento empresarial de Adobe, que también elimina los documentos de la carpeta. Después de agregar nuevos documentos al problema, la carpeta se vuelve a crear automáticamente. Los documentos eliminados no vuelven a colocarse en la carpeta.
* En los proyectos de almacenamiento empresarial de Adobe, la carpeta de documentos de un problema se muestra como una subcarpeta en la carpeta de documentos creada automáticamente para el proyecto.
* No puede copiar ni mover un problema de un proyecto de almacenamiento de Workfront a uno de almacenamiento de Adobe. Lo contrario tampoco es posible.
* Cuando se envía una solicitud con un documento adjunto a un proyecto de almacenamiento de Workfront, el área Documentos de la solicitud muestra el documento utilizando el tipo de almacenamiento del proyecto, incluso cuando la preferencia predeterminada de almacenamiento del sistema es Adobe enterprise.
* Existen los siguientes escenarios al convertir un problema en un proyecto: <!--this info also duplicated in Convert an issue to a project-->
   * Un problema de almacenamiento de Workfront crea un proyecto de almacenamiento de Workfront.
   * Un problema de almacenamiento empresarial de Adobe crea un proyecto de almacenamiento de Adobe.
   * El uso de una plantilla de almacenamiento de Workfront para convertir un problema de almacenamiento de Adobe crea un proyecto de almacenamiento de Adobe.
   * El uso de una plantilla de almacenamiento de Adobe para convertir un problema de almacenamiento de Workfront crea un proyecto de almacenamiento de Workfront.

### Administración de documentos para plantillas de proyecto

Tenga en cuenta lo siguiente al trabajar con plantillas:

* Cuando se crea una plantilla de almacenamiento empresarial de Adobe, Workfront crea una carpeta en la sección Documentos de la plantilla en la que se guardan los documentos. El nombre de la carpeta es el mismo nombre que el programa. No puede eliminar la carpeta ni cambiarle el nombre manualmente. Si cambia el nombre de la plantilla, se cambiará el nombre de la carpeta para que coincida con el nuevo nombre de la plantilla.
* Puede utilizar una plantilla de almacenamiento de Workfront para crear proyectos de almacenamiento de Workfront; puede utilizar una plantilla de almacenamiento de Adobe para crear un proyecto de almacenamiento de Adobe.
* Puede adjuntar una plantilla de almacenamiento de Workfront a un proyecto de almacenamiento de Adobe, lo cual no cambia la ubicación de almacenamiento del proyecto.
* Puede adjuntar una plantilla de almacenamiento de Adobe a un proyecto de almacenamiento de Workfront, lo cual no cambia la ubicación de almacenamiento del proyecto. Los documentos de la carpeta de almacenamiento de Adobe para la plantilla se agregan directamente al proyecto, sin la carpeta, mientras que los documentos de las carpetas de tareas de la plantilla se agregan a las carpetas adjuntas a las tareas del proyecto en la sección Documentos de las tareas.

### Administración de documentos para tareas de plantilla

Tenga en cuenta lo siguiente al trabajar con tareas de plantilla:

* Las tareas de plantilla heredan el tipo de almacenamiento de las plantillas.
* Cuando se carga un documento en una tarea de plantilla en una plantilla de Adobe Storage, Workfront crea automáticamente una carpeta en la sección Documents de la tarea de plantilla. El nombre de la carpeta es el mismo que el de la tarea de plantilla.
* Puede cambiar el nombre de la carpeta de documentos y eliminarla desde la tarea de plantilla de almacenamiento empresarial de Adobe, que también elimina los documentos de la carpeta. Después de agregar nuevos documentos a la tarea de plantilla, la carpeta se vuelve a crear automáticamente. Los documentos eliminados no vuelven a colocarse en la carpeta.
* Para las plantillas de almacenamiento empresarial de Adobe, la carpeta de documentos de una tarea de plantilla se muestra como una subcarpeta en la carpeta de documentos creada automáticamente para la plantilla.
* No puede copiar ni mover una tarea de plantilla de una plantilla de almacenamiento de Workfront a una plantilla de almacenamiento de Adobe. Lo contrario tampoco es posible.
* Cuando adjunta un documento a un problema enviado a una cola de solicitudes asociada al almacenamiento de Adobe, se crea una carpeta para cada problema enviado en el que se almacenan los documentos. La carpeta también se agrega como subcarpeta a la carpeta de proyecto creada automáticamente en la cola de solicitudes.
