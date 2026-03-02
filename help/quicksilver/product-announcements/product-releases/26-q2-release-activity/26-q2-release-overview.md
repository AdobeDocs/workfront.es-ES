---
title: Información general sobre la versión del segundo trimestre de 2026
description: Esta página proporciona información sobre la funcionalidad que se incluye en la versión del segundo trimestre de 2026. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7e440fc0-45ad-4f73-ae7e-5374e4ae1480
source-git-commit: 8fdc6d1b72967b2a52295c31cb83d43594817d6f
workflow-type: tm+mt
source-wordcount: '1323'
ht-degree: 41%

---

# Información general sobre la versión del segundo trimestre de 2026

Esta página proporciona información sobre la funcionalidad que se incluye en la versión del segundo trimestre de 2026 programada para abril de 2026.

Las mejoras de esta página están disponibles en el entorno de vista previa. Esta página se actualizará con mejoras adicionales a medida que la versión del segundo trimestre de 2026 se aproxime a su versión de producción planificada.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Está previsto que las versiones mensuales y trimestrales estén disponibles el jueves de la segunda semana completa del mes, salvo que se especifique lo contrario.
>
>| Versión mensual | Versión trimestral |
>|----|----|
>| <ul><li>26.2 (12 de febrero de 2026)</li><li>26.3 (12 de marzo de 2026)</li><li>26.4 (15 de abril de 2026)</li></ul> | <ul><li>26.1 (16 de abril de 2026)</li></ul> |
>
>Tenga en cuenta que, para la versión final de cada trimestre (26.4 este trimestre), los usuarios con la programación de versiones rápidas recibirán la versión un día antes (15 de abril de 2026).
>
>Para obtener más información sobre el proceso de versiones rápidas, consulte [Habilitar o deshabilitar el proceso de versiones rápidas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Mejoras de Adobe Workfront

* [Mejoras en el administrador](#administrator-enhancements)
* [Mejoras de documento](#document-enhancements)
* [Mejoras en los proyectos](#project-enhancements)
* [Mejoras en la creación de informes](#reporting-enhancements)
* [Solicitud de mejoras](#requesting-enhancements)
* [Otras mejoras](#other-enhancements)

### Mejoras en el administrador

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Característica</strong>
        </td>
        <td><strong>Vista previa</strong></td>
        <td><strong>Versión rápida</strong></td>
        <td><strong>Trimestralmente</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Contraer sección de formulario personalizado de forma predeterminada</a><p>De forma predeterminada, todas las secciones de un formulario personalizado se expanden cuando se expande el propio formulario. Una nueva opción del diseñador de formularios personalizado permite marcar una sección para que se contraiga de forma predeterminada cuando un usuario abre el formulario. Esta opción se aplica en el nivel de sección, no en los campos.</p>
        </td>
        <td><p>jueves, 26 de febrero de 2025</p></td>
        <td><p>viernes, 12 de marzo de 2026</p></td>
        <td><p>viernes, 16 de abril de 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">El tipo de campo de texto enriquecido ya está disponible en los formularios personalizados</a><p>El nuevo tipo de campo <b>Texto enriquecido</b> de los formularios personalizados es un editor de texto robusto con opciones de formato como superíndice y subíndice, encabezados y tablas, además de las opciones tradicionales de negrita, cursiva, subrayado, viñetas, numeración, hipervínculos y comillas de bloque. El límite de caracteres sigue siendo de 15 000.</p>
        </td>
        <td><p>viernes, 29 de enero de 2026</p></td>
        <td><p>viernes, 12 de febrero de 2026</p>
            <p>Esta función se eliminó temporalmente del entorno de producción el 13 de febrero de 2026.</p></td>
        <td><p>Por determinar</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Nuevas direcciones IP para notificaciones por correo electrónico de Workfront</a><p></p>
            <p>Estamos actualizando las direcciones IP utilizadas para enviar notificaciones por correo electrónico desde Workfront. Si su organización mantiene una lista de permitidos de correo electrónico o firewall, <b>debe</b> agregar las nuevas direcciones IP a continuación para garantizar el envío continuo de notificaciones de Workfront.</p><p>Estas actualizaciones se aplican a todos los correos electrónicos salientes generados por la aplicación Workfront, incluidas las aprobaciones, los recordatorios, las notificaciones de prueba y otros mensajes del sistema.</p>
            <ul>
            <li>US:
            <ul>
            <li>206.55.149.212</li>
            <li>206.55.149.214</li>
            <li>206.55.149.215</li>
            <li>206.55.149.213</li>
            <li>206.55.149.211</li>
            </ul>
            </li>
            <li>UE: 
            <ul>
            <li>24.110.76.224</li>
            <li>24 110 76 223</li>
            </ul>
            </li>
            </ul> </p>
        </td>
        <td><p>viernes, 15 de enero de 2026</p></td>
        <td><p>viernes, 15 de enero de 2026</p></td>
        <td><p>15 de enero de 2026</p></td>
    <tr>
            </tbody>
        </table>

<!--

### Document enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Feature</strong>
        </td>
        <td><strong>Preview</strong></td>
        <td><strong>Fast release</strong></td>
        <td><strong>Quarterly</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Multi‑stage approval workflows available for unified approvals</a><p></p>
            <p>Multi‑stage approval workflows are now available in unified approvals, helping organizations enforce structured, repeatable approval processes that reflect how work is reviewed in the real world. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Set up and use multi-stage approval workflow templates</a><p></p>
            <p>You can now configure and reuse multi-stage approval workflow templates, making it easier to apply consistent governance across repeatable approval workflows. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
             </tbody>
        </table>   

-->

### Mejoras en los proyectos

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Característica</strong>
        </td>
        <td><strong>Vista previa</strong></td>
        <td><strong>Versión rápida</strong></td>
        <td><strong>Trimestralmente</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}">Se actualizó la experiencia cuando y las tareas de plantilla de asignación única o masiva </a><p>[!BADGE Off schedule]{type=Neutral}</p><p> Hemos actualizado la sección Asignaciones en el cuadro Editar tareas de plantilla al editar tareas de plantilla únicas o editarlas por lotes.  </p>
        </td>
        <td><p>viernes, 05 de febrero de 2026</p></td>
        <td><p>A partir del 5 de febrero de 2026</p></td>
        <td><p>A partir del 5 de febrero de 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Experiencia actualizada al asignar tareas de forma única o masiva </a><p>[!BADGE Off schedule]{type=Neutral}</p><p> Hemos actualizado la sección Asignaciones en el cuadro Editar tareas al editar tareas únicas o editarlas por lotes. </p>
        </td>
        <td><p>martes, 26 de enero de 2026</p></td>
        <td><p>A partir del 5 de febrero de 2026</p></td>
        <td><p>A partir del 5 de febrero de 2026</p></td>
    </tr>
            </tbody>
        </table>

### Mejoras en la creación de informes

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Característica</strong>
        </td>
        <td><strong>Vista previa</strong></td>
        <td><strong>Versión rápida</strong></td>
        <td><strong>Trimestralmente</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Se muestran etiquetas de campo personalizado al generar informes</a><p></p>
            <p>La etiqueta de campo personalizado ahora se muestra antes del nombre del campo y el objeto en las herramientas de creación de informes, lo que le ayuda a localizar los campos con mayor facilidad. Las etiquetas de campo también se muestran al definir filtros, vistas y agrupaciones en listas.</p>
        </td>
        <td><p>jueves, 26 de febrero de 2025</p></td>
        <td><p>viernes, 12 de marzo de 2026</p></td>
        <td><p>viernes, 16 de abril de 2026</p></td>
    </tr>
   <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Carpetas de informe compartibles</a><p></p>
            <p>Ahora puede organizar y compartir informes utilizando carpetas de informes que se pueden compartir. Esta nueva función ayuda a los equipos que administran grandes volúmenes de informes a mantener un control de acceso escalable y coherente.</p>
        </td>
        <td><p>jueves, 26 de febrero de 2025</p></td>
        <td><p>viernes, 12 de marzo de 2026</p></td>
        <td><p>viernes, 16 de abril de 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Etiquetas de fecha mejoradas para agrupaciones de gráficos en paneles de lienzo</a><p></p>
            <p>Los gráficos que agrupan datos por fecha ahora muestran etiquetas de fecha más claras y legibles. Con esta actualización, las etiquetas de fecha se ajustan dinámicamente en función de la opción Agrupar por seleccionada, como día, semana, mes o año, lo que facilita la lectura e interpretación rápida de los gráficos.</p><p>Nota: Paneles de lienzo se encuentra en la versión beta.</p>
        </td>
        <td><p>jueves, 26 de febrero de 2025</p></td>
        <td><p>viernes, 12 de marzo de 2026</p></td>
        <td><p>viernes, 16 de abril de 2026</p></td>
    </tr>
             </tbody>
        </table>

### Solicitud de mejoras

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Característica</strong>
        </td>
        <td><strong>Vista previa</strong></td>
        <td><strong>Versión rápida</strong></td>
        <td><strong>Trimestralmente</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-requests.md" class="MCXref xref" xrefformat="{para}">Se ha actualizado la experiencia para compartir vistas mejoradas</a><p></p>
            <p>En el área Nuevas solicitudes, cuando comparte una vista mejorada con un usuario y le concede permisos de Vista, el usuario puede modificar los elementos de vista y esos cambios se guardan en las preferencias personales del usuario. Ahora tienen la opción de guardar una copia de la vista que incluye sus cambios o restablecer la vista compartida a su configuración original. Además, pueden compartir la vista copiada con otros usuarios. </p>
        </td>
           <td><p>jueves, 26 de febrero de 2025</p></td>
        <td><p>viernes, 12 de marzo de 2026</p></td>
        <td><p>viernes, 16 de abril de 2026</p></td>
 </tr>
            </tbody>
        </table>

### Otras mejoras

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Característica</strong>
        </td>
        <td><strong>Vista previa</strong></td>
        <td><strong>Versión rápida</strong></td>
        <td><strong>Trimestralmente</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience ya está disponible para más organizaciones de Workfront</a><p></p>
            <p>Para que las organizaciones puedan acceder a las ventajas de Adobe Unified Experience, seguimos poniéndola a disposición de los clientes de Workfront existentes.</p>
        </td>
        <td><p>viernes, 11 de diciembre de 2025</p></td>
        <td><p>jueves, 11 de febrero de 2026</p></td>
        <td><p>jueves, 11 de febrero de 2026</p></td>
    </tr>
            </tbody>
        </table>


<!--### Functionality soon to be removed from Workfront-->

<!--

## Interface modernization

We are updating the interface throughout Adobe Workfront to improve the user experience and unify it with other Adobe applications. These changes are released outside the standard release schedule. For a list of these changes, see [Interface Modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

-->

## Notas de la versión para otras áreas

### Mejoras de Workfront Fusion

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción a un ritmo distinto a la de la programación de la versión estándar. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Mejoras en Workfront Planning

Las nuevas funciones de Workfront Planning están disponibles en el entorno de producción. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión del segundo trimestre de 2026 para Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q2.md).

En este punto de la versión, no hay actualizaciones de lo siguiente:

* Planificador de escenarios
* Revisión
* Metas

## Actualizaciones del visor de revisión de escritorio

### Versión 2.1.54

**Versión de producción para todos los clientes: 11 de diciembre de 2025**

El visor de revisión de escritorio se ha actualizado de la versión 2.1.52 a la versión 2.1.54. Esta actualización incluye actualizaciones de las herramientas internas y no afecta a la funcionalidad para el usuario final.

La versión 2.1.53 también incluye cambios en las herramientas internas.

Esta actualización es para Mac y Windows.

## Anuncios

### Ya está disponible la versión de prueba de Workfront Planning

[!BADGE Fuera del horario]{type=Neutral}

>[!NOTE]
>
>* Vista previa y producción para todos: 2 de marzo de 2026
>* Debe aceptar el acuerdo de prueba disponible en su entorno para poder acceder al entorno de prueba de Planning.
>* No es necesario firmar el acuerdo de Adobe AI Agent para utilizar Planning Designer durante el período de prueba.

La versión de prueba de Workfront Planning ya está disponible para todos los clientes de Workfront.

La versión de prueba gratuita ofrece a los clientes de Workfront una licencia de Prime de 60 días para acceder a Workfront Planning a partir del 2 de marzo de 2026. El periodo de prueba finaliza el 1 de mayo de 2026.

La versión de prueba gratuita de Workfront Planning ofrece lo siguiente:

* Un entorno de Planning depurado y con varios espacios de trabajo
* Datos de muestra para que tenga una idea por dónde empezar
* Formación y orientación sobre el producto
* Indicación clara de los hitos durante la configuración que se adaptan a funciones específicas.
* Planning Designer: un asistente con tecnología de IA que puede ayudarle a crear el entorno que desee

Para obtener más información, consulte [Introducción a la versión de prueba gratuita de Adobe Workfront Planning](/help/quicksilver/planning/general/trial-workfront-planning.md).

### Versión 21 de la API

La versión 21 de la API de Workfront se publicó el 23 de octubre de 2025. Para la versión 21 de la API, hemos modificado algunos recursos y puntos finales. Algunos de los cambios admiten nuevas funciones y otros facilitan el uso de la información disponible a través de la API.

>[!IMPORTANT]
>
>Este cambio de versión de API presenta un cambio radical que puede afectar a sus llamadas de API existentes. Esto se debe a que la versión 21 de la API utiliza la versión 2 de Suscripciones a eventos.
>
> Para los campos de selección múltiple, la versión 2 de Suscripciones de eventos siempre envía como una matriz. La versión 1 enviaba una matriz si se seleccionaba más de un valor. Si solo se seleccionaba un valor, se enviaba una cadena.

Para obtener información sobre novedades y actualizaciones, consulte [Novedades de la versión 21 de la API](/help/quicksilver/wf-api/api/new-api-version-21.md).

Para obtener información sobre las versiones de API, consulte [Versiones de API y programación de soporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Otras transiciones de integración de Workfront

Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración de Workfront (Fusion). Como parte de este proceso de transición, las siguientes integraciones dejarán de estar disponibles después del **28 de febrero de 2026**:

* Workfront para G Suite
* Workfront para Jira
* Workfront para Salesforce.

Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Google Workspace.
Para obtener información general sobre la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Actualizaciones de mantenimiento de Workfront

Para obtener información sobre las actualizaciones de mantenimiento realizadas durante la versión del segundo trimestre de 2025, consulte [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=es).

### Actualizaciones de aprendizaje

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, rutas de aprendizaje, vídeos y guías de cada versión del producto de Adobe Workfront. Para obtener más información, consulte la sección “Novedades” de la [página de tutoriales de Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=es).
