---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Crear y administrar campos personalizados en  [!DNL Workfront Proof]
description: Se requiere un plan Select o Premium [!DNL Workfront] para usar esta función. Para obtener más información sobre los distintos planes disponibles, consulte Planes de Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 6e6cc1db8f89b76d9903905e6ee4cf9014727ba1
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 0%

---

# Crear y administrar campos personalizados en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Se requiere un plan Select o Premium [!DNL Workfront] para utilizar esta función. Para obtener más información sobre los diversos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

Los campos personalizados le permiten capturar datos adicionales al crear una nueva prueba, un nuevo usuario o un nuevo invitado.

Por ejemplo, es posible que los usuarios que creen una nueva prueba deseen incluir una sección adicional que les permita capturar un número de trabajo, un código de departamento o una referencia de proveedor.

>[!NOTE]
>
>* Capturar este tipo de información en la página Nueva prueba a través de Campos personalizados también le permitirá reducir la longitud del nombre de la prueba, ya que estos detalles no tienen que incluirse en el nombre. Para obtener información acerca de la página Nueva prueba, vea &quot;Crear pruebas en [!DNL Workfront Proof]&quot;.
>
>Una vez que se ha utilizado un campo personalizado en una prueba, un usuario o un contacto, no se puede eliminar ni editar el tipo de campo. Sin embargo, podrá ocultarlo (a través de la página [!UICONTROL Configuración de campo personalizado]) para que no se utilice en elementos nuevos.
>
>Si oculta una sección de campo personalizado, todos los campos de la sección también se ocultarán aunque los campos individuales estén configurados como visibles.

Este artículo explica cómo hacer lo siguiente:

## Creación de campos personalizados

Primero, debe configurar la sección Campo personalizado a la que agregará campos personalizados.

1. Haga clic en **[!UICONTROL Configuración]** >**[!UICONTROL Configuración de la cuenta]** y, a continuación, abra la ficha **[!UICONTROL Campos personalizados]**.

1. Haga clic en **[!UICONTROL Agregar sección de campo personalizado]** en el módulo correspondiente (Prueba, Usuarios o Contactos).
1. Escriba un **Nombre** para la sección de campo personalizado y haga clic en **[!UICONTROL Guardar]**.

   Ahora puede configurar campos personalizados dentro de la sección:

1. Haga clic en la ficha **[!UICONTROL Configuración de campos personalizados]** para actualizar la página.
1. Haga clic en el nombre de la nueva sección de campo personalizado para abrir la página **[!UICONTROL Campo personalizado] sección** para la nueva sección.
1. Haga clic en **[!UICONTROL Nuevo campo personalizado]** cerca de la esquina superior derecha.
1. En la página **[!UICONTROL Nuevo campo personalizado]** que aparece, especifique los detalles del campo personalizado:

   | **Obligatorio** | Workfront requiere que los usuarios completen el campo. |
   |---|---|
   | **Se puede buscar** | Permite a los usuarios encontrar elementos buscando en los datos del campo personalizado. |
   | **Oculto** | Oculta el campo personalizado en las páginas [!UICONTROL Nueva prueba], Nuevo invitado y [!UICONTROL Nuevo usuario] |

   {style="table-layout:auto"}

1. Haga clic en **[!UICONTROL Guardar]**.
1. En la página **Campo personalizado** que aparece, haga clic en la ficha **[!UICONTROL Configuración de campos personalizados]** para actualizar la página.

1. Realice más cambios en la configuración del campo:

   * Oculte o muestre la sección de campo personalizado haciendo clic en el menú **[!UICONTROL Más]** (tres puntos) a la derecha del nombre de la sección de campo personalizado y, a continuación, haciendo clic en **[!UICONTROL Ocultar sección]** o **[!UICONTROL Mostrar sección]**.

   * Oculte o muestre el campo personalizado haciendo clic en el menú **[!UICONTROL Más]** (tres puntos) a la derecha del nombre de sección del campo personalizado y, a continuación, haciendo clic en **[!UICONTROL Ocultar campo personalizado]** o **[!UICONTROL Mostrar campo personalizado]**.

   * Cambie el orden de los campos mediante las flechas arriba/abajo que se muestran a la derecha de sus nombres (si ha agregado varios campos en una sección).

