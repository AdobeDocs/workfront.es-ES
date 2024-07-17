---
content-type: release-notes
keywords: notas,trimestral,actualizar
navigation-topic: 2021-4-release-activity
title: 21.4 Información general de la versión
description: Esta página proporciona información acerca de la funcionalidad tanto de Adobe Workfront Classic como de la nueva experiencia de Adobe Workfront que se incluye en la versión 21.4. para ayudarle a desbloquear la productividad y la colaboración.[Marketing de línea única para la versión]
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0897b269-c6f3-4b63-8956-b7f9fbe0a553
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '4717'
ht-degree: 0%

---

# 21.4 Información general de la versión

Esta página proporciona información acerca de la funcionalidad tanto de Adobe Workfront Classic como de la nueva experiencia de Adobe Workfront que se incluye en la versión 21.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 21.4 release nears its planned Production release the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 21.4.</p>
-->

Estas mejoras están disponibles en el entorno de producción desde el 4 de octubre de 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
,
</MadCap:conditionalText>
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
unless otherwise specifiedthe week of May 10, 2021.
</MadCap:conditionalText>


For specific release dates and times for each cluster, see the [Adobe Workfront status page](https://status.adobe.com/en/products/5943) on [status.adobe.com](http://status.adobe.com/). You must log in to see specific release times.

-->

## Mejoras de Adobe Workfront

* [Mejoras del administrador](#administrator-enhancements)
* [Mejoras de Agile](#agile-enhancements)
* [Mejoras en el proyecto](#project-enhancements)
* [Mejoras en la administración de recursos](#resource-management-enhancements)
* [Mejoras en los informes](#reporting-enhancements)
* [Mejoras en las solicitudes](#requests-enhancements)
* [Mejoras de revisión](#proofing-enhancements)
* [Mejoras en la integración](#integration-enhancements)
* [Mejoras de Mobile](#mobile-enhancements)
* [Otras mejoras](#other-enhancements)

### Mejoras del administrador {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">Para administradores: vea qué grupos están asociados con un proceso de aprobación</a> </p> <p>Para ayudarle a averiguar qué grupos están asociados con los procesos de aprobación de su sistema, hemos agregado una columna Nombre de grupo a la vista Estándar en la página Aprobaciones de Configuración. Ahora puede ver esta información sin tener que crear una vista personalizada.</p> </td> 
   <td> <p><b>Disponible en estas fechas:</b> </p> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuevo para administradores: los grupos pueden configurar sus propias preferencias de horas y hojas de horas</a> </p> <p>En una organización grande, es posible que algunos grupos necesiten configurar las preferencias de horas y de plantillas de horas de forma independiente para ajustarse a sus flujos de trabajo únicos, en lugar de heredar las preferencias configuradas por un administrador a nivel de sistema. Ahora los administradores de Workfront pueden desbloquear una plantilla de horas y una preferencia de horas para todos los grupos del sistema y así poder configurarlas ellos mismos.</p> <p>Esta capacidad también se ha agregado recientemente para preferencias de proyecto y para preferencias de tarea y problema.</p> </td> 
   <td> <p><b>Disponible en estas fechas:</b> </p> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión <span style="color: #ff0000;"> de 21.4 (disponible inicialmente en el entorno de producción solamente para los clientes del clúster 4)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuevo para administradores de Workfront: configure plantillas de diseño para usuarios aprovisionados automáticamente en la nueva experiencia de Workfront</a> </p> <p>Ahora puede configurar las plantillas de diseño en la nueva experiencia de Workfront para los usuarios que se aprovisionan automáticamente. En el menú desplegable Atributo de usuario de Workfront, donde se asignan los atributos de usuario (Configuración &gt; Sistema &gt; Inicio de sesión único), ahora hay disponible un nuevo elemento de menú "Nueva plantilla de diseño" para realizar esta configuración. Anteriormente, solo se podían configurar plantillas de diseño para usuarios con aprovisionamiento automático en Workfront Classic.</p> </td> 
   <td> <p><b>Disponible en estas fechas:</b> </p> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">El nuevo campo muestra los grupos a los que pertenecen los usuarios</a> </p> <p>Ahora es fácil averiguar a qué grupos pertenecen sus usuarios. En un informe o vista que enumera usuarios, puede crear una columna con el nuevo campo Otros grupos. Este campo enumera los grupos a los que pertenece cada usuario.</p> </td> 
   <td> <p><b>Disponible en estas fechas:</b> </p> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">La página de detalles de modelos ahora muestra una imagen</a> </p> <p>La página de detalles de cada modelo ahora muestra una imagen de la plantilla de proyecto que se instala con el modelo. La imagen proporciona una vista previa del contenido del modelo para que sepa lo que va a instalar. Si lo desea, puede previsualizar la imagen completa en el explorador o descargar la imagen.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Preferencias de modelos para nuevos problemas</a> </p> <p>Ya están disponibles las nuevas preferencias de problema para algunos modelos. Se instalan de forma predeterminada, pero puede excluirse de la instalación de las preferencias al configurar los detalles de instalación.</p> <p>Las preferencias incluyen grupos de temas de colas, temas de colas y reglas de enrutamiento para recopilar la información correcta cuando se envía un problema o una solicitud, y enviar el problema o la solicitud al rol o equipo correcto. El uso de las preferencias ayuda a crear coherencia en la forma en que se capturan los nuevos problemas o solicitudes en los proyectos.</p> <p>Tenga en cuenta que el uso de estas preferencias no convierte los proyectos creados a partir de la plantilla en colas de solicitudes.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nuevo para administradores de grupos: vea y administre los elementos recientemente eliminados y restaurados de un grupo</a> </p> <p>Seguimos facilitando la administración de sus grupos y sus objetos asociados en un solo lugar. Ahora puede ver y trabajar con los elementos recientemente eliminados y restaurados de un grupo desde el área de Grupos. Esto evita tener que ir al área Eliminados recientemente o Restaurados recientemente en la Configuración para administrar esos elementos. Además, mantiene la lista de los elementos del grupo con los que está trabajando separada de los demás elementos eliminados y restaurados del sistema.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 26 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Nuevo para administradores de grupos: las preferencias de grupo ahora afectan a las plantillas de grupo</a> </p> <p>Ahora es más fácil asegurarse de que las plantillas de proyecto del grupo satisfacen las necesidades del grupo. Cuando asigna una nueva plantilla de proyecto a un grupo en el momento en que lo crea, la plantilla hereda varias configuraciones de las preferencias de proyecto y tarea del grupo.</p> <p>Cuando se crea una nueva tarea de plantilla dentro de una plantilla de proyecto asociada a un grupo, la tarea de plantilla hereda varias configuraciones de las preferencias de tareas del grupo.</p> <p>Anteriormente, las plantillas de proyecto y las tareas de plantilla de proyecto heredaban esta configuración de las preferencias de proyecto y tarea establecidas en el sistema.</p> <p>Si crea una plantilla o tarea de plantilla sin un grupo (por ejemplo, desde la página principal Plantillas), la configuración anterior se hereda de las preferencias de proyecto y tarea de nivel del sistema. Sin embargo, si posteriormente asigna un grupo a la plantilla o tarea de plantilla, las preferencias del grupo no le afectan.</p> </td> 
   <td> <p>Versión de vista previa: 26 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">Nuevo para administradores: descubra qué formularios personalizados están usando un campo personalizado</a> </p> <p>Ahora es más fácil cambiar un campo personalizado en un formulario personalizado. Con un solo clic en el formulario personalizado, puede obtener información sobre cualquier otro formulario personalizado que también utilice el campo. Es importante evaluar si esos formularios necesitarán ajustes para seguir funcionando correctamente después de realizar el cambio.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar: 19 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">Nuevo para administradores de grupos: bloquear y desbloquear las preferencias de proyectos, tareas y problemas de un grupo</a> </p> <p>Ahora puede asegurarse de que todos los miembros de su grupo y sus subgrupos estén utilizando la misma configuración para un proyecto, tarea o preferencia de problema. Una vez que un administrador de Workfront desbloquea una preferencia en el sistema, puede configurarla y después bloquearla para su grupo. Aunque todavía puede volver a configurar una preferencia de grupo bloqueado, los administradores de subgrupos inferiores no pueden hacerlo por separado para sus grupos.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 12 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">Nuevo para administradores de grupos: cree y edite plantillas desde el área de grupos</a> </p> <p>Seguimos facilitando la administración de sus grupos y sus objetos asociados en un solo lugar. Ahora puede ver y trabajar con las plantillas de un grupo desde el área Grupos en Configuración. Esto evita tener que ir al área Plantillas para administrar las plantillas de un grupo. Y mantiene la lista de plantillas de grupo en las que está trabajando separada de las demás en todo el sistema.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 12 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#enter" class="MCXref xref" xrefformat="{para}">Escriba y guarde información en un formulario personalizado adjunto a la vez</a> </p> <p>Ahora es más fácil proporcionar información en la sección Detalles de un objeto: escriba y guarde información en un único campo personalizado o área expansible (como Información general y Finanzas), incluso si los campos obligatorios de otros formularios personalizados del objeto aún no están rellenados.</p> <p>Anteriormente, cuando se especificaba información en un formulario personalizado o área expansible para un objeto, todos los formularios personalizados adjuntos al objeto entraban en modo de edición y todos sus campos obligatorios debían rellenarse antes de poder guardar los cambios. Este problema se producía si no se podía completar un campo obligatorio porque estaba destinado a otro usuario.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 22 de julio de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new9" class="MCXref xref" xrefformat="{para}">Nuevo para administradores de grupos: crea y administra estados para un grupo en cualquier nivel</a> </p> <p>Para facilitar a todos los niveles de una organización la administración y el control de sus flujos de trabajo de forma independiente, hemos introducido la capacidad de crear y administrar estados para subgrupos. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 3 de junio de 2021 (durante el ciclo de versión 21.3)<br></p> <p>Versión de producción: 22 de julio de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new10" class="MCXref xref" xrefformat="{para}">Nuevo para administradores de Workfront: migre las plantillas de diseño de Workfront Classic a la nueva experiencia de Workfront</a> </p> <p>Para ayudarle a administrar las plantillas de diseño mientras sus usuarios cambian a la nueva experiencia de Workfront, hemos creado un botón que puede utilizar para migrar las plantillas de diseño de Workfront Classic a la nueva experiencia sin depender de la asistencia al cliente de Workfront.</p> <p>Anteriormente, solo la Asistencia al cliente de Workfront podía migrar las plantillas de diseño de Workfront Classic a la nueva experiencia de Workfront.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 1 de julio de 2021<br></p> <p>Versión de producción: 15 de julio de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#when" class="MCXref xref" xrefformat="{para}">Al asociar una plantilla con un grupo, seleccione un proceso de aprobación de grupo en Detalles de cola y Temas de cola</a> </p> <p>Se ha añadido una nueva opción al proceso de asociar una plantilla con un grupo. Ahora puede seleccionar procesos de aprobación específicos del grupo para problemas en los Detalles de cola de la plantilla o en uno de sus Temas de cola.</p> <p>En la versión 21.3, cuando añadimos la capacidad de asociar una plantilla de grupo con un grupo, se podía seleccionar un proceso de aprobación específico de grupo en la plantilla, pero no se podía hacer en los Detalles de cola o en los Temas de cola de la plantilla.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 1 de julio de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras del proyecto {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#include" class="MCXref xref" xrefformat="{para}">Incluir imágenes en las actualizaciones</a> </p> <p>En la pestaña Actualizaciones de un objeto, ahora puede añadir imágenes haciendo clic en el icono Imagen de la barra de herramientas. También puede arrastrar y soltar una imagen en el área de actualización. Tenga en cuenta que el administrador de Workfront debe habilitar la adición de imágenes para poder ver el icono Imagen.</p> <p>Puede agregar imágenes tanto en las actualizaciones como en las respuestas. Una miniatura de imagen en la actualización indica que los destinatarios pueden obtener una vista previa de la imagen en el explorador o descargarla, y las notificaciones por correo electrónico y en la aplicación muestran que las imágenes están adjuntas a la actualización.</p> <p>Anteriormente, la única manera de compartir una imagen en Workfront era adjuntarla a un objeto como documento. Las imágenes agregadas en la ficha Actualizaciones sólo están disponibles en esa ficha y no en la ficha Documentos.</p> <p>Para que los usuarios de Workfront puedan incluir imágenes en las actualizaciones, el administrador de Adobe Workfront debe habilitar primero esta función.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Algoritmo actualizado para asignaciones inteligentes</a> </p> <p>Hemos mejorado el algoritmo utilizado al realizar asignaciones inteligentes. Con la nueva mejora, Workfront observa las 30 asignaciones más recientes realizadas por el usuario que ha iniciado sesión para hacer sugerencias al asignar tareas y problemas. La lista de sugerencias puede contener hasta 50 usuarios. </p> <p>Antes de esta mejora, Workfront tenía en cuenta las asignaciones de las tareas principales y otros atributos de usuario relacionados con esas asignaciones al sugerir usuarios.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nueva experiencia al crear un proyecto a partir de una plantilla</a> </p> <p>Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para crear un proyecto a partir de una plantilla. La funcionalidad para crear un proyecto con una plantilla no ha cambiado. Sin embargo, algunas de las mejoras de esta interfaz recién rediseñada incluyen las siguientes:</p> 
    <ul> 
     <li> <p>Vista previa de la información de plantilla antes de adjuntarla</p> </li> 
     <li> <p>Agregar plantillas a una lista de favoritos durante el proceso de creación del proyecto</p> </li> 
    </ul> <p>Hemos actualizado la interfaz para crear el proyecto tanto al crearlo desde el área Proyectos como desde el área Plantillas.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nueva experiencia al adjuntar plantillas a proyectos</a> </p> <p>Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para adjuntar una plantilla a un proyecto. La funcionalidad para adjuntar una plantilla no ha cambiado. Sin embargo, algunas de las mejoras de esta interfaz recién rediseñada incluyen lo siguiente:</p> 
    <ul> 
     <li> <p>Vista previa de la información de plantilla antes de adjuntarla</p> </li> 
     <li> <p>Agregar plantillas a una lista de favoritos durante el proceso de datos adjuntos</p> </li> 
     <li> <p>Ver todas las opciones para administrar la configuración de plantillas y proyectos en una página continua</p> </li> 
    </ul> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 26 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#unified" class="MCXref xref" xrefformat="{para}">Valores unificados de duración y unidad de duración para tareas</a> </p> <p>Para una experiencia de usuario más limpia y optimizada, hemos combinado el valor del campo Duración con la unidad de tiempo de la duración. Antes de esta mejora, la unidad de tiempo se mostraba en un campo desplegable independiente después del campo Duración.</p> <p>Además de los campos Duración en los cuadros Detalles de la tarea, Editar tareas y Nueva tarea, también vamos a actualizar los campos siguientes para que coincidan con esta experiencia:</p> 
    <ul> 
     <li> <p>Campo de duración al realizar asignaciones avanzadas</p> </li> 
     <li> <p>Retraso por nivelación del campo al crear o editar una tarea</p> </li> 
     <li> <p>Campo Frecuencia al crear una tarea recurrente (disponible próximamente)</p> </li> 
     <li> <p>Campo de retardo al añadir un predecesor (disponible próximamente)</p> </li> 
    </ul> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar: 19 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#disable" class="MCXref xref" xrefformat="{para}">Deshabilitar la adición de problemas en línea en proyectos</a> </p> <p>Para garantizar que los usuarios proporcionen información precisa al agregar problemas a los proyectos completando un formulario de problemas, hemos introducido una nueva configuración que le permite administrar si pueden agregar problemas a un proyecto o sus tareas en línea. Esta opción está habilitada de manera predeterminada en el área Nueva configuración de problema del cuadro Editar proyecto. Si se deshabilita, se atenúa la opción Agregar más problemas en la sección Problemas de un proyecto, de modo que los usuarios no puedan agregar más problemas en la lista. Los usuarios aún pueden agregar problemas a los proyectos mediante la opción Nuevo problema de la sección Problemas o mediante una cola de solicitudes, si hay alguna configurada para el proyecto.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar: 5 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#custom" class="MCXref xref" xrefformat="{para}">Mejora en la visualización de campos personalizados para casillas de verificación y botones de opción</a> </p> <p>Ver y seleccionar las opciones de casilla de verificación y botón de radio en los formularios personalizados se ha vuelto más fácil: ahora se muestra un campo personalizado con muchas opciones de casilla de verificación o botón de radio en varias columnas de la página. Anteriormente, se mostraban en una sola columna, lo que requería un desplazamiento adicional para los usuarios que rellenaban el formulario.</p> <p>Esto depende de cómo coloque los campos en el formulario personalizado: si coloca otro campo en la misma fila con el campo de casilla de verificación o del botón de radio, es posible que las opciones solo tengan espacio horizontal suficiente para mostrar en una sola columna.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 29 de julio de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras en Administración de recursos {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#make" class="MCXref xref" xrefformat="{para}">Realice asignaciones rápidas en el Distribuidor de cargas de trabajo</a> </p> <p>Ahora puede equilibrar eficazmente los recursos en el Distribuidor de cargas de trabajo con unos clics mínimos arrastrando un elemento del área No asignada y soltándolo en la línea de un usuario en el área Asignada. Con la función de arrastrar y soltar, también puede anular la asignación de elementos de los usuarios y moverlos de nuevo al área No asignada, así como moverlos a otros usuarios. </p> <p>Antes de esta mejora, solo podía asignar elementos haciendo clic en el menú Más de una tarea o un problema y, a continuación, utilizando la opción Asignar. Ahora, las horas planificadas asignadas al usuario se actualizan en tiempo real mientras arrastra las tareas.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nueva opción predeterminada para el Distribuidor de cargas de trabajo</a> </p> <p>Como parte de nuestro esfuerzo por descontinuar la programación y hacer que la herramienta de asignación de recursos principal de la Distribuidor de cargas de trabajo de Workfront, hemos hecho que la herramienta de asignación de recursos predeterminada sea la Workfront Balancer para todos los usuarios nuevos. En este momento, Programación es la opción predeterminada. Este cambio se aplica a todas las áreas en las que puede acceder a Programación desde, que incluyen el área de Recursos (en la nueva experiencia de Adobe Workfront) o el área de Personas (en Adobe Workfront Classic), así como a nivel de proyecto y de equipo.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nueva experiencia de filtro en el Distribuidor de cargas de trabajo</a> </p> <p>Hemos rediseñado la experiencia de filtrado en el Distribuidor de cargas de trabajo para incluir las siguientes funcionalidades adicionales:</p> 
    <ul> 
     <li> <p>Interfaz de usuario más sencilla y optimizada que coincide con la nueva experiencia de Workfront</p> </li> 
     <li> <p>Campos adicionales por los que puede filtrar</p> </li> 
     <li> <p>Capacidad para duplicar un filtro</p> </li> 
     <li> <p>Uso compartido de filtros con otros usuarios</p> </li> 
    </ul> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar: 16 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras de Agile {#agile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#user" class="MCXref xref" xrefformat="{para}">Asignaciones de usuarios en paneles Kanban y Scrum</a> </p> <p>Hemos actualizado las tarjetas de historia en los paneles de Kanban y Scrum para facilitar la asignación de un usuario a la historia. Ahora puede hacer clic en un avatar de equipo o usuario para agregar una asignación cuando se expanda la tarjeta de historia. Anteriormente, tenía que localizar y hacer clic en un icono de signo más independiente.</p> </td> 
   <td> <p>Versión de vista previa: 9 de septiembre de 2021 <br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurar cómo se aplican las fechas al agregar elementos de trabajo a una iteración de Scrum</a> </p> <p>De forma predeterminada, cuando se agrega un elemento de trabajo a una iteración, la Fecha planificada de inicio y la Fecha planificada de finalización del elemento de trabajo se modifican para que coincidan con las fechas de inicio y finalización de la iteración. Ahora puede elegir mantener la fecha planificada de inicio y la fecha planificada de finalización originales en todos los elementos de trabajo de un equipo.</p> <p>Esta opción solo se aplica a los equipos de Scrum y no a los equipos de Kanban.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#changes" class="MCXref xref" xrefformat="{para}">Cambios en la vista Agile en los proyectos</a> </p> <p>Como parte de la versión 21.3, hemos realizado mejoras en el encabezado de la tarjeta Agile y en los paneles de artículos (consulte <a href="../../../product-announcements/product-releases/21.3-release-activity/21-3-project-enhancements.md#agile" class="MCXref xref" xrefformat="{para}">Actualizaciones del encabezado y del panel de artículos de la tarjeta Agile</a>). Estas actualizaciones se aplicaron a iteraciones, así como a la vista Agile en proyectos.</p> <p>Con la versión 21.4, revertimos estas mejoras para la vista Agile en proyectos. No se están realizando cambios en las iteraciones Agile.</p> <p>A continuación se indican los cambios que se están revirtiendo con respecto a la vista Agile en los proyectos:</p> 
    <ul> 
     <li> <p>Las tarjetas de historia y las columnas del tablero tienen anchuras ajustables.</p> </li> 
     <li> <p>Las columnas no tienen sombreado de fondo.</p> </li> 
     <li> <p>Las tarjetas no tienen etiquetas de identificador (artículo principal, subtarea, artículo, tarea o problema).</p> </li> 
     <li> <p>Se ha cambiado el nombre de la columna Historia principal a Historias.</p> </li> 
    </ul> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar: 16 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Agregar nuevas historias y problemas del Panel Kanban</a> </p> <p>Ahora puede crear una nueva historia o problema directamente desde el Panel Kanban. Esto facilita la adición rápida de una nueva historia sin tener que ir a un proyecto, informe o panel para crear una tarea.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 22 de julio de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras de informes {#reporting-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nueva apariencia para el campo Asignaciones en listas e informes actualizados</a> </p> <p>Para que coincida con el aspecto moderno de otras áreas en la nueva experiencia de Workfront, el estilo ha cambiado para el campo Asignaciones en listas e informes actualizados. El rediseño incluye un nuevo icono de rol, un nuevo icono de Personas para asignaciones avanzadas, un nuevo icono de Acceso restringido y más.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 8 de abril de 2021 (con la versión 21.2)<br></p> <p>Versión de producción: 15 de julio de 2021<span class="uitext" style="color: #dc143c;">(Originalmente lanzada en Production el con la versión 21.2)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nueva apariencia para los campos de escritura anticipada en listas e informes actualizados</a> </p> <p>Para adaptarse al aspecto moderno de otras áreas en la nueva experiencia de Workfront, el estilo ha cambiado para los campos de escritura anticipada en las listas e informes actualizados. Estos cambios incluyen varias mejoras.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 8 de abril de 2021 (con la versión 21.2)<br></p> <p>Versión de producción: 15 de julio de 2021 <span class="uitext" style="color: #dc143c;">(Originalmente lanzada en Production el con la versión 21.2)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Solicitudes de mejoras {#requests-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">La búsqueda mejorada para solicitudes ahora incluye caracteres especiales</a> </p> <p>Para que la búsqueda de colas de solicitudes sea más rápida y sencilla al enviar solicitudes, hemos mejorado el algoritmo de búsqueda para encontrar ahora colas que puedan contener caracteres especiales.</p> <p>Por ejemplo, puede encontrar una cola de solicitudes llamada "*Workfront" escribiendo "*Workfront" o "Workfront" en el campo Tipo de Solicitud.</p> <p>Se admiten todos los caracteres especiales.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 9 de septiembre de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nueva apariencia para colas de solicitudes incrustadas en la nueva experiencia de Workfront</a> </p> <p>Para mantener la misma apariencia a la hora de enviar solicitudes en todas partes en la nueva experiencia de Workfront, hemos rediseñado la interfaz para agregar solicitudes a una cola de solicitudes incrustada. Antes de esta mejora, la interfaz para agregar solicitudes desde un panel coincidía con el entorno de Workfront Classic.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 26 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras de corrección {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Funciones de revisión mejoradas para revisores y solicitantes</a> </p> <p>Para proporcionar una experiencia más integrada entre Workfront y Proof, hemos realizado varias mejoras con respecto a las capacidades de prueba para revisores y solicitantes:</p> 
    <ul> 
     <li> <p>Puede otorgar funciones de Moderador o Autor a cualquier usuario de Workfront, independientemente de si tiene una licencia de Revisión, lo que le otorga derechos adicionales, como aplicar acciones o resolver comentarios.</p> </li> 
     <li> <p>Puede añadir revisores y solicitantes a las pruebas que requieran un inicio de sesión o que deban firmarse electrónicamente.</p> </li> 
     <li> <p>Todos los usuarios también se benefician de la conectividad mejorada entre Workfront y Proof. Ahora, al desactivar un usuario o actualizar la dirección de correo electrónico de un usuario, las actualizaciones se reflejan correctamente en la revisión cuando se cambian en Workfront.</p> </li> 
    </ul> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar: 5 de agosto de 2021 <br></p> <p>Versión de producción: con la versión de 21.4 <span class="uitext" style="color: #dc143c;"> (se eliminó de la vista previa y la producción el 20 de octubre de 2021). Lanzamiento original únicamente para clientes de EMEA totalmente integrados. Esta funcionalidad se volverá a presentar a todos los clientes más adelante.)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras de integración {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#link" class="MCXref xref" xrefformat="{para}">Enlazar documentos de la empresa del Dropbox</a> </p> <p>Se ha agregado Dropbox empresarial como una integración de documentos disponible. Ahora, puede acceder a los documentos que ha almacenado en Dropbox Business directamente desde Workfront.</p> <p>Dropbox Business le permite vincular documentos compartidos y cargar documentos en carpetas compartidas. Dropbox (no Dropbox Empresa) permite que solo el propietario de los documentos vea el documento en Workfront.</p> <p>El administrador de Workfront puede habilitar esta integración para su organización.</p> </td> 
   <td> <p><b>Disponible en estas fechas:</b> </p> <p>Versión de vista previa: N/D<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Actualizaciones en Workfront para Slack</a> </p> <p>Las siguientes actualizaciones ahora están visibles en la integración de Workfront para Slack:</p> <p>La integración de Workfront para Slack ahora tiene una nueva apariencia. Además, ahora recibe las notificaciones de Workfront para Slack en tiempo real. </p> <p>Por ejemplo, si se le asigna una tarea, recibirá esa notificación en cuanto se le asigne. </p> <p>Anteriormente, podía haber un retraso antes de que la notificación apareciera en Slack.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 29 de julio de 2021<br></p> <p>Versión de producción: 29 de julio de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#more" class="MCXref xref" xrefformat="{para}">Vea con mayor claridad los detalles de acceso a la cuenta al dar su consentimiento para las integraciones de Adobe Workfront</a> </p> <p>Ahora se actualizan las pantallas de consentimiento para integraciones de Adobe Workfront. Ahora puede ver las acciones y áreas específicas a las que tienen acceso las integraciones, para que pueda comprender mejor a qué está permitiendo el acceso a la integración o aplicación.</p> <p>Esta nueva pantalla de consentimiento se aplica a cualquier integración de Adobe Workfront que utilice OAuth 2.0. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 29 de julio de 2021<br></p> <p>Versión de producción: 29 de julio de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#api" class="MCXref xref" xrefformat="{para}">Ya no es necesaria la autenticación de claves API para las integraciones</a> </p> <p>Las integraciones de Workfront han comenzado recientemente a utilizar OAuth2 para una mayor seguridad y facilidad de uso. Como parte de este movimiento, Workfront ya no requiere claves API para la autenticación de integraciones.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar: 5 de agosto de 2021<br></p> <p>Versión de producción: 5 de agosto de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras de Mobile {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#review" class="MCXref xref" xrefformat="{para}">Revisar y aprobar pruebas en la aplicación móvil</a> </p> <p>La aplicación móvil de Adobe Workfront ahora muestra todas las aprobaciones de prueba que tiene asignadas en su lista de aprobaciones en Mi trabajo. Puede revisar un documento de prueba directamente en la aplicación y tomar una decisión al respecto.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: N/D<br></p> <p>Versión de producción: semana del 11 de octubre de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> 
    <ul> 
     <li> <p>tienda de aplicaciones de iOS</p> </li> 
     <li> <p>tienda de aplicaciones de Android</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}">Crear una solicitud nueva desde el área de inicio de la aplicación móvil</a> </p> <p>Ahora puede crear una nueva solicitud desde el área de inicio en la aplicación móvil de Adobe Workfront. Al pulsar el botón "añadir" en la barra de navegación flotante, se muestra una opción para Solicitud además de Tarea. Anteriormente, había que ir a la página de solicitudes para crear una solicitud.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: N/D<br></p> <p>Versión de producción: 4 de agosto de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> 
    <ul> 
     <li> <p>tienda de aplicaciones de iOS</p> </li> 
     <li> <p>tienda de aplicaciones de Android</p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuevos métodos abreviados de teclado para aplicar sangría y anular la sangría en listas</a> </p> <p>Para proporcionar una experiencia accesible para todos los usuarios del sistema y cumplir con los principios estándar de navegación mediante el teclado, los comandos de teclado para aplicar o anular sangría han cambiado. </p> <p>En Mac, pulse Opción + &gt; para aplicar sangría a un elemento de lista y Opción + &lt; para anular la sangría. </p> <p>En Windows, presione Alt + &gt; para aplicar sangría a un elemento de lista y Alt + &lt; para anular la sangría.</p> <p>Anteriormente, el método abreviado de teclado para aplicar sangría en una lista era Tab y la anulación de sangría era Mayús + Tab. Sin embargo, el uso del tabulador para sangrar y anular la sangría impedía desplazarse por todos los campos activos de la interfaz.</p> <p>Este cambio solo se aplica a las listas actualizadas y no a las listas heredadas. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa: 12 de agosto de 2021<br></p> <p>Versión de producción: con la versión 21.4</p> <p><strong>Disponible en estos entornos:</strong> </p> 
    <ul> 
     <li> <p>La nueva experiencia de Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Mejoras de Workfront Fusion

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción en una cadencia distinta a la de la versión 21.4. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Mejoras de Workfront Scenario Planner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.</p>
-->

Las nuevas funciones están llegando a la versión Workfront Scenario Planner con la versión 21.4. Para obtener información sobre estas nuevas características que ya están disponibles en Vista previa, consulte [Actividad de la versión de Adobe Workfront Scenario Planner](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof enhancements</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-may-17.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of May 17, 2021</a>.</p>
-->

## Mejoras en Workfront Goals

No hay actualizaciones de Workfront Goals en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## Versión de API 14

Para la versión 14 de la API, hemos modificado algunos recursos y extremos. Algunos de los cambios admiten nuevas funciones y otros facilitan el uso de la información disponible a través de la API.

Para obtener información sobre novedades y actualizaciones, consulte [Novedades de la versión 14](../../../wf-api/api/new-api-version-14.md) de la API.

Para obtener información sobre las versiones de API, consulte [Versiones de API y programación de soporte](../../../wf-api/api/api-version-support-schedule.md).

## Seminario web sobre la versión 21.4

El seminario web sobre la versión 21.4 de Workfront se presentó el 23 de septiembre de 2021. Puedes ver la grabación del seminario web desde la página [Eventos en Workfront One](https://one.workfront.com/s/event).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## Actualizaciones de formación

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, rutas de aprendizaje, vídeos y guías de cada versión del producto de Adobe Workfront. Para obtener más información, consulte la [página Actualizaciones de la versión de formación](https://one.workfront.com/s/training-release-updates).

## Funcionalidad ya no admitida

### Internet Explorer 11

Con la eliminación de la compatibilidad con Internet Explorer, Workfront ahora es compatible oficialmente con Microsoft Edge.

Para obtener más información sobre los exploradores admitidos, consulte [Requisitos para exploradores Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).
