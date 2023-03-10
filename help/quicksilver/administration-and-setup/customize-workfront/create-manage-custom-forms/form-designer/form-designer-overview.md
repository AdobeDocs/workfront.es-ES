---
title: Información general del diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede diseñar un formulario personalizado que los usuarios puedan adjuntar a un objeto de Workfront. Los usuarios que trabajan en el objeto pueden rellenar el formulario personalizado para proporcionar información sobre el objeto.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 9b32c41c9f2971f3b0bbded230680677cc0b3c64
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 1%

---

# Información general del diseñador de formularios

{{highlighted-preview-article-level}}

Puede utilizar el nuevo diseñador de formularios para diseñar un formulario personalizado que los usuarios puedan adjuntar a un objeto de Workfront. Los usuarios que trabajan en el objeto pueden rellenar el formulario personalizado para proporcionar información sobre el objeto.

El nuevo diseñador de formularios tiene un nuevo espacio de trabajo de estilo lienzo que le permite ver los campos, el lienzo y la configuración de los campos al mismo tiempo. También permite arrastrar y soltar campos dentro de las secciones mientras diseña el formulario.

<!-- add screenshot when field settings empty state is ready -->

## Cómo acceder al nuevo diseñador de formularios

Hay un nuevo botón en la parte superior del nuevo diseñador de formularios y del creador de formularios heredados. Puede utilizar este botón para cambiar entre el generador heredado y el nuevo diseñador.

![](assets/switch-views.png)

## Nueva funcionalidad disponible con el diseñador de formularios

Con el nuevo diseñador de formularios, hemos agregado la capacidad de

* **Copiar un campo**: Ahora puede copiar campos existentes haciendo clic en el icono Copiar en los campos directamente desde el lienzo.

* **Cambio del tamaño del texto descriptivo**: Ahora puede asignar tamaños pequeños, medianos o grandes a los campos de texto descriptivo. También puede utilizarlos en la misma fila con otros campos.

* **Utilizar una sección predeterminada**: Si el creador del formulario no ha agregado una sección en la parte superior del formulario, ahora se puede ver una sección Predeterminada en el lienzo para que los usuarios puedan ajustar los permisos de los campos que no tengan asignada ninguna sección personalizada.

   >[!NOTE]
   >
   >La sección predeterminada no es visible dentro de los objetos una vez que el formulario está adjunto al objeto.

## Funcionalidad próximamente

Los siguientes elementos no están disponibles actualmente en el diseñador de formularios, pero se agregarán próximamente:

* Ajuste del tamaño del texto descriptivo

* Lógica de visualización/omisión

* Filtrar por campos de escritura anticipada

>[!IMPORTANT]
>
>Las configuraciones existentes para la lógica y los filtros de escritura anticipada no se verán afectadas al trabajar con el nuevo diseñador de formularios.

## Funcionalidad quitada del diseñador de formularios

Se ha eliminado la siguiente funcionalidad del diseñador de formularios:


* Fichas Configuración de formulario, Uso compartido de formularios, Uso compartido de campos

   * La configuración de formulario ya está disponible en la parte superior del lienzo

   * Pestaña principal Compartir formularios y subpestaña Compartir campos
   >[!NOTE]
   >
   >Puede controlar el uso compartido de formularios y campos desde la pestaña Configuración > Forms personalizado > Forms o Campos.

* Seguir cambios de los campos en las fuentes de actualización
   >[!NOTE]
   >
   >Puede encontrarlo en Configuración > Interfaz > Actualizar fuentes
