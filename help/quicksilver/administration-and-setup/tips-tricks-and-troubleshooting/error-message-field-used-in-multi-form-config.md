---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensaje de error: Hay un pequeño problema. Ese campo se utiliza en una configuración de varios formularios'
description: Cuando se cambia un cálculo en un campo personalizado calculado en un formulario personalizado y un mensaje de error indica que el campo se utiliza en una configuración de varios formularios, se debe reemplazar el campo por un nuevo campo que contenga el cálculo que se desee utilizar.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# Mensaje de error: Hay un pequeño problema. Ese campo se utiliza en una configuración de varios formularios

## Problema

Cuando se cambia un cálculo en un campo personalizado calculado en un formulario personalizado, [!DNL Adobe Workfront] podría mostrar la siguiente advertencia:

Existe un problema leve

[El campo] se utiliza en una configuración de varios formularios, si desea cambiar esta fórmula, deberá quitar este campo y sustituirlo por uno nuevo que contenga el cálculo deseado.

## Causa

Al menos dos formularios personalizados que contienen el campo personalizado calculado que está intentando cambiar se adjuntan a un único objeto del [!DNL Workfront] instancia.

**Ejemplo:** Los formularios personalizados A y B están adjuntos a la misma tarea. Ambos formularios contienen un campo personalizado calculado llamado Beneficio. El error se produce al intentar editar el cálculo en el campo Beneficio del formulario personalizado A.

No se puede cambiar el cálculo del campo personalizado en uno de los formularios porque entraría en conflicto con la fórmula del mismo campo en el otro formulario.
Para resolver este conflicto, debe encontrar el objeto al que están adjuntos los varios formularios con el mismo campo personalizado calculado y, a continuación, realice una de las siguientes acciones:

* Elimine uno de los formularios del objeto.
* Cambie el cálculo según sea necesario, pero hágalo en todos los formularios personalizados adjuntos al objeto.
* En todos los formularios personalizados adjuntos al objeto, añada un nuevo campo personalizado calculado que contenga el cálculo que necesite y marque el antiguo campo personalizado calculado como obsoleto.

Este artículo explica cómo encontrar el objeto y luego resolver el problema de una de estas tres maneras.

## Busque el objeto al que están adjuntos los formularios personalizados {#find-the-object-where-the-custom-forms-are-attached}

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Usuarios]** ![](assets/users-icon-in-main-menu.png).

1. Haga clic en **[!UICONTROL Forms personalizado]** > **[!UICONTROL Campos]**.
1. Aplique la variable **[!UICONTROL Lista de campos]** para encontrar el campo calculado que está intentando modificar y tener en cuenta todos los formularios personalizados en los que se utiliza (por ejemplo, Formulario 1, Formulario 2, Formulario 3) .
1. Haga clic en **[!UICONTROL Forms]** y, a continuación, aplique la variable **[!UICONTROL Lista de formularios]** vista.
1. Haga clic en el **[!UICONTROL Filtro]** lista desplegable y, a continuación, **[!UICONTROL Nuevo filtro]**.

1. Haga clic en **[!UICONTROL Agregar una regla de filtro]** y, a continuación, empiece a escribir &quot;nombre de formulario personalizado&quot; y seleccione este valor cuando aparezca en la lista.
1. Select **[!UICONTROL Igual]** para el modificador de filtros, empiece a escribir el nombre de cada formulario del que ha realizado una nota en el paso 1 y, a continuación, selecciónelo cuando aparezca.

   **Ejemplo:** El Nombre Del Formulario Personalizado Es Igual A Formulario 1, Formulario 2, Formulario 3.

1. Haga clic en **[!UICONTROL Guardar filtro]**, asigne un nombre al nuevo filtro y haga clic en **[!UICONTROL Guardar filtro]**.

1. En la lista de formularios, tenga en cuenta el tipo de objeto del filtro, como Tarea o Problema, que se muestra en la **[!UICONTROL Tipo]** para abrir el Navegador.
1. En cada formulario personalizado que se encuentra en el paso 1, cree un nuevo campo personalizado de casilla de verificación con un único valor predeterminado de Sí.

   **Ejemplo:** Campo 1 del formulario 1 = Sí, Campo 2 del formulario 2 = Sí, Campo 3 del formulario 3 = Sí. Esto significa &quot;El campo personalizado calculado existe en el formulario 1&quot; o &quot;El campo personalizado calculado existe en el formulario 2&quot;, etc.

1. En el **[!UICONTROL Icono de búsqueda]** ![](assets/search-icon.png) en la esquina superior derecha de la pantalla, haga clic en **[!UICONTROL Búsqueda avanzada]**.
1. Haga clic en el objeto del formulario personalizado (como Problema) y haga clic en **[!UICONTROL Filtrar los resultados]** y haga clic en **[!UICONTROL Añadir un filtro]**.
1. Comience a escribir el nombre de un campo de casilla de verificación en la **[!UICONTROL Empezar a escribir el nombre del campo]** y selecciónelo cuando aparezca en la lista y, a continuación, seleccione **[!UICONTROL Igual]** y tipo **[!UICONTROL Sí]** (sin comillas) en el cuadro siguiente.

   **Ejemplo:** Campo 1 Igual (Distinción entre mayúsculas y minúsculas) Sí.

