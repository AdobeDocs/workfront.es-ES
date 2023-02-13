---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Cree y administre campos personalizados en [!DNL Workfront Proof]
description: Seleccione o Premium [!DNL Workfront] Se requiere un plan para utilizar esta función. Para obtener más información sobre los distintos planes disponibles, consulte Planes de Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# Cree y administre campos personalizados en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Seleccione o Premium [!DNL Workfront] Se requiere un plan para utilizar esta función. Para obtener más información sobre los distintos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

Los campos personalizados permiten capturar datos adicionales al crear una nueva prueba, un nuevo usuario o un nuevo invitado.

Por ejemplo, es posible que los usuarios que crean una prueba nueva deseen incluir una sección adicional que les permita capturar un número de trabajo, un código de departamento o una referencia de proveedor.

>[!NOTE]
>
>* La captura de este tipo de información en la página New proof a través de los campos Custom también le permitirá reducir la longitud del nombre de prueba, ya que estos detalles no tendrán que incluirse en el nombre. Para obtener información sobre la página Nueva prueba, consulte &quot;Creación de pruebas en [!DNL Workfront Proof].&quot;
>
>Una vez que se ha utilizado un campo personalizado en una prueba, un usuario o un contacto, no se puede eliminar ni editar el tipo de campo. Sin embargo, puede ocultarlo (a través del [!UICONTROL Configuración de campos personalizados] ) para que no se utilice en elementos nuevos.
>
>Si oculta una sección de campo personalizado, todos los campos de la sección también se ocultarán aunque los campos individuales estén definidos como visibles.

Este artículo explica cómo hacer lo siguiente:

## Crear campos personalizados

En primer lugar, debe configurar la sección Campo personalizado a la que desea agregar campos personalizados.

1. Haga clic en **[!UICONTROL Configuración]** >**[!UICONTROL Configuración de la cuenta]** y, a continuación, abra el **[!UICONTROL Campos personalizados]** pestaña .

1. Haga clic en **[!UICONTROL Agregar sección de campo personalizado]** en el módulo correspondiente (prueba, usuarios o contactos).
1. Tipo a **Nombre** para la sección campo personalizado , haga clic en **[!UICONTROL Guardar]**.

   Ahora puede configurar campos personalizados dentro de la sección :

1. Haga clic en el **[!UICONTROL Configuración de campos personalizados]** para actualizar la página.
1. Haga clic en la sección del nombre del nuevo campo personalizado para abrir el **[!UICONTROL Campo personalizado] sección** para la nueva sección.
1. Haga clic en el **[!UICONTROL Nuevo campo personalizado]** cerca de la esquina superior derecha.
1. En el **[!UICONTROL Nuevo campo personalizado]** que aparece, especifique los detalles del campo personalizado:

   | **Obligatorio** | Workfront requiere que los usuarios completen el campo. |
   |---|---|
   | **Buscable** | Permite a los usuarios encontrar elementos buscando en los datos de campo personalizados. |
   | **Oculto** | Oculta el campo personalizado del [!UICONTROL Nueva prueba], Cliente nuevo y [!UICONTROL Nuevo usuario] páginas |

   {style=&quot;table-layout:auto&quot;}

1. Haga clic en **[!UICONTROL Guardar]**.
1. En el **Campo personalizado** que aparecerá, haga clic en la **[!UICONTROL Configuración de campos personalizados]** para actualizar la página.

1. Realice cualquier otro cambio en la configuración del campo:

   * Oculte o muestre la sección de campos personalizados haciendo clic en el botón **[!UICONTROL Más]** menú (tres puntos) a la derecha del nombre de la sección del campo personalizado y, a continuación, haga clic en **[!UICONTROL Ocultar sección]** o **[!UICONTROL Mostrar sección]**.

   * Oculte o muestre el campo personalizado haciendo clic en el botón **[!UICONTROL Más]** menú (tres puntos) a la derecha del nombre de la sección del campo personalizado y, a continuación, haga clic en **[!UICONTROL Ocultar campo personalizado]** o **[!UICONTROL Mostrar campo personalizado]**.

   * Cambie el orden de los campos con las flechas arriba/abajo que se muestran a la derecha de sus nombres (si ha añadido varios campos en una sección).

