---
title: Mejoras del administrador en el tercer trimestre de 2026
description: Mejoras del administrador en el tercer trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 3d8439efd8a92042098fbf995aacf2fe3add43f2
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 4%

---

# Mejoras del administrador en el tercer trimestre de 2026

Esta página describe las mejoras realizadas por el administrador con la versión del tercer trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2026, consulte [Información general de la versión del tercer trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

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
