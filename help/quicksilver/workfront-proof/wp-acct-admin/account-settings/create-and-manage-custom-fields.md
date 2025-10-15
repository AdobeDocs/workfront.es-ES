---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Creación y administración de campos personalizados en  [!DNL Workfront Proof]
description: Se requiere un plan Select o Premium [!DNL Workfront] para usar esta función. Para obtener más información sobre los distintos planes disponibles, consulte Planes de Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 7f24186c8803237a6f5116293b3c6a5fd1ea90f6
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 50%

---

# Creación y administración de campos personalizados en [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Se requiere un plan Select o Premium [!DNL Workfront] para utilizar esta función. Para obtener más información sobre los diversos planes disponibles, consulte [Planes de Workfront](https://business.adobe.com/es/products/workfront/pricing.html).

Los campos personalizados le permiten capturar datos adicionales al crear una prueba, un usuario o un invitado nuevos. Por ejemplo, es posible que los usuarios que creen una nueva prueba deseen incluir una sección adicional que les permita capturar un número de trabajo, un código de departamento o una referencia de proveedor.

>[!NOTE]
>
>* La captura de este tipo de información en la página Nueva prueba mediante campos personalizados también le permite reducir la longitud del nombre de la prueba, ya que estos detalles no tienen que incluirse en el nombre.
>
>* Una vez que se ha utilizado un campo personalizado en una prueba, un usuario o un contacto, no se puede eliminar ni editar el tipo de campo. Sin embargo, puede ocultarlo a través de la página Configuración de campo personalizado para que no se utilice en elementos nuevos.
>
>* Si oculta una sección de campos personalizados, todos los campos de la sección también se ocultarán, aunque los campos individuales estén configurados como visibles.

## Crear campos personalizados

{{step1-to-proofing}}

1. En la esquina superior derecha de la página, haga clic en **Configuración de la cuenta**.

1. En la página **Configuración de cuenta**, seleccione la pestaña **Campos personalizados**.

1. Haga clic en **[!UICONTROL Agregar sección de campo personalizado]** en el lado derecho del módulo (**Prueba**, **Usuarios** o **Contactos**) al que desee agregar el campo personalizado. Se abre la ficha **Detalles de sección**.

1. Escriba un **Nombre** para la sección de campo personalizado y haga clic en **[!UICONTROL Guardar]**.

1. Haga clic en la ficha **[!UICONTROL Configuración de campos personalizados]** para actualizar la página. La nueva sección de campo personalizado se muestra debajo del módulo asignado.

   ![Ficha Configuración de campos personalizados](assets/custom-field-settings-tab.png)

1. Haga clic en el nombre de la nueva sección de campos personalizados para abrir la ficha **Sección de campos personalizados**.

1. En la parte superior derecha de la página, haga clic en el botón **[!UICONTROL Nuevo campo personalizado]**. Aparecerá la página **Nuevo campo personalizado**.

1. Especifique **detalles del campo**:

   * **Nombre**: escriba el nombre del campo personalizado.
   * **Ayuda**: escriba el texto de ayuda que se mostrará en la información del objeto.
   * **Obligatorio**: marque esta casilla para requerir que el usuario complete el campo.
   * **Buscable** (condicional): marque esta casilla para que el campo personalizado pueda buscarse.
   * **Oculto**: marca esta casilla para ocultar el campo personalizado en las páginas de **Nueva prueba**, **Nuevo invitado** y **Nuevo usuario**.

1. Especifique **Tipo de campo** y detalles:

   * **Tipo**: seleccione el tipo de campo personalizado.
   * **Elementos de lista**: (condicional) Agregue los elementos de lista que aparecerán en el campo personalizado.
   * **Valor predeterminado**: seleccione el valor predeterminado para este campo personalizado. Esta opción variará según el tipo de campo personalizado seleccionado.

1. Haga clic en **[!UICONTROL Guardar]**.

