---
product-area: projects
navigation-topic: manage-projects
title: Requerir tiempo para ser aprobado para un proyecto
description: Requerir tiempo para ser aprobado para un proyecto
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Requerir tiempo para ser aprobado para un proyecto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

Puede configurar el proyecto para que requiera que el propietario del proyecto apruebe las horas registradas en el proyecto. Cuando se configura de esta manera, el propietario del proyecto debe aprobar primero las horas antes de que se puedan usar en un registro de facturación.\
Para obtener más información sobre los registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Al habilitar esta opción, no se elimina la capacidad de un aprobador de hojas de horas de aprobar la hora en el parte de horas. Si el propietario del proyecto no aprueba o rechaza la hora, un aprobador de parte de horas puede aprobar la hora en un parte de horas.

## Requisitos de acceso

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
   <td> <p>Planificar para requerir tiempo para ser aprobado en el proyecto</p>
   <p>Revisar o superior para aprobar las horas registradas en un proyecto</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos o versiones posteriores</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para el proyecto o superior</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acceso adicional</td> 
   <td> <p>Debe cumplir al menos una de las siguientes condiciones para aprobar el tiempo de un proyecto:</p> 
    <ul> 
     <li>Usted es el propietario del proyecto con el acceso y los permisos especificados anteriormente. En este caso, puede hacer lo siguiente si existe una de las condiciones siguientes: 
      <ul>
       <li>Si tiene permisos de administración en el proyecto, puede aprobar o rechazar las horas registradas en el proyecto por cualquier otro usuario.</li>
       <li> Si tiene acceso a Contribute o View al proyecto, sólo podrá aprobar o rechazar las horas registradas por usted o por cualquier otro usuario que informe de usted.<br></li>
      </ul></li> 
     <li>Tiene una licencia de Plan con acceso administrativo a Hojas de Hora y Horas. En este caso:
      <ul>
       <li>Puede aprobar o rechazar cualquier hora en los proyectos que tenga al menos permisos para ver. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requerir tiempo para ser aprobado para un proyecto

Para requerir la aprobación del administrador de proyectos para horas en el proyecto:

1. Vaya al proyecto en el que desea requerir aprobación para horas.
1. Haga clic en el **Más** icono ![](assets/more-icon.png) a la derecha del nombre del proyecto y, a continuación, haga clic en **Editar**.\
   Aparece el cuadro de diálogo Editar proyecto .

1. En el **Configuración del proyecto** , seleccione **Requerir tiempo para ser aprobado para este proyecto**.
1. Haga clic en **Guardar**.\
   Ahora, cuando el tiempo se registra y aprueba, esas horas se bloquean y el usuario que las introdujo en el proyecto o en el parte de horas no puede modificarlas. Solo los administradores de Workfront pueden ajustar el tiempo registrado.

## Aprobar y rechazar la hora de un proyecto

Como administrador de proyectos, puede aprobar o rechazar las horas registradas para tareas, problemas o el proyecto.

La aprobación de las horas en el nivel de proyecto no tiene ningún impacto en el parte de horas de ninguno de los usuarios que registraron las horas. Por ejemplo, el administrador del proyecto puede aprobar las horas del proyecto, pero el administrador del usuario o el aprobador de hojas de horas aún no lo han aprobado. 

Si configura un proyecto para que requiera aprobación en las horas registradas, el administrador del proyecto debe aprobar las horas para que estén disponibles para incluirse en un registro de facturación del proyecto. Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

Para aprobar o rechazar horas en un proyecto:

1. Vaya al proyecto.
1. Haga clic en el **Horas** del panel izquierdo. Esto puede encontrarse en la sección **Mostrar más** .

1. Las horas registradas para problemas, tareas y la visualización del proyecto y deben tener un estado de **Enviado**.\
   Haga clic en el cuadro de la izquierda de las entradas de la hora para seleccionar las horas que desea aprobar.

1. Haga clic en **Aprobar**.\
   El estado de las horas cambia a **Aprobado**.\
   Si posteriormente rechaza las horas aprobadas, el estado de las horas cambia a **No aprobado**.\
   Cuando se incluyen las horas aprobadas en un registro de facturación, el estado de las horas cambia a **Facturado y aprobado**. Las horas agregadas a un registro de facturación no se pueden eliminar. Para obtener más información sobre la creación de registros de facturación, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Opcional) Haga clic en **Rechazar** para rechazar las entradas de hora del proyecto.\
   El estado de las horas cambia a **Rechazado**.
