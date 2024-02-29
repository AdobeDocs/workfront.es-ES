---
title: Mejoras del administrador en el segundo trimestre de 2024
description: Mejoras del administrador en el segundo trimestre de 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 980979bcc96739671ea69bdb1387d98c3f39d047
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Mejoras del administrador en el segundo trimestre de 2024

Esta página describe todas las mejoras de administrador realizadas con la versión del segundo trimestre de 2024 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del segundo trimestre de 2024, consulte [Información general sobre la versión del segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## Los campos nativos de Workfront están disponibles en la versión beta de Forms Designer

>[!NOTE]
>
>Versión preliminar: 29 de febrero de 2024; producción para versión rápida: con la versión 24.3 (14 de marzo de 2024); producción para todos los clientes: 24.4 (abril de 2024)

Los campos nativos de Workfront ya están disponibles para que los agregue a sus formularios personalizados. Este nuevo tipo de campo le permite organizar y presentar datos a los usuarios de una manera lógica, sin tener que volver a crear los datos existentes en los campos personalizados.

Después de seleccionar Campo nativo en la lista de campos de formulario personalizados para agregar el campo al diseñador de formularios, puede seleccionar cualquier campo nativo para los objetos del formulario. Por ejemplo, si la lista Tipos de objetos de la parte superior del diseñador de formularios muestra Proyecto, podrá seleccionar campos nativos para proyectos, pero no campos específicos de tareas.

Cuando el formulario personalizado se adjunta a un objeto, el campo se rellena a partir de los datos del objeto. Por ejemplo, el campo Descripción de un formulario personalizado adjunto a un proyecto extraerá la descripción del proyecto. (El campo puede mostrar &quot;N/D&quot; si no hay datos disponibles).

Los campos nativos utilizados en los formularios personalizados están disponibles en la biblioteca de campos del diseñador para su reutilización. También están visibles en el área Configuración > Forms personalizado > Campos para que pueda ver en qué formularios se utilizan.

Esta función solo está disponible en la versión beta de Forms Designer, no en el generador de formularios heredado.

Los artículos del Experience League para esta función se actualizarán el 7 de marzo.

## La asignación de atributos ya está disponible para las organizaciones que han migrado a Adobe IMS

>[!NOTE]
>
>Versión preliminar: 22 de febrero de 2024; producción para todos los clientes: 22 de febrero de 2024

Los administradores del sistema de Workfront ahora pueden configurar la asignación de atributos de usuario para la organización que ha migrado a Adobe IMS. Esto permite que la información del usuario pase a Workfront desde el proveedor de inicio de sesión único (SSO) de la organización, de modo que los datos del usuario no tengan que introducirse tanto en Workfront como en el proveedor de SSO.

Anteriormente, esta funcionalidad solo estaba disponible para organizaciones que aún no se habían incorporado a Adobe IMS.

Para obtener instrucciones sobre la configuración de la asignación de atributos, consulte **Asignar atributos de usuario en la experiencia unificada de Adobe** en el artículo [Asignar atributos de usuario y aprovisionar automáticamente nuevos usuarios](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## La lógica de omisión y la lógica de visualización ya están disponibles en la versión beta de Forms Designer

>[!NOTE]
>
>Versión de vista previa: 8 de febrero de 2024; producción para versión rápida: con la versión 24.2 (15 de febrero de 2024); producción para todos los clientes: por determinar

Ahora puede editar la visualización existente y la lógica de omisión y agregar nueva lógica a los formularios personalizados en la versión beta de Forms Designer. Un generador de lógica fácil de usar le ayuda a definir qué campos mostrar u omitir en función de las selecciones en el formulario.

Los iconos de un campo en el lienzo del diseñador de formularios indican que la lógica está configurada en ese campo o que el campo se utiliza en reglas lógicas configuradas en otros campos.

Para obtener más información, consulte [Agregar lógica de visualización y lógica de omisión con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).