1. Haga clic en **[!UICONTROL Añadir un filtro]** y agregue todos los campos de casilla de verificación a la búsqueda avanzada.

   Busque todas las combinaciones posibles.

   **Ejemplo:** Genere varios filtros con las combinaciones que encuentre, como se muestra a continuación. Debe buscar objetos con varios formularios personalizados adjuntos que contengan los mismos campos calculados. Puede encontrar las siguientes situaciones:

   * Campo 1= Sí + Campo 2 = Sí + Campo 3 = Sí (sin objetos, por ejemplo)
   * Campo 1= Sí + Campo 2 = Sí (sin objetos, por ejemplo)
   * Field 1= Yes + Field 3 = Yes (dos objetos, por ejemplo)

   Esto significa que el campo calculado existe tanto en el Formulario 1 como en el Formulario 3, ya que los campos de casilla de verificación correspondientes (Campo 1 y Campo 3) existen en estos objetos.

   Campo 2 = Sí + Campo 3 = Sí (sin objetos, por ejemplo)

1. Continúe con una de las siguientes secciones de este artículo:

   * [Elimine uno de los formularios personalizados del objeto y edite el cálculo allí](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Realizar ediciones idénticas en el cálculo de todos los formularios personalizados adjuntos](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Agregue un nuevo campo calculado que contenga el cálculo editado a uno o todos los formularios personalizados adjuntos](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Elimine uno de los formularios personalizados del objeto y edite el cálculo allí {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Busque el objeto al que están adjuntos los formularios personalizados, tal como se explica en [Busque el objeto al que están adjuntos los formularios personalizados](#find-the-object-where-the-custom-forms-are-attached) en este artículo, abra el objeto .
1. Elimine uno de los formularios personalizados del objeto y, a continuación, guarde el objeto.

   >[!NOTE]
   >
   >Para agregar los campos del formulario que quitó del objeto, es posible que tenga que editar el formulario personalizado que permanece adjunto al objeto. De este modo, puede conservar la información de datos personalizada en el objeto.

1. En el formulario personalizado que ha eliminado, edite el cálculo del campo personalizado que estaba intentando actualizar originalmente y, a continuación, haga clic en **[!UICONTROL Guardar]**.

   Esta vez, [!DNL Workfront] no debería encontrar un conflicto.

1. (Opcional) Elimine los campos de casilla de verificación de los formularios personalizados o [!DNL Workfront].

## Realizar ediciones idénticas en el cálculo de todos los formularios personalizados adjuntos {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>Se pierden datos en los objetos donde el formulario personalizado ya está adjunto cuando se siguen estos pasos. Sin embargo, si el campo calculado hace referencia a campos estáticos, no a campos calculados, puede utilizar [!UICONTROL Volver a calcular expresiones personalizadas] en el objeto para restaurar los datos perdidos

1. Busque el objeto al que están adjuntos los formularios personalizados, tal como se explica en [Busque el objeto al que están adjuntos los formularios personalizados](#find-the-object-where-the-custom-forms-are-attached) en este artículo.
1. Quite el campo de todos los formularios personalizados que estén adjuntos al objeto y, a continuación, guarde los formularios.

1. Agregue el campo personalizado que contiene el nuevo cálculo a los formularios personalizados.

   >[!IMPORTANT]
   >
   >Los cálculos deben ser idénticos en todos los formularios personalizados adjuntos.

1. (Opcional) Elimine los campos de casilla de verificación de los formularios o [!DNL Workfront].

## Agregue un nuevo campo calculado que contenga el cálculo editado a uno o todos los formularios personalizados adjuntos {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

Para evitar perder datos en el campo personalizado calculado existente o si necesita realizar el cálculo editado en solo uno de los formularios personalizados adjuntos al objeto que ha encontrado:

1. Busque el objeto al que están adjuntos los formularios personalizados, tal como se explica en [Busque el objeto al que están adjuntos los formularios personalizados](#find-the-object-where-the-custom-forms-are-attached) en este artículo.
1. Agregue un nuevo campo personalizado calculado que contenga el cálculo necesario a uno o a todos los formularios.
1. Cambiar el nombre del antiguo campo personalizado calculado **Obsoleto**.

   En todos los formularios adjuntos al objeto, este formulario personalizado calculado anterior conserva sus datos históricos, pero los usuarios dejan de utilizarlos.

   >[!IMPORTANT]
   >
   >Es posible que se haga referencia al campo anterior en otros campos personalizados calculados, por lo que debe actualizar esos cálculos después de cambiar su nombre.

1. (Opcional) Elimine los campos Casilla de verificación de los formularios o elimínelos de Workfront.

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
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->
