---
content-type: release-notes
navigation-topic: product-releases
title: Información general sobre la versión 20.4
description: La versión 20.4 se publicó en el entorno de producción la semana del 9 de noviembre de 2020. Para ver las fechas y horas de lanzamiento específicas de cada clúster, consulte el sitio de estado de Workfront.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7cf7f6ed-fe85-4c86-bb4b-dd93197338cf
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3695'
ht-degree: 99%

---

# Información general sobre la versión 20.4

La versión 20.4 se publicó en el entorno de producción la semana del 9 de noviembre de 2020.

Esta página proporciona información sobre la funcionalidad tanto para Adobe Workfront Classic como para la nueva experiencia de Adobe Workfront que se incluye en la versión 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 20.4 release nears its planned Production release, this page will be updated with all functionality included with 20.4.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of November 9, 2020. For specific release dates and times for each cluster, see the <a href="https://status.workfront.com/" target="_blank">Workfront Status Site</a>. </p>
-->

## Mejoras de Workfront

* [Mejoras del administrador](#administrator-enhancements)
* [Mejoras de administración de recursos](#resource-management-enhancements)
* [Mejoras de administración de proyectos](#project-management-enhancements)
* [Análisis mejorado](#enhanced-analytics)
* [Mejoras en la revisión](#proofing-enhancements)
* [Mejoras en la aplicación móvil y de integración](#mobile-and-integration-enhancements)
* [Otras mejoras](#other-enhancements)

### Mejoras en el administrador {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Nuevo para administradores: controle cómo se comparte un campo personalizado</a> </p> <p>Para brindar un mayor control sobre quién puede editar, eliminar y utilizar los campos personalizados que crea, hemos añadido la capacidad de configurar exactamente cómo desea que se compartan.</p> <p>Hasta ahora, cuando creaba un campo personalizado, todos los miembros del sistema podían editarlo. Este sigue siendo el estado predeterminado de un campo personalizado, pero ahora puedes limitar el uso compartido de un campo personalizado a ciertos usuarios, roles, equipos, grupos y empresas. Y puede determinar si los destinatarios pueden administrar o solo ver el campo personalizado.</p> <p>Además, para que esta experiencia te resulte familiar, hemos diseñado la interfaz de usuario de esta funcionalidad de manera similar a otras áreas de compartición de objetos en Workfront.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 15 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">Nuevo para administradores: uso compartido de formularios personalizados estandarizados</a> </p> <p>Hemos estandarizado el uso compartido de formularios personalizados para que puedas utilizar el mismo proceso de compartición de objetos de Workfront que ya conoces. Además, la nueva experiencia de uso compartido le proporciona un mayor control sobre quién puede editar, eliminar y utilizar formularios personalizados que cree. Puede limitar el uso compartido de un formulario personalizado a determinados usuarios, funciones, equipos, grupos y empresas. Además, puede determinar si esos destinatarios pueden ver o administrar el formulario personalizado.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 15 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nuevo para administradores: opción de cambio de entorno de Workfront disponible</a> </p> <p>Para obtener una experiencia más eficiente y práctica, los administradores de grupo y de Workfront ahora pueden cambiar rápidamente entre diferentes entornos de Workfront desde cualquier página de Workfront sin tener que cerrar la sesión.</p> <p>En la nueva experiencia de Workfront, la opción Cambiar a Classic aparece en el menú principal.</p> <p>En Workfront Classic, la opción Cambiar a la nueva experiencia aparece en el menú que se muestra al hacer clic en la imagen de perfil de la esquina superior derecha de la barra de navegación global.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 8 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">Nuevo para administradores: los administradores de un grupo asignado a una compañía pueden administrar la compañía</a> </p> <p>Hemos facilitado a un administrador de grupo la gestión de una empresa asociada a su grupo en Workfront. El acceso para administrar la compañía está disponible automáticamente cuando se realiza la asociación. Esto es especialmente importante cuando el administrador del grupo no tiene acceso administrativo a las empresas.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 8 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Nuevo para administradores: mejoras en las notificaciones por correo electrónico</a> </p> <p>Ahora, con un solo clic, puede habilitar o deshabilitar una notificación de evento por correo electrónico en Configuración. Simplemente, haga clic en el interruptor Activado/Desactivado junto al nombre de la notificación.</p> <p>Además, observe que con nuestro moderno estilo ahora ha mejorado la experiencia de configuración de notificaciones de eventos en el área Notificaciones por correo electrónico.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 8 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuevo para administradores: asociar portafolios, programas y compañías a grupos</a> </p> <p>Cuando los administradores de Workfront crean o editan un portafolio, un programa o una compañía, pueden asignarlo a un grupo. Con los grupos asignados a estos objetos, es fácil identificar las responsabilidades de tu grupo para ellos. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 25 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Asignar un grupo a un equipo</a> </p> <p>Para facilitar la gestión y generación de informes sobre los equipos asociados a un grupo, ahora puedes asignar cualquier grupo a un equipo que tengas acceso para editar.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 29 de agosto de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuevo para administradores: asignar un coordinador empresarial a un grupo</a> </p> <p>Para ayudarle a organizar y definir mejor sus grupos, hemos añadido la capacidad de asignar un usuario como coordinador empresarial para un grupo (o subgrupo). Un coordinador empresarial es un usuario de Workfront que toma decisiones comerciales para un grupo.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 21 de agosto de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Introducción de Workfront para MobileIron</a> </p> <p>Workfront se ha asociado a MobileIron, una plataforma de administración de dispositivos móviles (MDM) para ofrecer a las organizaciones una experiencia móvil más segura y controlada.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: N/D</p> <p>Versión de producción: 21 de agosto de 2020</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras en la administración de recursos {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#plan" class="MCXref xref" xrefformat="{para}">Planificar el trabajo mediante el campo Esfuerzo de trabajo en lugar de Horas planificadas</a> </p> <p>Para ofrecerle flexibilidad a la hora de planificar el trabajo en sus proyectos, hemos introducido el nuevo concepto de esfuerzo laboral para las tareas. Puede estimar si el esfuerzo laboral de una tarea es pequeño, mediano o grande sin estimar manualmente las horas planificadas para la tarea. Cada nivel de esfuerzo se calcula en función de un porcentaje de tiempo desde las horas típicas al día configuradas en la instancia.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 8 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#project" class="MCXref xref" xrefformat="{para}">Colores basados en el estado del proyecto para elementos de trabajo en el Distribuidor de cargas de trabajo</a> </p> <p>Para obtener una mejor visibilidad y una mayor personalización de la experiencia en el Distribuidor de cargas de trabajo, ahora puede cambiar los colores de los proyectos y sus elementos de trabajo para que coincidan con el estado de los proyectos. Los colores corresponden a estados de proyecto de nivel de grupo o de nivel de sistema. Los colores mostrados pueden corresponder tanto a los estados del sistema como a los del proyecto personalizado.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 8 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#adjust" class="MCXref xref" xrefformat="{para}">Ajustar la asignación de usuarios mediante valores de porcentaje en el Distribuidor de cargas de trabajo</a> </p> <p>Ahora puede administrar las asignaciones de los usuarios en el Distribuidor de cargas de trabajo mediante porcentajes en lugar de horas.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 8 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuevo icono para cambiar entre horas y valores de porcentaje, o entre el tiempo asignado y el tiempo restante en el Distribuidor de cargas de trabajo</a> <p>Se ha añadido una nueva configuración que le permite cambiar entre las horas asignadas y los porcentajes a medida que se ve el Distribuidor de cargas de trabajo. Con este nuevo icono, también hemos eliminado la sección Carga de trabajo del usuario en el panel Configuración. El Distribuidor de cargas de trabajo muestra el tiempo asignado de forma predeterminada y se ha movido la configuración de horas restantes al nuevo icono de porcentaje u horas.</p></td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 25 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#a" class="MCXref xref" xrefformat="{para}">Nuevo filtro integrado para el Distribuidor de cargas de trabajo: usuarios en proyectos</a> </p> <p>Para que su experiencia de filtrado en el Distribuidor de cargas de trabajo sea más eficiente, hemos añadido un nuevo filtro integrado en el área de Trabajo asignado. Ahora puede aplicar el filtro Usuarios en proyectos, que muestra los usuarios asignados a tareas y problemas en los proyectos que especifique.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 25 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#visualiz" class="MCXref xref" xrefformat="{para}">Visualice el trabajo completado en el distribuidor de cargas de trabajo</a> </p> <p>Para permitirle identificar fácilmente el trabajo que ya se ha completado y poder administrar las asignaciones de usuario correctamente, hemos habilitado un indicador visual en el Distribuidor de cargas de trabajo que muestra cuándo se han completado los elementos de un lapso de tiempo seleccionado. Ahora puede ver una marca de verificación verde para las tareas y los problemas cuando se completan. El proyecto también muestra la marca de verificación verde cuando hay elementos de trabajo completados durante el lapso de tiempo mostrado en la pantalla.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 11 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuevo filtro predeterminado para el área de trabajo asignado en el distribuidor de cargas de trabajo</a> </p> <p>El filtro predeterminado para el área de Trabajo asignado en el Distribuidor de cargas de trabajo ahora muestra solo los usuarios que son miembros de todos los equipos a los que usted, como usuario que ha iniciado sesión, está asociado. El nuevo filtro ahora muestra la información más relevante para usted, de forma predeterminada.</p> <p>Antes de esta mejora, todos los usuarios a los que tenía acceso se mostraban en esta área. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 11 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#user" class="MCXref xref" xrefformat="{para}">Gráfico de asignación de usuarios en el distribuidor de cargas de trabajo</a> </p> <p>Para permitirle tener una representación visual de alto nivel de la asignación de los usuarios en un lapso de tiempo determinado, una nueva configuración ahora habilita una vista de gráfico de cómo se muestran las asignaciones en el Distribuidor de cargas de trabajo. Al habilitar esta configuración, se muestra la asignación de los usuarios en un gráfico de líneas que indica las sobreasignaciones en bloques rojos y las infraasignaciones en azul. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 29 de agosto de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#show" class="MCXref xref" xrefformat="{para}">Mostrar u ocultar trabajo completado en el distribuidor de cargas de trabajo</a> </p> <p>Ahora, una nueva configuración le permite mostrar u ocultar los elementos de trabajo completados en el Distribuidor de cargas de trabajo. La configuración está habilitada de forma predeterminada y los elementos de trabajo completados que coinciden con los criterios de filtrado y el lapso de tiempo seleccionados se muestran en el Distribuidor de cargas de trabajo. </p> <p>Antes de esta mejora, los elementos de trabajo completados siempre se mostraban en el Distribuidor de cargas de trabajo.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 21 de agosto de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#usabilit" class="MCXref xref" xrefformat="{para}">Mejoras de uso del distribuidor de cargas de trabajo</a> </p> <p>Para garantizar una experiencia optimizada y fácil de usar al administrar los recursos en el distribuidor de cargas de trabajo, ahora hay disponibles varias mejoras de uso.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 21 de agosto de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras en la administración de proyectos {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Exportar formularios personalizados e información general desde la sección Detalles de un proyecto, tarea o problema</a> </p> <p>Ahora puede exportar la información del formulario personalizado a un archivo PDF. Puede exportar formularios personalizados desde proyectos, tareas o problemas cuando acceda al formulario en la sección de Detalles de los objetos. </p> <p>Además de exportar los formularios personalizados de proyectos, tareas y problemas, ahora puede incluir el área Información general en el PDF exportado.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 15 de octubre de 2020 (la exportación del área Información general se añadió el 3 de noviembre de 2020)</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#quickly" class="MCXref xref" xrefformat="{para}">Añadir rápidamente una iteración</a> </p> <p>Para simplificar la experiencia de creación de una iteración, se ha añadido un nuevo botón que permite añadir una iteración desde la pestaña iteraciones. Aquí puede crear una iteración y luego añadir tareas y problemas más adelante.</p> <p>Puede seguir creando una iteración en la etiqueta de registro de pendientes como antes.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 15 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4 <span style="color: #dc143c; font-weight: bold;">No disponible temporalmente</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">Nueva sección de métricas disponible en proyectos</a> </p> <p>Para ahorrar tiempo y aumentar la comprensión del estado general de un proyecto, ahora hay una sección de Métricas disponible en un proyecto que incluye información sobre lo siguiente:</p> 
    <ul> 
     <li>Trabajo completado, incompleto, vencido y próximo</li> 
     <li>Cantidades de tarea y problema agrupadas por estado o prioridad</li> 
     <li>Esfuerzo laboral asignado a cada usuario</li> 
    </ul> <p>Puede hacer selecciones en los gráficos para ver diferentes aspectos de las tareas y problemas de un proyecto y hacer clic en ciertos elementos para mostrar la información de las tareas.</p> <p>Para obtener más información, consulte <a href="../../../manage-work/projects/manage-projects/project-metrics.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Información general sobre las métricas del proyecto</a>.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 23 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nueva opción para cancelar su acción al descartar un borrador de solicitud</a> <p>Al descartar un borrador guardado, ahora puede hacer clic en Cancelar en el mensaje de confirmación que le informa de que se eliminará el borrador. De este modo, no perderá el borrador en caso de que cambie de opinión sobre su descarte.</p></td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 25 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#replace" class="MCXref xref" xrefformat="{para}">Reemplazar el botón Trabajar en ello por un botón Inicio</a> </p> <p>Para ayudar a registrar la fecha y hora en que realmente comienza el trabajo en un elemento, los usuarios pueden reemplazar el botón Trabajar en ello por el botón Inicio que actualiza automáticamente el estado y la Fecha de Inicio Real del elemento de trabajo.</p> </td> 
   <td> <p><strong>Disponible en estas fechas:</strong> </p> <p>Versión preliminar beta: 20 de agosto de 2020</p> <p>Versión de producción: 8 de octubre de 2020</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Los nuevos campos permiten informar sobre los datos de un grupo de nivel superior y todos sus subgrupos</a> </p> <p>Para identificar los datos asociados con un grupo de nivel superior y sus subgrupos, hemos añadido un nuevo campo de ID de Grupo Principal que puede usar en Filtros, Vistas y Agrupaciones cuando cree informes sobre objetos de Grupo.</p> <p>Este campo debe ser especialmente útil para los administradores de grupo que administran grupos que contienen varios subgrupos.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 29 de agosto de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#allow" class="MCXref xref" xrefformat="{para}">Permite varios borradores para un tema de la cola</a> </p> <p>Para darle más libertad al trabajar con solicitudes, ya no hay un límite para la cantidad de borradores que puede guardar para un tema en cola. Al crear una nueva solicitud, puedes seleccionar un borrador existente de una lista de borradores para el mismo tema de la cola, sobrescribirlo y enviarlo como una nueva solicitud o puedes crear una nueva solicitud desde cero. </p> <p>Antes de esta mejora, Workfront solo guardaba un borrador para cada tema de la cola en la cola de solicitudes. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 21 de agosto de 2020</p> <p>Versión de producción: 17 de septiembre de 2020</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Análisis mejorado  {#enhanced-analytics}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-analytics-enhancements.md#paginati" class="MCXref xref" xrefformat="{para}">Paginación y ordenación añadidas al análisis mejorado</a> </p> <p>Para permitirle ver la información que desea ver sin tener que aplicar filtros restrictivos, hemos añadido opciones de paginación y ordenación a cada gráfico en el área Análisis mejorado.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 8 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras de revisión {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#carry" class="MCXref xref" xrefformat="{para}">Arrastre el flujo de trabajo de prueba existente al generar una nueva versión</a> </p> <p>Ahora, el flujo de trabajo de revisión existente se transfiere a cualquier versión nueva que cree, independientemente del método en el que se genere.</p> <p>Anteriormente, había una ligera diferencia en la forma en que se transfería el flujo de trabajo de la revisión según el lugar donde se generaba en Workfront.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 8 de octubre de 2020</p> <p>Versión de producción: con la versión de 20.4 <span class="uitext" style="color: #dc143c;">(pospuesta a marzo de 2021)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#auto-gen" class="MCXref xref" xrefformat="{para}">Genere automáticamente una prueba al cargar una configuración de documento deshabilitada de forma predeterminada</a> </p> <p>La opción en el perfil de usuario para generar automáticamente pruebas al cargar documentos ahora está deshabilitada de forma predeterminada para los nuevos usuarios de revisión. Este cambio no afecta a los usuarios actuales. Si tiene esta configuración habilitada, seguirá siendo así.</p> <p>Anteriormente, esta configuración estaba habilitada para nuevos usuarios de forma predeterminada.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 18 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#document" class="MCXref xref" xrefformat="{para}">Botones de aprobación de documento disponibles en el Visor de corrección</a> </p> <p>Para alinearse con la experiencia de revisión en Campaign Classic, los botones de aprobación del documento ahora están disponibles en el Visor de corrección en la nueva experiencia de Adobe Workfront.</p> <p>Anteriormente, solo se podía aprobar un documento desde el área Detalles del documento.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 9 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras en aplicaciones móviles e integración {#mobile-and-integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#added" class="MCXref xref" xrefformat="{para}">Se añadió la funcionalidad en las notificaciones de Microsoft Teams</a> </p> <p>Para facilitar el uso de Workfront a través de Microsoft Teams, hemos añadido una nueva funcionalidad a las notificaciones de Microsoft Teams enviadas desde Workfront.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: por determinar</p> <p>Versión de producción: con la versión de 20.4 <strong> (pospuesta a diciembre de 2020 o principios de 2021)</strong></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#get" class="MCXref xref" xrefformat="{para}">Obtener ayuda con los comandos del asistente virtual de la aplicación móvil de Workfront</a> </p> <p>En la aplicación móvil, puede pedir al asistente virtual que le ayude con los comandos diciendo "¿Qué puedo hacer?" y "Ayúdame con los comandos".</p> <p>Estos comandos muestran una lista de las diferentes cosas que puede preguntarle al asistente.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: N/D</p> <p>Versión de producción: con la versión 20.4 </p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}">Crear una tarea rápidamente en la aplicación móvil de Workfront</a> </p> <p>Utilice la nueva opción de tarea rápida de la aplicación móvil de Workfront para crear tareas rápidamente. Solo tiene que introducir el nombre de la tarea y adjuntar los documentos que pueda tener. Si es necesario, puede seguir rellenando campos adicionales, como descripciones y asignaciones. Haga clic en la flecha a la derecha del nombre de la tarea.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar beta: 18 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Otras mejoras {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Se mejoró el cifrado para Workfront Proof</a> </p> <p>Estamos realizando algunos cambios para mejorar la seguridad del cifrado de datos en movimiento de la aplicación de corrección de Workfront. Los cifrados TLS débiles quedarán obsoletos el 11 de noviembre de 2020.</p> <p>Asegúrese de utilizar un explorador compatible al acceder a Workfront. </p> <p> </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 20 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nueva apariencia para 3 plantillas de correo electrónico</a> </p> <p>Para mejorar la legibilidad y la experiencia general, las siguientes plantillas de correo electrónico tienen una nueva apariencia</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 15 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nuevas notificaciones por correo electrónico para los equipos</a> </p> <p>Hemos añadido 2 nuevas notificaciones por correo electrónico para equipos: cuando se completa una sola tarea predecesora de una tarea asignada a su equipo y cuando se completan todas las tareas predecesoras de una tarea asignada a su equipo.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 15 de octubre de 2020</p> <p>Versión de producción: con la versión 20.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuevos objetos de API que activan las actualizaciones de suscripción de eventos</a> </p> <p>Se han creado dos nuevos objetos de API, documentVersion y proofApproval, que se configuran para activar actualizaciones de suscripción a eventos cuando se crea una versión de un documento o se aprueba uno. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 11 de septiembre de 2020</p> <p>Versión de producción: con la versión 20.4 en producción</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

## Mejoras en el Planificador de escenarios de Workfront

La mayoría de las nuevas funciones se incluyen en la versión del Planificador de escenarios de Workfront con la versión 20.4. Para obtener información sobre estas nuevas características que ya están disponibles en la vista previa, consulte [Planificador de escenarios de Workfront con la versión 20.4 (14 de octubre de 2020)](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-20-4.md).

## Mejoras de Workfront Goals

La mayoría de las nuevas funciones se incluyen en la versión 20.4 de Workfront Goals. Para obtener más información sobre estas nuevas características ya disponibles en vista previa, consulte [Workfront Goals con la versión 20.4](../../../product-announcements/product-releases/goals-release-activity/goals-release-20-4.md).

## Mejoras de Workfront Fusion

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción en una cadencia distinta a la de la versión 20.4. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)

## Mejoras de API

La versión 12 de la API ya está disponible con la versión 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Para obtener más información sobre novedades y actualizaciones, consulte [Novedades de la versión 12 de la API](https://experienceleague.adobe.com/es/docs/workfront/using/adobe-workfront-api/api-notes/new-api-version-12).

Para obtener más información sobre las versiones de API, consulte [Versiones de API y programación de soporte](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Actualizaciones de mantenimiento de Workfront 

Para obtener más información acerca de las actualizaciones de mantenimiento realizadas durante la versión 20.3, consulte [Actualizaciones de mantenimiento de Workfront](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Anuncios

* [Obsolescencia de Flash](#flash-deprecation)
* [Seminario web sobre la versión 20.4](#20-4-release-webinar)
* [Cambio en la cadencia de la versión preliminar](#change-in-preview-release-cadence)
* [Se requiere la lista de dominios adicionales permitidos para acceder a Workfront](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Workfront One](#workfront-one)

### Obsolescencia de Flash {#flash-deprecation}

A finales de 2020, Adobe y todos los exploradores principales dejarán de usar la tecnología Flash de Adobe, lo que significa que estas herramientas dejarán de funcionar.

El objetivo de Workfront es ayudarle a pasarse a las tecnologías más recientes mediante un conjunto de nuevas soluciones que no dependan de Flash. Obtenga más información acerca de soluciones de sustitución para cada herramienta específica basada en Flash en el siguiente artículo: [Reemplazo de herramientas basadas en Flash en Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

Todas las herramientas basadas en Flash se eliminarán de todos los productos el 19 de noviembre de 2020. Le recomendamos, por tanto, que comience a utilizar las nuevas herramientas y retire las herramientas de Flash antes de esa fecha que su instancia sea más segura. Si desea que deshabilitemos las herramientas de Flash antes del 19 de noviembre, puede ponerse en contacto con Atención al cliente.

### Seminario web sobre la versión 20.4 {#20-4-release-webinar}

El seminario web sobre la versión 20.4 de Workfront se presentará el miércoles, 28 de octubre de 2020 a las 11:00 h EDT. Regístrese al seminario web [aquí](https://webinars.on24.com/workfront/204release?partnerref=CXnewsletter).

### Cambio en la cadencia de la versión de vista previa {#change-in-preview-release-cadence}

A partir del 20 de mayo de 2020, Workfront empezó a ofrecer la funcionalidad en el entorno de vista previa de forma semanal. Antes de este cambio, la funcionalidad generalmente se publicaba en el entorno de vista previa cada dos semanas.

Para obtener más información, consulte [Preguntas frecuentes sobre el cambio en la cadencia de la versión preliminar de Workfront](https://experienceleague.adobe.com/es/docs/workfront/using/home)

### Lista de permitidos de dominios adicionales necesarios para acceder a Workfront {#allowlist-of-additional-domains-required-for-accessing-workfront}

Si su organización utiliza un cortafuegos, debe añadir los siguientes dominios adicionales a su lista de permitidos para garantizar un acceso ininterrumpido a Workfront:

* event.split.io
* sdk.split.io

Para obtener más información, consulte [Configurar la lista de permitidos del cortafuegos](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Workfront One {#workfront-one}

Con Workfront One, descubrirá el contenido, los recursos y las noticias más importantes de Workfront: todo en un solo lugar, con un solo inicio de sesión. Hemos unificado los sitios de experiencia, comunidad y formación, para que le resulte más fácil encontrar lo que busca.

[Más información sobre Workfront One](https://business.adobe.com/es/products/workfront.html).
