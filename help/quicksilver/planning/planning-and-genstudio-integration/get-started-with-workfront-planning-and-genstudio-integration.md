---
title: Introducción a la integración de Workfront Planning y GenStudio for Performance Marketing
description: El espacio de trabajo de GenStudio for Performance Marketing está disponible en Adobe Workfront Planning cuando su empresa ha adquirido ambos productos. Descubra algunos de los conceptos básicos sobre cómo puede optimizar los flujos de trabajo con esta integración.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: b6ced451cdd6b38b5661a076b2311a34c2c70432
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 6%

---

# Introducción a la integración de Adobe Workfront Planning y Adobe GenStudio for Performance Marketing

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->

Las organizaciones que utilizan Adobe Workfront Planning y Adobe GenStudio for Performance Marketing suelen definir los conceptos de marketing como Campañas, Productos y Personas con más detalle que lo que GenStudio admite de forma predeterminada.

Existe una integración nativa entre GenStudio for Performance Marketing y Workfront Planning. Esta integración permite a los usuarios de Workfront Planning administrar las campañas, los productos, las personas, las activaciones, los canales y las regiones utilizados en GenStudio. También les permite configurar GenStudio para que haga referencia a los tipos de registros existentes de Workfront Planning, lo que crea un flujo de trabajo de marketing más conectado y coherente.

Esta integración le ayuda a evitar la entrada de datos duplicados, a mantener la alineación en los esfuerzos de planificación y activación y a admitir su sistema de registro de marketing.

El espacio de trabajo de GenStudio for Performance Marketing está disponible en Adobe Workfront Planning cuando su empresa ha adquirido ambos productos.

Con la integración entre Workfront Planning y GenStudio for Performance Marketing, puede:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Vea el espacio de trabajo de GenStudio en Workfront Planning.
* Modifique sus campañas en GenStudio y tenga actualizaciones en tiempo real de la misma información en Workfront Planning.
* Modifique sus campañas en Workfront Planning y tenga actualizaciones en tiempo real de la misma información en GenStudio.

## Requisitos de integración

* Workfront y GenStudio for Performance Marketing deben estar habilitados para la misma organización.

  Para obtener más información sobre GenStudio, consulte [Guía del usuario de Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).

* GenStudio no estará disponible en Workfront Planning cuando su empresa tenga varias instancias de Workfront. <!--this will change-->

