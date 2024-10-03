---
title: Resumen de la versión del cuarto trimestre de 2024
description: Esta página proporciona información sobre la funcionalidad que se incluye en la versión del cuarto trimestre de 2024. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: 4f7e664123785235179418faa2a630e3c4c1c4d0
workflow-type: tm+mt
source-wordcount: '2017'
ht-degree: 0%

---

# Resumen de la versión del cuarto trimestre de 2024

Esta página proporciona información sobre la funcionalidad que se incluye en la versión del cuarto trimestre de 2024. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.

Las <span class="preview">funciones que no están en ciclo de producción (las que se lanzaron a Producción antes de la fecha de lanzamiento del cuarto trimestre de 2024) aparecen resaltadas en amarillo.</span>

>[!IMPORTANT]
>
>La versión 23.3 incluía la opción de mover su organización a versiones mensuales. Por lo tanto, Workfront ha cambiado el esquema de numeración de versiones para tener en cuenta las versiones mensuales y trimestrales. El primer número designa el año y el segundo número significa el mes de la versión. Ejemplo: La versión de abril de 2024 es la 24.4.
>
>Las versiones mensuales y trimestrales están planificadas para estar disponibles el jueves de la segunda semana completa del mes, a menos que se especifique lo contrario.
>
>| Versión mensual | Versión trimestral |
>|----|----|
>| <ul><li>24.8 (15 de agosto de 2024)</li><li>24.9 (12 de septiembre de 2024)</li><li>24.10 (17 de octubre de 2024)</li></ul> | <ul><li>24.10 (17 de octubre de 2024)</li></ul> |
>
>Tenga en cuenta que, para la versión final de cada trimestre (24.10 este trimestre), los usuarios con la programación de versiones rápidas recibirán la versión un día antes.
>
>Para obtener más información sobre el proceso de publicación rápida, consulte [Habilitar o deshabilitar el proceso de publicación rápida](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Mejoras de Adobe Workfront

* [Mejoras del administrador](#administrator-enhancements)
* [Mejoras en la administración de documentos](#document-management-enhancements)
* [Mejoras de integración](#integration-enhancements)
* [Mejoras de inicio](#home-enhancements)
* [Mejoras del proyecto](#project-enhancements)
* [Mejoras de corrección](#proofing-enhancements)
* [Mejoras de informes y paneles](#report-and-dashboard-enhancements)
* [Otras mejoras](#other-enhancements)
* [Funcionalidad que se eliminará pronto de Workfront](#functionality-soon-to-be-removed-from-workfront)

### Mejoras del administrador

<table>
        <col style="width: 50%;" />
        <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Característica</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Un contador de formularios personalizados muestra el número de campos</a></p>
                        <p>Los formularios personalizados están limitados a 500 campos. En un formulario largo, puede resultar difícil saber cuántos campos hay en el formulario y si se está acercando al límite. Se ha agregado un contador a los formularios personalizados en la parte inferior izquierda. El contador muestra cuántos campos se utilizan en el formulario y siempre está visible a medida que se desplaza por el diseñador de formularios.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 1 de octubre de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión de 24.10 (17 de octubre de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Ahora hay disponible una opción "Seleccionar todo" en las plantillas de diseño</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Para ayudarle a mostrar y ocultar más fácilmente los campos con las plantillas de diseño, se ha agregado la casilla de verificación "Seleccionar todo" a las áreas Información general y Finanzas de la vista Detalles en una plantilla de diseño. Esta opción está disponible cuando ha seleccionado Proyecto, Tarea, Problema, Portfolio o Programa en "Personalizar lo que ven los usuarios".</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 29 de agosto de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versión de producción para todos los clientes: 29 de agosto de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Revertir paquetes de promoción de entorno</a></p>
                        [!BADGE En producción para lanzamiento rápido ]{type=Positive}
                        <p>Para que la promoción del entorno sea más flexible y fácil de usar, hemos habilitado la funcionalidad de reversión. Ahora, puede revertir paquetes en un plazo de 24 horas, lo que le permite restaurar más fácilmente las configuraciones anteriores que se han visto afectadas por un paquete de promoción de entorno.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 29 de agosto de 2024</p>
                            </li>
                            <li>
                                <p>Producción para la versión rápida: con la versión 24.9 (12 de septiembre de 2024)</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión de 24.10 (17 de octubre de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">El botón Diseño del diseñador de formularios personalizados permite dos o tres columnas</a></p>
                        <p>Un botón "Diseño" en el diseñador de formularios personalizado le permite elegir entre un área de trabajo de dos o tres columnas. El diseñador de formularios original utiliza tres columnas y la configuración del campo se muestra en la columna del extremo derecho. Si selecciona dos columnas, la configuración del campo se muestra junto a la biblioteca de campos en la columna del extremo izquierdo.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p><s>Versión de vista previa: 12 de agosto de 2024</s></p>
                            </li>
                            <li>
                                <p>Producción para versión rápida: N/D</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: N/D</p>
                            </li>
                        </ul>
                        <p><i>Esta función se ha eliminado de la vista previa y no se lanzará en futuras versiones.</i></p>
                    </td>
                </tr>
           </tbody>
</table>

### Mejoras en la administración de documentos

>[!IMPORTANT]
>
>Las características enumeradas en **Mejoras en la administración de documentos** forman parte de una versión por fases y solo están disponibles para clientes específicos.

<table>
        <col style="width: 50%;" />
        <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Característica</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Ver el estado de la decisión del documento directamente en la lista de documentos</a></p>
                        <p>Ahora puede ver el estado de decisión de un documento directamente en la lista de documentos.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 3 de octubre de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión de 24.10 (17 de octubre de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Agregue rápidamente revisores y aprobadores anteriores a las nuevas versiones del documento</a></p>
                        <p>Ahora puede agregar rápidamente revisores y aprobadores de versiones de documentos anteriores.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 3 de octubre de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión de 24.10 (17 de octubre de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
</table>

### Mejoras de integración

<table>
        <col style="width: 50%;" />
        <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Característica</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mejoras en la experiencia de inicio de sesión de integración con Outlook</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>La experiencia de inicio de sesión para la integración con Outlook se ha optimizado para que todos los clientes vean el mismo botón para iniciar sesión en Workfront, independientemente de si están habilitados para IMS o no. Los pasos de inicio de sesión siguientes siguen siendo diferentes para las instancias de IMS y no de IMS, pero la página inicial es la misma para todos los usuarios.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 6 de agosto de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Lanzamiento de producción para todos los clientes: 6 de agosto de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
</table>

### Mejoras de inicio

<table>
        <col style="width: 50%;" />
        <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Característica</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Introducción a Prioridades: una experiencia de Workfront más sencilla, ágil e intuitiva para los propietarios de tareas</a></p>
                        <p>Las prioridades mejoran el enfoque y la productividad para ayudar a los clientes a lograr más en menos tiempo.</p>
                        <p>Con Prioridades, puede disfrutar de:</p>
                        <ul>
                        <li>Administre y priorice las tareas diarias: organice su día o semana con navegación consolidada para una mejor claridad</li>
                        <li>Mayor productividad: Acceda al contexto del proyecto y realice las tareas más rápido con menos clics</li>
                        <li>Funciones personalizadas: benefíciese de funciones diseñadas exclusivamente para propietarios de tareas</li>
                        </ul>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 3 de octubre de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión de 24.10 (17 de octubre de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
</table>


### Mejoras del proyecto

<table>
        <col style="width: 50%;" />
        <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Característica</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Se han agregado asignaciones más relevantes al flujo de trabajo Nueva tarea</a></p>
                        [!BADGE En producción para lanzamiento rápido ]{type=Positive}
                        <p>Hemos agregado la misma funcionalidad para asignaciones inteligentes más relevantes al campo Asignaciones en el cuadro Nueva tarea al agregar una tarea a un proyecto y en una lista de tareas de proyecto.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 13 de febrero de 2024</p>
                            </li>
                            <li>
                                <p>Producción para la versión rápida: con la versión 24.5 (16 de mayo de 2024)</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión de 24.10 (17 de octubre de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Asignaciones inteligentes más relevantes</a></p>
                        [!BADGE En producción para lanzamiento rápido ]{type=Positive}
                        <p>Hemos cambiado el algoritmo que utiliza Workfront para calcular y sugerir asignaciones inteligentes para las tareas. El nuevo algoritmo se aplica en las siguientes áreas de Workfront donde asigna una tarea: listas de tareas, el área Asignaciones del encabezado de la tarea, Inicio y el panel Resumen.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 21 de diciembre de 2023</p>
                            </li>
                            <li>
                                <p>Producción para la versión rápida: con la versión 24.5 (16 de mayo de 2024)</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión de 24.10 (17 de octubre de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
</table>

### Mejoras de corrección

<table>
        <col style="width: 50%;" />
        <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Característica</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Copiar/pegar corrección de problemas para el Visor de revisiones de escritorio</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Se ha corregido un problema por el cual el contenido se pegaba incorrectamente en la sección Actualizaciones del Visor de corrección de escritorio.</p>
                        <p>Nueva versión: 2.1.39</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 2 de octubre de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versión de producción para todos los clientes: 2 de octubre de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Corrección de pantalla en blanco para usuarios de Windows del Visor de corrección de escritorio</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Se ha corregido un problema con la nueva versión 2.1.36 del Visor de pruebas de escritorio que provocaba que algunos usuarios de Windows vieran una pantalla en blanco después de abrir el visor. </p>
                        <p>Nueva versión para usuarios de Windows: 2.1.37</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 30 de agosto de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versión de producción para todos los clientes: 30 de agosto de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Actualización de Chromium para el Visor de revisión de escritorio</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Estamos actualizando el Visor de pruebas de escritorio para que admita Chromium 126.0.6478.127, que solucionará los problemas con los elementos de la interfaz de usuario en las pruebas interactivas.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 29 de agosto de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versión de producción para todos los clientes: 29 de agosto de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
</table>

### Mejoras de informes y paneles

<table>
        <col style="width: 50%;" />
        <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Característica</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Fechas de lanzamiento</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront Data Connect está disponible para los nuevos planes</a></p>
                        <p>Workfront Data Connect estará disponible para las organizaciones que tengan uno de los nuevos planes de Workfront. Data Connect permite a las organizaciones acceder a sus datos como un lago de datos seguro y escalable, que se puede analizar y visualizar mediante herramientas de inteligencia empresarial o almacenarse de forma externa. Además, las organizaciones pueden utilizar la conexión de datos para ver análisis de datos que anteriormente no estaban disponibles, como el análisis de tendencias basado en el tiempo, la asignación de variables y el análisis de datos de sistemas externos en combinación con datos de Workfront.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión de 24.10 (17 de octubre de 2024)</p>
                            </li>
                        </ul>
                        <p><i>Solo disponible para organizaciones con uno de los nuevos planes de Adobe Workfront. Data Connect está incluido en el plan Ultimate o se puede adquirir como complemento de los planes Prime y Select.</i></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Resumir proyectos o actualizaciones con un solo clic</a></p>
                        <p>Para facilitar la visualización rápida de los aspectos destacados de un proyecto o de un flujo de actualización, hemos añadido botones de Resumen a esas áreas de Workfront. Ahora puede hacer clic en el botón para generar un resumen en el asistente de IA.</p><p>Anteriormente, los usuarios podían abrir el Ayudante de IA y escribir un mensaje para crear un resumen del proyecto o actualizar el flujo.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 3 de octubre de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión de 24.10 (17 de octubre de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md" class="MCXref xref" xrefformat="{para}">Disponibilidad general de Adobe Workfront Planning</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Workfront Planning está disponible para todos los clientes que adquirieron una licencia de Workfront Planning, además de su licencia de Workfront. Póngase en contacto con el representante de cuentas para obtener más información acerca de Workfront Planning.</p>
                        <p>Para obtener la información más reciente sobre la versión de Workfront Planning cada trimestre, consulte la sección <a href="#workfront-planning-enhancements">Mejoras de Workfront Planning</a> a continuación.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p><span class="preview">Versión de producción para todos los clientes: 28 de agosto de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Asistente de IA de Adobe disponible en Workfront</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Para facilitarle la realización de su trabajo, hemos agregado el asistente de IA de Adobe a Workfront. El asistente de IA puede ayudarle con lo siguiente:</p>
                        <ul>
                            <li>Resumir elementos y documentos de trabajo le permite obtener rápidamente una comprensión general de las tareas, los proyectos y los recursos.</li>
                            <li>Proporcionar información de la documentación del Experience League, incorporar instrucciones y material de referencia a Workfront y, al mismo tiempo, vincularla a documentación más detallada.</li>
                            <li>Crear y refinar fórmulas para campos de formulario personalizados calculados, generar fórmulas a partir de peticiones de texto o localizar errores en fórmulas existentes.</li>
                            </ul>
                            <p>El administrador de Workfront puede habilitar o deshabilitar el Asistente de IA para su organización. El asistente de IA está disponible para instancias con planes Select, Prime y Ultimate.</p>
                        </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 28 de agosto de 2024</p>
                            </li>
                            <li>
                                <p class="preview">Versión de producción: 28 de agosto de 2024</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Actualizaciones de aspecto durante el cuarto trimestre de 2024</a></p>
                        <p>En el cuarto trimestre de 2024 se realizarán actualizaciones menores del aspecto de varias áreas de la aplicación de Adobe Workfront. Revise las notas de la versión individuales para ver fechas de lanzamiento específicas.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: Durante el cuarto trimestre de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versión de producción: revise las notas de la versión para fechas específicas</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                            
           </tbody>
</table>

### Funcionalidad que se eliminará pronto de Workfront

Las siguientes funciones se eliminarán pronto de Workfront:

#### Obsolescencia de la experiencia de inicio heredada con 24.10

La versión 24.10 del Home heredado quedará obsoleta oficialmente. Se recomienda a los usuarios que empiecen a utilizar la nueva página de inicio, que se seguirá mejorando con funciones adicionales antes de que quede obsoleta. Para obtener más información sobre la transición, incluidos consejos sobre lo que los usuarios y administradores pueden hacer para prepararse, consulte la [Guía de obsolescencia de la página principal heredada](/help/quicksilver/product-announcements/announcements/legacy-home-deprecation.md).

## Anuncios

### Mejoras de Workfront Fusion

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción en una cadencia distinta a la del calendario de versiones del cuarto trimestre de 2024. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Mejoras de Workfront Planning

Las nuevas funciones de Workfront Planning están disponibles en el entorno de producción. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión del cuarto trimestre de 2024 de Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md).

### Mejoras de Workfront Scenario Planner

No hay actualizaciones de Scenario Planner en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras de Workfront Proof

No hay actualizaciones de Workfront Proof en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras en Workfront Goals

No hay actualizaciones de Workfront Goals en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Versión de API 18

Para la versión 18 de la API, hemos modificado algunos recursos y extremos. Algunos de los cambios admiten nuevas funciones y otros facilitan el uso de la información disponible a través de la API.

Para obtener información sobre novedades y actualizaciones, consulte [Novedades de la versión 18](/help/quicksilver/wf-api/api/new-api-version-18.md) de la API.

Para obtener información sobre las versiones de API, consulte [Versiones de API y programación de soporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Actualizaciones de mantenimiento de Workfront 

Para obtener información sobre las actualizaciones de mantenimiento realizadas durante la versión del cuarto trimestre de 2024, consulte [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Actualizaciones de formación

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, rutas de aprendizaje, vídeos y guías de cada versión del producto de Adobe Workfront. Para obtener más información, consulte la sección &quot;Novedades&quot; de la [página de Tutorials de Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=es).
