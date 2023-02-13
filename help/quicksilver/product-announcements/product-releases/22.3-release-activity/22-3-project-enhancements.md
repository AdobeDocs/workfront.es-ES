---
title: actualizaciones del proyecto durante el intervalo de tiempo de la versión 2.3
description: actualizaciones del proyecto durante el intervalo de tiempo de la versión 2.3
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 0fea13b0a1d8f14c2d601e0ed0a8d15684a3c4d7
workflow-type: tm+mt
source-wordcount: '1549'
ht-degree: 0%

---

# 22.3 Mejoras del proyecto

En esta página se describen todas las mejoras realizadas en el proyecto con la versión 2.3 del entorno de vista previa. Estas mejoras estaban disponibles en el entorno Producción durante la semana del 11 de julio de 2022. Para obtener una lista de todos los cambios disponibles con la versión 2.3, consulte [Información general sobre la versión 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Delegación de trabajo fuera de la oficina

Ahora, puede delegar temporalmente las tareas y los problemas que se le asignen a otros usuarios cuando tenga pensado salir de la oficina durante un breve período de tiempo. Esto garantiza que su ausencia no se convierta en un obstáculo para el trabajo que se está completando.

Antes de esta mejora, solo podía delegar aprobaciones.

Las siguientes son algunas de las funciones que agregamos con esta actualización:

* Una configuración en el área Preferencias de tareas y problemas de Configuración para el administrador del sistema o del grupo para habilitar la delegación en su entorno.

* Una nueva opción para &quot;Delegar tareas y problemas&quot; en el área de inicio para que los usuarios con una licencia de revisión o superior deleguen sus elementos de trabajo.

* Indicación en la página de inicio y en el área Asignaciones de encabezados de tarea y problema de que los elementos se delegan a otros.

* Notificaciones de eventos en el área Configuración y Notificaciones de correo electrónico en el perfil de usuario para controlar las notificaciones de correo electrónico sobre el trabajo delegado


>[!NOTE]
>
>Solo los usuarios con una licencia de revisión o superior pueden delegar su trabajo a otros. El trabajo se puede delegar a cualquier usuario, independientemente de su nivel de acceso. Los usuarios delegados reciben los mismos permisos que los usuarios asignados en los elementos delegados. Si estos permisos son inferiores a la configuración de nivel de acceso de un usuario, es posible que los usuarios delegados no puedan realizar algunas de las actividades en las tareas y problemas que se les delegan.


Para obtener más información, consulte [Resumen del problema y la tarea delegada](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Nueva experiencia al convertir un problema en una tarea

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para convertir un problema en una tarea.

Esta actualización incluye:

* Interfaz de usuario actualizada que coincide con el resto de la nueva experiencia de Workfront.

* Acceso para convertir un problema en tareas de una lista o un informe.

* Los formularios personalizados predeterminados definidos en el área Configuración de tareas del proyecto de destino añadido a la nueva tarea.


Para obtener más información, consulte [Conversión de un problema en una tarea en Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nueva experiencia al convertir un problema en un proyecto sin plantilla

Para que el uso de Workfront sea coherente con la nueva experiencia de Workfront, hemos rediseñado la interfaz para convertir un problema en un proyecto sin usar una plantilla.

Además de una interfaz de usuario actualizada que coincide con el resto de la nueva experiencia de Workfront, también hemos agregado la capacidad de convertir un problema en proyectos en blanco desde una lista o un informe.

Para obtener más información, consulte [Convertir un problema en un proyecto en Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Etiquetado inteligente en el flujo de actualización

Hemos mejorado el etiquetado de usuarios en el flujo de actualización al crear una nueva actualización o responder a una existente. Ahora, al etiquetar a un usuario para incluirlo en una actualización, además de su nombre y avatar, también mostramos su Función principal y su correo electrónico. Esto ayuda a distinguir entre varios usuarios con nombres similares o idénticos.

Para obtener más información, consulte [Etiquetar otros en actualizaciones](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nueva sintaxis para cálculos en campos personalizados

Para prepararse para futuras mejoras que le ayudarán a agregar cálculos a formularios personalizados, se ha estandarizado la sintaxis de los campos a los que se hace referencia y que se agregan a un cálculo. Es fácil utilizar esta nueva sintaxis, ya que el sistema la introduce cuando comienza a escribir el nombre de un campo y, a continuación, lo selecciona.

Para obtener más información, consulte la sección &quot;Generar el cálculo del campo personalizado calculado&quot; en la sección [artículo Añadir datos calculados a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Mantenga la información precisa cuando dos usuarios con una función común participen en un proceso de aprobación

Para garantizar la precisión de sus datos para la aprobación del trabajo, se ha modificado la forma en que se registra la información de aprobación en un elemento cuando se asocia un proceso de aprobación de funciones múltiples al elemento.

Algunos procesos de aprobación requieren la aprobación de dos funciones diferentes, y dos aprobadores diferentes pueden tener una de esas funciones en común. Ahora, cuando esto sucede, después de tomar las decisiones de aprobación, Workfront registra cada aprobador y su función respectiva asociada al proceso de aprobación.

Antes de este cambio, ambas aprobaciones se registraban para el segundo usuario porque compartían una de las funciones de aprobación con el primer aprobador. En este caso, el segundo aprobador sobrescribía la información del primer aprobador.

Para obtener más información sobre los procesos de aprobación en Workfront, consulte [Información general del proceso de aprobación](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Ya no se quitarán las horas de asignación al realizar cambios en las asignaciones

>[!NOTE]
>
>Esta función estaba originalmente planificada para su lanzamiento con la versión 2.2. Se publicó en Producción el 21 de abril de 2022.


Para garantizar la precisión de sus datos, se ha realizado un cambio para conservar las horas de asignación y mantener las horas planificadas de la tarea sin cambios al realizar cambios en las asignaciones de la tarea.

Se han realizado los siguientes cambios en las tareas con un tipo de duración simple:

* Las horas planificadas se conservan cuando se eliminan todos los asignadores.

* Las asignaciones de asignaciones individuales se conservan al reemplazar usuarios y funciones.

* Las asignaciones de asignaciones individuales se conservan en la función al eliminar el usuario. (Eliminado de la versión. Ahora, el valor de Horario planeado se establecerá en 0 después de eliminar todos los usuarios asignados).


Para obtener más información sobre las horas planificadas, consulte [Información general sobre las horas planificadas](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Mejoras en los tableros

Se han añadido las siguientes mejoras a los tableros de Adobe Workfront:

* Opciones de filtro : ahora puede filtrar por fecha de vencimiento o estado en un tablero. El filtro también se ha actualizado con secciones contraíbles para separar las opciones.

* Tablero de archivo : Ahora puede archivar un tablero mientras está en el tablero, en lugar de tener que ir al tablero.

* Agregar un equipo a un tablero : cuando busca miembros, puede agregar un equipo completo. Al elegir un equipo, se agregan todos los integrantes del equipo al tablero.

* Colocar zonas en columnas : al arrastrar y soltar una tarjeta de una columna de tablero a otra, ahora aparece una &quot;zona de colocación&quot; gris donde se colocará la tarjeta. Anteriormente no había un indicador visual de la colocación de la tarjeta.

* Tarjetas conectadas : ahora puede añadir tarjetas que estén conectadas a tareas y problemas de Workfront. Al actualizar el nombre, la descripción o el usuario asignado en la tarjeta o la tarea, se actualizarán los mismos campos en la otra ubicación.

* Campo de estado en todas las tarjetas: se han añadido un campo de estado y un botón de completado de marca a las tarjetas tanto ad hoc como conectadas. Al hacer clic en Marcar como completado, el estado cambia automáticamente a Completado.

* Convertir tarjeta ad hoc a tarjeta conectada : Ahora tiene la opción de convertir una tarjeta ad hoc a una tarjeta conectada desde los detalles de la tarjeta.

* Desconectar tarjeta conectada : al desconectar una tarjeta conectada, se rompe la conexión con el objeto Workfront. La tarjeta permanece como una tarjeta ad hoc en el tablero y el objeto Workfront no se ve afectado.

* Asignación de estado en columnas : La nueva configuración de columna y las políticas permiten definir un estado, un usuario asignado o una etiqueta que se aplique a las tarjetas movidas a esa columna. Además, los nombres de columna predeterminados en un tablero nuevo se han cambiado a Columna 1, Columna 2 y Columna 3.

* Indicador de actualización de campos : Ahora aparece un indicador al guardar una tarjeta, para confirmar que las actualizaciones se guardaron.


Para obtener más información, consulte [Introducción a los tableros en Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Compartir carpetas solo en los cinco niveles superiores de una jerarquía de carpetas

Para garantizar el mejor rendimiento para los usuarios que comparten carpetas, actualmente limitamos el uso compartido a los cinco niveles superiores de una jerarquía de carpetas en un objeto.

Cada carpeta del sexto nivel o inferior hereda sus configuraciones de uso compartido de la carpeta directamente superior.

Para obtener más información sobre cómo compartir carpetas, consulte [Compartir una carpeta de documentos de nivel superior](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Campañas de Workfront (Beta): una nueva forma de administrar su trabajo

>[!NOTE]
>
>Está previsto que esta función se elimine de Vista previa el 9 de enero de 2023. Para obtener más información, consulte la [Página de información general de la versión 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Esta función no se incluirá en la versión de producción de 22.3. Se lanzará a Producción con una versión futura.


>[!NOTE]
>
>Esta funcionalidad solo está disponible en versión beta y actualmente está en construcción. Seguiremos añadiendo funciones para el flujo de trabajo de Campaign con futuras versiones. La participación en el programa beta de Workfront Campaigns es voluntaria.

Presentamos un nuevo objeto a Adobe Workfront que tiene el potencial de cambiar la forma en que administra el trabajo.

Workfront Campaigns permite organizar proyectos de diferentes portafolios y programas en un nuevo contenedor de trabajo. Este nuevo contenedor evolucionará en futuras versiones para incluir eventualmente todos los objetos de trabajo que actualmente se administran en silos separados.

Esta versión incluye las siguientes funciones:

* Un nuevo objeto de Workfront llamado Campaign

* Un nuevo área de campañas (Beta) en el menú principal

* Una lista de campañas del área Campañas

* Una página Detalles de campaña que muestra información adicional sobre una campaña

* Posibilidad de agregar proyectos a una campaña

* Capacidad de editar información sobre una campaña

* Posibilidad de cambiar el nombre del objeto de campaña desde la plantilla de diseño

   Los administradores de sistemas y grupos de Workfront pueden agregar el área Campañas (Beta) en el menú principal de una plantilla Diseño. Esto lo hace disponible para todos los usuarios asignados a la plantilla. Una vez que esté disponible, cualquier usuario de Workfront puede crear una campaña.




