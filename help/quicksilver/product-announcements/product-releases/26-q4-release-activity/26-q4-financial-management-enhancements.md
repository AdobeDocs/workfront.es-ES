---
title: Mejoras de gestión financiera del cuarto trimestre de 2026
description: Mejoras de gestión financiera del cuarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 650684e66eb10bf2afacd88038d06a88b3308df4
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 2%
---
# Mejoras de gestión financiera del cuarto trimestre de 2026

Esta página describe las mejoras de Financial Management realizadas con la versión del cuarto trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del cuarto trimestre de 2026, consulte [Información general de la versión del cuarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Mejoras en las tarifas de facturación en las plantillas

>[!NOTE]
>
>Vista previa: 1 de octubre de 2026
>Versión rápida de producción: 14 de octubre de 2026
>Producción para todos: 15 de octubre de 2026

Se han realizado varias actualizaciones en la funcionalidad de tarifas de facturación en una plantilla de proyecto.

### Para clientes con todos los paquetes de Workfront y flujo de trabajo

El área Tasas de las plantillas se ha actualizado a una lista mejorada.

Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Para clientes solo en el paquete Workflow Ultimate

Los atributos de tarifa ya están disponibles para aplicarlos a las tarifas de facturación del rol en la plantilla.

Para obtener más información, consulte [Editar plantillas de proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md#add-more-items-to-a-template) y [Anular tarifas de facturación de rol en el nivel de proyecto](/help/quicksilver/manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

## Mejoras en las tarifas de facturación de la empresa

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Se han realizado varias actualizaciones en la funcionalidad de tarifas de facturación de la empresa.

### Para clientes con todos los paquetes de Workfront y flujo de trabajo

* Hemos actualizado los cuadros de diálogo para agregar y editar las tarifas de facturación de la empresa con un diseño más moderno y coherente con otras áreas de Workfront.
* La configuración &quot;Permitir que las tarifas de facturación en la compañía anulen las tarifas en el nivel de proyecto&quot; agrega correctamente las anulaciones de tarifas cuando se agrega una compañía a un proyecto y los cálculos de ingresos planificados utilizan las tarifas de facturación en la compañía.
* Los usuarios sin acceso a Editar finanzas generales y Editar tarifas de facturación en el nivel de proyecto ya no pueden agregar una compañía a un proyecto.

### Para clientes solo en el paquete Workflow Ultimate

Los atributos de tarifa ya están disponibles para aplicarlos a las tarifas de facturación en la empresa. Las fechas efectivas también se pueden aplicar a las tarifas de la compañía.

NOTA: Los tipos de cambio a nivel de compañía no se han añadido a la jerarquía de tipos de cambio.

Para obtener más información, consulte [Anular tarifas de facturación de rol a nivel de compañía](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md) y [Anular tarifas de facturación a nivel de proyecto con tarifas de facturación a nivel de compañía](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Las jerarquías de atributos ahora permanecen conectadas automáticamente

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026
>Esta función solo está disponible para organizaciones en el paquete Workflow Ultimate.

Al utilizar atributos de tasa como filtros en varias áreas de Workfront, como Asignaciones avanzadas, ahora se aplica una validación adicional al filtrado principal-secundario.

Anteriormente, si se vinculaba un atributo a un padre y dicho padre a un abuelo, el sistema no reconocía automáticamente el atributo original como perteneciente al abuelo también. Ahora, al elegir el atributo de nivel inferior, cada nivel por encima de él se asigna automáticamente.

Para obtener información acerca de los atributos, vea [Definir atributos de tasa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).
