---
title: Mejoras del administrador en el tercer trimestre de 2026
description: Mejoras del administrador en el tercer trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 34ec779f648db8c3f1a1fe2a76f5b7fda83679a6
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 3%

---

# Mejoras del administrador en el tercer trimestre de 2026

Esta página describe las mejoras realizadas por el administrador con la versión del tercer trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2026, consulte [Información general de la versión del tercer trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Ver el historial de cambios de los objetos de Workfront

>[!NOTE]
>
>Vista previa: 11 de junio de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Para facilitarle la visualización de los cambios que se han producido en una lista central, hemos creado la lista Historial de cambios. Esta lista muestra información como el objeto, la operación y el origen del cambio (como un usuario o el sistema de Workfront).

Anteriormente, los registros de auditoría estaban disponibles, pero no cubrían los objetos.

Para obtener más información, vea [Ver y administrar el historial de cambios](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Nueva preferencia del sistema para convertir portafolios de almacenamiento heredado al almacenamiento en la nube de Adobe

>[!NOTE]
>
>Vista previa: 11 de junio de 2026>Producción para todos: 11 de junio de 2026

Los administradores de Workfront ahora pueden convertir portafolios de almacenamiento heredado al almacenamiento en la nube de Adobe directamente desde Preferencias del sistema. Para convertir portafolios, selecciónelos en el nuevo campo Select portfolios to convert to enterprise storage y guarde la página.

Cuando un portafolio se convierte en almacenamiento en la nube de Adobe:

* Ya no puede mover proyectos que utilicen almacenamiento heredado de Workfront a esta cartera
* Todos los proyectos nuevos creados en esta cartera utilizan el almacenamiento en la nube de Adobe
* Frame.io es el visor de documentos que utilizan el almacenamiento en la nube de Adobe
* Los objetos secundarios que utilizan el almacenamiento heredado de Workfront permanecen en el almacenamiento heredado

Anteriormente, al agregar un proyecto de almacenamiento en la nube de Adobe a una cartera de almacenamiento heredado, esta se convertía automáticamente en almacenamiento en la nube de Adobe.

Para obtener más información, consulte [Configurar las preferencias del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Texto enriquecido reemplazar texto por tipo de campo de formato

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
