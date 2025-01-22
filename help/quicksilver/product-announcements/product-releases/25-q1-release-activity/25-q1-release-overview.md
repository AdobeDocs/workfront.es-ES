---
title: Información general sobre la versión del primer trimestre de 2025
description: En esta página se ofrece información sobre la funcionalidad incluida en la versión del primer trimestre de 2025. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5bb898fa-d74e-4174-bc93-d8ffb8937680
source-git-commit: 552e97c427e618f299b55a2eab5868c7b90a4156
workflow-type: tm+mt
source-wordcount: '2782'
ht-degree: 39%

---

# Información general sobre la versión del primer trimestre de 2025

En esta página se ofrece información sobre la funcionalidad incluida en la versión del primer trimestre de 2025. Se prevé que estas mejoras estén disponibles en el entorno de producción durante todo el trimestre.

<span class="preview">Las características que no están en ciclo de producción (las que se lanzaron a Producción antes de la fecha de la versión del primer trimestre de 2025) aparecen resaltadas en amarillo.</span>

>[!IMPORTANT]
>
>La versión 23.3 incluía la opción de pasar su organización a versiones mensuales. Por lo tanto, Workfront ha cambiado el esquema de numeración de versiones para tener en cuenta las versiones mensuales y las trimestrales. El primer número designa el año y el segundo número significa el mes de la versión. Ejemplo: la versión de abril de 2025 es la 25.4.
>
>Está previsto que las versiones mensuales y trimestrales estén disponibles el jueves de la segunda semana completa del mes, salvo que se especifique lo contrario.
>
>| Versión mensual | Versión trimestral |
>|----|----|
>| <ul><li>24.11 (14 de noviembre de 2024)</li><li>24.12 (12 de diciembre de 2024)</li><li>25.1 (15 de enero de 2025)</li></ul> | <ul><li>25.1 (16 de enero de 2025)</li></ul> |
>
>Tenga en cuenta que, para la versión final de cada trimestre (25.1 este trimestre), los usuarios de la programación de versiones rápidas recibirán la versión un día antes.
>
>Para obtener más información sobre el proceso de versiones rápidas, consulte [Habilitar o deshabilitar el proceso de versiones rápidas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Mejoras de Adobe Workfront

* [Mejoras en el administrador](#administrator-enhancements)
* [Mejoras de paneles](#boards-enhancements)
* [Mejoras en la administración de documentos](#document-management-enhancements)
* [Mejoras de prioridades](#priorities-enhancements)
* [Mejoras en el proyecto](#project-enhancements)
* [Mejoras de revisión](#proofing-enhancements)
* [Mejoras de informes y paneles](#report-and-dashboard-enhancements)
* [Actualizar mejoras del flujo](#update-stream-enhancements)
* [Otras mejoras](#other-enhancements)

### Mejoras en el administrador

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Función</span></p>
        </td>
        <td>
            <p><span class="bold">Fechas de lanzamiento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
           Ahora se admiten reglas de negocio para más objetos</a></p>
           [!BADGE In production ]{type=Informative}
            <p>Ahora puede crear reglas de negocio y aplicar la validación a estos objetos adicionales: compañía, iteración, categoría de recurso no laboral, rol, usuario, asignación, conjunto de recursos, tiempo libre, documento y hora.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: miércoles, 16 de enero de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
           Comparar objetos entre entornos para la promoción de entornos</a></p>
           [!BADGE In production ]{type=Informative}
            <p>Para facilitar la determinación de qué objeto debe incluirse en un paquete de promoción de entorno, se ha añadido la capacidad de comparar objetos entre entornos. A continuación, puede añadir objetos a un paquete directamente desde esta comparación.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión preliminar: 3 de enero de 2023</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Más objetos disponibles para la promoción del entorno</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Para ampliar las capacidades de la funcionalidad de promoción del entorno, hemos agregado más objetos.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión preliminar: 3 de enero de 2023</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>  
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Impedir mover tareas cuando hay horas registradas</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Debido a que mover tareas o problemas que han registrado horas a veces puede causar problemas de cumplimiento o auditoría, hemos agregado una preferencia en el área de Preferencias de tarea y problemas de la Configuración que le permite evitar que los usuarios muevan tareas y problemas si hay horas registradas en ellos.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 19 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Preferencia para utilizar la programación de proyecto o de usuario para tareas de asignación única</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Como administrador de sistemas o de grupos, ahora tiene una nueva preferencia que indica si Workfront debe utilizar la programación del proyecto o la del usuario para calcular la escala de tiempo del proyecto cuando asigna un usuario a una tarea y tanto el proyecto como el usuario están asociados a una programación.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 21 de noviembre de 2024</li>
                <li>Producción para la versión rápida: con la versión de 24.12 (12 de diciembre de 2024)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Las reglas empresariales ahora admiten hipervínculos</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Ahora puede incluir hipervínculos en el mensaje de error personalizado de una regla de negocio para guiar al usuario sobre cómo modificar su acción dentro de la restricción de la regla. La URL estática podría vincularse a la documentación u otras páginas que resultarían útiles para el usuario.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 21 de noviembre de 2024</li>
                <li>Producción para la versión rápida: con la versión de 24.12 (12 de diciembre de 2024)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ya está disponible el filtrado en los campos de escritura anticipada nativos</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Cuando se agrega una referencia de campo nativo a un formulario personalizado y hace referencia a un campo de escritura anticipada (como Portfolio, Empresa o Propietario), ahora está disponible una opción de filtro. El filtro permite limitar los objetos que los usuarios pueden elegir cuando utilizan el campo. Este filtro personalizado funciona igual que un filtro en un campo de escritura anticipada personalizado, utilizando el modo de texto para definir el filtro.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 21 de noviembre de 2024</li>
                <li>Producción para la versión rápida: con la versión de 24.12 (12 de diciembre de 2024)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Icono "Mover a" añadido a los campos personalizados</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Cuando un formulario personalizado contiene varias secciones con muchos campos, puede resultar difícil mover un campo de una sección a otra arrastrando y soltando. Se ha agregado un icono "mover a" a cada campo, que le permite seleccionar la sección en la que se coloca el campo.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión preliminar: miércoles, 29 de octubre de 2024</li>
                <li>Producción para la versión rápida: con la versión de 24.11 (14 de noviembre de 2024)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Mejoras de paneles

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Función</span></p>
        </td>
        <td>
            <p><span class="bold">Fechas de lanzamiento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Cambiar el propietario de un tablero</a></p>
            [!BADGE In production ]{type=Informative}
            <p>El creador de un tablero es el propietario de forma predeterminada. El propietario del tablero es la única persona que puede eliminar ese tablero o actualizar sus filtros en el panel Configurar.</p>
            <p>Se ha agregado funcionalidad para permitir que los administradores del sistema de Workfront cambien el propietario de un tablero. El propietario actual de un tablero también puede cambiar el propietario de ese tablero específico. Esta funcionalidad está disponible en tableros básicos, retrospectivos y Kanban, pero no en tableros dinámicos.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: jueves, 18 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
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
    <tr>
        <td>
            <p><span class="bold">Función</span></p>
        </td>
        <td>
            <p><span class="bold">Fechas de lanzamiento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Editar varios documentos a la vez</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Ahora puede editar varios documentos a la vez. Puede editar las descripciones y actualizar los formularios personalizados.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 21 de noviembre de 2024</li>
                <li>Producción para la versión rápida: con la versión de 24.12 (12 de diciembre de 2024)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nuevo estado Retirado disponible para aprobaciones de versiones de documentos</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Cuando se agrega una nueva versión a un documento con aprobaciones pendientes, la aprobación de la versión anterior ahora se mostrará como "Retirada", lo que indica que el proceso de aprobación anterior se ha cerrado debido a que se está agregando la nueva versión.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 07 de noviembre de 2024</li>
                <li>Producción para la versión rápida: con la versión de 24.11 (14 de noviembre de 2024)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
            <p><i>Esta función forma parte de una versión por fases y solo está disponible para clientes específicos.</i></p>
        </td>
    </tr>
</tbody>
</table>

### Mejoras de prioridades

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Función</span></p>
        </td>
        <td>
            <p><span class="bold">Fechas de lanzamiento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Utilice los filtros inteligentes para encontrar su trabajo en Prioridades</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Utilice un lenguaje natural para filtrar rápidamente el trabajo en la lista de trabajos de Prioridades. Puede escribir cosas como </p>
            <ul>
                <li>Mostrarme las tareas atrasadas</li>
                <li>Mostrar las tareas pendientes de esta semana</li>
                <li>Mostrar prioridades principales</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 09 de enero de 2025</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ponerse al día con el trabajo en Prioridades</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Puede usar Ponerme al día para ayudar a reducir el tiempo que se tarda en buscar información sobre proyectos activos.</p>
            <p>Con la tecnología del asistente de IA de Workfront, Catch me up resume las actualizaciones, los documentos cargados y otros cambios importantes sobre sus proyectos en los siguientes lapsos de tiempo: 24 horas, 3 días o 7 días.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: sábado, 20 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ver los cambios en directo en la página Detalles en Prioridades</a></p>
            <p>Ahora puede ver actualizaciones en tiempo real en la página Detalles de una tarea o un problema. También puede ver si otros usuarios están viendo la página al mismo tiempo que usted con indicadores de presencia en tiempo real.</p>
        </td>
        [!BADGE In production ]{type=Informative}
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 19 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Carga y visualización de documentos y pruebas en Prioridades</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Ahora puede interactuar con documentos y pruebas para tareas y problemas de la lista de trabajo y el calendario. En la nueva pestaña Documentos, puede</p>
            <ul>
                <li>Cargar un documento</li>
                <li>Crear una prueba</li>
                <li>Iniciar el visor de revisión</li>
                <li>Y más</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 19 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            La vista de calendario ya está disponible en Prioridades</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Puede realizar un seguimiento del trabajo con un calendario mensual claro y visual. Con el calendario de Prioridades, puede</p>
            <ul>
                <li>Utilice los filtros para encontrar su trabajo</li>
                <li>Aplique campos personalizados como estado y nivel de enfoque para identificar el trabajo de alta prioridad</li>
                <li>Aplicar colores para una organización rápida</li>
                <li>Y más</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 19 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Actualizaciones de la Lista de trabajos de prioridades</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Hemos actualizado la Lista de trabajo de prioridades para mejorar las capacidades y alinearnos con otras áreas de la aplicación.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 12 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Navegue hasta la página de detalles de un proyecto desde Prioridades</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Ahora puede navegar directamente a un proyecto en Workfront desde la lista de trabajo Prioridades.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 05 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Opciones actualizadas en la columna Mi enfoque en Prioridades</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Hemos actualizado las opciones de la columna Mi enfoque para ayudarle a priorizar y ordenar su trabajo de forma más intuitiva. Las nuevas etiquetas incluyen</p>
            <ul>
                <li>Urgente</li>
                <li>Alto</li>
                <li>Normal</li>
                <li>Bajo</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 14 de noviembre de 2024</li>
                <li><span class="preview">Versión de producción para todos los clientes: 14 de noviembre de 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ver detalles del proyecto en Prioridades</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Ahora puede ver los detalles y comentarios del proyecto desde la lista de trabajo en Prioridades.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: jueves, 06 de noviembre de 2024</li>
                <li>Producción para la versión rápida: con la versión de 24.11 (14 de noviembre de 2024)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
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
            <p><span class="bold">Función</span></p>
        </td>
        <td>
            <p><span class="bold">Fechas de lanzamiento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-project-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Las asignaciones más relevantes se han eliminado de los entornos de Previsualización y Producción para versiones rápidas</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Ahora se ha eliminado una funcionalidad que se encuentra en el entorno de vista previa desde diciembre de 2023 y en el entorno de producción de versión rápida desde marzo de 2024. Las funciones agregaron sugerencias de asignación inteligente más relevantes al asignar tareas.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 19 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
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
            <p><span class="bold">Función</span></p>
        </td>
        <td>
            <p><span class="bold">Fechas de lanzamiento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Actualización del Visor de corrección de escritorio</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Hemos actualizado Desktop Viewer con la última versión de Electron 33.3.0 que utiliza Chromium 130.0.6723.152. </p>
            <p>Última versión: 2.1.44 </p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: miércoles, 02 de enero de 2024</li>
                <li><span class="preview">Versión de producción para todos los clientes: 9 de enero de 2025</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><span class="bold">Función</span></p>
        </td>
        <td>
            <p><span class="bold">Fechas de lanzamiento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nueva extensión de explorador para revisión interactiva disponible en versión beta</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Presentamos una nueva extensión de explorador, la herramienta de revisión de Adobe Workfront, para reemplazar la extensión de explorador heredada para revisar el contenido ZIP interactivo. La nueva herramienta de revisión de Adobe Workfront admite la revisión del contenido ZIP en todos los exploradores comunes.</p>
            <p>La extensión del explorador heredado se eliminará el 28 de febrero de 2025.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 07 de noviembre de 2024</li>
                <li><span class="preview">Versión de producción para todos los clientes: 7 de noviembre de 2024</span></li>
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
            <p><span class="bold">Función</span></p>
        </td>
        <td>
            <p><span class="bold">Fechas de lanzamiento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nuevas entidades disponibles en Data Connect</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Se ha añadido compatibilidad con varias entidades nuevas en Data Connect, incluidas algunas entidades específicas de agencias.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: jueves, 15 de enero de 2025</li>
                <li>Versión de producción para todos los clientes: 15 de enero de 2025</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Límite de 25 informes, páginas externas o calendarios en los paneles</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Para mantener el rendimiento del panel, se ha implementado un límite en el número total de informes, páginas externas o calendarios que se pueden colocar en un panel. Al crear un nuevo tablero, se puede agregar un máximo de 25 elementos.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: martes, 16 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Botón de creación de cuenta del lector por primera vez para Data Connect</a></p>
            [!BADGE In production ]{type=Informative}
            <p>A los administradores que acceden a Data Connect por primera vez se les presenta la opción de crear una nueva cuenta de Snowflake reader haciendo clic en un solo botón. El proceso tarda unos minutos en completarse, pero no requiere ninguna acción adicional.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 14 de noviembre de 2024</li>
                <li><span class="preview">Versión de producción para todos los clientes: 14 de noviembre de 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Actualizar mejoras del flujo

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Función</span></p>
        </td>
        <td>
            <p><span class="bold">Fechas de lanzamiento</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Se ha actualizado la experiencia de comentarios en el widget Menciones del área de Inicio y Mis actualizaciones</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Estamos actualizando la experiencia de comentarios en el widget Menciones en Inicio y en la sección Menciones del área Mis actualizaciones. Ahora, la misma experiencia en el área de Actualizaciones de la mayoría de los objetos de Workfront también está disponible en el widget Menciones y en la sección Menciones de Mis actualizaciones.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 19 de diciembre de 2024</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
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
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Actualización de cómo se administran los recursos movidos o eliminados en las carpetas vinculadas</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Hemos cambiado la forma en que se gestionan los recursos movidos y eliminados al utilizar la integración de Adobe Workfront con Experience Manager Assets y Assets Essentials:</p>
            <ul>
                <li>Recursos eliminados: cuando se elimina un recurso dentro de una carpeta vinculada en Assets o Assets Essentials, el recurso eliminado se conservará en el área Documentos del proyecto.</li>
                <li>Recursos movidos: cuando se mueve un recurso fuera de una carpeta vinculada en Assets o Assets Essentials, el recurso movido se conservará en el área Documentos de proyectos.</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: viernes, 21 de noviembre de 2024</li>
                <li><span class="preview">Versión de producción para todos los clientes: 5 de diciembre de 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Las secciones de un formulario personalizado ahora se pueden contraer y expandir</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Cuando se adjunta un formulario personalizado con varias secciones a un objeto, ahora puede contraer y expandir todas las secciones excepto la predeterminada en la parte superior del formulario. El administrador también puede ver esta funcionalidad al obtener una vista previa del formulario en el diseñador de formularios.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: martes, 11 de noviembre de 2024</li>
                <li>Producción para la versión rápida: con la versión de 24.12 (12 de diciembre de 2024)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            El asistente de IA ahora puede trabajar con proyectos, tareas y problemas</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Para facilitar la administración de los elementos de trabajo en Workfront, hemos actualizado el Asistente de IA para que funcione con proyectos, tareas y problemas. Ahora, el Asistente de IA puede localizar proyectos, tareas y problemas en función de los criterios especificados.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión preliminar: viernes, 31 de octubre de 2024</li>
                <li>Producción para la versión rápida: con la versión de 24.11 (14 de noviembre de 2024)</li>
                <li>Versión de producción para todos los clientes: con la versión 25.1 (viernes, 16 de enero de 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Actualizaciones de aspecto durante el primer trimestre de 2025</a></p>
            <p>En el primer trimestre de 2025 se están realizando actualizaciones menores del aspecto de varias áreas de la aplicación de Adobe Workfront. Revise las notas de la versión individuales para ver fechas de lanzamiento específicas.</p>
        </td>
        <td>
            <p><b>Disponible en estas fechas:</b></p>
            <ul>
                <li>Versión de vista previa: Durante el primer trimestre de 2025</li>
                <li><span class="preview">Versión de producción: revise las notas de la versión para fechas específicas</span></li>
            </ul>
        </td>
    </tr>                            
</tbody>
</table>

<!--
### Functionality soon to be removed from Workfront

The following functionality is soon to be removed from Workfront:
-->

## Anuncios

### Mejoras de Workfront Fusion

>[!IMPORTANT]
>
>La documentación de Workfront Fusion se ha trasladado a una nueva ubicación. Para obtener información, instrucciones y versiones para Fusion, visite [Documentación de Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/home).
>
>Cada artículo actual de la documentación de Fusion contiene un vínculo al artículo correspondiente en la nueva ubicación. Actualice sus marcadores.
>
>El conjunto actual de documentación de Fusion ya no se actualiza y se eliminará en un futuro próximo.

Las nuevas funciones de Workfront Fusion están disponibles en el entorno de producción en una cadencia fuera de la programación de versiones del primer trimestre de 2025. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión de Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Mejoras de Workfront Planning

Las nuevas funciones de Workfront Planning están disponibles en el entorno de producción. Para obtener más información sobre las últimas funciones, consulte [Actividad de la versión del primer trimestre de 2025 de Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q1.md).

### Mejoras en el Planificador de escenarios de Workfront

No hay actualizaciones de Scenario Planner en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras de Workfront Proof

No hay actualizaciones de Workfront Proof en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Mejoras de Workfront Goals

No hay actualizaciones de Workfront Goals en este punto de la versión. Esta área se actualizará cuando haya actualizaciones disponibles.

### Versión 19 de la API

Para la versión 19 de la API, hemos modificado algunos recursos y puntos finales. Algunos de los cambios admiten nuevas funciones y otros facilitan el uso de la información disponible a través de la API.

Para obtener información sobre novedades y actualizaciones, consulte [Novedades de la versión 19 de la API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Para obtener información sobre las versiones de API, consulte [Versiones de API y programación de soporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Actualizaciones de mantenimiento de Workfront 

Para obtener información sobre las actualizaciones de mantenimiento realizadas durante la versión del primer trimestre de 2025, consulte [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=es).

### Actualizaciones de aprendizaje

Explore las últimas actualizaciones realizadas en los programas de aprendizaje, rutas de aprendizaje, vídeos y guías de cada versión del producto de Adobe Workfront. Para obtener más información, consulte la sección “Novedades” de la [página de tutoriales de Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=es).
