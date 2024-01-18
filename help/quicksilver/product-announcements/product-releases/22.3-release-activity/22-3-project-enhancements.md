---
title: actualizaciones del proyecto durante el periodo de tiempo de la versión 22.3
description: actualizaciones del proyecto durante el periodo de tiempo de la versión 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# 22.3 Mejoras del proyecto

Esta página describe todas las mejoras de Project realizadas con la versión 22.3 en el entorno de vista previa. Estas mejoras estuvieron disponibles en el entorno de producción la semana del 11 de julio de 2022. Para obtener una lista de todos los cambios disponibles con la versión 22.3, consulte [Información general de la versión 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Delegación de trabajo fuera de la oficina

Ahora puede delegar temporalmente las tareas y problemas asignados a otros usuarios cuando planee estar fuera de la oficina por un breve período de tiempo. Esto garantiza que su ausencia no se convierta en un obstáculo para que el trabajo se complete.

Antes de esta mejora, solo se podían delegar aprobaciones.

Las siguientes son algunas de las funciones que agregamos con esta actualización:

* Una configuración en el área de Preferencias de tareas y problemas de Configuración para que el administrador del sistema o del grupo habilite la delegación en su entorno.

* Una nueva opción para &quot;Delegar tareas y problemas&quot; en el área de Inicio para que los usuarios con una licencia de revisión o superior deleguen sus elementos de trabajo.

* Indicación en la página de inicio y en el área de asignaciones de los encabezados de tarea y problema de que los elementos se delegan en otros.

* Notificaciones de eventos en el área de Configuración y notificaciones por correo electrónico en el perfil de usuario para controlar las notificaciones por correo electrónico sobre el trabajo delegado


>[!NOTE]
>
>Solo los usuarios con una licencia de revisión o superior pueden delegar su trabajo a otros. El trabajo se puede delegar a cualquier usuario, independientemente de su nivel de acceso. Los usuarios delegados reciben los mismos permisos que los usuarios asignados a los elementos delegados. Si estos permisos son inferiores a la configuración de nivel de acceso de un usuario, es posible que se impida a los usuarios delegados realizar algunas de las actividades en las tareas y problemas que se les han delegado.


Para obtener más información, consulte [Delegar tarea y descripción general del problema](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Nueva experiencia al convertir un problema en una tarea

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para convertir un problema en una tarea.

Esta actualización incluye:

* Una interfaz de usuario actualizada que coincide con el resto de la nueva experiencia de Workfront.

* Acceso para convertir un problema en tareas de una lista o un informe.

* Los formularios personalizados predeterminados definidos en el área Configuración de tareas del proyecto de destino se agregaron a la nueva tarea.


Para obtener más información, consulte [Conversión de un problema en una tarea en Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nueva experiencia al convertir un problema en un proyecto sin plantilla

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para convertir un problema en un proyecto sin usar una plantilla.

Además de una interfaz de usuario actualizada que coincide con el resto de la nueva experiencia de Workfront, también hemos agregado la capacidad de convertir un problema en proyectos en blanco de una lista o un informe.

Para obtener más información, consulte [Conversión de un problema en un proyecto en Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Etiquetado inteligente en el flujo de actualización

Hemos mejorado el etiquetado de usuarios en el flujo de actualización cuando se crea una nueva actualización o se responde a una existente. Ahora, cuando etiquete a un usuario para incluirlo en una actualización, además de su nombre y avatar, también mostramos su función principal y su correo electrónico. Esto ayuda a distinguir entre varios usuarios con nombres similares o idénticos.

Para obtener más información, consulte [Etiquetar a otros en las actualizaciones](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nueva sintaxis para cálculos en campos personalizados

Con el fin de prepararse para futuras mejoras que le ayudarán a agregar cálculos a los formularios personalizados, hemos estandarizado la sintaxis de los campos a los que se hace referencia que agregue a un cálculo. Es fácil utilizar esta nueva sintaxis porque el sistema la introduce automáticamente cuando empieza a escribir el nombre de un campo y, a continuación, lo selecciona.

Para obtener más información, consulte la sección &quot;Generar el cálculo para el campo personalizado calculado&quot; en la [Artículo Agregar datos calculados a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Mantener información precisa cuando dos usuarios con una función común participen en un proceso de aprobación

Para garantizar la precisión de sus datos a la hora de aprobar el trabajo, hemos realizado un cambio en la forma en que se registra la información de aprobación en un elemento cuando se asocia un proceso de aprobación de varias funciones con dicho elemento.

Algunos procesos de aprobación requieren la aprobación de dos funciones diferentes, y dos aprobadores diferentes pueden tener una de esas funciones en común. Ahora, cuando esto sucede, una vez tomadas las decisiones de aprobación, Workfront registra a cada aprobador y su función respectiva asociada al proceso de aprobación.

Antes de este cambio, ambas aprobaciones se registraban para el segundo usuario porque compartían una de las funciones de aprobación con el primer aprobador. En este caso, el segundo aprobador sobrescribía la información del primer aprobador.

Para obtener más información sobre los procesos de aprobación en Workfront, consulte [Resumen del proceso de aprobación](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Las horas de asignación ya no se eliminarán al realizar cambios en las asignaciones

>[!NOTE]
>
>Originalmente, esta función se había planificado para su lanzamiento con la versión 22.2. Se publicó en Production el 21 de abril de 2022.


Para garantizar la precisión de sus datos, hemos realizado un cambio para conservar las horas de asignación y mantener las Horas planificadas de la tarea sin cambios al realizar cambios en las asignaciones de la tarea.

Se han realizado los siguientes cambios en las tareas con un tipo de duración simple:

* Las horas planificadas se conservan al eliminar a todas las personas asignadas.

* Las asignaciones de asignación individuales se conservan al reemplazar usuarios y roles.

* Las asignaciones de asignación individuales se conservan en el rol al eliminar el usuario. (Se ha eliminado de la versión. Ahora, las horas planificadas se establecerán en 0 después de eliminar a todas las personas asignadas).


Para obtener más información sobre las horas planificadas, consulte [Resumen de horas planificadas](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Mejoras de tableros

Se han añadido las siguientes mejoras a los tableros de Adobe Workfront:

* Opciones de filtro: ahora puede filtrar por fecha de vencimiento o estado en un tablero. El filtro también se ha actualizado con secciones contraíbles para separar las opciones.

* Archivar tablero: ahora puede archivar un tablero mientras está en el tablero, en lugar de tener que ir al tablero de tableros.

* Agregar un equipo a un tablero: cuando busca miembros, puede agregar un equipo completo. Elegir un equipo agrega a todos los integrantes del equipo al tablero.

* Zonas de colocación en columnas: al arrastrar y soltar una tarjeta de una columna de tablero a otra, ahora una &quot;zona de colocación&quot; gris muestra dónde se colocará la tarjeta. Anteriormente no había un indicador visual de la ubicación de la tarjeta.

* Tarjetas conectadas: ahora puede agregar tarjetas conectadas a tareas y problemas de Workfront. Al actualizar el nombre, la descripción o el usuario asignado en la tarjeta o la tarea, se actualizarán los mismos campos en la otra ubicación.

* Campo de estado en todas las tarjetas: se han agregado un campo de estado y un botón Marcar como completado a las tarjetas ad hoc y conectadas. Al hacer clic en Marcar como completado, el estado cambia automáticamente a Completo.

* Convertir una tarjeta ad hoc en una tarjeta conectada: ahora tiene la opción de convertir una tarjeta ad hoc en una tarjeta conectada a partir de los detalles de la tarjeta.

* Desconectar la tarjeta conectada: al desconectar una tarjeta conectada, se interrumpe la conexión con el objeto Workfront. La tarjeta permanece como una tarjeta ad hoc en el tablero y el objeto Workfront no se ve afectado.

* Asignación de estado en columnas: la nueva configuración de columnas y directivas permiten definir un estado, un usuario asignado o una etiqueta que se aplica a las tarjetas que se mueven a esa columna. Además, los nombres de columna predeterminados en un nuevo tablero se han cambiado a Columna 1, Columna 2 y Columna 3.

* Indicador de actualización de campo: ahora se muestra un indicador al guardar una tarjeta para confirmar que se han guardado las actualizaciones.


Para obtener más información, consulte [Introducción a los tableros en Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Compartir carpetas solo en los cinco niveles principales de una jerarquía de carpetas

Para garantizar el mejor rendimiento a los usuarios que comparten carpetas, actualmente limitamos el uso compartido a los cinco niveles principales de una jerarquía de carpetas en un objeto.

Cada carpeta del sexto nivel o inferior hereda sus configuraciones de uso compartido de la carpeta directamente superior a ella.

Para obtener más información sobre cómo compartir carpetas, consulte [Compartir una carpeta de documentos de nivel superior](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Campañas de Workfront (beta): una nueva forma de administrar su trabajo

>[!NOTE]
>
>Está previsto eliminar esta función de la vista previa el 9 de enero de 2023. Para obtener más información, consulte la [Página de información general de la versión 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Esta función no se incluirá en la versión de producción 22.3. Se lanzará al entorno de producción en una versión futura.


>[!NOTE]
>
>Esta funcionalidad solo está disponible como una versión beta y actualmente está en construcción. En futuras versiones seguiremos añadiendo funciones para el flujo de trabajo de Campaign. La participación en el programa beta de Workfront Campaign es voluntaria.

Presentamos un nuevo objeto para Adobe Workfront que tiene el potencial de cambiar la forma en que administra el trabajo.

Workfront Campaigns permite organizar proyectos de diferentes portafolios y programas en un nuevo contenedor de trabajo. Este nuevo contenedor evolucionará en futuras versiones para incluir finalmente todos los objetos de trabajo que se administran actualmente en silos independientes.

Esta versión incluye las siguientes funciones:

* Un nuevo objeto de Workfront llamado Campaign

* Una nueva área de Campañas (Beta) en el menú principal

* Una lista de campañas en el área Campañas

* Página de detalles de la campaña que muestra información adicional sobre una campaña

* Capacidad para añadir proyectos a una campaña

* Capacidad para editar información sobre una campaña

* Posibilidad de cambiar el nombre del objeto de campaña desde la plantilla de diseño

  Los administradores de sistemas y grupos de Workfront pueden añadir el área de Campañas (beta) en el menú principal de una plantilla de diseño. Esto lo hace disponible para todos los usuarios asignados a la plantilla. Una vez disponible, cualquier usuario de Workfront puede crear una campaña.




