---
content-type: release-notes
title: Actividad de la versión del cuarto trimestre de 2026 para Adobe Workfront Planning
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el cuarto trimestre de 2026.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 10d95f7fc71d72edd5cbb292af69a348b648b4ba
workflow-type: tm+mt
source-wordcount: '2057'
ht-degree: 3%
---
# Actividad de la versión del cuarto trimestre de 2026 para Adobe Workfront Planning

Este artículo describe las funciones que se lanzarán para Workfront Planning durante la versión del cuarto trimestre de 2026.

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## CX Coworker ahora disponible en Workfront Planning

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

CX Coworker ya está disponible en Workfront Planning. Ahora puede acceder a CX Coworker en un panel disponible en Workfront Planning.

CX Coworker Chat es una interfaz conversacional para hacer el trabajo. Describa un objetivo en lenguaje sencillo y su Compañero de trabajo planificará el trabajo, lo ejecutará en Workfront Planning y en los sistemas Adobe conectados, validará los resultados y le devolverá el trabajo terminado para su aprobación.

El compañero respeta los controles de acceso existentes en su organización, con acceso de solo lectura de forma predeterminada, y los administradores del sistema controlan cuándo los usuarios obtienen acceso de escritura.

El compañero está reemplazando al asistente de IA actual como una forma más potente de realizar el trabajo. Los compañeros de trabajo forman parte del ecosistema de Adobe y no se limitan a Workfront Planning.

>[!IMPORTANT]
>
>CX Coworker no está disponible actualmente para organizaciones de atención médica, finanzas u otros sectores con datos confidenciales. Estas organizaciones disponen de un asistente de IA.

