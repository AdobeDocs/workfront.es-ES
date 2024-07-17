---
content-type: release-notes
keywords: notas,trimestral,actualizar
navigation-topic: product-releases
title: Información general de la versión 21.1
description: La versión 21.1 se publicó en el entorno de producción la semana del .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3658'
ht-degree: 0%

---

# Información general de la versión 21.1

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

Esta página proporciona información acerca de la funcionalidad tanto de Adobe Workfront Classic como de la nueva experiencia de Adobe Workfront que se incluye en la versión 21.1.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

Con esta versión, lanzamos nuevas funciones y mejoras para ayudarle a liderar el regreso en 2021 con estrategias adaptables, procesos de trabajo automatizados y una infraestructura digital conectada para permitir el éxito en toda la empresa.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

Estas mejoras ya están disponibles

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the Preview environment and will be made available
</MadCap:conditionalText>
-->

en el entorno Producción.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the first quarter of 2021
</MadCap:conditionalText>
-->

Fueron puestos en libertad la semana del 15 de febrero de 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Mejoras de Adobe Workfront

* [Mejoras del administrador](#administrator-enhancements)
* [Mejoras en la administración de recursos](#resource-management-enhancements)
* [Mejoras en la administración de proyectos](#project-management-enhancements)
* [Mejoras mejoradas de análisis](#enhanced-analytics-improvements)
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Introducir nueva configuración de nivel de acceso para copiar proyectos</a> </p> <p>Para darle más control, como administrador del sistema, sobre lo que los planificadores pueden hacer con un proyecto, hemos hecho que el acceso de edición a proyectos en el nivel de acceso sea más granular, al introducir una nueva configuración que le permite habilitar o deshabilitar su capacidad para copiar proyectos. Antes de este cambio, cuando habilitaba el acceso de los usuarios a Editar proyectos, automáticamente tenían acceso para copiarlos. Con la nueva función, puede otorgar acceso a alguien para editar proyectos sin tener necesariamente acceso para copiarlos deshabilitando la nueva configuración Copiar.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 13 de enero de 2021</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">En un formulario personalizado de un objeto, seleccione todos los elementos de un campo desplegable de selección múltiple</a> </p> <p>En la página Detalles de un objeto, cuando rellene un campo desplegable de selección múltiple en un formulario personalizado, puede hacer clic en Seleccionar todo si necesita seleccionar todas las opciones disponibles.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 13 de enero de 2021</p> <p>Versión de producción: con la versión de 21.1 <span style="color: #dc143c; font-weight: bold;">(actualmente no disponible cuando envía una nueva solicitud)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">Volver a calcular todos los campos de formulario personalizados de un objeto</a> </p> <p>Ahora es más fácil asegurarse de que todos los datos de los campos personalizados calculados estén actualizados para un objeto. La nueva opción de menú Recalcular expresiones permite volver a calcular rápidamente todos los datos de estos campos.</p> <p>Esto resulta especialmente útil después de que alguien edite datos en otro objeto al que se hace referencia mediante un campo personalizado calculado en el objeto.</p> <p>Anteriormente, los usuarios tenían que usar soluciones alternativas para asegurarse de que todos los datos de los campos personalizados calculados estuvieran actualizados. Por ejemplo, editaron el objeto junto con otros objetos para utilizar la opción de recálculo que está disponible para la edición masiva.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 10 de diciembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">Desbloquear tareas y preferencias de problemas para administradores de grupos</a> </p> <p>Los administradores de Workfront ahora pueden dar más autonomía a los administradores de grupos desbloqueando las preferencias de tareas y problemas individuales. Cuando una preferencia está desbloqueada, los administradores de grupos pueden configurarla para que sus grupos sirvan a las necesidades únicas y a los procesos internos de cada grupo.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 2 de diciembre de 2020</p> <p>Versión de producción: con la versión de 21.1 <span style="color: #dc143c; font-weight: bold;"> (antes del 24 de junio de 2021), esto estaba disponible como parte de un despliegue gradual solo para clientes de los clústeres 4 y 6 y algunos otros clientes. Ahora está disponible en producción para todos los clientes)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurar por separado el nivel de acceso para portafolios y programas</a> </p> <p>Ahora es más fácil administrar el acceso de los usuarios a portafolios y programas porque puede establecer la configuración de su nivel de acceso por separado.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 2 de diciembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">Seleccionar todas las casillas de verificación de una serie al editar información en un formulario personalizado</a> </p> <p>En la página Detalles de un objeto, cuando rellene un campo Formulario personalizado que contenga casillas de verificación, puede hacer clic en Seleccionar todo si necesita seleccionar todas las casillas de verificación disponibles.</p> <p>Esta opción solo se muestra si el campo contiene más de dos casillas de verificación.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 2 de diciembre de 2020</p> <p>Versión de producción: con la versión de 21.1 <span style="color: #dc143c; font-weight: bold;">(actualmente no disponible al enviar una solicitud)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">Configuración de la lista de permitidos de correo electrónico de Workfront</a> </p> <p>Para proteger mejor sus datos, ahora puede utilizar una lista de permitidos de dominio de correo electrónico para lo siguiente:</p> 
    <ul> 
     <li> <p>Controlar adónde pueden ir los correos electrónicos de Workfront si contienen informes o documentos almacenados en Workfront</p> </li> 
     <li> <p>Los dominios de control de correo electrónico pueden estar en la dirección de correo electrónico que los usuarios pueden especificar en su perfil de usuario</p> </li> 
    </ul> <p>Por ejemplo, si desea proteger datos confidenciales, como un informe que enumere los clientes en riesgo, puede incluir solo el dominio o los dominios de correo electrónico internos en la lista de permitidos de correo electrónico. De este modo, los usuarios no podrán enviar dicho informe (ni ningún otro informe de Workfront) a una dirección de correo electrónico externa.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 20 de noviembre de 2020</p> <p>Versión de producción: con la versión 21.1 </p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Asignar un administrador de grupo para un subgrupo</a> </p> <p>Para facilitar el funcionamiento independiente de los niveles de su organización, se ha añadido la capacidad de asignar un administrador de grupo a un subgrupo. Ahora puede asegurarse de delegar la administración de subgrupos a las personas adecuadas.</p> <p>Anteriormente, solo un grupo de nivel superior podía tener Administradores de grupo y estos administradores administraban todos los subgrupos debajo del grupo de nivel superior.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 20 de noviembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">Trabaje con proyectos de grupo y procesos de aprobación en el área de Grupos</a> </p> <p>Si es administrador de grupos, es fácil ver y trabajar con los proyectos y procesos de aprobación de su grupo ahora que están enumerados en el área de Grupos. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 20 de noviembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">Configurar notificaciones de eventos para grupos</a> <span style="color: #dc143c; font-weight: bold;">Novedades en vista previa!</span></p> <p>Los administradores de Workfront ahora pueden dar más autonomía a los administradores de grupos, ya que les permite configurar notificaciones de eventos para sus grupos de nivel superior. Los subgrupos heredan las configuraciones de notificación de eventos de su grupo principal superior.</p> <p>Anteriormente, solo un administrador de Workfront podía configurar las notificaciones de eventos en el sistema, lo que significa que todos los grupos tenían que utilizar el mismo conjunto de notificaciones de eventos.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 22 de enero de 2021</p> <p>Versión de producción: con la versión <span style="color: #dc143c; font-weight: bold;"> de 21.1 (disponible inicialmente en el modo de producción solo para los clientes del clúster 4 como parte de un despliegue gradual; disponible para otros clústeres poco después)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">Ver el número de licencias utilizadas y asignadas en un grupo</a> </p> <p>Para determinar cómo se distribuyen las licencias, ahora puede ver el número de licencias que se usan en un grupo y en los subgrupos que haya debajo de él.</p> <p>Si administra un grupo de nivel superior, puede ver tanto el número de licencias que se usan en un grupo (y sus subgrupos) como el número máximo de licencias asignadas para el grupo.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 20 de noviembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">Distribuidor de cargas de trabajo para proyectos</a> </p> <p>El Distribuidor de cargas de trabajo ya está disponible dentro de un proyecto. Ahora tiene la opción de seleccionar entre utilizar el Distribuidor de cargas de trabajo o la herramienta Programación para administrar los recursos del proyecto.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 17 de diciembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront Balancer disponible para un equipo</a> </p> <p>El Distribuidor de cargas de trabajo ya está disponible en un equipo. Ahora tiene la opción de seleccionar entre utilizar el Distribuidor de cargas de trabajo o la herramienta de programación para administrar los recursos del equipo. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 20 de noviembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras en Administración de proyectos {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">La exportación ya está disponible en la sección Métricas de un proyecto</a> </p> <p>Para compartir más fácilmente el estado y el progreso de un proyecto, ahora puede exportar todo el tablero de la sección Métricas de un proyecto a un archivo .png.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 15 de enero de 2021</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">Actualizar el porcentaje completado del problema cuando el proyecto o la tarea se convirtieron a partir de la actualización del problema</a> </p> <p>Hemos actualizado el modo en que funciona el porcentaje completado de problemas para problemas que se han convertido en proyectos o tareas. Con la nueva funcionalidad, cuando un problema se convierte en una tarea o un proyecto, el porcentaje completado del problema se actualiza de forma sincronizada con el porcentaje completado de la tarea o el proyecto de resolución cuando la configuración "Actualizar automáticamente el estado del problema solucionable cuando cambia el estado del objeto de resolución" está habilitada desde la configuración.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 13 de enero de 2021</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">Campos eliminados de la página Nueva solicitud</a> </p> <p>Como parte del rediseño de la página Nueva solicitud, se han actualizado los campos Nuevo problema que se configuran en la sección Configuración de cola de un proyecto.</p> <p>Varios campos de nuevos problemas solo se muestran al crear un problema desde la sección Problemas del proyecto. No se muestran al enviar un problema mediante una cola de solicitudes en el área de Solicitudes.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 13 de enero de 2021</p> <p>Versión de producción: con la versión de 21.1 <span style="color: #dc143c; font-weight: bold;">(se eliminó de la versión)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nueva experiencia al enviar solicitudes en el área de solicitudes</a> </p> <p>Para mantener la coherencia con la nueva experiencia de Workfront y aumentar la eficacia al enviar solicitudes, hemos rediseñado el cuadro Nueva solicitud en el área Solicitudes.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 13 de enero de 2021</p> <p>Versión de producción: con la versión de 21.1 <span style="color: #dc143c; font-weight: bold;">(se eliminó de la versión; permanecerá en la vista previa y se lanzará a producción con 21.2)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Compartir un vínculo a una cola de solicitudes al enviar una solicitud</a> </p> <p>Ahora, es posible compartir un vínculo a una cola de solicitudes, a un grupo de temas o a un tema de la cola cuando se crea una solicitud.</p> <p>Antes de enviar una nueva solicitud, puede copiar un vínculo a la cola de solicitudes, al grupo de temas o al tema de la cola de la solicitud y compartirlo con otros usuarios, o incrustarlo en un panel.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 13 de enero de 2021</p> <p>Versión de producción: con la versión de 21.1 <span style="color: #dc143c; font-weight: bold;">(se eliminó de la versión; permanecerá en la vista previa y se lanzará a producción con 21.2)</span></p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nueva lista de solicitudes enviadas</a> </p> <p>Para permitirle administrar sus Solicitudes enviadas de una manera más fácil y coherente, hemos eliminado las secciones Solicitudes que he enviado y Todas las solicitudes en el área Solicitudes y las hemos sustituido por una nueva lista de enviadas. La lista tiene un aspecto familiar que coincide con todas las demás listas del sistema, lo que le permite filtrar por diferentes categorías de solicitudes enviadas y buscar rápidamente una solicitud que pueda ser difícil de encontrar.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 2 de diciembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">Busque un grupo que desee asignar a un proyecto y vea sus detalles</a> </p> <p>Ahora es más fácil asegurarse de identificar el grupo correcto al asignar un grupo a un proyecto. Pase el ratón sobre el nombre de un grupo que encuentre en el cuadro Grupo y luego haga clic en el icono de información que aparece junto al nombre para ver la información sobre el grupo.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 17 de diciembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nuevo informe de delegación de usuario</a> </p> <p>Anteriormente, la información de las delegaciones de tareas, problemas y aprobaciones de proyectos solo la podía ver el delegado en el área de Inicio. Para permitir que otros usuarios vean esta información, los usuarios de Plan ahora pueden crear el informe de delegación de usuarios, que le informa:</p> 
    <ul> 
     <li> <p>Quién ha delegado estas aprobaciones a otro usuario</p> </li> 
     <li> <p>Qué usuario ha delegado estas aprobaciones</p> </li> 
     <li> <p>La fecha de inicio y finalización de estas delegaciones</p> </li> 
    </ul> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 17 de diciembre de 2020</p> <p>Versión de producción: 21 de enero de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mejoras de análisis mejoradas {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Característica</strong> </p> </td> 
   <td> <p><strong>Entornos y fechas de lanzamiento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>La página <a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">Personas ya está disponible para todos los clústeres</a> </p> <p>La página Personas ya está disponible en Workfront Classic para el clúster 4. Esta página incluye los gráficos de Actividad por equipo, Capacidad de los recursos y Capacidad del equipo.</p> <p>Esta página estaba disponible anteriormente con la versión 20.3 tanto en Workfront Classic como en la nueva experiencia de Workfront para todos los demás clústeres.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 28 de enero de 2021</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront (disponible anteriormente)</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">Ahora se muestra el análisis mejorado de forma predeterminada</a> </p> <p>Nota: Este cambio solo se aplica a los usuarios que se han añadido recientemente a las plantillas de diseño. Los usuarios asignados a una plantilla de diseño personalizada tampoco se ven afectados por este cambio.</p> <p>En la plantilla de diseño predeterminada, el área de Analytics está ahora habilitada de forma predeterminada, lo que significa que los usuarios asignados a esta plantilla de diseño ahora ven el área de Analytics en la barra de navegación global de Workfront Classic y el menú principal en la nueva experiencia de Workfront.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 6 de noviembre de 2020</p> <p>Versión de producción: 3 de diciembre de 2020</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">Análisis mejorado disponible para todos los clústeres</a> </p> <p>El análisis mejorado está disponible para todos los clústeres de Workfront, incluidos los clientes del clúster 6.</p> <p>Anteriormente, el análisis mejorado no estaba disponible con Google Cloud Platform, lo que impedía a los clientes del clúster 6 acceder al área de Analytics. Ahora, los clientes empresariales y empresariales del clúster 6 pueden acceder al área de Analytics.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 20 de noviembre de 2020</p> <p>Versión de producción: 3 de diciembre de 2020</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Mejoras en las notificaciones de Adobe Workfront en Microsoft Teams</a> </p> <p>Para facilitar el uso de Workfront a través de Microsoft Teams, hemos añadido varias mejoras a las notificaciones de Microsoft Teams enviadas desde Workfront.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: N/D</p> <p>Versión de producción: 12 de enero de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuevas rutas de navegación en la aplicación Adobe Workfront</a> </p> <p>Se ha agregado la navegación por ruta de exploración a la aplicación móvil de Workfront. Ahora puede utilizar esta función para desplazarse a los elementos de trabajo principales de un proyecto.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: N/D</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Se admite texto enriquecido en formularios personalizados en la aplicación de Workfront</a> </p> <p>Ahora puede utilizar el formato de texto enriquecido en campos de texto de formulario personalizados en la aplicación móvil de Workfront.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: N/D</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">Los usuarios de SSO ahora pueden volver a iniciar sesión en la aplicación de Workfront con Face ID o tecnología de huella digital</a> </p> <p>Si su organización utiliza SSO, ahora puede utilizar su Face ID o huella digital para iniciar sesión en la aplicación móvil de Workfront después de que su sesión haya superado el tiempo de espera. Sin embargo, debe iniciar sesión con sus credenciales de SSO inicialmente.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: N/D</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
--&gt;

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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Actualizaciones de los requisitos para errores de suscripción a eventos</a> </p> <p>Estamos actualizando los requisitos de deshabilitación de software de los errores de suscripción de evento. Además de los requisitos existentes, las suscripciones a eventos ahora estarán desactivadas si no se consigue un envío correcto en un plazo de 2000 intentos. Esto sirve para reforzar la regla de fallo del 70 % existente, que puede llevar a cantidades excesivas de fallos, en algunas condiciones.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: N/D</p> <p>Versión de producción: 11 de enero de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nuevos campos de equipo disponibles para el resumen diario</a> </p> <p>Hemos agregado los campos de Aprobación del equipo y Asignaciones al correo electrónico de resumen diario de la acción necesaria.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 17 de diciembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">Reemplazando opción de correo electrónico POP en las colas de solicitudes</a> </p> <p>Estamos reemplazando la opción de correo electrónico POP para las colas de solicitud con un nuevo sistema administrado por Workfront. Todavía podrá enviar solicitudes por correo electrónico, pero en su lugar deberá configurar una nueva dirección de correo electrónico administrada por Workfront en el área de Cola de solicitudes. </p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 17 de diciembre de 2020</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">Restringir la edición de horas en hojas de horas</a> </p> <p>Para proporcionar más control sobre las plantillas de horas y la edición de horas, hemos agregado una configuración que le permite restringir la edición de horas a los propietarios de plantillas de horas y a los administradores del sistema.</p> <p>Anteriormente, los usuarios con la opción Plantillas de horas y Horas habilitada en su nivel de acceso podían editar las horas en cualquier plantilla de horas.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 21 de enero de 2021</p> <p>Versión de producción: con la versión 21.1</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Filtros y vistas mejorados en el área de Plantillas de horas</a> </p> <p>Hemos agregado filtros para proyectos y problemas, así como opciones de Ver y Agrupar a la página Buscar.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 2 de diciembre de 2020</p> <p>Versión de producción: 21 de enero de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">Ocultar la casilla de horas extra en Plantillas de horas</a> </p> <p>Ahora puede ocultar el cuadro de horas extra para facilitar la confusión del usuario si no rastrea las horas extra en Workfront. Puede ocultar el cuadro de horas extra de una plantilla de horas de un solo uso o en el Perfil de plantilla de horas.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 2 de diciembre de 2020</p> <p>Versión de producción: 16 de diciembre de 2020</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">Expandir o contraer elementos en la navegación de la ruta de exploración</a> </p> <p>Para facilitar la visualización de la ruta de exploración completa, se ha agregado la funcionalidad de expandir y contraer.</p> <p>Ahora, todos los elementos truncados se agrupan antes del proyecto con el texto "más". Por ejemplo, "3 más" indica que hay 3 objetos que no se muestran.</p> <p>Anteriormente, se tenía que hacer clic en los puntos suspensivos para mostrar los objetos truncados en un menú desplegable.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión preliminar de Beta: 7 de enero de 2020</p> <p>Versión de producción: 21 de enero de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nueva apariencia para la navegación por rutas de exploración</a> </p> <p>Para ayudar a los usuarios a identificar mejor dónde se encuentran en Workfront y navegar más fácilmente entre objetos, hemos mejorado varias veces la navegación por la ruta de exploración.</p> </td> 
   <td><strong>Disponible en estas fechas:</strong> <p>Versión de vista previa de Beta: 10 de diciembre de 2020</p> <p>Versión de producción: 21 de enero de 2021</p> <p><strong>Disponible en estos entornos:</strong> </p> <p>La nueva experiencia de Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

## Mejoras en Workfront Goals

La mayoría de las nuevas funciones que se incluyen en la versión Workfront Goals son la versión 21.1. Para obtener más información sobre estas nuevas características que ya están disponibles en Vista previa, consulte [Objetivos de Adobe Workfront con la versión 21.1](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Mejoras de Workfront Scenario Planner

Nuevas funciones incluidas en la versión 21.1 de Workfront Scenario Planner. Para obtener información sobre estas nuevas características que ya están disponibles en la vista previa, consulte [Adobe Workfront Scenario Planner con la versión 21.1](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Mejoras de Workfront Fusion

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción en una cadencia fuera del calendario de versiones 21.1. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## Mejoras de API

La versión 12 de la API ya está disponible con la versión 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Para obtener información sobre novedades y actualizaciones, consulte [Novedades de la versión 12](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm) de la API.

Para obtener más información sobre las versiones de API, consulte [Versiones de API y programación de soporte](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Actualizaciones de mantenimiento de Workfront 

Para obtener información acerca de las actualizaciones de mantenimiento realizadas durante la versión 21.1, consulte [Actualizaciones de mantenimiento de Workfront](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Anuncios

* [Nuevas direcciones IP para correo electrónico de Workfront con la versión 21.1](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [Lista de permitidos de direcciones IP adicionales para suscripciones a eventos](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [Se requiere la Lista de permitidos de dominios adicionales para acceder a Workfront](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Desaprobación de Flash](#flash-deprecation)
* [Seminario web sobre la versión 21.1](#21-1-release-webinar)
* [Cambio en la cadencia de la versión de vista previa](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### Nuevas direcciones IP para correo electrónico de Workfront con la versión 21.1 {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

En un esfuerzo por aumentar el envío de correo electrónico exitoso, agregamos nuevas direcciones IP con la versión de producción 21.1 para los clústeres 1, 2, 3, 4 y 5.

Para obtener más información sobre las direcciones IP que debe agregar al clúster, consulte [Nuevas direcciones IP para el correo electrónico de Adobe Workfront con la versión 21.1](../../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md).

Para saber en qué clúster se encuentra su instancia, vaya a Configuración > Sistema > Información del cliente.

### Lista de permitidos de direcciones IP adicionales para suscripciones a eventos {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

En un esfuerzo por aumentar la entrega de suscripciones a eventos, agregamos 4 direcciones IP nuevas con la versión de producción 21.1 en el primer trimestre de 2021. Debe añadir estas direcciones IP a su lista de permitidos antes de febrero de 2021 para garantizar que los usuarios sigan recibiendo suscripciones a eventos.

Póngase en contacto con el departamento de seguridad o de TI interno para obtener ayuda con la adición de las nuevas direcciones IP que se encuentran en el artículo [API de suscripción a evento](../../../wf-api/general/event-subs-api.md).

### Lista de permitidos de dominios adicionales necesarios para acceder a Workfront {#allowlist-of-additional-domains-required-for-accessing-workfront}

Si su organización utiliza un cortafuegos, debe añadir los siguientes dominios adicionales a su lista de permitidos para garantizar un acceso ininterrumpido a Workfront:

* event.split.io
* sdk.split.io

Para obtener más información, consulte [Configuración de la lista de permitidos del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Desaprobación de Flash {#flash-deprecation}

Todas las herramientas basadas en Flash se eliminaron de todos los productos el 19 de noviembre de 2020.

Obtenga más información acerca de soluciones de reemplazo para cada herramienta específica basada en Flash en el siguiente artículo: [Reemplazo de herramientas basadas en Flash en Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### Seminario web sobre la versión 21.1 {#21-1-release-webinar}

El seminario web sobre la versión 21.1 de Workfront se presentará el 3 de febrero a las 11:00 h EDT/16:00 h BST. Regístrese para el seminario web [aquí](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register).

### Cambio en la cadencia de versión de previsualización {#change-in-preview-release-cadence}

A partir del 20 de mayo de 2020, Workfront empezó a ofrecer la funcionalidad en el entorno de vista previa de forma semanal. Antes de este cambio, la funcionalidad generalmente se lanzaba al entorno de vista previa cada dos semanas.

Para obtener más información, consulte [Preguntas frecuentes sobre el cambio en la cadencia de la versión de vista previa de Workfront](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### Workfront One {#workfront-one}

Con Workfront One, descubrirá el contenido, los recursos y las noticias más importantes de Workfront, todo en un solo lugar, con un solo inicio de sesión. Hemos unificado los sitios de experiencia, comunidad y formación, lo que facilita la búsqueda de lo que busca.

[Más información sobre Workfront One](https://www.workfront.com/campaigns/workfront-one).
