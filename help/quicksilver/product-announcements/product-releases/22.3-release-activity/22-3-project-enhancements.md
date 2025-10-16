---
title: actualizaciones del proyecto durante el período de tiempo de la versión 22.3
description: actualizaciones del proyecto durante el período de tiempo de la versión 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1535'
ht-degree: 99%

---

# 22.3 Mejoras del proyecto

Esta página describe todas las mejoras del proyecto realizadas con la versión 22.3 en el entorno de vista previa. Estas mejoras se incorporaron en el entorno de producción la semana del 11 de julio de 2022. Para obtener una lista de todos los cambios disponibles con la versión 22.3, consulte [Información general sobre la versión 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Delegación de trabajo fuera de la oficina

Ahora, puede delegar temporalmente a otros usuarios las tareas y asuntos que le hayan sido asignados cuando tenga previsto ausentarse de la oficina durante un breve período de tiempo. De este modo se garantiza que su ausencia no se convierta en un obstáculo para la finalización del trabajo.

Antes de esta mejora, solo se podían delegar aprobaciones.

Las siguientes son algunas de las funciones que añadimos con esta actualización:

* Una configuración en el área de Preferencias de tareas y problemas de Configuración para que el administrador del sistema o del grupo habilite la delegación en su entorno.

* Una nueva opción para “Delegar tareas y problemas” en el área de Inicio para que los usuarios con una licencia de revisión o superior deleguen sus elementos de trabajo.

* Indicación en la página de inicio y en el área de asignaciones de los encabezados de tareas y problemas de que los elementos se delegan a otros.

* Notificaciones de eventos en el área de configuración y notificaciones por correo electrónico en el perfil de usuario para controlar las notificaciones por correo electrónico sobre el trabajo delegado


>[!NOTE]
>
>Solo los usuarios con una licencia de revisión o superior pueden delegar su trabajo a otros. El trabajo se puede delegar a cualquier usuario, independientemente de su nivel de acceso. Los usuarios delegados reciben los mismos permisos que los usuarios asignados a los elementos delegados. Si estos permisos son inferiores a la configuración de nivel de acceso de un usuario, es posible que se impida a los usuarios delegados realizar algunas de las actividades en las tareas y problemas que se les han delegado.


Para obtener más información, consulte [Información general sobre la delegación de tareas y problemas](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Nueva experiencia al convertir un problema en una tarea

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para convertir un problema en una tarea.

Esta actualización incluye lo siguiente:

* Una interfaz de usuario actualizada que coincide con el resto de la nueva experiencia de Workfront.

* Acceso para convertir un problema en tareas de una lista o un informe.

* Los formularios personalizados predeterminados definidos en el área de configuración de tareas del proyecto de destino se han añadido a la nueva tarea.


Para obtener más información, consulte [Convertir un problema en una tarea](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nueva experiencia al convertir un problema en un proyecto sin una plantilla

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para convertir un problema en un proyecto sin usar una plantilla.

Además de una interfaz de usuario actualizada que coincide con el resto de la nueva experiencia de Workfront, también hemos añadido la capacidad de convertir un problema en proyectos en blanco de una lista o un informe.

Para obtener más información, consulte [Convertir un problema en un proyecto en Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Etiquetado inteligente en el flujo de actualizaciones

Hemos mejorado el etiquetado de usuarios en el flujo de actualizaciones cuando se crea una nueva actualización o se responde a una existente. Ahora, cuando etiquete a un usuario para incluirlo en una actualización, además de su nombre y avatar, también mostramos su función principal y su correo electrónico. Esto ayuda a distinguir entre varios usuarios con nombres similares o idénticos.

Para obtener más información, consulte [Etiquetar a los usuarios en las actualizaciones](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nueva sintaxis para cálculos en campos personalizados

Con el fin de prepararse para futuras mejoras que le ayudarán a añadir cálculos a los formularios personalizados, hemos estandarizado la sintaxis de los campos referenciados que añade a un cálculo. Es fácil utilizar esta nueva sintaxis, ya que el sistema la introduce automáticamente cuando empieza a escribir el nombre de un campo y, a continuación, lo selecciona.

## Mantener información precisa cuando dos usuarios con una función en común participan en un proceso de aprobación

Para garantizar la precisión de sus datos a la hora de aprobar el trabajo, hemos realizado un cambio en la forma en que se registra la información de aprobación en un elemento cuando se asocia un proceso de aprobación de varias funciones con dicho elemento.

Algunos procesos de aprobación requieren la aprobación de dos funciones diferentes y dos aprobadores diferentes pueden tener una de esas funciones en común. Ahora, cuando esto sucede, una vez tomadas las decisiones de aprobación, Workfront registra a cada aprobador y su función respectiva asociada con el proceso de aprobación.

Antes de este cambio, ambas aprobaciones se registraban para el segundo usuario porque compartían una de las funciones de aprobación con el primer aprobador. En este caso, el segundo aprobador sobrescribía la información del primer aprobador.

Para obtener más información sobre los procesos de aprobación en Workfront, consulte [Información general sobre el proceso de aprobación](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Las horas de asignación ya no se eliminarán al realizar cambios en las asignaciones

>[!NOTE]
>
>Originalmente, esta función se había planificado para su lanzamiento con la versión 22.2. Se publicó en producción el 21 de abril de 2022.


Para garantizar la precisión de sus datos, hemos realizado un cambio para conservar las horas de asignación y mantener las horas planificadas de la tarea sin cambios al realizar cambios en las asignaciones de la tarea.

Se han realizado los siguientes cambios en las tareas con un tipo de duración simple:

* Las horas planificadas se conservarán al eliminar a todas las personas asignadas.

* Las asignaciones de asignación individuales se conservan al reemplazar usuarios y funciones.

* Las asignaciones individuales se conservan en la función al eliminar el usuario. (Se ha eliminado de la versión. Ahora, las horas planificadas se establecerán en 0 después de eliminar a todas las personas asignadas).


Para obtener más información sobre las horas planificadas, consulte [Resumen de horas planificadas](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Mejoras de paneles

Se han añadido las siguientes mejoras a los paneles de Adobe Workfront:

* Opciones de filtro: ahora puede filtrar por fecha de vencimiento o estado en un tablero. El filtro también se ha actualizado con secciones contraíbles para separar las opciones.

* Archivar panel: ahora puede archivar un panel mientras está en el panel, en lugar de tener que ir al panel de control de paneles.

* Añadir un equipo a un panel: cuando busca miembros, puede añadir un equipo completo. Elegir un equipo añade a todos los integrantes del equipo al panel.

* Zonas de colocación en columnas: al arrastrar y soltar una tarjeta de una columna de panel a otra, ahora una &quot;zona de colocación&quot; gris muestra dónde se colocará la tarjeta. Anteriormente no había un indicador visual de la ubicación de la tarjeta.

* Tarjetas conectadas: ahora puede añadir tarjetas conectadas a tareas y problemas de Workfront. Al actualizar el nombre, la descripción o el usuario asignado en la tarjeta o la tarea, se actualizarán los mismos campos en la otra ubicación.

* Campo de estado en todas las tarjetas: se han añadido un campo de estado y un botón Marcar como completado a las tarjetas ad hoc y conectadas. Al hacer clic en Marcar como completado, el estado cambia automáticamente a Completo.

* Convertir una tarjeta ad hoc en una tarjeta conectada: ahora tiene la opción de convertir una tarjeta ad hoc en una tarjeta conectada a partir de los detalles de la tarjeta.

* Desconectar la tarjeta conectada: al desconectar una tarjeta conectada, se interrumpe la conexión con el objeto de Workfront. La tarjeta permanece como una tarjeta ad hoc en el panel y el objeto de Workfront no se ve afectado.

* Asignación de estado en columnas: la nueva configuración de columnas y directivas permite definir un estado, un usuario asignado o una etiqueta que se aplica a las tarjetas que se mueven a esa columna. Además, los nombres de columna predeterminados en un nuevo panel se han cambiado a Columna 1, Columna 2 y Columna 3.

* Indicador de actualización de campo: ahora se muestra un indicador al guardar una tarjeta para confirmar que se han guardado las actualizaciones.


Para obtener más información, consulte [Introducción a los paneles en Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Compartir carpetas solo en los cinco niveles principales de una jerarquía de carpetas

Para garantizar el mejor rendimiento a los usuarios que comparten carpetas, actualmente limitamos el uso compartido a los cinco niveles principales de una jerarquía de carpetas en un objeto.

Cada carpeta del sexto nivel o inferior hereda sus configuraciones de uso compartido de la carpeta directamente superior a ella.

Para obtener más información sobre cómo compartir carpetas, consulte [Compartir una carpeta de documentos de nivel superior](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Campañas de Workfront (Beta): una nueva forma de administrar su trabajo

>[!NOTE]
>
>Está previsto eliminar esta función de la vista previa el 9 de enero de 2023. Para más información, consulte la [página Resumen de la versión 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Esta función no se incluirá en la versión de producción 22.3. Se lanzará a Producción con una versión posterior.


>[!NOTE]
>
>Esta funcionalidad solo está disponible como una versión beta y actualmente está en construcción. En futuras versiones seguiremos añadiendo funciones para el flujo de trabajo de Campaign. La participación en el programa beta de Workfront Campaign es voluntaria.

Presentamos un nuevo objeto en Adobe Workfront que tiene el potencial de cambiar la forma en que administra el trabajo.

Workfront Campaigns permite organizar proyectos de diferentes portafolios y programas en un nuevo contenedor de trabajo. Este nuevo contenedor evolucionará en futuras versiones para incluir finalmente todos los objetos de trabajo que se administran actualmente en silos independientes.

Esta versión incluye las siguientes funciones:

* Un nuevo objeto de Workfront llamado Campaign

* Una nueva área de Campaigns (Beta) en el menú principal

* Una lista de campañas en el área Campañas

* Página de detalles de la campaña que muestra información adicional sobre una campaña

* Capacidad para añadir proyectos a una campaña

* Capacidad para editar información sobre una campaña

* Posibilidad de cambiar el nombre del objeto de campaña desde la plantilla de diseño

  Los administradores de sistemas y de grupos de Workfront pueden añadir el área de Campañas (Beta) en el menú principal de una plantilla de diseño. Esto la hace disponible para todos los usuarios asignados a la plantilla. Una vez disponible, cualquier usuario de Workfront puede crear una campaña.




