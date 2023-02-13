---
product-area: projects
navigation-topic: create-projects
title: Importar un proyecto desde un proyecto de Microsoft
description: Puede importar proyectos de Microsoft Project a Adobe Workfront y administrarlos en una aplicación. Cada vez que se importa un proyecto desde Microsoft Project, se crea un nuevo proyecto en Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 1%

---

# Importar un proyecto desde un proyecto de Microsoft

Puede importar proyectos de Microsoft Project a Adobe Workfront y administrarlos en una aplicación. Cada vez que se importa un proyecto desde Microsoft Project, se crea un nuevo proyecto en Workfront.

>[!IMPORTANT]
>
>No todos los campos de proyecto de Microsoft se transfieren a Workfront.
>
>Para obtener más información sobre la compatibilidad de los campos entre Workfront y Microsoft Project, consulte [Asignación de campos de proyecto de Microsoft a proyectos de Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Requisitos de acceso

redactado para P&amp;P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Licencia actual: Estándar </p> 
   O
   <p>Licencia heredada: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los proyectos, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concesión de acceso a proyectos</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Cuando crea un proyecto, automáticamente recibe permisos de administración para el proyecto </p> <p> Para obtener información sobre los permisos del proyecto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Uso compartido de un proyecto en Adobe Workfront</a>.</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los proyectos, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concesión de acceso a proyectos</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Cuando crea un proyecto, automáticamente recibe permisos de administración para el proyecto </p> <p> Para obtener información sobre los permisos del proyecto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Uso compartido de un proyecto en Adobe Workfront</a>.</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un proyecto a partir de un proyecto de MS

Puede crear un proyecto desde el área Proyectos del menú Principal o desde el área Proyectos de un portafolio o un programa.

1. Vaya a Proyecto de Microsoft y abra un proyecto que desee importar en Workfront.
1. Haga clic en **Archivo**, luego **Guardar como** para guardar el proyecto como archivo .xml.

1. Inicie sesión en Workfront.
1. Realice una de las siguientes acciones:

   * Haga clic en el **Menú principal** ![](assets/main-menu-icon.png), haga clic en **Proyectos** y, a continuación, expanda **Nuevo proyecto**.
   * Vaya a un portafolio y, a continuación, expanda **Nuevo proyecto**.
   * Vaya a un programa y, a continuación, expanda **Nuevo proyecto**.
   * Si es administrador de un grupo, también puede crear un proyecto en la sección Proyectos de un grupo que administre. Para obtener más información, consulte [Creación y modificación de los proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Elija la **Importar proyecto de MS** .

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Haga clic en **Seleccionar archivo**, busque el archivo .xml en el equipo que exportó desde Microsoft Project.
1. Importe el archivo seleccionado.

   Workfront inicia el proceso de importación y crea un nuevo proyecto basado en el archivo exportado desde Microsoft Project.

   Una vez completado el proceso de importación, se le dirige a la nueva página del proyecto que muestra una confirmación de que la importación se ha completado correctamente.

   >[!NOTE]
   >
   >Workfront tiene un límite de tiempo de 15 minutos en las cargas de archivos. Si la carga del archivo tarda más de eso, le recomendamos que divida el proyecto en proyectos más pequeños e los importe por separado. Una vez importadas en Workfront, mueva las tareas de un proyecto a otro para combinarlas en un proyecto. Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Opcional) Continúe editando el proyecto en Workfront. Para obtener información sobre la edición de proyectos, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

   El estado de un nuevo proyecto creado a partir de una plantilla se corresponde con el estado definido por el administrador de Workfront en el área Preferencias del proyecto o por un administrador de grupo en el área Preferencias del proyecto de grupo . Para obtener información sobre cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
