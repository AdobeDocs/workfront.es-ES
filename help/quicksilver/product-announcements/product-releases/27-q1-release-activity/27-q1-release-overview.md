---
title: Información general sobre la versión del primer trimestre de 2027
description: Esta página proporciona información sobre la funcionalidad que se incluye en la versión del primer trimestre de 2027. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 3c6235a01af5a18a6ab4b2b80bbdea2c447009aa
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 25%
---

# Información general sobre la versión del primer trimestre de 2027

Esta página proporciona información sobre la funcionalidad que se incluye en la versión del primer trimestre de 2027 programada para enero de 2027.

Las mejoras de esta página están disponibles en el entorno de vista previa. Esta página se actualizará con mejoras adicionales a medida que la versión del primer trimestre de 2027 se aproxime a su versión de producción planificada.

>[!IMPORTANT]
>
>
>Está previsto que las versiones mensuales y trimestrales estén disponibles el jueves de la segunda semana completa del mes, salvo que se especifique lo contrario.
>
>| Versión mensual | Versión trimestral |
>|----|----|
>| <ul><li>2026.11 (12 de noviembre de 2026)</li><li>2026.12 (17 de diciembre de 2026)</li><li>2027.01 (21 de enero de 2027)</li></ul> | <ul><li>2027.01 (21 de enero de 2027)</li></ul> |
>
>Para obtener más información sobre el proceso de versiones rápidas, consulte [Habilitar o deshabilitar el proceso de versiones rápidas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Mejoras de Adobe Workfront

* [Mejoras en el proyecto](#project-enhancements)


### Mejoras en el proyecto

<table>
    <tbody>
        <tr>
            <td><strong>Característica</strong>
            </td>
            <td><strong>Vista previa</strong></td>
            <td><strong>Versión rápida</strong></td>
            <td><strong>Trimestralmente</strong></td>
        </tr>
        <tr>
            <td>
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">Anclar subprocesos a la parte superior de las actualizaciones</a></p>
                <p>Ahora puede fijar los hilos más importantes en la parte superior del área de Actualizaciones en un proyecto, tarea, problema o solicitud para que la información clave permanezca visible para su equipo.</p>
            </td>
            <td><p>15 de octubre de 2026</p></td>
            <td><p>12 de noviembre de 2026</p></td>
            <td><p>21 de enero de 2027</p></td>
        </tr>
    </tbody>
</table>

## Notas de la versión para otras áreas

* [Actividad de la versión de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).
* [Actividad de la versión de Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

En este punto de la versión, no hay actualizaciones de lo siguiente:

* Planificador de escenarios
* Revisión
* Metas

## Actualizaciones del visor de revisión de escritorio

### Versión 2.3.0

>[!NOTE]
>
>Vista previa: 27 de octubre de 2026
>Versión de producción para todos los clientes: 28 de octubre de 2026

El Visor de corrección de escritorio se ha actualizado a la versión 2.3.0. Esta actualización incluye los siguientes cambios:

* Se ha resuelto un problema con las pruebas interactivas por el que, al hacer clic en el vínculo debajo de la captura de pantalla mientras se movía por varias versiones, se abría la página en varias pestañas. El vínculo ahora abre la página en una sola pestaña.

* Se ha actualizado el marco subyacente (Electron) a la última versión, que se ejecuta en la versión 156 de Chrome, para mejorar el rendimiento y la seguridad.

Para obtener información sobre cómo descargar y actualizar el Visor de corrección de escritorio, consulte [Actualizar el Visor de corrección de escritorio](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/use-the-desktop-proofing-viewer/update-the-desktop-proofing-viewer).

## Anuncios

### Obsolescencia de los campos de facturación y tasa de coste heredados en las vistas de lista de funciones del puesto

Con el tiempo, hemos introducido funcionalidades mejoradas de administración de tarifas y experiencias de función de trabajo dedicadas que proporcionan un enfoque más completo y escalable para mantener la información de tarifas. Como resultado, la administración de tasas se está moviendo hacia estas experiencias dedicadas en lugar de flujos de trabajo de administración basados en listas.

Con la versión de enero de 2027, los campos heredados **Facturación por hora** y **Costo por hora** ya no estarán disponibles en la API de Workfront ni en las vistas de lista de funciones, incluidas las configuraciones de filtro/vista/agrupación (referencias directas y columnas calculadas en modo de texto).

Como reemplazo en los informes, puede usar el código de modo de texto recomendado (use `costRates` o `billingRates` según sea necesario):

    &quot;
    displayname=Test
    listdelimiter=&lt;br>
    listmethod=nested(costRates).lists
    type=iterate
    valueexpression=CONCAT({startDate},&quot; - &quot;,{endDate},&quot;: &quot;,{value})
    valueformat=HTML
    &quot;

Para administrar y revisar las tasas de funciones del puesto, utilice las experiencias de administración de tasas dedicadas:

* Acceda y administre las tasas de funciones directamente desde la página Función del puesto > Tasas.
* Utilice los informes de tasas para revisar, analizar e informar sobre la información de tasas en los roles.

No se requiere ninguna acción para prepararse para el cambio. Sin embargo, los administradores que actualmente muestran los campos **Facturación por hora** y **Costo por hora** en las vistas de la lista de roles deben actualizar sus flujos de trabajo para utilizar las experiencias de administración de tarifas recomendadas descritas anteriormente.

Para obtener información sobre las tasas de rol, consulte [Crear y administrar roles](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

-->

### Actualizaciones de aprendizaje

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, rutas de aprendizaje, vídeos y guías de cada versión del producto de Adobe Workfront. Para obtener más información, consulte la sección “Novedades” de la [página de tutoriales de Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=es).
