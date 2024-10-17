---
title: Información general sobre la versión del tercer trimestre de 2024
description: Esta página proporciona información sobre la funcionalidad que se incluye en la versión del tercer trimestre de 2024. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '1824'
ht-degree: 0%

---

# Información general sobre la versión del tercer trimestre de 2024

Esta página proporciona información sobre la funcionalidad que se incluye en la versión del tercer trimestre de 2024. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.

El seminario web de la versión 24.7 se canceló, pero [puedes ver una demostración en vídeo de las características de la versión 24.7 aquí](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Las características que no están en ciclo de producción (las que se lanzaron a Producción antes de la fecha de lanzamiento del tercer trimestre de 2024) aparecen resaltadas en amarillo.</span>

>[!IMPORTANT]
>
>La versión 23.3 incluía la opción de mover su organización a versiones mensuales. Por lo tanto, Workfront ha cambiado el esquema de numeración de versiones para tener en cuenta las versiones mensuales y trimestrales. El primer número designa el año y el segundo número significa el mes de la versión. Ejemplo: La versión de abril de 2024 es la 24.4.
>
>Las versiones mensuales y trimestrales están planificadas para estar disponibles el jueves de la segunda semana completa del mes, a menos que se especifique lo contrario.
>
>| Versión mensual | Versión trimestral |
>|----|----|
>| <ul><li>24.5 (16 de mayo de 2024)</li><li>24.6 (13 de junio de 2024)</li><li>24.7 (18 de julio de 2024)</li></ul> | <ul><li>24.7 (18 de julio de 2024)</li></ul> |
>
>Para obtener más información sobre el proceso de publicación rápida, consulte [Habilitar o deshabilitar el proceso de publicación rápida](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Mejoras de Adobe Workfront

* [Mejoras del administrador](#administrator-enhancements)
* [Mejoras en la gestión financiera](#financial-management-enhancements)
* [Mejoras de integración](#integration-enhancements)
* [Mejoras del proyecto](#project-enhancements)
* [Mejoras de corrección](#proofing-enhancements)
* [Mejoras en la administración de recursos](#resource-management-enhancements)
* [Otras mejoras](#other-enhancements)

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Ya están disponibles las reglas de negocio</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Los administradores ahora pueden agregar reglas empresariales en el área de Configuración de Workfront.</p>
                        <p>Una regla de negocio permite aplicar la validación a objetos de Workfront e impedir que los usuarios creen, editen o eliminen un objeto cuando se cumplen determinadas condiciones. Las reglas se crean mediante una fórmula similar a los campos calculados en los formularios personalizados.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 4 de julio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 de (18 de julio de 2024)</p>
                            </li>
                        </ul>
                        <p><i>Solo disponible para organizaciones con el nuevo plan Ultimate.</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Diseñador de formularios personalizados disponible en general en Adobe Workfront</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Con la versión 24.7, el diseñador de formularios estará disponible de forma general y se convertirá en la experiencia predeterminada para crear y editar formularios personalizados en Adobe Workfront. Cuando cree un nuevo formulario personalizado o abra un formulario existente, verá el área de trabajo de estilo lienzo del diseñador de formularios.</p>
                        <p>Después de esta versión, ya no tendrá la opción de volver al generador de formularios heredado.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 19 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 de (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Mover objetos entre entornos de Workfront con promoción de entorno</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>La promoción de entornos permite mover objetos de un entorno de Workfront a otro, como de un entorno de zona protegida a un entorno de producción. Puede configurar y probar objetos sin ningún riesgo para los datos y registros de su organización. A continuación, puede mover esos objetos a producción sin tener que volver a configurarlos, lo que ahorra tiempo y esfuerzo.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.6 (13 de junio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Compartir formularios y campos personalizados en el diseñador de formularios personalizados</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Ahora puede compartir formularios personalizados y campos personalizados dentro del nuevo diseñador de formularios. Esto permite una mayor colaboración entre los usuarios en los formularios personalizados.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 6 de junio de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Lanzamiento de producción para todos los clientes: 13 de junio</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Agregar un nuevo campo personalizado desde el área Campos</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Ahora puede agregar un nuevo campo o widget personalizado directamente desde el área Campos de Workfront, sin abrir un formulario personalizado para crear el campo. Esto le permite crear rápidamente campos personalizados reutilizables.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 6 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 de (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Tipo de campo desplegable de selección múltiple disponible en el diseñador de formularios</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Para ayudarle a definir los campos desplegables con mayor facilidad, hemos agregado el campo desplegable Selección múltiple al diseñador de formularios personalizado. Este tipo de campo permite a los usuarios elegir más de una opción en una lista desplegable.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 4 de junio de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: 4 de junio de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Mejoras en la gestión financiera

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Campos de gastos facturables y no facturables disponibles para proyectos y tareas</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Para ayudarle a ver con mayor facilidad los tipos de gastos, los gastos se han separado en gastos facturables y no facturables en proyectos y tareas. Los campos siguientes están disponibles para agregarlos a vistas e informes:</p>
                        <ul>
                            <li><p>Coste de gastos planificados facturables</p></li>
                            <li><p>Costo de gasto no facturable planificado</p></li>
                            <li><p>Costo de gasto real no facturable</p></li>
                            <li><p>Costo de gasto real no facturable</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 10 de mayo de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: 10 de mayo de 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mejoras de Workfront para Experience Manager Assets y Assets Essentials</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Hemos realizado las siguientes mejoras para las integraciones de Workfront para Experience Manager Assets y Assets Essentials:</p>
                        <ul>
                            <li><p>La integración ahora es compatible con GCP como proveedor de servicios en la nube. AWS y Azure eran compatibles anteriormente.</p></li>
                            <li><p>El límite de tamaño para los archivos enviados al Experience Manager a través de la integración de ha aumentado a 30 GB. Anteriormente, el límite era de 5 GB.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 27 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Producción para todos los clientes: con la versión 24.7 de (18 de julio de 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Edite la tarea y emita la fecha y condición de confirmación desde el encabezado o la sección de detalles</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Para facilitar la actualización de tareas y problemas, ahora se han añadido los campos Fecha de confirmación y Condición como opciones para agregar a las secciones Encabezados de tareas y problemas y Detalles en una plantilla de diseño. Los usuarios ahora pueden actualizar estos campos desde el encabezado o la sección Detalles de una página cuando se les asigna a la plantilla de diseño modificada.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 30 de mayo de 2024</p>
                            </li>
                            <li>
                                <p>Producción para lanzamiento rápido: con la versión 24.6 (13 de junio de 2024)</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 de (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Se han agregado asignaciones más relevantes al flujo de trabajo Nueva tarea</a></p>
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
                                <p>Lanzamiento de producción para todos los clientes: por anunciar</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Asignaciones inteligentes más relevantes</a></p>
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
                                <p>Lanzamiento de producción para todos los clientes: por anunciar</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Actualizaciones de seguridad para el Visor de revisiones de escritorio</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>La actualización de seguridad del Visor de pruebas de escritorio de Workfront Proof 2.1.35 proporciona correcciones de errores de seguridad para vulnerabilidades que se han identificado en versiones anteriores.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 4 de julio de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: 4 de julio de 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">Tiempo libre ahora reflejado en el Distribuidor de cargas de trabajo</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Para ajustar sin problemas el trabajo cuando el usuario asignado principal de una tarea tiene tiempo libre programado, el Distribuidor de cargas de trabajo ahora reasigna horas tanto a los usuarios principales como a los secundarios cuando se recalcula la cronología del proyecto.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 6 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 de (18 de julio de 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Cambio de servidor en las guías internas del producto</a></p>
                        <p>En las próximas semanas implementaremos un cambio tecnológico en nuestras guías de producto. Aunque hemos intentado minimizar el impacto de esta transición, algunos usuarios pueden encontrar guías que han visto anteriormente.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Producción para todos los clientes: de forma incremental hasta mediados de agosto de 2024</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">La experiencia unificada de Adobe ya está disponible para más organizaciones de Workfront</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Para permitir que las organizaciones accedan a las ventajas de la experiencia unificada de Adobe, hemos comenzado a ponerla a disposición de los clientes de Workfront existentes. </p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 20 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Producción para clientes especificados: con la versión 24.7 de (18 de julio de 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">El shell unificado de Adobe está disponible en un despliegue gradual. Se incorporarán organizaciones adicionales al Unified Shell de Adobe con las versiones 24.10 y 25.1. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Botón de ayuda eliminado de la barra de navegación principal</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Para unificar la experiencia de los usuarios que no están en Unified Shell, se ha eliminado el botón Ayuda de la barra de navegación principal. Este botón, que no está presente para los usuarios de Unified Shell, estaba vinculado a la documentación de Workfront y era redundante con un botón de Ayuda similar disponible para todos los usuarios en el menú principal.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 6 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 de (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Se ha mejorado la experiencia de usuario para los usuarios con acceso limitado a objetos</a></p>
                        [!BADGE en producción ]{type=Informative}
                        <p>Cuando un usuario no tiene acceso a un objeto, verá "Sin acceso" en cualquier lugar donde aparezca el nombre de ese objeto en Workfront. Esta experiencia mejorada también se aplica a la API de Workfront.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 27 de marzo de 2024</p>
                            </li>
                            <li>
                                <p>Producción para la versión rápida: con la versión 24.5 (16 de mayo de 2024)</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión 24.7 (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Actualizaciones de aspecto durante el tercer trimestre de 2024</a></p>
                        <p>En el tercer trimestre de 2024 se realizarán actualizaciones menores del aspecto de varias áreas de la aplicación de Adobe Workfront. Revise las notas de la versión individuales para ver fechas de lanzamiento específicas.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: Durante el tercer trimestre de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versión de producción: revise las notas de la versión para fechas específicas</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## Anuncios

### Mejoras de Workfront Fusion

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción en una cadencia fuera del calendario de versiones del tercer trimestre de 2024. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

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

Para obtener información sobre las actualizaciones de mantenimiento realizadas durante la versión del tercer trimestre de 2024, consulte [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Actualizaciones de formación

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, rutas de aprendizaje, vídeos y guías de cada versión del producto de Adobe Workfront. Para obtener más información, consulte la sección &quot;Novedades&quot; de la [página de Tutorials de Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=es).