1. Abra el **[!UICONTROL Reglas de visibilidad]** pestaña .\
   Las reglas de visibilidad permiten dictar qué campos adicionales se muestran, según la finalización del campo personalizado inicial. Por ejemplo, si el campo dependiente es A y el campo Control es X, significa que el Campo A solo estará visible si se completa el campo X.

   Puede utilizar valores de control para determinar los valores del campo de control que, si se seleccionan, harán que el campo dependiente sea visible. Por ejemplo, imagine que el campo dependiente es A y que el campo de control es X, y que los valores de control en X son solo las opciones 1 y 2. Esto significa que el campo A solo estará visible si se selecciona la opción 1 o 2 del campo X. Esto significa que si se seleccionan las opciones 3 o 4 del campo X, el campo A no se muestra. Abra el **[!UICONTROL Reglas de visibilidad]** pestaña .

   Para añadir una regla de visibilidad:

   1. Haga clic en **[!UICONTROL Nueva regla de visibilidad]** para el módulo en el que desea agregar la regla.
   1. Seleccione la configuración que desee para la regla y haga clic en **[!UICONTROL Guardar]**.

1. Abra el **[!UICONTROL Reglas de dependencia]** pestaña .

   Las reglas de dependencia permiten determinar las opciones disponibles en el campo dependiente cuando se seleccionan determinadas opciones en el campo de control. Por ejemplo, si el campo dependiente es &quot;B&quot; y el campo de control es &quot;Y&quot;, puede configurarlo de la siguiente manera:

   Si se elige la opción 1 en el campo Y, solo se muestran las opciones 1 y 2 en el campo B.

   Si se elige la opción 2 en el campo Y, solo se muestran las opciones 3 y 4 en el campo B.

   Para agregar una regla de dependencia:

   1. Haga clic en **[!UICONTROL Nueva regla de dependencia]** para el módulo que desea agregar la regla.
   1. Seleccione la configuración que desee para la dependencia y haga clic en **[!UICONTROL Guardar]**.

## Administrar los campos personalizados

Puede ver y editar los detalles de la sección Campo personalizado o los campos personalizados individuales.

1. Haga clic en **[!UICONTROL Configuración]** >**[!UICONTROL Configuración de la cuenta]** y, a continuación, abra el **[!UICONTROL Campos personalizados]** pestaña .

1. Haga clic en el nombre de la sección de campos personalizados o del campo personalizado individual.
1. (Condicional) Si está administrando una sección de campos personalizados, realice cualquiera de los cambios siguientes en la sección **[!UICONTROL Sección Campo personalizado]** página:

   * Edite el nombre de la sección.
   * Muévalo a un módulo diferente.
   * Ocultar/mostrar la sección.

1. (Condicional) Si está administrando un campo personalizado, realice cualquiera de los siguientes cambios en la variable **[!UICONTROL Campo personalizado]** página:

   * Mueva el campo a otra sección.
   * Edite el nombre del campo.
   * Texto de ayuda de entrada (aparecerá un icono de signo de interrogación junto a la sección de campos y el texto aparecerá al pasar el ratón).
   * Habilitar/deshabilitar el **[!UICONTROL Obligatorio]** en el campo .
   * Habilitar/deshabilitar el **[!UICONTROL Buscable]** en el campo .
   * Oculte/muestre el campo.
   * Edite el tipo de campo.
   * Defina o edite un valor predeterminado para el campo.
   * Configure las reglas de visibilidad y dependencia (como se describe anteriormente en los pasos 11 y 12).
