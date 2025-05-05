---
title: Información general sobre la versión del segundo trimestre de 2025
description: Esta página proporciona información sobre la funcionalidad que se incluye en la versión del segundo trimestre de 2025. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9b78a58e-7ced-4b13-8108-40bd36339667
source-git-commit: 7f24186c8803237a6f5116293b3c6a5fd1ea90f6
workflow-type: tm+mt
source-wordcount: '1653'
ht-degree: 25%

---

# Información general sobre la versión del segundo trimestre de 2025

Esta página proporciona información sobre la funcionalidad que se incluye en la versión del segundo trimestre de 2025. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.

<span class="preview">Las características que no están en ciclo de producción (las que se lanzaron a Producción antes de la fecha de lanzamiento del segundo trimestre de 2025) aparecen resaltadas en amarillo.</span>

## Programación de versiones

Las versiones de Workfront están numeradas para tener en cuenta las pistas de versión mensuales y trimestrales. El primer número designa el año y el segundo número significa el mes de la versión. Ejemplo: La versión de abril de 2025 tiene el número 25.4.

Las versiones mensuales y trimestrales están planificadas para estar disponibles el jueves de la segunda semana completa del mes, a menos que se especifique lo contrario.

| Versión mensual | Versión trimestral |
| ----------------- | ----------------- |
| <ul><li>25.2 (13 de febrero de 2025)</li><li>25.3 (13 de marzo de 2025)</li><li>25.4 (10 de abril de 2025)</li></ul> | <ul><li>25.4 (10 de abril de 2025)</li></ul> |

