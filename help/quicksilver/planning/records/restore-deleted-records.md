---
title: Restaurar registros eliminados
description: Puede recuperar los registros eliminados del área Eliminados recientemente en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 17%

---

# Restauración de registros eliminados

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede recuperar los registros eliminados del área Eliminados recientemente en Adobe Workfront Planning.

Para obtener información acerca de cómo eliminar registros, vea [Eliminar registros](/help/quicksilver/planning/records/delete-records.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de contribución o superiores para un área de trabajo <span class="preview"> y tipo de registro </span> </a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>En el entorno de producción, todos los usuarios, incluidos los administradores del sistema, deben estar asignados a una plantilla de diseño que incluya Planning.</p>
<p><span class="preview">En el entorno de vista previa, los usuarios estándar y los administradores del sistema tienen Planning habilitado de forma predeterminada.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Consideraciones acerca de la recuperación de registros eliminados

* Los registros se almacenan en el grupo Eliminados recientemente durante 30 días. Después de 30 días, los registros se eliminan permanentemente de Workfront Planning.
* Si los registros eliminados están vinculados a otros registros, los registros vinculados no se eliminan, pero también se elimina la información del registro eliminado. La restauración de los registros eliminados restaurará la información de los registros conectados.
* Puede restaurar registros de forma masiva.
* Cuando se eliminan los registros, se almacena la siguiente información en el grupo Eliminados recientemente:
   * **Nombre**: Esta es la información del campo Principal del registro. Para obtener más información acerca de los campos primarios de registro, vea [Información general sobre el campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Fecha de eliminación**: La hora y la fecha en que se eliminó el registro.
   * **Tiempo en eliminaciones recientes**: El tiempo desde que se eliminó el registro. Los registros que se eliminaron más de 30 días antes de la fecha actual no se muestran en la bandeja Eliminados recientemente.
   * **Eliminado por**: Nombre del usuario que eliminó el registro.

## Restauración de registros eliminados

1. Vaya a la página de tipo de registro donde ha eliminado registros.
1. Haga clic en el icono **Deshacer** ![Deshacer icono](assets/undo-icon.png) en la esquina superior derecha de cualquier vista de página de tipo de registro y, a continuación, haga clic en **Eliminados recientemente**.

   Se muestra el cuadro **Eliminados recientemente**.

   ![Caja eliminada recientemente](assets/recently-deleted-box.png)

1. Seleccione los registros que desee eliminar y, a continuación, haga clic en **Restaurar** > **Restaurar**. Puede seleccionar más de un registro.

   Si la restauración se realizó correctamente, recibirá una notificación de éxito en la parte inferior de la pantalla.
1. Vaya a la vista de tabla y revise los registros restaurados.