1. Abra la pestaña **[!UICONTROL Reglas de visibilidad]**.\
   Las reglas de visibilidad permiten dictar qué campos adicionales se muestran, según la finalización del campo personalizado inicial. Por ejemplo, si el campo dependiente es A y el campo de control es X, significa que el campo A solo estará visible si el campo X está completado.

   Puede utilizar valores de control para determinar los valores del campo de control que, si se seleccionan, hacen que el campo dependiente sea visible. Por ejemplo, imaginemos que el campo dependiente es A y el campo de control es X y que los valores de control de X se establecen únicamente como opciones 1 y 2. Esto significa que el campo A solo estará visible si se selecciona la opción 1 o 2 del campo X. Esto significa que si se seleccionan las opciones 3 o 4 del campo X, el campo A no se muestra. Abra la pestaña **[!UICONTROL Reglas de visibilidad]**.

   >[!NOTE]
   >
   >Solo se pueden utilizar tipos de campo personalizados Lista y Radio para el campo de control en una regla de visibilidad, mientras que el campo dependiente puede ser cualquier tipo de campo.

   Para añadir una regla de visibilidad:

   1. Haga clic en **[!UICONTROL Nueva regla de visibilidad]** para el módulo donde quiera agregar la regla.
   1. Seleccione la configuración que desee para la regla y haga clic en **[!UICONTROL Guardar]**.

1. Abra la ficha **[!UICONTROL Reglas de dependencia]**.

   Las reglas de dependencia permiten determinar las opciones disponibles en el campo dependiente cuando se seleccionan determinadas opciones en el campo de control. Por ejemplo, si el campo dependiente es &quot;B&quot; y el campo de control es &quot;Y&quot;, puede configurarlo de la siguiente manera:

   Si se elige la opción 1 del campo Y, solo se muestran las opciones 1 y 2 del campo B.

   Si se elige la opción 2 del campo Y, solo se muestran las opciones 3 y 4 del campo B.

   >[!NOTE]
   >
   >Solo se pueden utilizar tipos de campo personalizados Lista y Radio para los campos dependientes y de control en una regla de dependencia.

   Para agregar una regla de dependencia:

   1. Haga clic en **[!UICONTROL Nueva regla de dependencia]** para el módulo al que desee agregar la regla.
   1. Seleccione la configuración que desee para la dependencia y, a continuación, haga clic en **[!UICONTROL Guardar]**.

## Administrar los campos personalizados

Puede ver y editar los detalles de la sección Campo personalizado o de los campos personalizados individuales.

1. Haga clic en **[!UICONTROL Configuración]** >**[!UICONTROL Configuración de la cuenta]** y, a continuación, abra la ficha **[!UICONTROL Campos personalizados]**.

1. Haga clic en el nombre de la sección del campo personalizado o del campo personalizado individual.
1. (Condicional) Si está administrando una sección de campos personalizados, realice cualquiera de los siguientes cambios en la página **[!UICONTROL Sección de campos personalizados]**:

   * Edite el nombre de la sección.
   * Muévalo a un módulo diferente.
   * Ocultar/mostrar la sección.

1. (Condicional) Si está administrando un campo personalizado, realice cualquiera de los cambios siguientes en la página **[!UICONTROL Campo personalizado]**:

   * Mueva el campo a una sección diferente.
   * Edite el nombre del campo.
   * Introduzca el texto de ayuda (aparecerá un icono de signo de interrogación junto a la sección del campo y el texto aparecerá al pasar el ratón por encima).
   * Habilite/deshabilite la configuración **[!UICONTROL Obligatoria]** en el campo.
   * Habilite/deshabilite la configuración **[!UICONTROL en la que se pueden realizar búsquedas]** en el campo.
   * Ocultar/mostrar el campo.
   * Edite el tipo de campo.
   * Establezca/edite un valor predeterminado para el campo.
   * Configure las reglas de visibilidad y dependencia (como se describe en los pasos 11 y 12).