>[!NOTE]
>
>Para la versión final de cada trimestre (25,4 este trimestre), los usuarios con la programación de versiones rápidas recibirán la versión un día antes.
>
>Para obtener más información sobre el proceso de versiones rápidas, consulte [Habilitar o deshabilitar el proceso de versiones rápidas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Mejoras de Adobe Workfront

* [Mejoras en el administrador](#administrator-enhancements)
* [Mejoras en la administración de documentos](#document-management-enhancements)
* [Mejoras en la aplicación móvil](#mobile-enhancements)
* [Mejoras en el proyecto](#project-enhancements)
* [Mejoras en la creación de informes](#reporting-enhacements)
* [Otras mejoras](#other-enhancements)

### Mejoras en el administrador

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mejoras en la lógica de los formularios personalizados</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p>
            <p>El creador de lógica de formularios personalizado tiene una interfaz actualizada para que pueda crear reglas lógicas con mayor libertad. Este nuevo diseño puede adaptarse más fácilmente a tipos de lógica adicionales que se pueden añadir en el futuro.</p><p>Además de las opciones de visualización y de lógica de omisión actuales, también está disponible la lógica de validación.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión preliminar: viernes, 13 de marzo de 2025</li>
                <li>Versión de producción para todos los clientes: con la versión 25.4 (abril de 2025)</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Expresiones agregadas a campos personalizados calculados</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Ahora están disponibles las siguientes expresiones en los campos personalizados calculados de Workfront: ARRAY, FORMAT, SWITCH, SORTASCARRAY, SORTDESCARRAY, ARRAYLENGTH, ARRAYELEMENT y ADDHOUR. Las definiciones y los ejemplos de cada expresión están disponibles en el editor de cálculos y en Experience League.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: sábado, 31 de enero de 2025</li>
                <span class="preview"><li>Versión de producción para todos los clientes: 31 de enero de 2025</li></span>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Mejoras en la administración de documentos

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
<!--    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            New document approval decision buttons available in proofing viewer</a></p>
            <p>The new document approval decision buttons now appear in the proofing viewer. Now, when you create a simple proof and then add approvers and reviewers from the Document summary, they can make their decision directly inside the proofing viewer.</p>
        </td>
        <td>
            <p><b>Available on these dates:</b></p>
            <ul>
                <li>Preview release: April 9, 2025</li>
                <li>Production release for a limited set of customers: With the 25.4 release (April 2025)</li>
            </ul>
        </td>
    </tr>   -->                     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Actualización del visor de corrección de escritorio </a></p>[!BADGE In production &#x200B;]{type=Informative}
            <p>El Visor de corrección de escritorio se ha actualizado a la versión 2.1.45. Esta actualización permite al usuario utilizar
            <ul><li>Versión 35 de Electron</li><li>Chromium versión 134</li><ul></p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión preliminar: viernes, 20 de marzo de 2025</li>
                <span class="preview"><li>Versión de producción para todos los clientes: 20 de marzo de 2025</li></span>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Editar varios documentos a la vez en un informe de documento </a></p>[!BADGE In production &#x200B;]{type=Informative}
            <p>Ahora puede editar varios documentos a la vez en un informe de documento. Puede editar las descripciones y actualizar los formularios personalizados.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 06 de febrero de 2025</li>
                <span class="preview"><li>Versión de producción para todos los clientes: 13 de marzo de 2025</li></span>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Mejoras en la aplicación móvil

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mejoras en las pruebas de la aplicación móvil (solo iOS)</a><p>[!BADGE In production &#x200B;]{type=Informative}</p></p>
            <p>Hay varias mejoras disponibles para la funcionalidad de prueba en la aplicación móvil de Adobe Workfront:
            <ul>
            <li>Ahora puede abrir un archivo de prueba desde la aplicación de correo electrónico móvil, desde un vínculo compartido con usted. Anteriormente, los vínculos de los correos electrónicos no eran compatibles y tenía que acceder a las pruebas desde la aplicación móvil de Workfront.</li>
            <li>Los archivos de prueba multimedia ahora son compatibles con la aplicación móvil.</li>
            </ul>
            </p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión preliminar: N/D</li>
                <span class="preview"><li>Versión de producción para todos los clientes: 12 de marzo de 2025</li> 
            </ul>
            <p><b>Disponible en estos entornos:</b></p>
            <ul>
                <li>Aplicación móvil de iOS</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Mejoras en el proyecto

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Agregar un comentario a los proyectos al editarlos en el cuadro Editar proyecto</a><p>[!BADGE In production &#x200B;]{type=Informative}</p>
            <p>Ahora puede agregar un comentario a un proyecto a medida que lo edita en el cuadro Editar proyecto. También puede agregar un comentario a varios proyectos al mismo tiempo cuando los edita por lotes. Antes de esta actualización, esta funcionalidad no existía al editar proyectos.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 13 de febrero de 2025</li>
                <li>Producción para la versión rápida: con la versión 25.3 (marzo de 2025)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.4 (abril de 2025)</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Mejoras de informes

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Los datos de aprobación y decisión de documentos ya están disponibles en Data Connect</a><p>[!BADGE In production &#x200B;]{type=Informative}</p>
            <p>Ahora puede acceder a los datos para las aprobaciones y decisiones de documentos en Data Connect. Este conjunto de datos vincula las aprobaciones de documentos de las funciones de revisión de Workfront y las aprobaciones Frame.io que se producen en los documentos de Workfront. Ahora podrá ilustrar el tiempo del ciclo, el número de ciclos y los impactos de la cronología para las aprobaciones tardías a través de sus visualizaciones de BI.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión preliminar: miércoles, 25 de marzo de 2025</li>
                <li>Versión de producción para todos los clientes: 25 de marzo de 2025</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">Actualizaciones en el calendario de Workfront</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p>
            <p>Hemos actualizado el aspecto del Workfront Calendar a un diseño moderno que es coherente con otras áreas de Workfront. Existen pequeñas diferencias de funcionalidad con respecto al calendario actual de Workfront, incluido lo siguiente:
            <ul>
            <li>Cómo se agregan elementos ad hoc al calendario</li>
            <li>Cómo crear y cambiar el nombre del calendario</li>
            <li>Las acciones del calendario se han trasladado al menú Más junto al nombre del calendario</li>
            <li>Un nuevo panel lateral para ver la información del calendario</li>
            <li>Y más</li>
            <ul>        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 27 de febrero de 2025</li>
                <li>Esta función se lanzará a producción en tres fases: a partir de la versión 25.4 (10 de abril de 2025) y hasta el 17 de abril de 2024</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Otras mejoras

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Actualización a la nueva versión de suscripción de evento con puntos finales de actualización de versión</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Workfront ahora tiene versiones de suscripciones a eventos. La nueva versión no es un cambio en la API de Workfront, sino un cambio en la funcionalidad de suscripción de evento. Puede cambiar las suscripciones de evento a la nueva versión sin crear un hueco en la suscripción de evento</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <span class="preview"><li>Versión de producción para todos los clientes: 6 de marzo de 2025</li></span>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Representar los cambios del usuario de Adobe Admin Console como "Sistema" en la fuente de actualización de Workfront</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>Ahora, cuando el administrador de Adobe Admin Console realiza un cambio en la información de usuario de un usuario de Workfront, Workfront registra este cambio en la pestaña de actividad del sistema del área de Actualizaciones del usuario como perteneciente al "Sistema". Hace referencia al administrador de Adobe Admin Console.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 23 de enero de 2025</li>
                <li>Producción para la versión rápida: con la versión 25.2 (13 de febrero de 2025)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.4 (abril de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Actualizaciones de aspecto durante el segundo trimestre de 2025</a></p>
            <p>En el segundo trimestre de 2025 se realizarán actualizaciones menores del aspecto de varias áreas de la aplicación de Adobe Workfront. Revise las notas de la versión individuales para ver fechas de lanzamiento específicas.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: Durante el segundo trimestre de 2025</li>
                <span class="preview"><li>Versión de producción: revise las notas de la versión para fechas específicas</li></span>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Funcionalidad que se eliminará pronto de Workfront

Las siguientes funciones se eliminarán pronto de Workfront:

#### Desaprobación de la versión de API 2-15

A medida que mejoramos la plataforma de Workfront, es crucial mantener nuestras API actualizadas. Esto garantiza un rendimiento y seguridad óptimos y admite nuevas funciones. Por lo tanto, estamos desaprobando las versiones 2-15 de la API de Workfront.

* **Septiembre de 2025**: Las versiones de API 2-14, que actualmente no son compatibles, quedarán obsoletas. Después de esta fecha, ya no se podrá acceder a estas versiones.
* **Diciembre de 2025**: La versión 15 de la API quedará obsoleta.

#### Se está eliminando la vista de Agile heredada en un proyecto

La vista de Agile heredada en un proyecto se eliminará de Workfront con la versión 25.3 el 13 de marzo de 2025. Aún podrá ver sus tareas en una vista de Agile en un proyecto haciendo clic en el icono Tableros. Las herramientas Agile heredadas existentes siguen estando disponibles en el área de Equipos.

La siguiente imagen muestra la opción Agile heredada que se eliminará:
![vínculo de vista Agile heredado](assets/project-agile-board-view.png)


#### Desaprobación de Analytics mejorada

Debido a un uso bajo y decreciente, hemos tomado la decisión de dejar de utilizar el producto de Analytics mejorado en la semana del 25 de mayo de 2025.
Recomendamos considerar nuestro producto Data Connect como un reemplazo. Data Connect le permite crear visualizaciones personalizables similares utilizando sus herramientas de inteligencia empresarial preferidas.
Para obtener más información sobre esta desaprobación, consulte la [Guía de desaprobación mejorada de Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).

## Anuncios

### Modernización de interfaces

Estamos actualizando la interfaz a través de Adobe Workfront para mejorar la experiencia del usuario y unificarla con otras aplicaciones de Adobe. Estos cambios se liberan fuera de la programación de versiones estándar. Para obtener una lista de estos cambios, consulte [Modernización de la interfaz](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

### Mejoras de Workfront Fusion

>[!IMPORTANT]
>
>La documentación de Workfront Fusion se ha trasladado a una nueva ubicación. Para obtener información, instrucciones y versiones para Fusion, visite [Documentación de Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/home).
>
>Cada artículo actual de la documentación de Fusion contiene un vínculo al artículo correspondiente en la nueva ubicación. Actualice sus marcadores.
>
>El conjunto actual de documentación de Fusion ya no se actualiza y se eliminará en un futuro próximo.

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción en una cadencia fuera de la programación de versiones estándar. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Mejoras de Workfront Planning

Las nuevas funciones de Workfront Planning están disponibles en el entorno de producción. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión del segundo trimestre de 2025 de Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q2.md).

### Mejoras en el Planificador de escenarios de Workfront

No hay actualizaciones de Scenario Planner en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras de Workfront Proof

No hay actualizaciones de Workfront Proof en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras de Workfront Goals

No hay actualizaciones de Workfront Goals en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Versión 19 de la API

Para la versión 19 de la API, hemos modificado algunos recursos y puntos finales. Algunos de los cambios admiten nuevas funciones y otros facilitan el uso de la información disponible a través de la API.

Para obtener información sobre novedades y actualizaciones, consulte [Novedades de la versión 19 de la API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Para obtener información sobre qué versiones de API son compatibles actualmente, consulte [Versiones de API y programación de soporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Actualizaciones de mantenimiento de Workfront 

Para obtener información sobre las actualizaciones de mantenimiento realizadas durante la versión del segundo trimestre de 2025, consulte [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/es/docs/workfront-known-issues/releases/current-updates).

### Actualizaciones de aprendizaje

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, rutas de aprendizaje, vídeos y guías de cada versión del producto de Adobe Workfront. Para obtener más información, consulte la sección “Novedades” de la [página de tutoriales de Workfront](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/home).
