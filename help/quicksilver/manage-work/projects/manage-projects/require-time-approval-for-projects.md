---
product-area: projects
navigation-topic: manage-projects
title: Requerir tiempo de aprobación de un proyecto
description: Requerir tiempo de aprobación de un proyecto
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Requerir tiempo de aprobación de un proyecto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

Puede configurar el proyecto para que requiera que el propietario del proyecto apruebe las horas registradas en el proyecto. Cuando se configura de esta manera, el propietario del proyecto debe aprobar primero las horas para que puedan utilizarse en un registro de facturación.\
Para obtener más información acerca de los registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Al habilitar esta opción, no se elimina la capacidad de un aprobador de hojas de horas para aprobar las horas en la hoja de horas. Si el propietario del proyecto no aprueba ni rechaza el tiempo, un aprobador de plantilla de horas puede aprobarlo de todos modos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar para requerir tiempo para ser aprobado en el proyecto</p>
   <p>Revisar o superior para aprobar las horas registradas en un proyecto</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos o superior</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos del proyecto o superior</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acceso adicional</td> 
   <td> <p>Debe cumplir al menos una de las siguientes condiciones para aprobar el tiempo de un proyecto:</p> 
    <ul> 
     <li>Usted es el propietario del proyecto con el acceso y los permisos especificados anteriormente. En este caso, puede hacer lo siguiente si se da una de las siguientes condiciones: 
      <ul>
       <li>Si tiene permisos de administración en el proyecto, puede aprobar o rechazar horas registradas en el proyecto por cualquier otro usuario.</li>
       <li> Si tiene acceso de Contribute o Ver al proyecto, solo podrá aprobar o rechazar las horas registradas por usted o por cualquier otro usuario que informe sobre usted.<br></li>
      </ul></li> 
     <li>Tiene una licencia de planificación con acceso administrativo a hojas de horas y horas. En este caso:
      <ul>
       <li>Puede aprobar o rechazar cualquier hora de los proyectos para los que tenga al menos permisos de visualización. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requerir tiempo de aprobación de un proyecto

Para requerir la aprobación del administrador del proyecto para las horas del proyecto:

1. Vaya al proyecto en el que desea requerir la aprobación de horas.
1. Haga clic en el icono **Más** ![](assets/more-icon.png) a la derecha del nombre del proyecto y luego haga clic en **Editar**.\
   Aparece el cuadro de diálogo Editar proyecto.

1. En la sección **Configuración del proyecto**, seleccione **Requerir tiempo para aprobar este proyecto**.
1. Haga clic en **Guardar**.\
   Ahora, cuando se registra y aprueba el tiempo, esas horas se bloquean y el usuario que las introdujo en el proyecto o en la hoja de horas no las puede modificar. Solo un administrador de Workfront puede ajustar el tiempo registrado.

## Aprobar y rechazar tiempos en un proyecto

Como jefe de proyecto, puede aprobar o rechazar horas que se hayan registrado para tareas, problemas o el proyecto.

La aprobación de horas en el nivel de proyecto no afecta la hoja de horas de ninguno de los usuarios que han registrado las horas. Por ejemplo, las horas del proyecto pueden ser aprobadas por el jefe de proyecto, pero la hoja de horas aún no ha sido aprobada por el jefe de usuario o por el aprobador de la hoja de horas. 

Si configura un proyecto para que requiera aprobación sobre las horas registradas, el administrador del proyecto debe aprobar las horas para que estén disponibles para ser incluidas en un registro de facturación para el proyecto. Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

Para aprobar o rechazar horas en un proyecto:

1. Vaya al proyecto.
1. Haga clic en el área **Horas** del panel izquierdo. Puede encontrarse en el área **Mostrar más**.

1. Se muestran las horas registradas para problemas, tareas y el proyecto, y deben tener un estado de **Enviado**.\
   Haga clic en el cuadro de la izquierda de las entradas de horas para seleccionar las horas que desea aprobar.

1. Haga clic en **Aprobar**.\
   El estado de las horas cambia a **Aprobado**.\
   Si posteriormente rechaza las horas aprobadas, el estado de las horas cambia a **No aprobado**.\
   Cuando se incluyen las horas aprobadas en un registro de facturación, el estado de las horas cambia a **Facturado y aprobado**. Las horas agregadas a un registro de facturación no se pueden eliminar. Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Opcional) Haga clic en **Rechazar** para rechazar las entradas de tiempo del proyecto.\
   El estado de las horas cambia a **Rechazado**.
