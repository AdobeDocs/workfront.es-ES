---
title: Información general del diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede diseñar un formulario personalizado que los usuarios puedan adjuntar a un objeto de Workfront. Los usuarios que trabajen en el objeto pueden rellenar el formulario personalizado para proporcionar información sobre el objeto.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 1%

---

# Información general del diseñador de formularios

Puede utilizar el nuevo diseñador de formularios para diseñar un formulario personalizado que los usuarios puedan adjuntar a un objeto de Workfront. Los usuarios que trabajen en el objeto pueden rellenar el formulario personalizado para proporcionar información sobre el objeto.

El nuevo diseñador de formularios tiene un nuevo espacio de trabajo de estilo lienzo que le permite ver los campos, el lienzo y la configuración de campo al mismo tiempo. También le permite arrastrar y soltar campos dentro de las secciones mientras diseña el formulario.

<!-- add screenshot when field settings empty state is ready -->

## Cómo acceder al nuevo diseñador de formularios

Hay un nuevo botón en la parte superior del nuevo diseñador de formularios y del generador de formularios heredado. Puede utilizar este botón para cambiar entre el generador heredado y el nuevo diseñador.

![](assets/switch-views.png)

## Nueva funcionalidad disponible con el diseñador de formularios

Con el nuevo diseñador de formularios, hemos agregado la capacidad de

* **Copiar un campo**: Ahora puede copiar campos existentes haciendo clic en el icono Copiar de los campos directamente desde el lienzo.

* **Cambiar el tamaño del texto descriptivo**: Ahora puede asignar tamaños pequeños, medios o grandes a los campos de texto descriptivo. También puede utilizarlos en la misma fila con otros campos.

* **Usar una sección predeterminada**: Si el creador del formulario no ha agregado ninguna sección en la parte superior del formulario, ahora se puede ver una sección predeterminada en el lienzo, de modo que los usuarios puedan ajustar los permisos de los campos que no tengan una sección personalizada asignada.

   >[!NOTE]
   >
   >La sección predeterminada no está visible en los objetos una vez que el formulario está adjunto al objeto.

## Funcionalidad próximamente

Los siguientes elementos no están disponibles actualmente en el diseñador de formularios, pero se agregarán próximamente:

* Ajustar el tamaño del texto descriptivo

* Mostrar/Omitir lógica

* Filtro para campos tipográficos

>[!IMPORTANT]
>
>Las configuraciones existentes para los filtros lógicos y typeforward no se verán afectadas cuando trabaje con el nuevo diseñador de formularios.

## Funcionalidad eliminada del diseñador de formularios

Se ha eliminado la siguiente funcionalidad del diseñador de formularios:


* Fichas Configuración de formulario, Uso compartido de formularios, Uso compartido de campos

   * La configuración de formulario ya está disponible en la parte superior del lienzo

   * Ficha principal de Uso compartido de formularios y subficha Uso compartido de campos
   >[!NOTE]
   >
   >Puede controlar el uso compartido de formularios y campos desde la ficha Configuración > Forms personalizado > Forms o Campos .

* Seguir cambios de los campos en las fuentes de actualización
   >[!NOTE]
   >
   >Puede encontrarlo en Configuración > Interfaz > Actualizar fuentes .
