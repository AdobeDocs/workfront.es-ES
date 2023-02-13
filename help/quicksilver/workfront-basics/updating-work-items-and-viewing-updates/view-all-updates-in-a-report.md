---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Ver todas las actualizaciones en un informe de Nota
description: Ver todas las actualizaciones en un informe de Nota
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Ver todas las actualizaciones en un informe de Nota

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

El área Actualizaciones de un objeto muestra un número máximo de 200 actualizaciones de forma predeterminada. Para ver todas las actualizaciones que cualquiera de los usuarios ha introducido para un objeto, puede crear un informe de Nota que muestre todas las actualizaciones.

>[!NOTE]
>
>Puede crear un informe para ver las actualizaciones de los objetos en Vista previa con el informe de entrada de Journal. Para obtener más información, consulte [Informe del área Actualizaciones](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a:</p> 
    <ul> 
     <li> <p>Creación de informes, tableros y calendarios</p> </li> 
     <li> <p>Crear filtros, vistas y grupos</p> </li> 
    </ul> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Vista</p> <p>Nota: Si no tiene el permiso Ver o superior a un objeto, la información de ese objeto no se muestra en el informe.</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un informe de notas

La creación de un informe para Notas para cualquier objeto es idéntica, independientemente del objeto.

Por ejemplo, para crear un informe de Nota para todas las notas de un proyecto:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, elija **Nota**.

1. (Opcional) Haga clic en **Vistas**, luego **Agregar columna** para agregar la variable **Nombre** del **Proyecto** en la vista del informe. 

1. (Opcional) Haga clic en **Agrupaciones**, luego **Agregar agrupación** para agrupar por **Nombre del proyecto**, si va a generar informes sobre varios proyectos al mismo tiempo.\
   Esto garantiza que las notas se agrupen por sus respectivos proyectos, lo que facilita la lectura del informe. 

1. (Opcional) Haga clic en **Filtros,** then **Agregar una regla de filtro** para filtrar solo por un proyecto o por proyectos específicos.

1. (Condicional y opcional) Configure el **Nombre del proyecto** como **Igual** al nombre del proyecto para el que desea ver las actualizaciones.  

1. Haga clic en **Guardar + Cerrar**.\
   En el informe se muestran todas las actualizaciones introducidas en el proyecto por todos los usuarios con permisos para al menos Ver el proyecto.
