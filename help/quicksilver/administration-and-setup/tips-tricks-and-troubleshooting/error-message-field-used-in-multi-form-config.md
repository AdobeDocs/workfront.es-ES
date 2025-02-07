---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensaje de error: Hay un problema leve. Este campo se utiliza en una configuración multiformulario'
description: Cuando cambie un cálculo en un campo personalizado calculado en un formulario personalizado y un mensaje de error le indique que el campo se utiliza en una configuración multiformulario, deberá sustituir el campo por uno nuevo que contenga el cálculo que desea utilizar.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 98%

---

# Mensaje de error: Hay un ligero problema. Este campo se utiliza en una configuración multiformulario

## Problema

Al cambiar un cálculo en un campo personalizado calculado en un formulario personalizado, [!DNL Adobe Workfront] podría mostrar la siguiente advertencia:

Existe un problema leve

[El campo] se utiliza en una configuración multiformulario, si desea cambiar esta fórmula, necesita quitar este campo y reemplazarlo con uno nuevo que contenga el cálculo deseado.

## Causa

Al menos dos formularios personalizados que contienen el campo personalizado calculado que intenta cambiar se adjuntan a un único objeto de la instancia [!DNL Workfront].

**Ejemplo:** Los formularios personalizados A y B se adjuntan a la misma tarea. Ambos formularios contienen un campo personalizado calculado llamado Beneficio. El error se produce al intentar editar el cálculo en el campo Beneficio en el formulario personalizado A.

No se puede cambiar el cálculo del campo personalizado en uno de los formularios porque eso entraría en conflicto con la fórmula del mismo campo del otro formulario.
Para resolver este conflicto, debe encontrar el objeto donde se adjuntan varios formularios con el mismo campo personalizado calculado y, a continuación, realice una de las siguientes acciones:

* Quite uno de los formularios del objeto.
* Cambie el cálculo según sea necesario, pero hágalo en todos los formularios personalizados adjuntos al objeto.
* En todos los formularios personalizados adjuntos al objeto, añada un nuevo campo personalizado calculado que contenga el cálculo que necesita y marque el antiguo campo personalizado calculado como obsoleto.

Este artículo explica cómo encontrar el objeto y luego resolver el problema de una de estas tres maneras.

## Busque el objeto donde se adjuntan los formularios personalizados {#find-the-object-where-the-custom-forms-are-attached}

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Formularios personalizados]** > **[!UICONTROL Campos]**.
1. Aplique la vista **[!UICONTROL Lista de campos]** para encontrar el campo calculado que intenta modificar y anote todos los formularios personalizados en los que se utiliza (por ejemplo, Formulario 1, Formulario 2, Formulario 3).
1. Haga clic en **[!UICONTROL Formularios]**, y luego aplique la vista **[!UICONTROL Lista de formularios]**.
1. Haga clic en el menú **[!UICONTROL Filtro]** y seleccione **[!UICONTROL Nuevo filtro]**.

1. Haga clic en **[!UICONTROL Añadir una regla de filtro]**, a continuación, empiece a escribir “nombre de formulario personalizado” y seleccione este valor cuando se muestre en la lista.
1. Seleccione **[!UICONTROL Igual]** para el modificador de filtro, empiece a escribir el nombre de cada formulario del que tomó nota en el paso 1 y, a continuación, selecciónelo cuando se muestre.

   **Ejemplo:** El Nombre De Formulario Personalizado Es Igual A Formulario 1, Formulario 2, Formulario 3.

1. Haga clic en **[!UICONTROL Guardar filtro]**, asigne un nombre al nuevo filtro y haga clic en **[!UICONTROL Guardar filtro]**.

1. En la lista de formularios, anote el tipo de objeto del filtro, como Tarea o Problema, que se muestra en la columna **[!UICONTROL Tipo]**.
1. En cada formulario personalizado que haya encontrado en el paso 1, cree un nuevo campo personalizado de casilla de verificación con un solo valor predeterminado de Sí.

   **Ejemplo:** Campo 1 en Formulario 1 = Sí, Campo 2 en Formulario 2 = Sí, Campo 3 en Formulario 3 = Sí. Esto significa que “El campo personalizado calculado existe en el formulario 1”, “El campo personalizado calculado existe en el formulario 2”, etc.

1. En el **[!UICONTROL icono de búsqueda]** ![icono de búsqueda](assets/search-icon.png) en la esquina superior derecha de la pantalla, haz clic en **[!UICONTROL Búsqueda avanzada]**.
1. Haga clic en el objeto del formulario personalizado (por ejemplo, Problema), haga clic en **[!UICONTROL Filtrar los resultados]** y, a continuación, haga clic en **[!UICONTROL Añadir un filtro]**.
1. Empiece a escribir el nombre de un campo Casilla de verificación en el campo **[!UICONTROL Empiece a escribir el nombre del campo]** y selecciónelo cuando se muestre en la lista; a continuación, seleccione **[!UICONTROL Igual]** y escriba **[!UICONTROL Sí]** (sin comillas) en el siguiente cuadro.

   **Ejemplo:** Campo 1 Igual (con distinción de mayúsculas y minúsculas) Sí.

