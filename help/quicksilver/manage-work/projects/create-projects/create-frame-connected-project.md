---
product-area: projects
navigation-topic: create-projects
title: Cree un proyecto conectado con Frame.io
description: Un proyecto es una gran unidad de trabajo en Adobe Workfront. Puede crear proyectos desde cero, utilizar una plantilla o convertir problemas o tareas en proyectos.
author: Courtney
feature: Work Management
exl-id: 230d8e62-a3c9-4e38-9b26-5ba1c4f56391
source-git-commit: 0d737bc410f3db4eeff52fa8954acdb8a0eb1a6e
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 1%

---

# Cree un proyecto conectado con Frame.io

La integración de Workfront y Frame.io le permite crear proyectos en Workfront que se reflejan en Frame.io, lo que proporciona una experiencia de revisión y aprobación sin problemas.

Cuando un proyecto de Workfront está conectado con Frame.io, puede

* **Asignar usuarios de Frame.io a tareas**: se notifica por correo electrónico a los usuarios habilitados para Frame.io cuando se les asigna una tarea de Workfront, indicando que hay trabajo que completar.
* **Compartir el proyecto con usuarios de Frame.io**: Cuando se comparte un proyecto con usuarios habilitados para Frame.io, tienen acceso al proyecto tanto dentro de Workfront como en Frame.io.
* **Compartir materiales creativos con Frame.io**: los coordinadores de proyectos pueden enviar instrucciones y materiales desde Workfront directamente al usuario creativo en Frame.io mediante una carpeta de proyectos de sincronización unidireccional. [!BADGE Próximamente]{type=Informative}
* **Seguimiento del progreso de las tareas**: los creativos pueden enviar los recursos finalizados y marcar las tareas como completadas, todo sin salir de Frame.io.

## Requisitos de acceso

>[!IMPORTANT]
>
>Esta funcionalidad solo está disponible para las organizaciones que se han incorporado a [!DNL Adobe Admin Console].

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Al crear un proyecto, recibirá automáticamente permisos de administración en el proyecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

* Configure la cuenta predeterminada de Frame.io en el área de configuración de Workfront
* Habilitar usuarios de Frame.io en el perfil de usuario de Workfront

Para obtener más información sobre los requisitos previos anteriores, consulte [Configurar la [!DNL Workfront] integración y [!DNL Frame.io] integración](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).


## Crear una nueva plantilla de proyecto

Al crear una plantilla nueva, puede introducir la información de todas las tareas y de la configuración futura del proyecto. Esta información se transferirá a cualquier proyecto que cree a partir de la plantilla.

Los proyectos de Frame.io están organizados por equipos conectados a grupos de Workfront. Se recomienda utilizar una plantilla de proyecto para crear proyectos conectados, ya que puede establecer el grupo de proyectos antes que.

Si decide crear el proyecto desde cero, Workfront agrega automáticamente el grupo de proyectos Predeterminado y el proyecto Frame.io reflejado se crea en ese equipo predeterminado en Frame.io.

>[!NOTE]
>
>La actualización del grupo después de la creación del proyecto no cambia el equipo de Frame.io.


### Cree la plantilla y especifique el grupo de proyectos

{{step1-to-templates}}

1. Haga clic en **Nueva plantilla**.
1. Escriba un nombre para la plantilla y presione **Intro** para guardar el nombre.
1. En el panel izquierdo, haga clic en **Detalles de plantilla**.
1. En la sección **Asociación de plantillas**, asegúrese de especificar un grupo. Si no agrega ningún grupo, se agregará el grupo de proyecto predeterminado y el proyecto de Frame.io se creará en el equipo predeterminado correspondiente de Frame.io.

Continúe con la sección siguiente.

![](assets/template-group.png)

### Agregue tareas y asigne usuarios habilitados para Frame.io

1. En el panel izquierdo, haga clic en **Tareas de plantilla**.
1. Haga clic en **Comenzar a agregar tareas de plantilla** para agregar rápidamente tareas a su plantilla. Puede configurar opciones adicionales más adelante.

   O

   Haga clic en **Nueva tarea de plantilla** para agregar una tarea a la vez y configurar opciones adicionales.
   ![](assets/add-tasks-to-template.png)
1. Añada un nombre de tarea.
1. En el área **Asignaciones**, asigne usuarios o equipos. Si asigna a un usuario habilitado para Frame.io, ya sea de forma individual o en equipo, se le concede acceso de colaborador al proyecto Frame.io y se le notifica la tarea en el proyecto Frame.io por correo electrónico. Desde ese correo electrónico, pueden unirse al proyecto Frame.io y comenzar a trabajar.
1. Repita los pasos 1 y 2 según sea necesario.

Continúe con la sección siguiente.

### Configuración de detalles de plantilla adicionales

Workfront tiene funcionalidades sólidas de administración de proyectos. Se recomienda usar el artículo [Editar plantillas de proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) para configurar las siguientes áreas de la plantilla:

