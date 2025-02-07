---
title: Mejoras en el administrador con la versión 22.2
description: Mejoras en el administrador con la versión 22.2
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 97%

---

# Mejoras en el administrador con la versión 22.2

En esta página se describen todas las mejoras realizadas en el administrador con la versión 22.2 en el entorno de Vista previa. Estas mejoras estarán disponibles en el entorno de producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 4 de abril de 2022. Para obtener una lista de todos los cambios disponibles con la versión 22.2, consulte [Información general sobre la versión 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Configuración de un formulario personalizado para que funcione con varios tipos de objetos

Ahora puede configurar un formulario personalizado, nuevo o existente, para que funcione con varios tipos de objetos, lo que hace que el formulario sea mucho más útil. Los usuarios podrán adjuntar y rellenar el formulario en objetos de todos los tipos para los que lo configure.

Anteriormente, se podía configurar un formulario personalizado para que funcionase con un solo tipo de objeto.

Esta funcionalidad funciona con todos los formularios personalizados que haya creado anteriormente en su sistema de Workfront. Por ejemplo, si ya tiene un formulario personalizado creado para el tipo de objeto Tarea, ahora puede configurar el formulario para que funcione también con otros tipos de objeto, como Proyecto o Problema.

>[!NOTE]
>
>* En el momento de la versión preliminar inicial de esta funcionalidad, deshabilitamos temporalmente la capacidad de copiar un formulario personalizado de varios objetos. Esta capacidad se habilitó el 24 de marzo.
>* En un campo personalizado calculado, es posible que algunos campos a los que hace referencia no sean compatibles con los tipos de objetos configurados para el formulario. Nuestra solución es un comodín que permite que el cálculo muestre valores diferentes según el objeto al que esté adjunto el formulario. Añadimos el comodín el 24 de marzo.
>* Para los saltos de sección en los formularios personalizados, hemos creado un conjunto de permisos comunes de visualización y edición que funcionan para todos los tipos de objetos que se pueden configurar para un formulario. En un escenario, descubrimos que uno de estos permisos, Edición limitada, podía provocar errores en un formulario. Este problema se corrigió el 24 de marzo.
>

## El catálogo de modelos está disponible para todos los usuarios y los administradores pueden permitir solicitudes

Ahora todos los usuarios de Adobe Workfront pueden examinar el catálogo de modelos disponibles. Para obtener más información, vea [Examinar el catálogo de modelos y solicitar la instalación de modelos](../../../administration-and-setup/blueprints/browse-catalog.md).

Además, el administrador del sistema puede habilitar el acceso para que los usuarios soliciten la instalación de modelos. La asignación de una cola de solicitudes para almacenar las solicitudes permite a los usuarios realizar solicitudes desde el catálogo de modelos. Para obtener más información, consulte [Configurar el acceso a los modelos](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Añadir una imagen a un formulario personalizado

En un formulario personalizado que cree o edite, ahora puede añadir una imagen e incluir información sobre el objeto o instrucciones que los usuarios podrán leer cuando pasen el puntero por encima.

Esto puede resultar útil, por ejemplo, para mostrar la marca de un nuevo producto o para proporcionar la información visual que las personas necesitan cuando rellenan el formulario.

Anteriormente, los formularios personalizados estaban completamente basados en texto.

>[!NOTE]
>
>En las nuevas áreas de experiencia de Adobe Workfront que aún no se han modernizado, como el cuadro que se muestra al editar elementos de forma masiva, las imágenes de formulario personalizadas no se muestran. Se mostrarán a medida que actualicemos esas áreas.


## Nuevas configuraciones predeterminadas del nivel de acceso

Para satisfacer mejor las necesidades de la mayoría de los administradores que crean nuevos niveles de acceso, hemos cambiado la configuración predeterminada de las opciones “Ajustar la configuración” que se enumeran a continuación. Se muestran al hacer clic en el icono de engranaje ![Acceder a los niveles del icono de engranaje](assets/gear-icon-in-access-levels.png) en un botón Editar.

Todos estos cambios deshabilitan la opción que estaba activada anteriormente de forma predeterminada. Si esto no se adapta a las necesidades de su organización, puede habilitarlas al configurar un nuevo nivel de acceso o puede hacerlo más tarde.

>[!IMPORTANT]
>
>Este cambio de la configuración predeterminada solo afecta a los niveles de acceso que cree a partir de ahora, no a los que haya creado anteriormente.

* En un nuevo nivel de acceso con un tipo de licencia de planificación:

   * La opción de compartir en todo el sistema ahora está deshabilitada para proyectos, tareas, problemas, portafolios, programas, informes, filtros, documentos y plantillas.
   * Las opciones Ver informes integrados y Compartir informes públicamente también están desactivadas para los informes.
   * La opción Compartir documentos públicamente también está deshabilitada para documentos.

* En un nuevo nivel de acceso con un tipo de licencia de trabajo:

   * La opción Compartir en todo el sistema ahora está desactivada para filtros y documentos.
   * La opción Compartir documentos públicamente también está deshabilitada para documentos.

* En un nuevo nivel de acceso con un tipo de licencia de solicitud o revisión:

   * La opción Compartir en todo el sistema ahora está desactivada para los filtros.

## Desactivar un grupo

A medida que cambien sus organizaciones internas, es posible que tenga que dejar de utilizar ciertos grupos en Workfront y crear otros nuevos. Para ayudarle con esto, hemos añadido la capacidad de desactivar un grupo sin perder sus datos históricos. Para los usuarios habituales que no necesitan verlos, los grupos inactivos se borran de los campos de escritura anticipada de grupo.

Puede seguir buscando y configurando opciones, preferencias y asociaciones de objetos para los grupos inactivos que administre. Y desactivar un grupo no cambia nada sobre los objetos a los que está unido.

Anteriormente, no era posible desactivar ningún grupo.

Para obtener más información, vea [Desactivar o reactivar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Mejoras en el historial de instalación de modelos

Al instalar un modelo, ahora aparece un mensaje con los objetos específicos (como funciones, equipos o grupos) que se instalaron correctamente con el modelo y los objetos que no se instalaron. También puede ver la lista de objetos instalados en la página Detalles del modelo haciendo clic en Ver detalles junto a una instalación específica en la tabla del historial de instalación.

Para obtener más información, consulte [Instalar un modelo](../../../administration-and-setup/blueprints/blueprints-install.md).

![Historial de instalación de modelos](assets/blueprints-installation-history-350x95.png)

## Ahora se muestra una advertencia al instalar un modelo de solo Vista previa en Producción

Algunos modelos solo están disponibles para su instalación en el entorno de vista previa con fines de prueba.

Al acceder al contenido de solo vista previa en el entorno de producción, en la zona protegida 1 o en la zona protegida 2, el botón de instalación no estará activo y podría ver un mensaje de advertencia.

Para obtener más información, consulte [Instalar un modelo](../../../administration-and-setup/blueprints/blueprints-install.md).
