---
title: 22.2 Mejoras del administrador
description: 22.2 Mejoras del administrador
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 0%

---

# 22.2 Mejoras del administrador

En esta página se describen todas las mejoras realizadas por el administrador con la versión 2.2 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno Producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 4 de abril de 2022. Para obtener una lista de todos los cambios disponibles con la versión 2.2, consulte [Resumen de la versión 2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Configuración de un formulario personalizado para que funcione con varios tipos de objetos

Ahora puede configurar un formulario personalizado nuevo o existente para que funcione con varios tipos de objetos, lo que hace que el formulario sea mucho más útil. Los usuarios podrán adjuntar y rellenar el formulario en objetos de todos los tipos para los que lo configure.

Anteriormente, se podía configurar un formulario personalizado para que funcionara con un solo tipo de objeto.

Esta funcionalidad funciona con todos los formularios personalizados creados anteriormente en el sistema Workfront. Por ejemplo, si ya tiene un formulario personalizado creado para el tipo de objeto Task , puede configurar el formulario para que funcione también con otros tipos de objetos, como Project y Problema.

Para obtener más información, consulte la sección [Empezar a crear un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) en el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* En el momento de nuestra versión de Vista previa inicial de esta funcionalidad, deshabilitamos temporalmente la capacidad de copiar un formulario personalizado de varios objetos. Esa capacidad se habilitó el 24 de marzo. Para obtener información sobre cómo copiar un formulario personalizado, consulte [Copiar un formulario personalizado para crear uno nuevo](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* En un campo personalizado calculado, es posible que algunos campos a los que hace referencia no sean compatibles con los tipos de objeto configurados para el formulario. Nuestra solución es un comodín que permitirá que el cálculo arroje valores diferentes, según el objeto al que esté adjunto el formulario. El 24 de marzo agregamos la comodín. Para obtener información sobre cómo utilizarla, consulte la sección [Campos personalizados calculados en formularios personalizados con varios objetos](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) en el artículo [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* Para los saltos de sección en formularios personalizados, hemos creado un conjunto de permisos comunes de visualización y edición que funcionan para todos los tipos de objeto que se pueden configurar para un formulario. En un escenario, se encontró que uno de estos permisos, Edición limitada, podía causar errores en un formulario. Esto se corrigió el 24 de marzo. Para obtener más información sobre los saltos de sección, consulte [Agregar un salto de sección a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>


## El catálogo de modelos está disponible para todos los usuarios y los administradores pueden permitir solicitudes

Todos los usuarios de Adobe Workfront ahora pueden examinar el catálogo de modelos disponibles. Para obtener más información, consulte [Examine el catálogo de modelos y solicite la instalación de modelos](../../../administration-and-setup/blueprints/browse-catalog.md).

Además, el administrador del sistema puede permitir el acceso de los usuarios para solicitar la instalación de modelos. La asignación de una cola de solicitudes para almacenar las solicitudes permite a los usuarios realizar solicitudes desde el catálogo de modelos. Para obtener más información, consulte [Configuración del acceso a los modelos](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Añadir una imagen a un formulario personalizado

En un formulario personalizado que cree o edite, ahora puede agregar una imagen e incluir una información de objeto instructiva o informativa que los usuarios pueden leer cuando pasan el ratón por encima de ella.

Esto podría resultar útil, por ejemplo, para mostrar la marca de un nuevo producto o para proporcionar la información visual que las personas necesitan cuando rellenan el formulario.

Anteriormente, los formularios personalizados estaban completamente basados en texto.

>[!NOTE]
>
>En las nuevas áreas de experiencia de Adobe Workfront que aún no se han modernizado, como el cuadro que aparece al editar elementos por lotes, no se muestran las imágenes de formulario personalizadas. Se mostrarán a medida que continuemos actualizando esas áreas.

Para obtener más información, consulte [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Nuevas configuraciones predeterminadas de nivel de acceso

Para adaptarse mejor a las necesidades de la mayoría de los administradores que crean nuevos niveles de acceso, hemos cambiado la configuración predeterminada para las opciones &quot;Ajustar su configuración&quot; que se enumeran a continuación. Se muestran al hacer clic en el icono de engranaje ![](assets/gear-icon-in-access-levels.png) en un botón Editar.

Todos estos cambios desactivan una opción que anteriormente estaba activada de forma predeterminada. Si esto no se ajusta a las necesidades de su organización, puede habilitarlas cuando configure un nuevo nivel de acceso o en cualquier momento posterior.

>[!IMPORTANT]
>
>Este cambio de configuración predeterminado solo afecta a los niveles de acceso que cree a partir de ahora, no a los que creó anteriormente.

* En un nuevo nivel de acceso con un tipo de licencia Plan:

   * Share System-wide ahora está desactivado para proyectos, tareas, problemas, portafolios, programas, informes, filtros, documentos y plantillas.
   * Ver informes integrados y Compartir informes públicamente también están desactivados para los informes.
   * Compartir documentos públicamente también está desactivado para los documentos.

* En un nuevo nivel de acceso con un tipo de licencia de trabajo:

   * Share System-wide ahora está desactivado para filtros y documentos.
   * Compartir documentos públicamente también está desactivado para los documentos.

* En un nuevo nivel de acceso con un tipo de licencia de Solicitud o Revisión:

   * Compartir todo el sistema ahora está desactivado para los filtros.

## Desactivar un grupo

A medida que cambien las organizaciones internas, es posible que tenga que dejar de usar ciertos grupos en Workfront y crear otros nuevos. Para ayudarle con esto, hemos agregado la capacidad de desactivar un grupo sin perder sus datos históricos. Para los usuarios normales que no necesitan verlos, los grupos inactivos se borran de los campos de avance de tipo de grupo.

Aún puede encontrar y configurar opciones, preferencias y asociaciones de objetos para los grupos inactivos que administra. Y desactivar un grupo no cambia nada acerca de los objetos a los que está conectado el grupo.

Anteriormente, no era posible desactivar un grupo.

Para obtener más información, consulte [Desactivar o reactivar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Mejoras en el historial de instalación de modelos

Al instalar un modelo, ahora aparece un mensaje que muestra los objetos específicos (como roles, equipos o grupos) que se instalaron correctamente con el modelo y cualquier objeto que no se instaló. También puede ver la lista de objetos instalados en la página Detalles del modelo haciendo clic en Ver detalles junto a una instalación específica en la tabla del historial de instalación.

Para obtener más información, consulte [Instalación de un modelo](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## Ahora aparece una advertencia al instalar un modelo de solo vista previa en producción

Ciertos modelos solo están disponibles para instalarse en el entorno de Vista previa para realizar pruebas.

Si accede al contenido de solo vista previa en el entorno de producción, el Simulador para pruebas 1 o el Simulador para pruebas 2, el botón de instalación no está activo y puede que aparezca un mensaje de advertencia.

Para obtener más información, consulte [Instalación de un modelo](../../../administration-and-setup/blueprints/blueprints-install.md).
