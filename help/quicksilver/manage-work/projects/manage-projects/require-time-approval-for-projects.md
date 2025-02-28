---
product-area: projects
navigation-topic: manage-projects
title: Requerir tiempo de aprobación de un proyecto
description: Requerir tiempo de aprobación de un proyecto
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 79%

---

# Requerir tiempo de aprobación de un proyecto

<!--audited: 08/2024-->

Puede configurar el proyecto para requerir que el propietario del proyecto apruebe las horas registradas en el proyecto. Cuando se configura de esta manera, el propietario del proyecto debe aprobar primero las horas para que puedan utilizarse en un registro de facturación.\
Para obtener más información sobre los registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Al habilitar esta opción, no se elimina la posibilidad de que un aprobador de plantilla de horas apruebe las horas en la plantilla de horas. Si el propietario del proyecto no aprueba ni rechaza el tiempo, un aprobador puede aprobarlo en una plantilla de horas.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Para requerir tiempo para aprobarse en el proyecto:</p>
   <ul><li>Nuevo: estándar</li>
   <li>Actual: plan</li></ul>

<p>Para aprobar horas registradas en un proyecto:</p>
   <ul><li>Nuevo: Light o superior</li>
   <li>Revisión o superior</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a Proyectos o superior</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización del proyecto o superiores</p>
  </tr> 
  <tr> 
   <td role="rowheader">Acceso adicional</td> 
   <td> <p>Debe cumplir al menos una de las siguientes condiciones para aprobar el tiempo en un proyecto:</p> 
    <ul> 
     <li>Ser el propietario del proyecto con el acceso y los permisos especificados anteriormente. En este caso, puede hacer lo siguiente si se da una de las siguientes condiciones: 
      <ul>
       <li>Si tiene permisos de administración en el proyecto, puede aprobar o rechazar las horas registradas en el proyecto por cualquier otro usuario.</li>
       <li> Si tiene acceso de aportación o visualización en el proyecto, solo podrá aprobar o rechazar las horas registradas por usted o por cualquier otro usuario que le informe de ello.<br></li>
      </ul></li> 
     <li>Tiene una licencia de planificación con acceso administrativo a hojas de horas y horas. En este caso:
      <ul>
       <li>Puede aprobar o rechazar cualquier hora de los proyectos para los que tenga al menos permisos de visualización. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requerir tiempo de aprobación de un proyecto

Para requerir la aprobación por parte del gerente del proyecto de las horas del proyecto:

1. Vaya al proyecto en el que desea requerir la aprobación de horas.
1. Haga clic en el icono **Más** ![Más icono](assets/more-icon.png) a la derecha del nombre del proyecto y, a continuación, haga clic en **Editar**.\
   Aparecerá el cuadro de diálogo Editar proyecto.

1. En la sección **Configuración del proyecto**, seleccione **Requerir tiempo de aprobación de este proyecto**.
1. Haga clic en **Guardar**.\
   Ahora, cuando se registra y aprueba el tiempo, esas horas se bloquean y el usuario que las introdujo en el proyecto o en la hoja de horas no las puede modificar. Solo un administrador de Workfront puede ajustar el tiempo registrado.

## Aprobar y rechazar tiempos en un proyecto

Como gerente del proyecto, puede aprobar o rechazar las horas que se hayan registrado para tareas, problemas o el proyecto.

La aprobación de horas a nivel de proyecto no tiene ningún impacto en la plantilla de horas de ninguno de los usuarios que han registrado las horas. Por ejemplo, las horas del proyecto pueden ser aprobadas por el gerente del proyecto, pero la plantilla de horas aún no ha sido aprobada por el administrador del usuario o por el aprobador de la plantilla de horas.

Si configura un proyecto para que requiera la aprobación de las horas registradas, el administrador del proyecto debe aprobar las horas para que se puedan incluir en un registro de facturación del proyecto. Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

Para aprobar o rechazar las horas de un proyecto:

1. Vaya al proyecto. 
1. Haga clic en el área **Horas** del panel izquierdo. Puede encontrarse en el área **Mostrar más**.

1. Se muestran las horas registradas para problemas, tareas y el proyecto, y deben tener un estado de **Enviado**.\
   Haga clic en el cuadro situado a la izquierda de las entradas de horas para seleccionar las horas que desea aprobar.

1. Haga clic en el icono **Aprobar** ![](assets/approve-hours-icon.png) en la parte superior de la lista de horas.\
   El estado de las horas cambia a **Aprobado**.\
   Si posteriormente rechaza las horas aprobadas, el estado de las horas cambia a **No aprobado**.\
   Cuando se incluyen las horas aprobadas en un registro de facturación, el estado de las horas cambia a **Facturado y aprobado**. Las horas añadidas a un registro de facturación no se pueden eliminar. Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Opcional) Haga clic en el icono **Rechazar** ![](assets/reject-hours-icon.png) para rechazar las entradas de tiempo del proyecto.\
   El estado de las horas cambia a **Rechazado**.

   >[!NOTE]
   >
   >   Si las horas que selecciona se incluyen en un Registro de facturación que se ha marcado como Facturado o Facturado y aprobado, no se muestran los iconos Aprobar y Rechazar. Solo puede aprobar horas que aún no se hayan facturado en un Registro de facturación.

