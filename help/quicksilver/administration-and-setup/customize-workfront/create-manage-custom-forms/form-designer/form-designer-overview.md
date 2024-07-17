---
title: Información general del diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede diseñar un formulario personalizado que los usuarios puedan adjuntar a un objeto de Workfront. Los usuarios que trabajan en el objeto pueden rellenar el formulario personalizado para proporcionar información sobre el objeto.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: 2a2f6d93c916863177d7a9d2f46f8124d1430354
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 1%

---

# Información general del diseñador de formularios

Puede utilizar el nuevo diseñador de formularios para diseñar un formulario personalizado que los usuarios puedan adjuntar a un objeto de Workfront. Los usuarios que trabajan en el objeto pueden rellenar el formulario personalizado para proporcionar información sobre el objeto.

El nuevo diseñador de formularios tiene un nuevo espacio de trabajo de estilo lienzo que le permite ver los campos, el lienzo y la configuración de los campos al mismo tiempo. También permite arrastrar y soltar campos dentro de las secciones mientras diseña el formulario.

![Diseñador de formularios de ejemplo](assets/form-designer-example.png)

## Cómo acceder al diseñador de formularios

Un botón en la parte superior del nuevo diseñador de formularios y del creador de formularios heredados le permite cambiar entre las versiones.

![Cambiar al nuevo diseñador de formularios](assets/switch-views.png)

## Nueva funcionalidad disponible con el diseñador de formularios

Con el nuevo diseñador de formularios, se ha agregado la capacidad de:

* **Copiar un campo**: ahora puede copiar campos existentes haciendo clic en el icono Copiar en los campos directamente desde el lienzo.

* **Cambiar el tamaño del texto descriptivo**: ahora puede asignar tamaños pequeños, medianos o grandes a los campos de texto descriptivo. También puede utilizarlos en la misma fila con otros campos.

* **Usar una sección predeterminada**: si el creador del formulario no ha agregado una sección en la parte superior del formulario, ahora se ve una sección predeterminada en el lienzo para que los usuarios puedan ajustar los permisos de los campos que no tengan asignada ninguna sección personalizada.

  >[!NOTE]
  >
  >La sección Predeterminada no está visible dentro de los objetos una vez que el formulario está adjunto al objeto.

* **Usar un campo de búsqueda externa**: Este tipo de campo llama a una API externa y devuelve valores como opciones en un campo desplegable.

## Funcionalidad quitada del diseñador de formularios

Se ha quitado la siguiente funcionalidad del diseñador de formularios:

* La configuración de formulario ya está disponible en la parte superior del lienzo

* Seguir cambios de los campos en las fuentes de actualización

  >[!NOTE]
  >
  >Puede encontrar esta opción en Configuración > Interfaz > Actualizar fuentes

