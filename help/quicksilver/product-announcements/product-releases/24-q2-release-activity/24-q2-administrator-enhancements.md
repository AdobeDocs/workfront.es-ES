---
title: Mejoras del administrador en el segundo trimestre de 2024
description: Mejoras del administrador en el segundo trimestre de 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 0%

---

# Mejoras del administrador en el segundo trimestre de 2024

Esta página describe todas las mejoras de administrador realizadas con la versión del segundo trimestre de 2024 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del segundo trimestre de 2024, consulte [Información general de la versión del segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## La lógica de visualización y la lógica de omisión ya están disponibles en el modo de vista previa del diseñador de formularios

>[!NOTE]
>
>Versión de vista previa: 28 de marzo de 2024; producción para todos los clientes: 24.4 (11 de abril de 2024)

El diseñador de formularios personalizado beta ahora le permite probar la lógica de visualización y omitir la lógica en el modo de vista previa. Anteriormente, todos los campos se mostraban en la vista previa incluso cuando se aplicaba la lógica.

Para obtener más información sobre la vista previa de un formulario personalizado en el diseñador de formularios, vea [Organizar y obtener una vista previa de un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Las empresas y los usuarios ahora admiten campos de formulario personalizados avanzados

>[!NOTE]
>
>Versión de vista previa: 14 de marzo de 2024; producción para todos los clientes: 24.4 (11 de abril de 2024)

Las funciones de formulario personalizadas avanzadas, como los campos de búsqueda externa y los campos nativos de Workfront, ahora están disponibles al adjuntar un formulario personalizado a una empresa o a un usuario. Las funciones avanzadas están disponibles en las páginas Detalles de la empresa y Detalles del usuario, no en los cuadros de diálogo Editar empresa y Editar usuario. El formulario personalizado debe crearse en el nuevo diseñador de formularios para aprovechar estos tipos de campos.

Para obtener más información acerca de los campos de formulario personalizados, vea [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## La integración de JumpSeat ya está disponible para nuevos tipos de paquetes

>[!NOTE]
>
>Versión preliminar: 26 de febrero de 2024; producción para versión rápida: con la versión 24.3 (14 de marzo de 2024); producción para todos los clientes: 24.4 (11 de abril de 2024)

La integración existente de JumpSeat ya está disponible para las cuentas que utilizan uno de los nuevos tipos de paquete (es decir, Select, Prime o Ultimate). Debe seguir teniendo una suscripción JumpSeat activa para habilitar la integración.

Para obtener más información sobre la integración de JumpSeat, consulte [Configurar la integración de JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Los campos nativos de Workfront están disponibles en la versión beta de Forms Designer

>[!NOTE]
>
>Versión preliminar: 29 de febrero de 2024; producción para versión rápida: con la versión 24.3 (14 de marzo de 2024); producción para todos los clientes: 24.4 (11 de abril de 2024)

Los campos nativos de Workfront ya están disponibles para que los agregue a sus formularios personalizados. Este nuevo tipo de campo le permite organizar y presentar datos a los usuarios de una manera lógica, sin tener que volver a crear los datos existentes en los campos personalizados.

Después de seleccionar Campo nativo en la lista de campos de formulario personalizados para agregar el campo al diseñador de formularios, puede seleccionar cualquier campo nativo para los objetos del formulario. Por ejemplo, si la lista Tipos de objetos de la parte superior del diseñador de formularios muestra Proyecto, podrá seleccionar campos nativos para proyectos, pero no campos específicos de tareas.

Cuando el formulario personalizado se adjunta a un objeto, el campo se rellena a partir de los datos del objeto. Por ejemplo, el campo Descripción de un formulario personalizado adjunto a un proyecto extraerá la descripción del proyecto. (El campo puede mostrar &quot;N/D&quot; si no hay datos disponibles).

Los campos nativos utilizados en los formularios personalizados están disponibles en la biblioteca de campos del diseñador para su reutilización. También están visibles en el área Configuración > Forms personalizado > Campos para que pueda ver en qué formularios se utilizan.

Esta función solo está disponible en la versión beta de Forms Designer, no en el generador de formularios heredado.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Ver una demostración en vídeo de esta característica.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## La asignación de atributos ya está disponible para las organizaciones que han migrado a Adobe IMS

>[!NOTE]
>
>Versión preliminar: 22 de febrero de 2024; producción para todos los clientes: 22 de febrero de 2024

Los administradores del sistema de Workfront ahora pueden configurar la asignación de atributos de usuario para la organización que ha migrado a Adobe IMS. Esto permite que la información del usuario pase a Workfront desde el proveedor de inicio de sesión único (SSO) de la organización, de modo que los datos del usuario no tengan que introducirse tanto en Workfront como en el proveedor de SSO.

Anteriormente, esta funcionalidad solo estaba disponible para organizaciones que aún no se habían incorporado a Adobe IMS.

Para obtener instrucciones sobre cómo configurar la asignación de atributos, consulte [Asignar atributos de usuario en la experiencia unificada de Adobe](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) en el artículo **Asignar atributos de usuario y aprovisionar automáticamente nuevos usuarios**.

## La lógica de omisión y la lógica de visualización ya están disponibles en la versión beta de Forms Designer

>[!NOTE]
>
>Versión preliminar: 8 de febrero de 2024; producción para versión rápida: con la versión 24.2 (15 de febrero de 2024); producción para todos los clientes: 24.4 (11 de abril de 2024)

Ahora puede editar la visualización existente y la lógica de omisión y agregar nueva lógica a los formularios personalizados en la versión beta de Forms Designer. Un generador de lógica fácil de usar le ayuda a definir qué campos mostrar u omitir en función de las selecciones en el formulario.

Los iconos de un campo en el lienzo del diseñador de formularios indican que la lógica está configurada en ese campo o que el campo se utiliza en reglas lógicas configuradas en otros campos.

Para obtener más información, consulte [Agregar lógica de visualización y omitir lógica con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
