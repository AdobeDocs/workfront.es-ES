---
title: Información general sobre la versión 23.2
description: Información general sobre la versión 23.2
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '1455'
ht-degree: 0%

---


# Resumen de la versión 23.2

Esta página proporciona información sobre las funciones que se incluyen en la versión 23.2 programada para abril de 2023.

Las mejoras de esta página están disponibles en el entorno Vista previa . Esta página se actualizará con mejoras adicionales a medida que la versión 23.2 se acerca a la versión de producción planificada.

Para obtener sugerencias sobre la preparación de la próxima versión, consulte [Preparación para una versión trimestral de Adobe Workfront](/help/quicksilver/product-announcements/product-releases/release-readiness.md).

<!-- The 23.2 release webinar will be held on ___. You can [register for the webinar here](link). -->

<span class="preview">Las funciones fuera de ciclo (las que se lanzaban a Producción antes de la fecha de versión 23.2) se resaltan en amarillo.</span>

## Mejoras de Adobe Workfront

* [Mejoras en el administrador](#administrator-enhancements)
* [Mejoras en Agile](#agile-enhancements)
* [Mejoras en la administración de proyectos](#project-management-enhancements)
* [Mejoras en la administración de recursos](#resource-management-enhancements)
* [Otras mejoras](#other-enhancements)

### Mejoras en el administrador

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Función</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-6.md" class="MCXref xref" xrefformat="{para}">Cambiar el nombre de los pines en la plantilla de diseño</span></a>
                        </span></a><p>Ahora puede cambiar el nombre de los pines en una plantilla de diseño para que sea más significativo para los usuarios, en lugar de usar el nombre predeterminado para la página anclada. Los pines que crean los administradores se muestran para todos los usuarios asignados a la plantilla de diseño y los usuarios no pueden cambiar el nombre de esos pines.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 9 de febrero de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versión de producción: Con la versión 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Mejoras en Agile

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Función</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-20.md" class="MCXref xref" xrefformat="{para}">Registro de horas en tarjetas conectadas en un tablero</a><span style="color: #ff0000;"> Novedades de Vista previa</span></p>
                        <p>Ahora puede registrar horas en tarjetas conectadas, del mismo modo que lo haría en una tarea o problema. Debe tener los permisos correctos para la tarea o el problema para registrar la hora.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 23 de febrero de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versión de producción para la inclusión anticipada: 2 de marzo de 2023 <span style="color: #ff0000;"> Esta función está disponible en Producción en esta fecha solo mediante la opción de inclusión de la función inicial para Workfront Boards.</span></p>
                                <p>Versión de producción para todos los clientes: Con la versión 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
              <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">Personalización de la visualización de campos en una tarjeta</a></p>
                        <p>La personalización ya está disponible para configurar qué campos se muestran en una tarjeta, tanto en la vista completa cuando la tarjeta está abierta como en la vista de tarjeta condensada en el tablero. Cuando desactiva un campo, no se muestra en ninguna de las vistas. También puede activar un campo en la vista completa y ocultarlo de la vista condensada.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 16 de febrero de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versión de producción para la inclusión anticipada: 23 de febrero de 2023 <span style="color: #ff0000;"> Esta función está disponible en Producción en esta fecha solo mediante la opción de inclusión de la función inicial para Workfront Boards.</span></p>
                                <p>Versión de producción para todos los clientes: Con la versión 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">Definir un estado predeterminado para las tarjetas movidas a una columna de tablero</a></p>
                        <p>Ahora puede establecer un estado predeterminado para aplicarlo a las tarjetas movidas a una columna específica; para ello, seleccione un estado personalizado y un estado del sistema en las políticas de columna. Al mover una tarjeta a la columna , Workfront intenta primero aplicar el estado personalizado (por ejemplo, Esperando comentarios). Si el estado personalizado no está disponible para esa tarjeta, Workfront aplicará el estado del sistema en su lugar (por ejemplo, En espera). Además, si el estado de la tarea o problema conectado se cambia al estado personalizado o del sistema establecido en la directiva de columna, la tarjeta se mueve automáticamente a la columna .</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 16 de febrero de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versión de producción para la inclusión anticipada: 23 de febrero de 2023 <span style="color: #ff0000;"> Esta función está disponible en Producción en esta fecha solo mediante la opción de inclusión de la función inicial para Workfront Boards.</span></p>
                                <p>Versión de producción para todos los clientes: Con la versión 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">Colecciones ahora disponibles en Adobe Workfront Boards</a></p>
                        <p>Ahora puede crear colecciones en el panel de tableros. Una colección es un grupo de tableros para colaborar en el trabajo. Una vez que haya asignado un nombre a la colección, puede agregar tableros a la colección mediante un conjunto de plantillas que ofrezcan una configuración predefinida, como los nombres de columna.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 16 de febrero de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versión de producción para la inclusión anticipada: 23 de febrero de 2023 <span style="color: #ff0000;"> Esta función está disponible en Producción en esta fecha solo mediante la opción de inclusión de la función inicial para Workfront Boards.</span></p>
                                <p>Versión de producción para todos los clientes: Con la versión 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-1-jan-23.md" class="MCXref xref" xrefformat="{para}">El campo Estimation de las tarjetas conectadas se asigna al campo Story Points de los objetos Workfront</a></p>
                        <p>El campo Estimation de las tarjetas conectadas en Workfront Boards ahora se asigna al campo Story Points para el objeto Workfront asociado. </p>
                        <p>El nuevo campo Puntos de artículo es un campo de forma libre editable que se puede agregar a una vista de una lista o informe para tareas o problemas. No está vinculado a las horas planificadas ni a las asignaciones de equipo.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 26 de enero de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versión de producción para la inclusión anticipada: Esta función se retrasó y se lanzará el 9 de febrero. <span style="color: #ff0000;">Esta función está disponible en Producción en esta fecha solo mediante la opción de inclusión de la función inicial para Workfront Boards.</span></p>
                                <p>Versión de producción para todos los clientes: Con la versión 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-1-jan-23.md" class="MCXref xref" xrefformat="{para}">Tarjeta de vista previa en la columna de admisión</a></p>
                        <p>Ahora puede hacer clic en una tarjeta conectada en la columna de admisión para ver una versión de solo visualización de su contenido. No se puede editar el contenido de la tarjeta hasta que la tarjeta se mueva de la columna de admisión a otra columna del tablero.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 26 de enero de 2023<br /></p>
                            </li>
                            <li>
                                 <p>Versión de producción para la inclusión anticipada: 2 de febrero de 2023 <span style="color: #ff0000;"> Esta función está disponible en Producción en esta fecha solo mediante la opción de inclusión de la función inicial para Workfront Boards.</span></p>
                                <p>Versión de producción para todos los clientes: Con la versión 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Mejoras en la administración de proyectos

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Función</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">Copiar horas presupuestadas al copiar un proyecto</a>
                        <p>Ahora, tiene la opción de copiar las horas presupuestadas en el área de Presupuestación de Recursos del Caso de Negocio o el Planificador de Recursos cuando copia un proyecto. Antes de esta mejora, las horas presupuestadas para el proyecto no se transferían al proyecto copiado.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 16 de febrero de 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Versión de producción: 2 de marzo de 2023 (fuera de ciclo)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Mejoras en la administración de recursos

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Función</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">Presentación del campo Tiempo de Trabajo para calcular con precisión la capacidad del usuario</a>
                        <p>Para permitir que los administradores de recursos calculen con precisión la disponibilidad de sus usuarios y tengan en cuenta el tiempo que los usuarios dedican al trabajo real relacionado con el proyecto, presentamos el concepto de tiempo de trabajo a Adobe Workfront.</p>
                        <p>Puede definir el valor del campo Tiempo de trabajo para cada usuario, al crear o editar su perfil.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 16 de febrero de 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Versión de producción: 2 de marzo de 2023 (fuera de ciclo)</span></p>
                            </li>
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
                        <p><span class="bold">Función</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-6.md" class="MCXref xref" xrefformat="{para}">Exportar tableros como un solo PDF o como varios archivos de PDF en Adobe Workfront para XD</span></a>
                        </span></a><p>En el complemento Adobe Workfront for XD, ahora puede elegir exportar las mesas de trabajo como un solo archivo de PDF o como varios archivos de PDF.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: N/D<br /></p>
                            </li>
                            <li>
                                 <p>Versión de producción: 6 de febrero de 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-look-and-feel.md" class="MCXref xref" xrefformat="{para}">Actualizaciones de apariencia durante el periodo de tiempo de la versión 23.2</a></p>
                        <p>Se están realizando actualizaciones menores del aspecto de varias áreas de la aplicación Adobe Workfront dentro del periodo de publicación 23.2. Estas mejoras estarán disponibles en el entorno Producción al menos 2 semanas después de su publicación en Vista previa. </p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: a lo largo del intervalo de tiempo de la versión 23.2<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Versión de producción: Un mínimo de 2 semanas después de la publicación en Vista previa (a menos que se especifique lo contrario)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

## Anuncios

### Mejoras de Workfront Fusion

Las nuevas funciones de Workfront Fusion están disponibles en Producción en una cadencia fuera de la programación de versiones 23.2. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Mejoras en el planificador de escenarios de Workfront

En este punto de la versión no hay actualizaciones de Scenario Planner. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras en la prueba de Workfront

No hay actualizaciones de Workfront Proof en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras en los objetivos de Workfront

En este punto de la versión no hay actualizaciones de objetivos de Workfront. Esta área se actualizará cuando haya actualizaciones disponibles.

### Versión de API 15

Para la versión 15 de la API, hemos modificado algunos recursos y extremos. Algunos de los cambios admiten nuevas funciones y otros facilitan el uso de la información disponible a través de la API.

Para obtener información sobre las novedades y las actualizaciones, consulte [Novedades de la versión 15 de la API](/help/quicksilver/wf-api/api/new-api-version-15.md).

Para obtener información sobre las versiones de API, consulte [Programación de versiones y asistencia de API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Actualizaciones de mantenimiento de Workfront 

Para obtener información sobre las actualizaciones de mantenimiento realizadas durante la versión 23.2, consulte [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Actualizaciones de formación

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, las rutas de aprendizaje, los vídeos y las guías para cada versión de producto de Adobe Workfront. Para obtener más información, consulte la [Página de actualizaciones de la versión de capacitación](https://one.workfront.com/s/training-release-updates).

### Funcionalidad que se eliminará próximamente de Workfront

Pronto se eliminará la siguiente funcionalidad de Workfront:

#### **Cambios en la API predeterminada de Workfront**

Para garantizar que las llamadas de API puedan aprovechar la funcionalidad de API de Workfront más actualizada, se está actualizando la API predeterminada. Cuando una llamada de API no especifica una versión de la API, la llamada se realiza a la API predeterminada.

Ahora, la API predeterminada reflejará la versión más reciente de la API. Más adelante, actualizaremos la API predeterminada cada vez que se publique una nueva versión de la API, de modo que las llamadas a la API predeterminada siempre utilizarán la versión más reciente de la API.

Anteriormente, la API predeterminada utilizaba la versión 2.0 de la API de Workfront, que ya no se utilizaba.

Si su organización está utilizando la API predeterminada obsoleta, su administrador de Workfront ha recibido un mensaje del Centro de anuncios con más instrucciones sobre la API predeterminada.

Para obtener más información, consulte [Actualizar integraciones que utilizan versiones de API predeterminadas](/help/quicksilver/wf-api/api/update-default-api-versioning.md).


<!--
<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>  

        -->