* La instancia de Workfront forma parte de la experiencia unificada de Adobe, incluido el uso del sistema Identity Management (IMS).

  Para obtener más información, consulte [Adobe Unified Experience para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Los usuarios que utilizan Planning y GenStudio solo pueden pertenecer a una instancia de Workfront dentro de la organización IMS.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Requisitos de acceso

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
   <li><p> Adobe GenStudio for Performance Marketing</p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete de flujo de trabajo de Workfront</p>  
<p>Cualquier paquete de Workfront Planning</p>
   </td> </tr>

<tr> 
   <td role="rowheader"><p>paquete de Adobe GenStudio</p></td> 
   <td> 
<p>???</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p> Administrador del sistema</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe GenStudio</p></td> 
   <td><p> ???</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>  
   <p>Configuración de GenStudio: ???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  
   <p>En Workfront Planning: </p>
   <ul>
   <li><p>Permisos de contribución o superiores para un espacio de trabajo y tipo de registro  </p> </li> 
   <li><p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p></li>
   </ul>
   <p>En Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Cualquier permiso de Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Crear permisos en Adobe GenStudio for Performance Marketing para crear elementos</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
*Para obtener más información sobre Adobe GenStudio for Performance Marketing, consulte [Guía del usuario de Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).


## Información general sobre la integración de Workfront Planning y GenStudio

Las secciones siguientes describen lo siguiente:

* Capacidades para actualizar información de Workfront Planning desde GenStudio
* Funciones para actualizar información de GenStudio desde Workfront Planning
* Limitaciones de lo que se puede y no se puede administrar en un espacio de trabajo de GenStudio desde Workfront Planning.

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### El espacio de trabajo de GenStudio en Workfront Planning

* Si su organización tiene varias instancias de Workfront, el espacio de trabajo de GenStudio no es visible desde ninguna instancia de Workfront. <!-- this might change-->
* El espacio de trabajo de GenStudio muestra un indicador visual que indica claramente que se importa desde GenStudio. Para obtener más información, consulte [Administrar el espacio de trabajo de GenStudio en Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Todos los usuarios que tienen acceso a GenStudio y a Workfront Planning también pueden ver el espacio de trabajo de GenStudio en Workfront Planning.
* Los usuarios de Workfront Planning deben administrarse a través de Adobe Identity Management System (IMS) para poder ver y utilizar GenStudio Workspace desde Workfront.

  Los usuarios solo de Workfront no pueden ver GenStudio Workspace, aunque esté disponible en Workfront.

  Para obtener más información, consulte [Adobe Unified Experience para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


### Tipos de registro

* Puede editar la información de los tipos de registro (por ejemplo, su aspecto) desde GenStudio en Workfront Planning.
* Puede compartir tipos de registros de GenStudio con otros usuarios en Planning.
* Puede crear tipos de registros desde Planning en GenStudio Workspace. Estos tipos de registros permanecen únicamente en Planning. No se muestran en GenStudio.
* Los tipos de registro sincronizados con GenStudio muestran un indicador visual en Workfront Planning que deja en claro que los tipos de registro se importan desde GenStudio.

### Registros

* Puede añadir o eliminar registros en GenStudio para que sean visibles en Workfront Planning (o se eliminen de ella).
* Puede agregar o eliminar registros en Workfront Planning para que sean visibles en GenStudio (o se eliminen de ella).
* Cuando se eliminan registros de Workfront Planning o GenStudio, se colocan en el grupo Eliminados recientemente durante 30 días. GenStudio no tiene un grupo eliminado recientemente.
* La restauración de un registro del grupo eliminado recientemente los coloca de nuevo en Workfront Planning y GenStudio.
* Puede agregar registros desde Workfront Planning de las siguientes maneras:

   * Manualmente, desde cero, desde cualquier vista con el botón Nuevo registro
   * Importándolos con un archivo CSV o de Excel
   * Manualmente, en línea, en la vista de tabla
   * Manualmente, directamente en la vista de cronología

  Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
* No puede crear ni eliminar registros de activación desde Workfront Planning.
* Puede editar la información de registro de todos los registros del espacio de trabajo de GenStudio en Planning en cualquiera de los campos visibles desde Workfront Planning.

  Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Campos

* Los campos de registro se importan desde GenStudio. Puede editar la configuración de campo en Workfront Planning.
* Puede crear campos para tipos de registros de GenStudio en Workfront Planning si tiene acceso de administración en Gen Studio.
* Cuando se crean campos para tipos de registros de GenStudio en Planning, son visibles desde las áreas siguientes:
   * Vistas de planificación
   * Páginas de detalles del registro de planificación
   * páginas de detalles de registro de GenStudio

  >[!TIP]
  >
  >Los campos creados en Workfront Planning no son visibles en la vista de lista de GenStudio.

* Puede ocultar campos en la vista de tabla de un tipo de registro de GenStudio en Planning.
* No se pueden eliminar campos importados de GenStudio desde Workfront Planning.
* Puede eliminar campos creados en Workfront Planning para tipos de registros de GenStudio desde Workfront Planning.


### Los campos Creado por y Aprobado por

* Puede agregar los campos Creado por y Aprobado por para los tipos de registro de GenStudio en Workfront Planning desde Workfront Planning.
* Los registros que se muestran en los tipos de registro Canal y Región mostrarán &quot;Sistema&quot; como el usuario Creado por. Estos registros se crean automáticamente cuando el espacio de trabajo de GenStudio se crea en Workfront Planning.
* Los registros creados en GenStudio después de que el espacio de trabajo estuviera disponible en Workfront Planning mostrarán el nombre del usuario de IMS que creó el registro en el campo Creado por, aunque el usuario haya creado los registros en GenStudio y no sea un usuario de Workfront.
* El campo Aprobado por muestra el nombre del aprobador cuando se envía un formulario de solicitud para crear un registro.

### Vistas

* Puede crear vistas para tipos de registros de GenStudio.

  Para obtener más información, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

* Puede compartir la vista de un tipo de registro de GenStudio como lo haría con una vista de un tipo de registro de Planning.
* No se pueden crear varias vistas en GenStudio.

### Conexiones

* Puede realizar las siguientes conexiones entre los tipos de registros de GenStudio y otros tipos de registros u objetos en Workfront Planning:

   * Dos tipos de registros GenStudio
   * Un tipo de registro GenStudio y un tipo de registro Planning del mismo espacio de trabajo
   * Un tipo de registro GenStudio y un tipo de registro Planning de otro espacio de trabajo, si los tipos de registro están configurados para conectarse desde otro espacio de trabajo.
   * Un tipo de registro GenStudio y un tipo de objeto Workfront (proyectos, portafolios, programas, empresas, grupos)
   * Un tipo de registro GenStudio y un tipo de objeto AEM Assets.

### Solicitar formularios y automatizaciones

* Puede agregar formularios de solicitud y automatizaciones a un tipo de registro de GenStudio en Workfront Planning.

### El entorno de vista previa

* El espacio de trabajo de GenStudio accesible desde el entorno de producción también se muestra en el entorno de vista previa.
* Puede realizar todas las actividades descritas en este artículo en el espacio de trabajo de GenStudio en Workfront Planning en su entorno de vista previa, pero estos cambios no se transferirán a GenStudio.
Solo los cambios que realice en los elementos del entorno de producción se sincronizan entre Workfront Planning y GenStudio.
GenStudio no tiene un entorno de vista previa.

