---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Reutilizar un campo personalizado calculado existente en un formulario personalizado con el generador de formularios heredado
description: Puede utilizar el mismo campo personalizado calculado en formularios personalizados que pertenezcan a objetos diferentes. Por ejemplo, puede utilizar el campo calculado de beneficios que ha creado para el formulario personalizado del proyecto en un formulario personalizado de tareas.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 24482fca-94e4-406d-9d62-3db9f51481e6
source-git-commit: ac5b7e0237dbcaea14010eda658f7d5a6be089cc
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Reutilizar un campo personalizado calculado existente en un formulario personalizado con el generador de formularios heredado

Puede utilizar el mismo campo personalizado calculado en formularios personalizados que pertenezcan a objetos diferentes. Por ejemplo, puede utilizar el campo calculado de beneficios que ha creado para el formulario personalizado del proyecto en un formulario personalizado de tareas.

Para obtener información sobre cómo agregar un campo personalizado calculado a un formulario personalizado, consulte [Agregar datos calculados a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Cuando se utiliza un campo personalizado calculado existente, el cálculo no se transfiere al nuevo formulario. Debe volver a agregar el cálculo, en el mismo campo, en el nuevo formulario personalizado.

>[!TIP]
>
>Esto se produce al utilizar el cálculo almacenado en la variable **Instrucciones** del formulario personalizado es útil.

También puede tener un cálculo diferente para el mismo campo, en el nuevo formulario. Mantener el mismo nombre para el campo personalizado calculado garantiza la coherencia y coherencia en la convención de nombres.

>[!IMPORTANT]
>
>Los campos personalizados calculados pueden quedar obsoletos con el tiempo. Para asegurarse de que siempre ve el cálculo actualizado en estos campos, realice una de las siguientes acciones:
>
>* Después de guardar un objeto en el que haya editado datos en un formulario personalizado adjunto, haga clic en el icono Más ![](assets/more-icon.png) en la página principal del objeto y, a continuación, vuelva a calcular expresiones personalizadas.
>* Seleccione la opción Volver a calcular expresiones personalizadas al editar objetos de forma masiva.
>* Seleccione la opción Update previous calculations al editar un campo personalizado calculado en un formulario personalizado.
>