1. Realice más cambios en la configuración del campo:

   * Oculte o muestre la sección de campo personalizado haciendo clic en el menú de **Más** ![Más botón](assets/more-button-small.png) a la derecha del nombre de la sección de campo personalizado y, a continuación, haciendo clic en **[!UICONTROL Ocultar sección]** o **[!UICONTROL Mostrar sección]**.
   * Oculte o muestre el campo personalizado haciendo clic en el menú de **Más** ![Más botón](assets/more-button-small.png) situado a la derecha del nombre de la sección del campo personalizado y, a continuación, haciendo clic en **[!UICONTROL Ocultar campo personalizado]** o **[!UICONTROL Mostrar campo personalizado]**.
   * Cambie el orden de los campos mediante las flechas arriba/abajo que se muestran a la derecha de sus nombres (si ha añadido varios campos en una sección).

1. Haga clic en la ficha **[!UICONTROL Reglas de visibilidad]**.

   Las reglas de visibilidad le permiten dictar qué campos adicionales se muestran en función de la finalización del campo personalizado inicial. Por ejemplo, si el campo dependiente es A y el campo de control es X, significa que el campo A solo estará visible si se ha completado el campo X.

   Puede utilizar valores de control para determinar los valores del campo de control que, si se seleccionan, hacen que el campo dependiente sea visible. Por ejemplo, imaginemos que el campo dependiente es A y el campo de control es X y que los valores de control en X se establecen únicamente como opciones 1 y 2. Esto significa que el campo A solo estará visible si se selecciona la opción 1 o 2 del campo X. Además, si se seleccionan las opciones 3 o 4 del campo X, el campo A no se muestra.

   >[!NOTE]
   >
   >Solo se pueden utilizar tipos de campo personalizados Lista y Radio para el campo de control en una regla de visibilidad, mientras que el campo dependiente puede ser cualquier tipo de campo.

   Para añadir una regla de visibilidad:

   1. Haga clic en **[!UICONTROL Nueva regla de visibilidad]** para el módulo al que desee agregar la regla.

   1. Seleccione la configuración que desee para la regla y haga clic en **[!UICONTROL Guardar]**.

1. Abra la pestaña **[!UICONTROL Reglas de dependencia]**.

   Las reglas de dependencia permiten determinar las opciones disponibles en el campo dependiente cuando se seleccionan determinadas opciones en el campo de control. Por ejemplo, si el campo dependiente es &quot;B&quot; y el campo de control es &quot;Y&quot;, podría configurarlo de la siguiente manera:

   * Si se elige la opción 1 del campo Y, solo se muestran las opciones 1 y 2 del campo B.

   * Si se elige la opción 2 del campo Y, solo se muestran las opciones 3 y 4 del campo B.

   >[!NOTE]
   >
   >Solo se pueden utilizar los tipos de campo personalizados Lista y Radio para los campos dependientes y de control en una regla de dependencia.

   Para añadir una regla de dependencia:

   1. Haga clic en **[!UICONTROL Nueva regla de dependencia]** para el módulo al que desee agregar la regla.

   1. Seleccione la configuración que desee para la dependencia y, a continuación, haga clic en **[!UICONTROL Guardar]**.

## Administración de los campos personalizados

Puede ver y editar los detalles de la sección Campo personalizado o de los campos personalizados individuales.

{{step1-to-proofing}}

1. En la esquina superior derecha de la página, haga clic en **Configuración de la cuenta**.

1. En la página **Configuración de cuenta**, seleccione la pestaña **Campos personalizados**.

1. Haga clic en el nombre de la sección del campo personalizado o del campo personalizado individual.

1. (Condicional) Si va a administrar una sección de campos personalizados, realice cualquiera de los siguientes cambios en la página **[!UICONTROL Sección de campos personalizados]**:

   * Edite el nombre de la sección.
   * Muévala a un módulo diferente.
   * Oculte/muestre la sección.

1. (Condicional) Si va a administrar un campo personalizado, realice cualquiera de los cambios siguientes en la página **[!UICONTROL Campo personalizado]**:

   * Mueva el campo a una sección diferente.
   * Edite el nombre del campo.
   * Editar texto de ayuda.
   * Habilite/deshabilite la configuración **[!UICONTROL Obligatoria]** en el campo.
   * (Condicional) Habilite/deshabilite la configuración **[!UICONTROL Buscable]** en el campo.
   * Oculte/muestre el campo.
   * Edite el tipo de campo.
   * Establezca/edite un valor predeterminado para el campo.
   * Configure las reglas de visibilidad y dependencia.
