---
title: Administrar registros en la sección de planificación de objetos de Adobe Workfront
description: Puede mostrar los registros de Workfront Planning conectados a objetos de Adobe Workfront en la sección Planning de un objeto de Workfront, en el panel izquierdo.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# Administrar registros en la sección Planificación de objetos de Adobe Workfront

{{planning-important-intro}}

Puede mostrar los registros de Workfront Planning conectados a objetos de Adobe Workfront en la sección Planning de un objeto de Workfront, en el panel izquierdo.

La sección Planificación está disponible para los siguientes objetos de Workfront:

* Proyecto
* Portafolio
* Programar
<!--* Group
* Company-->

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

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
   <td role="rowheader"><p>plan Adobe Workfront*</p></td>
   <td>
<p>Cualquiera de los siguientes planes de Workfront:</p>
<ul><li>Seleccionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning no está disponible para planes Workfront heredados</p>
   </td>

<tr>
   <td role="rowheader"><p>Plan de planificación de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera</p>
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td>
   <td>
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p>
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>Acceso de visualización o superior a Proyectos, Programas y Portfolio</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td>
   <p>En Workfront, vea o supere los permisos de un proyecto, portafolio o programa</a> </p> 
   <p>En Workfront Planning, Contribute o permisos superiores para un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo de Workfront Planning, incluidos los que no crearon</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal y el área de Planning para proyectos, portafolios y programas. </p> Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Información general sobre el acceso</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre la sección Planificación de objetos de Workfront

Tenga en cuenta lo siguiente cuando vea los registros de Workfront Planning desde la sección Planning de un objeto Workfront:

* Los tipos de registros de Workfront Planning deben conectarse primero a los tipos de objetos de Workfront.

  Para obtener más información, consulte los siguientes artículos:

   * [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Conectar registros](/help/quicksilver/planning/records/connect-records.md)
* Puede ver la sección de Planning desde un objeto de Workfront, incluso cuando no haya registros asociados al objeto de Workfront.
* Además de conectar objetos de Workfront desde el área de Planning de Workfront, puede conectar registros de Planning con objetos de Workfront desde Workfront desde la sección Planning.

## Administrar registros en la sección Planificación

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en la tarjeta de un tipo de registro conectado a un proyecto, portafolio o programa de Workfront.
1. Vaya a un campo de registro conectado que tenga una conexión con un objeto Workfront, ya sea en la vista de tabla o desde la página de detalles de un registro. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Haga clic en el nombre de un objeto Workfront en el campo de registro conectado.
La página del objeto se abre en Workfront.

   >[!NOTE]
   >
   >  Si conoce un objeto de Workfront que ya está conectado a un registro de Planning, puede desplazarse a la sección de Planning desde el objeto de Workfront.

1. Haga clic en **Planificación** en el panel izquierdo.

   >[!NOTE]
   >
   >   El administrador de Workfront o de grupo debe agregar la sección de planificación a la plantilla de diseño para que se muestre para un proyecto, portafolio o programa de Workfront.

   La sección Planificación se muestra con la siguiente información:

   * Los registros conectados se muestran en tarjetas individuales que contienen la siguiente información:
      * Nombre del registro
      * La miniatura del registro
      * Nombre del campo de registro conectado tal como se muestra en Workfront Planning.
   * Los registros se muestran en su espacio de trabajo respectivo.

   ![](assets/planning-section-on-project.png)

1. (Opcional) Haga clic en **Mostrar todas las conexiones** para mostrar todos los tipos de registros conectados, incluidos los que no tienen registros conectados. De forma predeterminada, no se muestran los tipos de registros sin registros conectados.
1. Haga clic en una tarjeta de registro para mostrar más información sobre el registro. Se muestra el cuadro de vista previa de registros.
1. (Opcional) Comience a modificar los campos en el cuadro de vista previa del registro. Los cambios se guardarán automáticamente.
1. (Opcional) Haga clic en el icono **Abrir en una nueva ficha** ![](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha del cuadro de vista previa para abrir la página de detalles del registro. Se abre la página de detalles del registro en Workfront Planning.
1. (Opcional) Pase el ratón sobre una tarjeta de registro, haga clic en el icono de registro de desconexión **-** y, a continuación, haga clic en **Desconectar**.
Ocurren lo siguiente:
   * El registro ya no está conectado al objeto Workfront.
   * El objeto Workfront también se quita del campo conectado del registro de Workfront Planning.
   * También se eliminan los valores de los campos de búsqueda de Workfront conectados al registro de Planning.
1. Haga clic en **Conectar** para conectar más registros para los tipos de registros conectados. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   Ocurren lo siguiente:

   * Los registros se conectan inmediatamente al objeto Workfront y se muestran en la sección Planificación.
   * El objeto Workfront se agrega al campo conectado del registro de Workfront Planning.
   * Los valores de los campos de búsqueda de Workfront conectados al registro de Planning se rellenan en Workfront Planning.


