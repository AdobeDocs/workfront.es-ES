---
title: Mejoras del administrador en el tercer trimestre de 2026
description: Mejoras del administrador en el tercer trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '1543'
ht-degree: 5%

---

# Mejoras del administrador en el tercer trimestre de 2026

Esta página describe las mejoras realizadas por el administrador con la versión del tercer trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2026, consulte [Información general de la versión del tercer trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).


## Seguimiento de cambios para revisión y aprobación unificadas

>[!NOTE]
>
>Vista previa: 10 de julio de 2026>Versión rápida de producción: 15 de julio de 2026>Producción para todos: 16 de julio de 2026

La página Historial de cambios de Workfront ahora captura la actividad en los flujos de trabajo unificados de revisión y aprobación, lo que proporciona a los administradores un registro de control completo para los eventos de ciclo vital de revisión y documento.

Ahora se realiza un seguimiento de las acciones de aprobación, fase y participante. Estas acciones pueden incluir:

* Toma de una decisión de aprobación en el visor Frame.io
* Creación o eliminación de una aprobación
* Actualizar un documento, como cambiarle el nombre, moverlo o eliminarlo

Cada entrada incluye los campos rastreados estándar: fecha y hora, operación, nombre de usuario (o &quot;generado por el sistema&quot;) y nombre de objeto. No se incluyen los comentarios del visor de Frame.io.

Esta fase del seguimiento de cambios no incluye eventos MCP. Formarán parte de una versión futura.