1. Haga clic en **[!UICONTROL Añadir filtro]** y añada todos los campos de las casillas de verificación a la búsqueda avanzada.

   Busca todas las combinaciones posibles.

   **Ejemplo:** Cree varios filtros con las combinaciones que encuentre, como se indica a continuación. Debe buscar objetos con varios formularios personalizados adjuntos que contengan los mismos campos calculados. Puede encontrar los siguientes escenarios:

   * Campo 1= Sí + Campo 2 = Sí + Campo 3 = Sí (sin objetos, por ejemplo)
   * Field 1= Yes + Field 2 = Yes (sin objetos, por ejemplo)
   * Campo 1= Sí + Campo 3 = Sí (dos objetos, por ejemplo)

   Esto significa que el campo calculado existe tanto en el Formulario 1 como en el Formulario 3, ya que los campos de casilla de verificación correspondientes (Campo 1 y Campo 3) existen en estos objetos.

   Campo 2 = Sí + Campo 3 = Sí (sin objetos, por ejemplo)

1. Continúe con una de las siguientes secciones de este artículo:

   * [Elimine uno de los formularios personalizados del objeto y edite allí el cálculo](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Realice ediciones idénticas en el cálculo de todos los formularios personalizados adjuntos](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Añada un nuevo campo calculado que contenga el cálculo editado a uno o todos los formularios personalizados adjuntos](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Elimine uno de los formularios personalizados del objeto y edite allí el cálculo {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Busque el objeto donde se adjuntan los formularios personalizados, como se explica en [Buscar el objeto donde se adjuntan los formularios personalizados](#find-the-object-where-the-custom-forms-are-attached) en este artículo y, a continuación, abra el objeto.
1. Elimine uno de los formularios personalizados del objeto y, a continuación, guarde el objeto.

   >[!NOTE]
   >
   >Para añadir los campos del formulario que ha eliminado del objeto, es posible que tenga que editar el formulario personalizado que permanece adjunto al objeto. De este modo, puede conservar la información de los datos personalizados del objeto.

1. En el formulario personalizado que ha eliminado, edite el cálculo del campo personalizado que intentaba actualizar originalmente y a continuación, haga clic en **[!UICONTROL Guardar]**.

   Esta vez, [!DNL Workfront] no debería encontrar ningún conflicto.

1. (Opcional) Elimine los campos de casilla de verificación de los formularios personalizados o bórrelos de [!DNL Workfront].

## Realice ediciones idénticas en el cálculo de todos los formularios personalizados adjuntos {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>Los datos se pierden en los objetos en los que el formulario personalizado ya está adjunto cuando se siguen estos pasos. Sin embargo, si el campo calculado hace referencia a campos estáticos y no a campos calculados, puede utilizar la opción [!UICONTROL Recalcular expresiones personalizadas] en el objeto para restaurar los datos perdidos

1. Busque el objeto donde se adjuntan los formularios personalizados, como se explica en [Buscar el objeto donde se adjuntan los formularios personalizados](#find-the-object-where-the-custom-forms-are-attached) en este artículo.
1. Elimine el campo de todos los formularios personalizados adjuntos al objeto y, a continuación, guarde los formularios.

1. Vuelva a añadir el campo personalizado que contiene el nuevo cálculo a los formularios personalizados.

   >[!IMPORTANT]
   >
   >Los cálculos deben ser idénticos en todos los formularios personalizados adjuntos.

1. (Opcional) Elimine los campos de la casilla de verificación de los formularios o bórrelos de [!DNL Workfront].

## Añada un nuevo campo calculado que contenga el cálculo editado a uno o todos los formularios personalizados adjuntos {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

Para evitar la pérdida de datos en el campo personalizado calculado existente, o si necesita el cálculo editado en sólo uno de los formularios personalizados adjuntos al objeto encontrado:

1. Busque el objeto donde se adjuntan los formularios personalizados, como se explica en [Buscar el objeto donde se adjuntan los formularios personalizados](#find-the-object-where-the-custom-forms-are-attached) en este artículo.
1. Añada un nuevo campo personalizado calculado que contenga el cálculo que necesita a uno o todos los formularios.
1. Cambie el nombre del antiguo campo personalizado calculado **Obsoleto**.

   En todos los formularios que se adjuntaron al objeto, este antiguo formulario personalizado calculado conserva sus datos históricos, pero los usuarios dejan de utilizarlo.

   >[!IMPORTANT]
   >
   >Es posible que se haga referencia al campo antiguo en otros campos personalizados calculados, por lo que es necesario actualizar esos cálculos después de cambiarle el nombre.

1. (Opcional) Elimine los campos de la casilla de verificación de los formularios o bórrelos de Workfront.

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
</blockquote>
-->