* Información general
* Finanzas
* Formularios personalizados
* Configuración de proyecto
* Configuración de tareas
* Configuración de problema
* Acceso

### Cree un proyecto a partir de la plantilla

Una vez creada una plantilla, puede utilizarla para crear proyectos.

{{step1-to-projects}}

1. Haga clic en **Nuevo proyecto de la plantilla**.
1. Con el cuadro de búsqueda, empiece a escribir el nombre de la plantilla que necesita.
1. Seleccione el nombre de la plantilla y luego haga clic en **Usar plantilla**.
   ![](assets/find-your-template.png)
1. Ajuste la configuración del proyecto según sea necesario y haga clic en **Crear proyecto**.
1. En el panel izquierdo, haga clic en **Documentos**.
1. Utilice la carpeta de sincronización unidireccional para compartir automáticamente los materiales creativos con Frame.io. [!BADGE Próximamente]{type=Informative}

   >[!NOTE]
   >
   >Esta función está actualmente en desarrollo. Para compartir información con los usuarios en Frame.io, cargue los archivos en la pestaña Documento. Cuando el estado del proyecto se establece en Actual, esos archivos se insertan automáticamente en Frame.io.

1. En el encabezado del proyecto, cambie el proyecto de **Planning** a **Current**.

Una vez creado el proyecto y cargado por los creativos los recursos finalizados, puede asignar un flujo de trabajo de revisión y aprobación al recurso en Workfront. Para obtener más información, vea [Crear una solicitud de revisión o aprobación de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->

## Creación de un nuevo proyecto desde cero

Puede crear un nuevo proyecto desde cero según sea necesario.

>[!IMPORTANT]
>
>* Los proyectos de Frame.io están organizados por equipos conectados a grupos de Workfront. Se recomienda utilizar una plantilla de proyecto para crear proyectos conectados, ya que puede establecer el grupo de proyectos antes que.
>
>
>* Si decide crear el proyecto desde cero, Workfront agrega automáticamente el grupo de proyectos Predeterminado y el proyecto Frame.io reflejado se crea en ese equipo predeterminado en Frame.io.
>
>La actualización del grupo después de la creación del proyecto no cambia el equipo de Frame.io.

### Creación del proyecto

{{step1-to-projects}}

1. Haga clic en **Nuevo proyecto**.
1. Escriba un nombre para el proyecto y presione **Intro** para guardar el nombre.

Continúe con la sección siguiente.

### Agregue tareas y asigne usuarios habilitados para Frame.io

1. En el panel izquierdo, haga clic en **Tareas**.
1. Haga clic en **Comenzar a agregar tareas** para agregar rápidamente tareas al proyecto. Puede configurar opciones adicionales más adelante.

   O

   Haga clic en **Nueva tarea** para agregar una tarea a la vez y configurar opciones adicionales.
   ![](assets/add-project-tasks.png)
1. Añada un nombre de tarea.
1. En el área **Asignaciones**, asigne usuarios o equipos. Si asigna a un usuario habilitado para Frame.io, ya sea de forma individual o en equipo, se le concede acceso de colaborador al proyecto Frame.io y se le notifica la tarea en el proyecto Frame.io por correo electrónico. Desde ese correo electrónico, pueden unirse al proyecto Frame.io y comenzar a trabajar.
1. Repita los pasos 1 y 2 según sea necesario.

Continúe con la sección siguiente.

### Cargar materiales creativos

1. En el panel izquierdo, haga clic en **Documentos**.
1. Utilice la carpeta de sincronización unidireccional para compartir automáticamente los materiales creativos con Frame.io. [!BADGE Próximamente]{type=Informative}

   >[!NOTE]
   >
   >Esta función está actualmente en desarrollo. Para compartir información con los usuarios en Frame.io, cargue los archivos en la pestaña Documento. Cuando el estado del proyecto se establece en Actual, esos archivos se insertan automáticamente en Frame.io

Continúe con la sección siguiente.

### Configurar detalles adicionales del proyecto

Workfront tiene funcionalidades sólidas de administración de proyectos. Se recomienda usar el artículo [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) para configurar las siguientes áreas del proyecto:

* Información general
* Finanzas
* Formularios personalizados
* Configuración de proyecto
* Configuración de tareas
* Configuración de problema
* Acceso

### Establecer el proyecto en actual

1. En la cabecera del proyecto, cambie el proyecto de Planificación a Actual.
Una vez creado el proyecto y cargado por los creativos los recursos finalizados, puede asignar un flujo de trabajo de revisión y aprobación al recurso en Workfront.

Una vez creado el proyecto y cargado por los creativos los recursos finalizados, puede asignar un flujo de trabajo de revisión y aprobación al recurso en Workfront.

Para obtener más información, vea [Crear una solicitud de revisión o aprobación de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->
