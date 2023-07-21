---
title: Información general del diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede diseñar un formulario personalizado que los usuarios puedan adjuntar a un objeto de Workfront. Los usuarios que trabajan en el objeto pueden rellenar el formulario personalizado para proporcionar información sobre el objeto.
author: Courtney / Lisa
feature: System Setup and Administration
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: ad04b732adac345bc015bb290dfd12898bb0a604
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Información general del diseñador de formularios

Puede utilizar el nuevo diseñador de formularios para diseñar un formulario personalizado que los usuarios puedan adjuntar a un objeto de Workfront. Los usuarios que trabajan en el objeto pueden rellenar el formulario personalizado para proporcionar información sobre el objeto.

El nuevo diseñador de formularios tiene un nuevo espacio de trabajo de estilo lienzo que le permite ver los campos, el lienzo y la configuración de los campos al mismo tiempo. También permite arrastrar y soltar campos dentro de las secciones mientras diseña el formulario.

<!-- add screenshot when field settings empty state is ready -->

## Cómo acceder al nuevo diseñador de formularios

Hay un nuevo botón en la parte superior del nuevo diseñador de formularios y del creador de formularios heredados. Puede utilizar este botón para cambiar entre el generador heredado y el nuevo diseñador.

![Cambiar al nuevo diseñador de formularios](assets/switch-views.png)

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

* Lógica de visualización/omisión

* Filtrar por campos de escritura anticipada

>[!IMPORTANT]
>
>Las configuraciones existentes para la lógica y los filtros de escritura anticipada no se verán afectadas al trabajar con el nuevo diseñador de formularios.

### Lógica de visualización/omisión

Aunque todavía no puede agregar lógica de visualización u omisión al diseñar un nuevo formulario personalizado, puede ver la lógica de visualización u omisión existente en los formularios creados en el generador de formularios heredados.

Los iconos de un campo en el diseñador de formularios indican que se aplica lógica al campo.

El ![Mostrar lógica para el campo de destino](assets/display-logic-bottom-left.png) en la parte inferior izquierda significa que el campo es el campo de destino para la lógica de visualización (si se realiza una selección específica en el formulario, se muestra este campo). El ![Definir icono de lógica de visualización](assets/display-logic-bottom-right.png) en la parte inferior derecha significa que el campo se utiliza para definir la lógica de visualización (una selección o valor específico de este campo mostrará el campo de destino).

El ![Omitir lógica para campo de destino](assets/skip-logic-bottom-left.png) en la parte inferior izquierda significa que el campo es el campo de destino para la lógica de omisión (si se realiza una selección específica en el formulario, este se salta este campo). El ![Definir icono de lógica de omisión](assets/skip-logic-bottom-right.png) en la parte inferior derecha significa que el campo se utiliza para definir la lógica de omisión (una selección o valor específico de este campo omitirá otros campos e irá directamente al campo de destino).

![Iconos lógicos](assets/logic-icons-3.png)

Al seleccionar un campo con lógica aplicada, se muestran las reglas lógicas existentes en la configuración del campo.

![Reglas lógicas](assets/form-designer-view-only-logic.png)

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
