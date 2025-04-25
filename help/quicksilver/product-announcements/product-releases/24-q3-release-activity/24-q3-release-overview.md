---
title: Información general sobre la versión del tercer trimestre de 2024
description: Esta página proporciona información sobre la funcionalidad que se incluye en la versión del tercer trimestre de 2024. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 98%

---

# Información general sobre la versión del tercer trimestre de 2024

Esta página proporciona información sobre la funcionalidad que se incluye en la versión del tercer trimestre de 2024. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.

El seminario web de la versión 24.7 se canceló, pero es posible [ver aquí una demostración en vídeo de las características de la versión 24.7](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Las características que no están en ciclo de producción (aquellas que se lanzaron a producción antes de la fecha de lanzamiento del tercer trimestre de 2024) aparecen resaltadas en amarillo.</span>

>[!IMPORTANT]
>
>La versión 23.3 incluía la opción de pasar su organización a versiones mensuales. Por lo tanto, Workfront ha cambiado el esquema de numeración de versiones para tener en cuenta las versiones mensuales y las trimestrales. El primer número designa el año y el segundo número significa el mes de la versión. Ejemplo: la versión de abril de 2024 es la 24.4.
>
>Está previsto que las versiones mensuales y trimestrales estén disponibles el jueves de la segunda semana completa del mes, salvo que se especifique lo contrario.
>
>| Versión mensual | Versión trimestral |
>|----|----|
>| <ul><li>24.5 (16 de mayo de 2024)</li><li>24.6 (13 de junio de 2024)</li><li>24.7 (18 de julio de 2024)</li></ul> | <ul><li>24.7 (18 de julio de 2024)</li></ul> |
>
>Para obtener más información sobre el proceso de versiones rápidas, consulte [Habilitar o deshabilitar el proceso de versiones rápidas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Mejoras de Adobe Workfront

* [Mejoras en el administrador](#administrator-enhancements)
* [Mejoras de administración financiera](#financial-management-enhancements)
* [Mejoras en la integración](#integration-enhancements)
* [Mejoras en el proyecto](#project-enhancements)
* [Mejoras de revisión](#proofing-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Ya están disponibles las reglas empresariales</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Los administradores ya pueden añadir reglas empresariales en el área de configuración de Workfront.</p>
                        <p>Una regla empresarial permite aplicar la validación a objetos de Workfront e impedir que los usuarios creen, editen o eliminen un objeto cuando se cumplen determinadas condiciones. Las reglas se crean mediante una fórmula similar a los campos calculados en los formularios personalizados.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 4 de julio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 (18 de julio de 2024)</p>
                            </li>
                        </ul>
                        <p><i>Solo está disponible para organizaciones que tengan el nuevo plan Ultimate.</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">El diseñador de formularios personalizados está disponible con carácter general en Adobe Workfront</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Con la versión 24.7, el diseñador de formularios estará disponible de forma general y se convertirá en la experiencia predeterminada de creación y edición de formularios personalizados en Adobe Workfront. Al crear nuevos formularios personalizados o abrir formularios existentes, se verá el área de trabajo de estilo lienzo del diseñador de formularios.</p>
                        <p>Después de esta versión, ya no será posible volver al generador de formularios heredado.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 19 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Mover objetos entre entornos de Workfront con promoción de entorno</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>La promoción de entornos permite mover objetos de un entorno de Workfront a otro, como de un entorno de zona protegida a un entorno de producción. Es posible configurar y probar objetos sin ningún riesgo para los datos y registros de la organización. A continuación, es posible mover esos objetos a producción sin tener que volver a configurarlos, lo que ahorrará tiempo y esfuerzo.</p>
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
                        [!BADGE In production ]{type=Informative}
                        <p>Ya es posible compartir formularios y campos personalizados en el nuevo diseñador de formularios. Esto permitirá una mayor colaboración entre usuarios con los formularios personalizados.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 6 de junio de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Versión de producción para todos los clientes: 13 de junio</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Añadir un nuevo campo personalizado desde el área Campos</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Ya es posible añadir nuevos campos o widgets personalizados directamente desde el área Campos de Workfront, sin abrir formularios personalizados para crear el campo. Esto permitirá crear campos personalizados reutilizables rápidamente.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 6 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Tipo de campo desplegable de selección múltiple disponible en el diseñador de formularios</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Para facilitar la definición de campos desplegables, se añadió el campo desplegable de selección múltiple al diseñador de formularios personalizado. Este tipo de campo permite a los usuarios elegir más de una opción en una lista desplegable.</p>
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

### Mejoras de administración financiera

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Campos de gastos facturables y no facturables disponibles para proyectos y tareas</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Para ayudarle a ver con mayor facilidad los tipos de gastos, los gastos se han separado en gastos facturables y no facturables en proyectos y tareas. Los campos siguientes están disponibles para añadirlos a vistas e informes:</p>
                        <ul>
                            <li><p>Coste de gastos planificados facturables</p></li>
                            <li><p>Coste de gastos planificados no facturables</p></li>
                            <li><p>Coste de gastos reales no facturables</p></li>
                            <li><p>Coste de gastos reales no facturables</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 10 de mayo de 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: 10 de mayo de 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### Mejoras en la integración

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
                        [!BADGE In production ]{type=Informative}
                        <p>Hemos realizado las siguientes mejoras para las integraciones de Workfront para Experience Manager Assets y Assets Essentials:</p>
                        <ul>
                            <li><p>La integración ahora es compatible con GCP como proveedor de servicios en la nube. AWS y Azure eran compatibles anteriormente.</p></li>
                            <li><p>El límite de tamaño para los archivos enviados a Experience Manager a través de la integración ha aumentado a 30 GB. Anteriormente, el límite era de 5 GB.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 27 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Producción para todos los clientes: con la versión 24.7 (18 de julio de 2024)</p>
                            </li>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Editar la tarea y la fecha de compromiso y la condición del problema desde el encabezado o la sección Detalles</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Para facilitar la actualización de tareas y problemas, ahora se han añadido los campos Fecha de confirmación y Condición como opciones para añadir a las secciones Encabezados de tareas y problemas y Detalles en una plantilla de diseño. Los usuarios ahora pueden actualizar estos campos desde el encabezado o la sección Detalles de una página cuando se les asigna a la plantilla de diseño modificada.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 30 de mayo de 2024</p>
                            </li>
                            <li>
                                <p>Producción para lanzamiento rápido: con la versión 24.6 (13 de junio de 2024)</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Se han añadido asignaciones más relevantes al flujo de trabajo Nueva tarea</a></p>
                        [!BADGE In production for Fast Release ]{type=Positive}
                        <p>Hemos añadido la misma funcionalidad para asignaciones inteligentes más relevantes al campo Asignaciones en el cuadro Nueva tarea al añadir una tarea a un proyecto y en una lista de tareas de proyecto.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 13 de febrero de 2024</p>
                            </li>
                            <li>
                                <p>Producción para la versión rápida: con la versión 24.5 (16 de mayo de 2024)</p>
                            </li>
                        </ul>
                    <p><i>Esta función se ha eliminado de la vista previa y de la producción de lanzamiento rápido.</i></p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Asignaciones inteligentes más relevantes</a></p>
                        [!BADGE In production for Fast Release ]{type=Positive}
                        <p>Se ha modificado el algoritmo que utiliza Workfront para calcular y sugerir asignaciones inteligentes para las tareas. El nuevo algoritmo se aplica en las siguientes áreas de Workfront donde asigna una tarea: listas de tareas, el área Asignaciones en el encabezado de la tarea, Inicio y el panel Resumen.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 21 de diciembre de 2023</p>
                            </li>
                            <li>
                                <p>Producción para la versión rápida: con la versión 24.5 (16 de mayo de 2024)</p>
                            </li>
                        </ul>
                    <p><i>Esta función se ha eliminado de la vista previa y de la producción de lanzamiento rápido.</i></p>
                    </td>
                 </tr>
           </tbody>
        </table>

### Mejoras de revisión

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Actualizaciones de seguridad para el Visor de corrección de escritorio</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>La actualización de seguridad del Visor de corrección de escritorio de Workfront Proof 2.1.35 proporciona correcciones de errores de seguridad para vulnerabilidades que se han identificado en versiones anteriores.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 4 de julio de 2024</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">La opción Días libres ahora reflejada en el Distribuidor de cargas de trabajo</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Para ajustar sin problemas el trabajo cuando el principal asignado de una tarea tiene tiempo libre programado, el Distribuidor de cargas de trabajo ahora reasigna horas tanto a los usuarios principales como a los secundarios cuando se recalcula la línea de tiempo del proyecto.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 6 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 (18 de julio de 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Cambio del servidor en las guías internas del producto</a></p>
                        <p>En las próximas semanas implementaremos un cambio tecnológico en nuestras guías internas de producto. Aunque hemos intentado minimizar el impacto de esta transición, es posible que algunos usuarios encuentren guías que habían visto anteriormente.</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience ya está disponible para más organizaciones de Workfront</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Para que las organizaciones puedan acceder a las ventajas de Adobe Unified Experience, hemos comenzado a ponerla a disposición de los clientes de Workfront existentes. </p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 20 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Producción para clientes especificados: con la versión 24.7 (18 de julio de 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">Adobe Unified Shell está disponible en un despliegue gradual. Se incorporarán organizaciones adicionales a Adobe Unified Shell con las versiones 24.10 y 25.1. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Botón Ayuda eliminado de la barra de navegación principal</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Para unificar la experiencia de los usuarios que no están en Unified Shell, se ha quitado el botón Ayuda de la barra de navegación principal. Este botón, que no está presente para los usuarios de Unified Shell, estaba vinculado a la documentación de Workfront y era redundante al haber un botón de Ayuda similar disponible para todos los usuarios en el menú principal.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 6 de junio de 2024</p>
                            </li>
                            <li>
                                <p>Versión de producción para todos los clientes: con la versión 24.7 (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Se ha mejorado la experiencia de usuario para los uspuarios con acceso limitado a objetos</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Cuando un usuario no tenga acceso a un objeto, verá “Sin acceso” en cualquier lugar en que se muestre el nombre de ese objeto en Workfront. Esta experiencia mejorada también se aplica a la API de Workfront.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 27 de marzo de 2024</p>
                            </li>
                            <li>
                                <p>Producción para la versión rápida: con la versión 24.5 (16 de mayo de 2024)</p>
                            </li>
                            <li>
                                <p>Producción para lanzamiento trimestral: con la versión 24.7 (18 de julio de 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Actualizaciones de apariencia durante el periodo de tiempo del tercer trimestre de 2024</a></p>
                        <p>En el tercer trimestre de 2024 se realizarán actualizaciones menores de la apariencia de varias áreas de la aplicación de Adobe Workfront. Revise las notas de la versión individuales para ver fechas de lanzamiento específicas.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: durante el periodo de tiempo del lanzamiento en el tercer trimestre de 2024</p>
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

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción en una cadencia fuera del calendario de lanzamientos del tercer trimestre de 2024. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Mejoras en el Planificador de escenarios de Workfront

No hay actualizaciones de Scenario Planner en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras de Workfront Proof

No hay actualizaciones de Workfront Proof en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras de Workfront Goals

No hay actualizaciones de Workfront Goals en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Versión 18 de la API

Para la versión 18 de la API, hemos modificado algunos recursos y puntos finales. Algunos de los cambios admiten nuevas funciones y otros facilitan el uso de la información disponible a través de la API.

Para obtener más información sobre novedades y actualizaciones, consulte [Novedades de la versión 18 de la API](/help/quicksilver/wf-api/api/new-api-version-18.md).

Para obtener más información sobre las versiones de la API, consulte [Versiones de la API y programación de soporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Actualizaciones de mantenimiento de Workfront 

Para obtener más información sobre las actualizaciones de mantenimiento realizadas durante la versión del tercer trimestre de 2024, consulte [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/en/docs/workfront-known-issues/releases/current-updates).

### Actualizaciones de aprendizaje

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, rutas de aprendizaje, vídeos y guías de cada versión del producto de Adobe Workfront. Para obtener más información, consulte la sección “Novedades” de la [página de tutoriales de Workfront](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home).