Para obtener más información, vea [Ver y administrar el historial de cambios](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

-->

## Nuevos campos de tipo de licencia para los niveles de acceso

>[!NOTE]
>
>Vista previa y producción para todos los clientes: 16 de julio de 2026
>
>[!BADGE Fuera del horario]{type=Neutral}

Hemos realizado los siguientes cambios en el campo del cuadro Nivel de acceso:

* Hemos cambiado el nombre del campo Tipo de licencia en el cuadro Nivel de acceso a Tipo de licencia de flujo de trabajo. No hay cambios en la funcionalidad al volver a etiquetar.\
  Para obtener más información,[consulte Crear y modificar niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Para los clientes que también han adquirido un paquete de Workfront Planning, se ha añadido un nuevo campo Tipo de licencia de planificación para ilustrar la licencia de un usuario en Workfront Planning.
Los clientes que han adquirido el mismo número de licencias de flujo de trabajo y planificación tienen disponibles los siguientes tipos de licencias:

  * Estándar de planificación
  * Colaborador de Planning
  * Ninguno

  >[!NOTE]
  >
  >Puede asignar a los usuarios una combinación mixta de licencias entre flujo de trabajo y Planning, pero el tipo de licencia de Planning no puede ser superior al tipo de licencia de flujo de trabajo.
  >
  >Por ejemplo, no se puede asignar una licencia de Planning Standard a un usuario colaborador de flujo de trabajo. A un usuario con una licencia Workflow Light ahora se le puede otorgar una licencia Standard a Planning y, por lo tanto, administrar espacios de trabajo y su contenido. Anteriormente, solo podían tener acceso de solo vista a los datos de Planning.
  >
  >Los nuevos clientes pueden adquirir licencias de Planning y Workflow en diferentes cantidades y utilizarlas con cualquier combinación. En esta situación, el tipo de licencia de colaborador de Planning no está disponible.
  >
  >Para obtener más información, consulte [Información general sobre el acceso a Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

## Campo de búsqueda interna que reemplaza el tipo de campo de escritura anticipada

>[!NOTE]
>
>Vista previa: 7 de julio de 2026>Versión rápida de producción: 15 de julio de 2026>Producción para todos: 16 de julio de 2026

El nuevo tipo de campo **Búsqueda interna** de los formularios personalizados proporciona filtrado dinámico. Es similar al tipo de campo Escribir delante y permite a los usuarios buscar y seleccionar objetos de Workfront existentes escribiendo parte del nombre. El filtro de la búsqueda interna puede hacer referencia al valor en otro campo del formulario, lo cual no es posible con Typeaheads.

La selección múltiple se admite en búsquedas internas y este tipo de campo también proporciona un rendimiento mejorado para conjuntos de datos grandes. Los siguientes objetos nativos de Workfront son compatibles con las búsquedas internas: proyecto, compañía, grupo, función de trabajo, Portfolio, programa, equipo, plantilla, usuario, tarea, problema, documento y ubicación.

El tipo de campo de búsqueda interna reemplaza al tipo de campo de escritura anticipada. Puede convertir rápidamente los campos de escritura anticipada existentes en búsquedas internas haciendo clic en el botón en las opciones de campo a la derecha. Al realizar la conversión, los datos históricos permanecen en el campo y se utilizan del mismo modo en los informes.

>[!IMPORTANT]
>
>Las integraciones externas, como los escenarios de Workfront Fusion o las automatizaciones basadas en API, pueden hacer referencia a estructuras de campo heredadas y requerir actualizaciones después de la conversión. Debe verificar cualquier integración antes de convertir los campos de escritura anticipada a campos de búsqueda interna.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Lógica de valor predeterminada admitida en los campos de referencia nativos

>[!NOTE]
>
>Vista previa: 7 de julio de 2026>Versión rápida de producción: 15 de julio de 2026>Producción para todos: 16 de julio de 2026
>
>Esta función solo está disponible para organizaciones con los paquetes de flujo de trabajo Prime o Ultimate.

En los formularios personalizados, los campos de referencia nativos ahora permiten agregar una lógica de valor predeterminada.

Este tipo de lógica en campos de referencia nativos solo está disponible en la interfaz de usuario y no en la API de Workfront.

Para obtener más información, consulte [Agregar lógica de valor predeterminada a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) en el artículo [Agregar reglas lógicas a formularios y campos personalizados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

## Actualizaciones del filtrado de campos nativos en formularios personalizados

>[!NOTE]
>
>Vista previa: 7 de julio de 2026>Versión rápida de producción: 15 de julio de 2026>Producción para todos: 16 de julio de 2026

Los filtros del sistema que existen en los campos nativos ahora se aplican a los campos de los formularios personalizados y son visibles para los administradores.

Cuando se agrega un campo de referencia nativo que tiene aplicado un filtro del sistema, se puede aplicar el mismo filtro al campo en el formulario personalizado y modificar el filtro si es necesario en el cuadro Modo de texto.

Si agrega su propio filtro personalizado al campo, se anulará el filtro del sistema del campo. Si no introduce un filtro personalizado, el filtro del sistema se aplica de forma predeterminada.

Además, el filtrado dinámico ya está disponible en los campos de referencia nativos. Un filtro dinámico permite reducir la lista de elementos en función del valor de otro campo.

Por ejemplo, cuando se usa `?portfolioID={portfolio}.{ID}` en un filtro de campo de proyecto y un campo nativo de Portfolio está en el formulario personalizado, el campo Proyecto muestra únicamente los proyectos que se encuentran en el portafolio seleccionado. Si el campo Portfolio se deja en blanco, todos los proyectos estarán disponibles en el campo Proyecto.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Proteger los nombres de campo de un cambio de nombre accidental

>[!NOTE]
>
>Vista previa: 7 de julio de 2026>Versión rápida de producción: 15 de julio de 2026>Producción para todos: 16 de julio de 2026

Para proteger las integraciones y la integridad de los datos, hemos actualizado cómo se pueden editar los nombres de campo en el panel de configuración de campo de un formulario personalizado.

Los nombres de campo del panel de configuración de campo ahora son de solo lectura de forma predeterminada. Puede seguir editando el nombre del campo, pero el cambio de nombre requiere un paso de confirmación explícito. El campo anteriormente llamado **Name** también se ha actualizado a **API Name** para reflejar mejor su relevancia técnica. El campo **Etiqueta** permanece editable.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

## Ver el historial de cambios de los objetos de Workfront

>[!NOTE]
>
>Vista previa: 11 de junio de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Para facilitarle la visualización de los cambios que se han producido en una lista central, hemos creado la lista Historial de cambios. Esta lista muestra información como el objeto, la operación y el origen del cambio (como un usuario o el sistema de Workfront).

Anteriormente, los registros de auditoría estaban disponibles, pero no cubrían los objetos.

Para obtener más información, vea [Ver y administrar el historial de cambios](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Nueva preferencia del sistema para convertir portafolios de almacenamiento heredado al almacenamiento en la nube de Adobe

>[!NOTE]
>
>Vista previa: 11 de junio de 2026>Producción para todos: 11 de junio de 2026>[!BADGE Fuera de horario]{type=Neutral}

Los administradores de Workfront ahora pueden convertir portafolios de almacenamiento heredado al almacenamiento en la nube de Adobe directamente desde Preferencias del sistema. Para convertir portafolios, selecciónelos en el nuevo campo Select portfolios to convert to enterprise storage y guarde la página.

Cuando un portafolio se convierte en almacenamiento en la nube de Adobe:

* Ya no puede mover proyectos que utilicen el almacenamiento de Workfront heredado a este portafolio
* Todos los nuevos proyectos creados en este portafolio utilizan el almacenamiento en la nube de Adobe
* Frame.io es el visor de documentos que utilizan el almacenamiento en la nube de Adobe
* Los objetos secundarios que utilizan el almacenamiento heredado de Workfront permanecen en el almacenamiento heredado

Anteriormente, al agregar un proyecto de almacenamiento en la nube de Adobe a una cartera de almacenamiento heredado, esta se convertía automáticamente en almacenamiento en la nube de Adobe.

Para obtener más información, consulte [Configurar las preferencias del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Texto se sustitución enriquecido con tipo de campo de formato

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

El nuevo tipo de campo **Texto enriquecido** de los formularios personalizados es un editor de texto robusto con opciones de formato como superíndice y subíndice, encabezados y tablas, además de las opciones tradicionales de negrita, cursiva, subrayado, viñetas, numeración, hipervínculos y comillas de bloque. El límite de caracteres sigue siendo de 15 000.

El tipo de campo Texto enriquecido reemplaza el tipo de campo Texto con formato. Puede convertir rápidamente el texto existente con campos de formato a texto enriquecido haciendo clic en el botón de las opciones de campo a la derecha. Al realizar la conversión, los datos históricos permanecen en el campo y se utilizan del mismo modo en los informes.

>[!IMPORTANT]
>
>Las integraciones externas, como los escenarios de Workfront Fusion o las automatizaciones basadas en API, pueden hacer referencia a estructuras de campo heredadas y requerir actualizaciones después de la conversión. Debe verificar cualquier integración antes de convertir los campos a texto enriquecido.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campos financieros nativos admitidos en los formularios personalizados

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Ahora puede incluir campos financieros nativos de Workfront en formularios personalizados. Anteriormente, los campos financieros no eran compatibles.

Los campos financieros disponibles a los que se puede hacer referencia dependen del tipo de formulario.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Los formularios personalizados se pueden compartir en todo el sistema con acceso para adjuntarlos

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Se ha agregado una nueva opción de uso compartido, &quot;Todas las personas del sistema pueden ver y adjuntar&quot;, a los formularios personalizados. Al seleccionar esta opción, todos los usuarios de todo el sistema pueden adjuntar el formulario a otros objetos.

Al compartir en todo el sistema, se elimina la necesidad de compartir manualmente formularios y actualizar los permisos entre grupos u agencias cuando se agregan nuevos grupos.

Para obtener más información, consulte [Compartir un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Nueva preferencia del sistema para aplicar campos obligatorios en la edición por lotes

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Actualmente, cuando se editan objetos por lotes, los campos obligatorios solo se aplican cuando un usuario modifica el campo. Si un campo no se modifica, se trata como opcional y no se valida.

Una nueva preferencia del sistema ahora le permite aplicar los campos obligatorios en la edición masiva. Para no permitir que se guarden objetos editados en lotes a menos que todos los campos obligatorios tengan valores, seleccione la opción **Aplicar siempre los campos obligatorios en la edición en lotes** en la página Configuración > Sistema > Preferencias.

Para obtener más información, consulte [Configurar las preferencias del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