Para obtener más información, consulte [Información general de CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

<!--

## Removed the AI Assistant icon in the Details preview box in preparation for the CX Coworker launch

>[!NOTE]
>
>Preview: September 16, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026
>[!BADGE Off schedule]{type=Neutral}

This change is available for customers who have the CX Coworker in Workfront.

In preparation for the launch of the Adobe CX Coworker in Workfront, we have removed the AI Assistant icon from the Details preview page. The icon still exists on the Details page, when opened in full screen. Clicking it will open the CX Coworker.

For information, see [CX Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-in-workfront.md).

-->

## Se ha mejorado la experiencia al duplicar registros que tienen campos conectados con un tipo de conexión Uno a uno o Uno a varios

>[!NOTE]
>
>Vista previa: 17 de septiembre de 2026
>Versión rápida de producción: 14 de octubre de 2026
>Producción para todos: 15 de octubre de 2026

Ahora se pueden duplicar registros incluso cuando existen registros conectados uno a uno o uno a varios. Después de la duplicación, los usuarios pueden elegir mantener el registro conectado en el registro original o conectarlo al nuevo registro. Mantener activado el original es la opción predeterminada.

El cuadro de diálogo de resolución de conflictos de conexión se ha actualizado para reflejar este nuevo comportamiento y proporcionar una mayor flexibilidad al administrar registros conectados.

Para obtener más información, consulte [Registros duplicados](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

## Administrar la visibilidad de las miniaturas y los colores de los registros desde la columna del campo principal en la vista de tabla

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Ahora puede administrar la visibilidad de las miniaturas y los colores de los registros al editar la columna del campo principal en la vista de tabla.

Con esta actualización, la configuración de Miniatura y Color se eliminará del icono Campos de la barra de herramientas de la vista de tabla.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

## Crear reglas de negocio para los tipos de registro

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Como administrador del espacio de trabajo, ahora puede establecer reglas empresariales para los tipos de registro que posteriormente reflejarán cómo se administran los registros de ese tipo. Puede definir reglas que permitan a los usuarios editar o eliminar registros sólo cuando se cumplan determinadas condiciones o se rellenen determinados campos.

Puede crear una condición para la regla de negocio que haga referencia a todos los tipos de campo excepto a los siguientes:

* Campos de fórmula
* Campos de búsqueda
* Campos de referencia

No se pueden agregar reglas de negocio a los tipos de registro globales.

Para obtener más información, consulte [Configurar reglas de negocio de tipo de registro](/help/quicksilver/planning/architecture/configure-business-rules.md).

>[!NOTE]
>
>Con esta actualización, también se han actualizado las siguientes opciones de menú del menú Más de un tipo de registro:
>
>* **Crear formularios de solicitud** y **Administrar formularios de solicitud** han cambiado a **Formularios de solicitud**
>* **Administrar automatizaciones** ha cambiado a **Automaciones**

## Introducción de semanas personalizadas para la vista de cronología

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Como administrador de Workfront, ahora puede configurar semanas personalizadas, además de trimestres personalizados. Las semanas y trimestres personalizados están visibles desde la vista de cronología de Workfront Planning. Workfront genera semanas secuenciales a partir de la semana 1 al principio del trimestre personalizado 1.

Puede personalizar las etiquetas de semana que están visibles en la vista de cronología. Puede elegir un formato predefinido o introducir uno personalizado.

Las semanas personalizadas no son visibles en Workfront. Solo están visibles en la vista de cronología de Workfront Planning.

Para obtener más información, consulte [Habilitar trimestres personalizados](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Filtros para campos de registro conectados

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Ahora puede filtrar por determinados tipos de registros que cumplen un criterio de filtro cuando agrega conexiones en Planning.

Solo los registros que cumplan los criterios de filtrado se mostrarán como opciones en los campos conectados.

Para esta función, hemos agregado una nueva opción Reglas de filtrado de registros en la pestaña Nueva conexión al conectar tipos de registros.

Para obtener más información, consulte [Administrar conexiones dependientes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Contraer y expandir todas las agrupaciones en la vista de cronología

>[!NOTE]
>
>Vista previa: 27 de agosto de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Las vistas de cronología ahora incluyen las opciones Contraer todo y Expandir todo para cronologías agrupadas. Esto facilita la navegación por vistas de hoja de ruta grandes: puede reducir rápidamente la vista a encabezados de agrupación y, a continuación, expandir solo las secciones que desee revisar.

Para obtener más información, consulte [Administrar la vista de cronología](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Ver nombres de grupos completos y cambiar el tamaño del panel de agrupación en la vista de cronología

>[!NOTE]
>
>Vista previa: 27 de agosto de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

En la vista de línea de tiempo, al pasar el ratón por encima de una etiqueta de grupo truncada, ahora se muestra el texto completo en una información de objeto, tanto en la visualización de la pista de baño como en la de la agrupación apilada. Las etiquetas no truncadas no muestran información sobre herramientas.

Ahora se puede cambiar el tamaño del panel izquierdo de agrupación en la pantalla de la calle arrastrando su divisor. La vista se actualiza en tiempo real, lo que es coherente con la vista de tabla. La anchura del panel de cada usuario se guarda entre sesiones, con una anchura predeterminada para los usuarios nuevos.

Para obtener más información, consulte [administrar la vista de cronología](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Se ha mejorado el rendimiento del calendario para grandes conjuntos de registros en la vista de semana

>[!NOTE]
>
>Vista previa: 27 de agosto de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

La vista de semana del calendario ahora muestra solo los primeros 1000 registros en el período de semana visible. Si hay más registros, aparece el siguiente mensaje en la parte inferior del calendario que indica que hay registros adicionales disponibles: &quot;Hay más registros. Cargue más&quot;.

Para obtener más información, vea [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Encabezados de columna actualizados para campos de registro conectados dependientes

>[!NOTE]
>
>Vista previa: 20 de agosto de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Se han realizado mejoras visuales en los encabezados de columna de un campo de registro conectado dependiente en la vista de tabla.

Para obtener más información, consulte [Administrar conexiones dependientes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Mejoras en la vista de tabla al arrastrar y soltar varias filas

>[!NOTE]
>
>Vista previa: 13 de agosto de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026
>[!BADGE Fuera del horario]{type=Neutral}

Hay nuevos indicadores visuales cuando arrastra y suelta varias filas en la vista de tabla. Un signo más destacado y un indicador de número ahora muestran cuántas filas se han seleccionado para la acción de arrastrar y soltar.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

## Distribuya el objeto de solicitud enviado al espacio de trabajo correcto cuando utilice tipos de registros globales

>[!NOTE]
>
>Vista previa: 13 de agosto de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Los registros creados para tipos de registros globales al enviar un formulario de solicitud ahora se dirigen automáticamente al espacio de trabajo desde el que se enviaron.

Los registros creados al enviar una solicitud desde un espacio de trabajo secundario de un tipo de registro global se agregan a ese espacio de trabajo secundario. Los registros creados al enviar una solicitud desde el espacio de trabajo original o desde el área de solicitudes principal se agregan al espacio de trabajo original.

Si el formulario de entrada incluye un campo de Workspace y un usuario selecciona un espacio de trabajo antes de enviarlo, la solicitud se dirigirá al espacio de trabajo seleccionado independientemente de dónde se haya iniciado el formulario. Esto garantiza que los registros estén organizados en el espacio de trabajo deseado desde el momento en que se crean.

Para obtener más información, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Presentación de la aptitud de arquitecto de Workfront Planning Solution

>[!NOTE]
>
>Vista previa: 10 de agosto de 2026
>Producción: 10 de agosto de 2026

Estamos lanzando una nueva habilidad, el arquitecto de soluciones de Workfront Planning, que trae una orientación auténtica y de prácticas recomendadas para Workfront Planning directamente a Claude:

* **Configure** nuevos espacios de trabajo de Planning para especificar, con el servidor MCP de Workfront ejecutando la configuración en su entorno.
* **Auditoría** configuraciones existentes para antipatrones a escala.
* **Comprobar el uso** con los límites recomendados (registros, conexiones, profundidad de jerarquía).
* **Formule preguntas** sobre Planning anytime.

Más allá de la configuración inicial, la aptitud admite la gobernanza continua al detectar la deriva de la configuración antes de que cause fricción, marcar los límites que se aproximan antes de que se conviertan en bloqueadores, aplicar estándares coherentes en todos los espacios de trabajo, independientemente de quién lo configure y dar a cualquier miembro del equipo respuestas precisas sin esperar a un especialista. En conjunto, esto cubre el ciclo de vida completo de la configuración correcta de un espacio de trabajo y lo mantiene así a medida que aumenta el uso.

Para obtener más información, consulte [Aptitudes disponibles para la instalación directa](/help/quicksilver/workfront-basics/workfront-mcp-server/direct-skills.md).

## Arrastrar y soltar filas en la vista de tabla

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Se ha mejorado visualmente la experiencia de arrastrar y soltar filas en la vista de tabla.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).


## Campos de registro conectados dependientes

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Los administradores de Workspace ahora pueden definir dependencias entre tipos de registros conectados. Por ejemplo, si se garantiza un campo de Región, solo se muestran los valores vinculados a la Información geográfica seleccionada. Esto se configura directamente en la configuración del campo de conexión: al agregar una conexión desde un tipo de registro geográfico a un tipo de registro dependiente (como Región), una nueva configuración permite a los administradores de espacio de trabajo marcarlo como dependiente del tipo de registro geográfico, utilizando las relaciones ya establecidas entre esos tipos de registro.

Una vez configurado, cualquier tipo de registro que haga referencia a ambos campos (como una campaña) verá el efecto inmediatamente: al seleccionar un valor geográfico, el selector de regiones se reduce a solo las regiones realmente vinculadas a esa región geográfica. Esto aplica la estructura de registros automáticamente, eliminando las combinaciones que no coinciden y reduciendo la limpieza manual.

Esta actualización incluye las siguientes funciones:

* Hemos agregado la nueva sección Configuración de conexión en la pestaña Nueva conexión, al conectar tipos de registro
* Hemos añadido la opción Hacer esta conexión dependiente en la nueva sección
* Hemos cambiado la forma de agregar campos de búsqueda a las conexiones


Para obtener más información, consulte [Administrar conexiones dependientes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).




## Mostrar el nuevo indicador de comentario de un registro en la vista de tabla

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Se ha agregado un nuevo indicador que muestra cuándo hay comentarios no leídos en un registro. El indicador se muestra en la esquina superior derecha del campo principal del registro en la vista de tabla.

Para obtener más información, consulte [Administrar comentarios de registro](/help/quicksilver/planning/records/manage-record-comments.md).

## Color de registro personalizable y codificación de color basada en la conexión

>[!NOTE]
> 
>Vista previa: 23 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Los registros ahora admiten paletas de color personalizables que permiten actualizar los colores asignados automáticamente a los nuevos registros a colores estándar o personalizados.

En esta mejora se incluyen los siguientes cambios: 

* Se ha añadido la opción Color a las siguientes áreas:
  * El icono Campos de la vista de tabla. 
  * La sección Estilo de barra del área Configuración de una vista de cronología y calendario

    Cuando la opción Color está activada, el color asignado a un nuevo registro se muestra en todas partes donde el registro se muestra en estas vistas. 

* Se agrega un círculo de color a la página Detalles del registro. 
* Ahora puede agregar campos de registro de selección única, múltiple y conectada a la codificación de color de las barras en las vistas de cronología y calendario al colorear por valores de campo. 
* Puede habilitar la visualización del color, además del nombre y la imagen de un registro al crear campos de registro conectados. 
* La sección Color del área de Configuración también se ha optimizado eliminando la opción &quot;Ninguno&quot;.  

Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md). 

## La planificación de Designer ahora requiere la aceptación del acuerdo de Beta

>[!NOTE]
>Vista previa y producción para todos los clientes: 20 de julio de 2026
>[!BADGE Fuera del horario]{type=Neutral}

La planificación de Designer ahora requiere un acuerdo de Beta aceptado para su uso. Su empresa no tiene que firmar un acuerdo de IA. Esto está disponible para todos los clientes.

Para ello, hemos trasladado la opción de Planning Designer a la sección Configuración en la sección Inclusión en las pruebas beta de IA.

Al iniciar Planning Designer sin un acuerdo de Beta aceptado, ahora se solicitará la aceptación antes de que se abra el generador de espacios de trabajo.

Para obtener más información, consulte [Introducción a Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).
