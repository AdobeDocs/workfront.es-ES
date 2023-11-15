---
title: Resumen de la versión del cuarto trimestre de 2023
description: Resumen de la versión del cuarto trimestre de 2023
author: Becky
feature: Product Announcements
exl-id: 6c14bd61-60b1-49aa-84bd-d494a226d70e
source-git-commit: 63d043a85c2e5300d8b5872b2ec7983de4ba1f50
workflow-type: tm+mt
source-wordcount: '2700'
ht-degree: 0%

---

# Resumen de la versión del cuarto trimestre de 2023

Esta página proporciona información sobre la funcionalidad que se incluye en la versión del cuarto trimestre de 2023. Estas mejoras están planificadas para que estén disponibles en el entorno de producción para todos los clientes con la versión 23.10 del 26 y 27 de octubre de 2023.

<!--
These enhancements will be included in the following releases:

>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>23.8 (August 31, 2023)</li><li>23.9 (September 28, 2023)</li><li>23.10 (October 26, 2023)</li></ul>| <ul><li>23.10 (Week of October 26, 2023)</li></ul>|
-->

El seminario web de la versión 23.10 fue el 5 de octubre de 2023. Puede [regístrese en el seminario web para ver una grabación bajo demanda aquí](https://webinars.on24.com/adobe_workfront/whatsnewin2310?partnerref=releasenotes).

<span class="preview">Las funciones fuera de ciclo (las que se lanzaron a Producción antes de la fecha de lanzamiento del cuarto trimestre de 2023) se resaltan en amarillo.</span>

>[!IMPORTANT]
>
>La versión 23.3 incluía la opción de mover su organización a versiones mensuales. Por lo tanto, Workfront está cambiando el esquema de numeración de versiones para tener en cuenta las versiones mensuales y trimestrales.
>
>* Si está en la **versión rápida (mensual)** seguimiento, la versión posterior a 23.3 es **23,8**, el 31 de agosto de 2023.
> * Si está en la **trimestral** pista de lanzamiento, la versión posterior a 23.3 es **23,10**, en la semana del 26 de octubre de 2023.
> 
> Las versiones trimestrales incluirán la funcionalidad de tres versiones mensuales. Por ejemplo, la versión trimestral 23.10 incluirá la funcionalidad lanzada en las versiones mensuales 23.8, 23.9 y 23.10.
>
>Se ha planificado que las versiones mensuales y trimestrales estén disponibles el último jueves del mes.
>
>| Versión mensual | Versión trimestral |
>|----|----|
>| <ul><li>23.8 (31 de agosto de 2023)</li><li>23.9 (28 de septiembre de 2023)</li><li>23.10 (26 de octubre de 2023)</li></ul> | <ul><li>23.10 (semana del 26 de octubre de 2023)</li></ul> |
>| <ul><li>Sin versión (noviembre de 2023)</li><li>Sin versión (diciembre de 2023)</li><li>24.1 (enero de 2024)</li></ul> | <ul><li>24.1 (enero de 2024)</li></ul> |
>
>Para obtener más información sobre el proceso de liberación rápida, consulte [Habilitar o deshabilitar el proceso de liberación rápida](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Mejoras de Adobe Workfront

* [Mejoras del administrador](#administrator-enhancements)
* [Mejoras de tableros](#boards-enhancements)
* [Mejoras de Financial Management](#financial-management-enhancements)
* [Mejoras de inicio](#home-enhancements)
* [Mejoras de integración](#integration-enhancements)
* [Mejoras del proyecto](#project-enhancements)
* [Otras mejoras](#other-enhancements)

### Mejoras del administrador

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Decisiones de pruebas y documentos disponibles para los clientes del modelo de licencia heredado</a></p><p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Los clientes heredados que aún no han realizado la transición al nuevo modelo de licencia de Adobe Workfront ahora pueden ver en un solo informe los datos con el número de decisiones de prueba/documento por usuario al mes. Estos datos están disponibles cuando se ejecuta un informe de decisiones de usuarios.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 12 de octubre de 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: 12 de octubre de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>            
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Los campos calculados en formularios personalizados ahora pueden utilizar el comodín $$USER</a></p><p>[!BADGE en producción ]{type=Informative}</p>
                        <p>El comodín $$USER ya está disponible en los campos personalizados calculados y en los campos de búsqueda externos del nuevo diseñador de formularios.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 5 de octubre de 2023</p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.10</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Añadir opciones de valor de una API externa a un formulario personalizado</a></p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Un nuevo tipo de campo, <strong>Búsqueda externa</strong>, ahora está disponible en el diseñador de formularios personalizado. Cuando los datos están almacenados en un sistema externo, este tipo de campo le permite cargar opciones desde una API externa y filtrar según otros valores de campo del formulario personalizado.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 14 de septiembre de 2023</p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.9</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Mejoras de tableros

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Subtareas ahora disponibles en los tableros de Adobe Workfront</a></p><p>[!BADGE en producción ]{type=Informative}</p><p>Cuando se agrega una tarjeta conectada a un tablero para una tarea de Workfront, las subtareas existentes se importan en la tarjeta. Además, cuando se crea una subtarea en una tarjeta conectada, se agrega una subtarea a la tarea de Workfront.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 12 de octubre de 2023</p>
                            </li>
                            <li>
                                <p>Producción para acceso anticipado a placas: N/D</p>
                            </li>
                            <li>
                                <p>Producción para versión rápida: N/D</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Mejoras en las asignaciones de usuarios a tableros y tarjetas</a></p><p>[!BADGE en producción ]{type=Informative}</p><p>Ya hay disponibles mejoras que añaden flexibilidad al añadir usuarios a tableros y tarjetas en los tableros de Adobe Workfront.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 21 de agosto de 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: 24 de agosto de 2023</span>
                            </li> 
                       </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Agregar documentos en tarjetas conectadas</a></p><p>[!BADGE en producción ]{type=Informative}</p><p>Ahora puede adjuntar documentos en tarjetas conectadas en los paneles de Adobe Workfront. Cualquier documento que agregue a la tarjeta estará disponible en la ficha Documentos de la tarea o el problema conectado y se admitirán los mismos tipos de archivo en ambas áreas.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 21 de agosto de 2023</p>
                            </li>
                            <li>
                                <p>Producción para tableros Acceso anticipado: 24 de agosto de 2023</p>
                            </li>
                            <li>
                                <p>Producción para versión rápida: N/D</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Documentos disponibles en tarjetas conectadas como de solo lectura</a></p><p>[!BADGE en producción ]{type=Informative}</p><p>Para las tarjetas conectadas en los paneles de Adobe Workfront, ahora puede ver documentos como imágenes y PDF. Puede obtener una vista previa de un documento en el explorador o descargarlo en el equipo. </p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 3 de agosto de 2023</p>
                            </li>
                            <li>
                                <p>Producción para tableros acceso anticipado: 10 de agosto de 2023</p>
                            </li>
                            <li>
                                <p>Producción para versión rápida: N/D</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">La vista de tablero de un proyecto ya está disponible para los problemas</a></p><p>[!BADGE en producción ]{type=Informative}</p><p>Ahora puede acceder a la vista del tablero de una lista de problemas del proyecto. El panel Kanban puede ayudarle a realizar un seguimiento del progreso de los problemas de una manera más visual que verlos en la lista. </p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 3 de agosto de 2023</p>
                            </li>
                            <li>
                                <p>Producción para acceso anticipado a placas: N/D</p>
                            </li>
                             <li>
                                <p>Producción para versión rápida: N/D</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>    
           </tbody>
        </table>

### Mejoras de Financial Management

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Coste efectivo por fecha y tarifas de facturación</a></p><p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Ya están disponibles las tarifas de facturación y los costes efectivos por fecha en los objetos de empresa, usuario y rol de Workfront. Cuando se aplican tasas efectivas por fecha a un proyecto y las horas se registran en las tareas del proyecto, los costos e ingresos se calculan usando las tasas especificadas para cada período de tiempo.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 29 de junio de 2023</p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.10</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Botón Delegar trabajo para widgets de proyecto, tarea y problema</a> </p><p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Característica que se solicita con frecuencia en la página principal antigua, ahora hemos agregado un botón delegado a los widgets Mi trabajo, Mis tareas y Mis problemas para que pueda delegar fácilmente el trabajo cuando esté fuera de la oficina. Tenga en cuenta que la delegación de trabajo debe estar habilitada en el entorno de Workfront para que aparezca el botón.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 12 de octubre de 2023</p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.10</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuevo widget de tableros para nueva página de inicio</a> </p><p>[!BADGE en producción ]{type=Informative}</p>
                        <p>En una nueva adición importante a las opciones de administración de trabajo disponibles en Nueva página de inicio, ahora puede mostrar un tablero en su página de inicio.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 12 de octubre de 2023</p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.10</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nueva página de aterrizaje predeterminada del colaborador: Nueva página de inicio</a>  </p><p>[!BADGE en producción ]{type=Informative}</p>
                        <p>La nueva página de inicio es ahora la página de aterrizaje predeterminada para las cuentas de colaborador/solicitante. Esta nueva página de inicio predeterminada incluye una serie de widgets seleccionados específicamente para permitir a los colaboradores administrar mejor su trabajo de inmediato.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 12 de octubre de 2023</p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.10</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Cambios en el seguimiento de trabajo en la nueva página de inicio </a> </p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>En función de los comentarios de los usuarios, hemos eliminado el filtro de intervalo de tiempo para toda la página y la barra de resumen que contabilizaba las tareas pendientes y completadas. Los widgets Proyecto, Tarea y Problema tienen funciones de filtrado integradas que le permiten personalizar su ámbito de manera individual.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 13 de septiembre de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.9</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuevos botones de acción rápida para el widget Mi trabajo</a> </p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Para ampliar aún más su capacidad de administrar el trabajo directamente desde la nueva página de inicio, se han agregado nuevos botones de acción rápida al widget Mi trabajo.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 13 de septiembre de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.9</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuevas opciones de filtro para Nuevo inicio</a> </p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Ahora hay nuevas opciones de filtro disponibles para el widget Mi trabajo en Nueva página de inicio. Las opciones incluyen filtros para tipos de objeto (tareas, problemas y solicitudes) y estados (no listo, listo para iniciar, trabajando en y completado).</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 17 de agosto de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.8</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Compatibilidad con terminología personalizada para el nuevo inicio</a> </p><p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Para satisfacer mejor las necesidades únicas de las organizaciones, la nueva página de inicio ahora utiliza terminología personalizada para los objetos tal como se definen en las plantillas de diseño de una instancia. Por ejemplo, si los objetos de "Proyecto" se han vuelto a etiquetar como "Campañas" en la instancia de Workfront, el widget Mis proyectos se mostrará como Mis campañas en la nueva página de inicio.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 17 de agosto de 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: 31 de agosto de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Se ha eliminado el botón Probar nueva página de inicio en las cuentas que tienen deshabilitada la nueva página de inicio</a> </p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>El botón Probar nueva página de inicio ya no está presente en las cuentas en las que se ha deshabilitado la nueva página de inicio. El administrador del sistema debe volver a habilitar la nueva página de inicio para que los usuarios individuales puedan utilizar el botón para probar la nueva página de inicio.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 17 de agosto de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.8</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Cambiar al conjunto de widgets predeterminado Nuevo inicio</a> </p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>El widget Tareas pendientes, que requiere permiso para crear tareas, ahora solo está presente en el widget predeterminado para usuarios con los tipos de licencia Estándar, Planificar o Trabajo. Además, el widget se ha eliminado automáticamente de las páginas de inicio de los usuarios con todos los demás tipos de licencias.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 17 de agosto de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para la versión rápida: 17 de agosto de 2023</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: 17 de agosto de 2023</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mejoras en la experiencia al enviar documentos a SharePoint (GraphAPI)</a></p><p>[!BADGE en producción ]{type=Informative}</p><p>Se han realizado algunos cambios para facilitar la localización de carpetas al enviar documentos a las carpetas de SharePoint (GraphAPI)</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 24 de agosto de 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: 31 de agosto de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Actualizaciones a arrastrar y soltar para integraciones de documentos</a></p><p>[!BADGE en producción ]{type=Informative}</p><p>Se han realizado algunas mejoras para aclarar y eliminar los errores de usuario al arrastrar y soltar un archivo en una carpeta vinculada.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 24 de agosto de 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: después de la versión de 23.10</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuevas aprobaciones de documentos</a> </p><p>[!BADGE en producción ]{type=Informative}</p>
                        <p>En esta versión, el proceso de aprobación se ha optimizado tanto para la creación de aprobaciones como para la aprobación/revisión de documentos, además de las nuevas funcionalidades.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 12 de octubre de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.10</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Esta función forma parte de una versión por fases y actualmente solo está disponible para clientes específicos.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Actualizaciones en tiempo real en la lista de tareas</a> </p>
                        <p>[!BADGE en producción]{type=Informative}</p>
                        <p>Las listas de tareas ahora se actualizan en tiempo real. Los cambios realizados en una tarea se actualizan en la lista de tareas, de modo que un usuario que vea la lista de tareas pueda ver el cambio sin actualizar la página.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: N/D<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Producción para todos los clientes: Despliegue gradual, completado el 19 de octubre de 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Diseño actualizado al agregar un problema nuevo a un proyecto</a> </p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Esta actualización se ha anunciado con la versión 23.3.</p>
                        <p>Hemos actualizado el cuadro Nuevo problema que se muestra al enviar un problema nuevo a un proyecto. Ahora, la interfaz coincide con el cuadro Nueva solicitud que se muestra al enviar una nueva solicitud a una cola de solicitudes.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 26 de julio de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.8</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nuevo cálculo dinámico de los campos calculados en los formularios</a></p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Los campos calculados de un formulario adjunto a un objeto ahora se vuelven a calcular dinámicamente en tiempo real cuando se modifican los valores dependientes de cualquier formulario de la página. Esto le permite ver los resultados actualizados sin guardar el formulario.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 17 de agosto de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.8</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Establecer horas planificadas en tareas secundarias recurrentes con tipo de duración simple sin asignaciones</a></p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Hemos realizado un cambio en la forma en que se asignan las horas planificadas a tareas recurrentes sin asignaciones y con un tipo de duración sencillo. Ahora, cuando establece Horas planificadas en una nueva tarea recurrente con un Tipo de duración simple y sin asignaciones, las horas también se asignan a las recurrencias individuales. Antes de este cambio, las horas no se guardaban para repeticiones individuales cuando se quitaba la asignación de las tareas principales.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión preliminar: 17 de agosto de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.8</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Cambios en el menú principal del colaborador</a> </p><p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Para informar mejor a los colaboradores/solicitantes de las funciones disponibles con un tipo de licencia de Workfront de pago, ahora pueden ver todas las opciones disponibles en el menú principal.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: 12 de octubre de 2023</p>
                            </li>
                            <li>
                                <p>Producción para una versión rápida: con la versión 23.10</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Nuevas mejoras en la versión beta de comentarios</a> </p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Las mejoras de la sección Actualizaciones se están poniendo a disposición de los usuarios dentro del periodo de tiempo de la versión del cuarto trimestre de 2023 para la experiencia de comentarios beta. Estas mejoras estarán disponibles en el entorno de producción para todos los clientes con la versión del cuarto trimestre de 2023 (octubre de 2023).</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: Durante el cuarto trimestre de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para versiones rápidas: a partir de la versión 23.8</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10 (a menos que se especifique lo contrario)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Nuevas mejoras en la versión beta de Paneles de lienzo</a> </p>
                        <p>[!BADGE en producción ]{type=Informative}</p>
                        <p>Las mejoras en los paneles de lienzo están disponibles dentro del periodo de tiempo de la versión del cuarto trimestre de 2023 como parte de la versión beta en curso. Estas mejoras estarán disponibles en el entorno de producción para todos los clientes con la versión del cuarto trimestre de 2023 (octubre de 2023).</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: Durante el cuarto trimestre de 2023<br /></p>
                            </li>
                            <li>
                                <p>Producción para versiones rápidas: a partir de la versión 23.8</p>
                            </li>
                            <li>
                                <p>Producción para versión trimestral: con la versión de 23.10 (a menos que se especifique lo contrario)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Actualizaciones de aspecto durante el cuarto trimestre de 2023</a></p><p>[!BADGE en producción ]{type=Informative}</p><p>En el cuarto trimestre de 2023 se realizarán actualizaciones menores del aspecto de varias áreas de la aplicación de Adobe Workfront. Revise las notas de la versión individuales para ver fechas de lanzamiento específicas.</p>
                    </td>
                    <td><p><b>Disponible en estas fechas:</b></p>
                        <ul>
                            <li>
                                <p>Versión de vista previa: Durante el cuarto trimestre de 2023</p>
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

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción en una cadencia distinta a la del calendario de versiones del cuarto trimestre de 2023. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Mejoras de Workfront Scenario Planner

No hay actualizaciones de Scenario Planner en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras de Workfront Proof

No hay actualizaciones de Workfront Proof en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras en Workfront Goals

No hay actualizaciones de Workfront Goals en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Versión de API 17

La versión 17 de la API se publicó el 12 de octubre de 2023. Para la versión 17 de la API, hemos modificado algunos recursos y extremos. Algunos de los cambios admiten nuevas funciones y otros facilitan el uso de la información disponible a través de la API.

Para obtener información sobre novedades y actualizaciones, consulte [Novedades de la versión 17 de la API](/help/quicksilver/wf-api/api/new-api-version-17.md).

Para obtener información sobre las versiones de API, consulte [Versiones de API y programación de asistencia](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Actualizaciones de mantenimiento de Workfront 

Para obtener información sobre las actualizaciones de mantenimiento realizadas durante la versión 22.3, consulte [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Actualizaciones de formación

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, rutas de aprendizaje, vídeos y guías de cada versión del producto de Adobe Workfront. Para obtener más información, consulte la sección &quot;Novedades&quot; de la [Página de Tutorials de Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

### Funcionalidad que se eliminará pronto de Workfront

Las siguientes funciones se eliminarán pronto de Workfront:

#### Obsolescencia de la aplicación móvil Proof con 23.10

La aplicación móvil Proof quedará obsoleta oficialmente con la versión 23.10. La aplicación móvil de Workfront general se ha mejorado con nuevas funciones de corrección (consulte la nota de la versión en Mejoras de Workfront Mobile para obtener más información), y se recomienda a los usuarios que empiecen a utilizarla para revisar el trabajo lo antes posible.

Tenga en cuenta que la aplicación móvil de Workfront requiere un inicio de sesión de Workfront. Los usuarios e invitados externos pueden seguir utilizando la aplicación Proof para trabajos de revisión; sin embargo, ya no es compatible y no estará disponible con la versión 23.10.

#### Secuencias de trabajo eliminados para las cuentas que no se utilizan

En el caso de las cuentas que nunca han creado un flujo de trabajo en los paneles de Adobe Workfront, el área Flujos de trabajo se ha eliminado del panel Tableros al 11 de octubre de 2023. Las cuentas que sí utilizan secuencias de trabajo siguen teniendo acceso a ellas. En futuras versiones se abordará la funcionalidad mejorada de depuración.

<!-- HTML you might need

New table

### add product area name

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

New row for table 

<tr>
  <td>
    <a href="ADD%20LINK">Title</a> New in Preview!
    <p>Body</p>
  </td>
  <td>
    <p><strong>Available on these dates:</strong></p>
    <ul>
      <li>
        <p>Preview release:</p>
      </li>
      <li>
        <p>Production release:</p>
      </li>
    </ul>
  </td>
</tr>


New in preview, prod, and coming soon text

<span style="color: #ff0000;"> New in Preview!</span>
<span style="color: #ff0000;"> New in Production!</span>
<span style="color: #ff0000;"> Coming soon!</span>

Badge for available in Fast Release

[!BADGE In production for Fast Release ]{type=Positive}
[!BADGE In production ]{type=Informative}



Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
