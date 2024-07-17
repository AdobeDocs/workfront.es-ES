---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Configurar una revisión con un flujo de trabajo automatizado en  [!DNL Workfront Proof]
description: Esto repite la información que se encuentra en Configuración de pruebas en Workfront. Consolidar aquí o allá. Quizás mejor aquí.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1637'
ht-degree: 0%

---

# Configurar una revisión con un flujo de trabajo automatizado en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

El flujo de trabajo automatizado facilita la administración de la revisión y aprobación de contenido cuando tiene procesos de revisión complejos o si envía contenido para su revisión a los mismos grupos de personas con regularidad.

La prueba se crea y luego se mueve de una etapa a otra hasta la aprobación final. Se notifica a los usuarios correspondientes cada vez que se les requiere que realicen una aprobación.

![stages_Diagram.png](assets/stages-diagram-350x81.png)

Puede añadir un flujo de trabajo automatizado a una prueba al cargar el documento o después de cargarlo.

## Creación de una prueba con Flujo de trabajo automatizado

1. Empiece a crear la prueba.
1. En la sección **[!UICONTROL Compartir]**, haga clic en **[!UICONTROL Usar flujo de trabajo automatizado]**.

   Puede desmarcar esta opción para volver a un flujo de trabajo estándar.

1. (Opcional) Si desea usar una plantilla de flujo de trabajo automatizado que el administrador de [!DNL Workfront] haya configurado y compartido con usted, selecciónela en el menú desplegable **[!UICONTROL Seleccionar una plantilla de flujo de trabajo]**.

   >[!NOTE]
   >
   >Su capacidad para modificar la plantilla depende de la configuración de la plantilla establecida por el administrador de [!DNL Workfront]. Si la capacidad para modificar la plantilla está desactivada, solo el propietario de la plantilla puede modificarla.

1. Especifique la siguiente información para configurar la primera fase del flujo de trabajo automatizado:

   * **[!UICONTROL Nombre]:** El nombre de la fase aparece en el diagrama de flujo de trabajo y se incluye en las notificaciones por correo electrónico enviadas a los revisores.
   * **[!UICONTROL Plazo]:** La funcionalidad de este campo difiere según la opción que seleccione en la lista desplegable **[!UICONTROL Plazo calculado a partir de]**.

   * **[!UICONTROL Desde la creación de la prueba]:** Seleccione la fecha límite para la prueba.
   * **[!UICONTROL Desde la activación de la fase]:** Seleccione el número de días laborables que se agregarán a la fecha de activación de la fase para establecer automáticamente un plazo en la prueba.
   * **[!UICONTROL Activar fase]:** Para cada fase del flujo de trabajo, puede decidir cuándo debe activarse. Para su primera etapa, están disponibles las siguientes opciones.

      * Al crear la prueba
      * En una fecha y hora específicas
      * Manualmente\

        Hay opciones adicionales disponibles para las etapas siguientes. Estas opciones requieren una fase principal. Estos son:
      * Después de alcanzar el plazo anterior
      * Todas las decisiones se aprueban o aprueban con cambios
      * Todas las decisiones se aprueban
      * Todas las decisiones se toman
   * **[!UICONTROL Plazo calculado a partir de]:** La opción que seleccione en esta lista desplegable afecta a las opciones disponibles en el campo **[!UICONTROL Plazo]**.

   * **[!UICONTROL Creación de revisión]:** En el campo **[!UICONTROL Plazo]**, seleccione la fecha límite para la revisión.

   * **[!UICONTROL Activación de fase]:** En el campo **[!UICONTROL Plazo]**, seleccione el número de días laborables que se agregarán a la fecha de activación de fase para establecer automáticamente un plazo en la prueba.

   * **[!UICONTROL Bloquear fase]:** Seleccione cuándo se puede bloquear la fase.
   * **[!UICONTROL Responsable principal de la toma de decisiones]:** Seleccione el Responsable principal de la toma de decisiones en el escenario. Los responsables de la toma de decisiones solo están disponibles en la lista desplegable después de agregar revisores a la fase.
   * **[!UICONTROL Solo se requiere una decisión]:** Seleccione esta opción para que la revisión se complete después de que uno de los encargados de tomar decisiones tome la decisión.\

     Esta opción no está disponible si ha designado un usuario en el menú desplegable **[!UICONTROL Responsable principal de la toma de decisiones]**.

   * **[!UICONTROL Fase privada]:** Cuando se selecciona esta opción, los comentarios y las decisiones no son visibles para las personas que no se agregan a esta fase o que no son supervisores, administradores o administradores de facturación en la cuenta


1. (Opcional) Añada revisores a la fase.
1. Tenga en cuenta lo siguiente al agregar revisores:

   * Un revisor solo se puede agregar a una prueba una vez. (No se puede agregar a la misma persona a más de un paso de la prueba).
   * Los revisores que se agregan a una fase privada solo pueden ver la fase a la que se agregan en la prueba y los comentarios realizados en esa fase.
   * De forma predeterminada, añadir un usuario a una fase concede a ese usuario acceso para ver la prueba desde el momento en que se crea la prueba.\

     El administrador del sistema puede configurar el sistema de prueba para restringir el acceso de los usuarios a la prueba hasta que el flujo de trabajo entre en la fase en la que se agregó el usuario. Para obtener más información, consulte

1. (Opcional) Haga clic en **[!UICONTROL Nueva etapa]** y, a continuación, repita los pasos 4 y 5 para agregar varias etapas al flujo de trabajo automatizado.
1. Continúe creando la revisión especificando la información necesaria en las secciones [!UICONTROL Organizar] y [!UICONTROL Más configuraciones] de la página [!UICONTROL Nueva revisión], tal como se describe en

## Diagramas de flujo de trabajo automatizado

Al configurar el flujo de trabajo para la prueba, verá que se está creando un diagrama. Cada fase que añada a la prueba aparecerá en el diagrama, lo que indica claramente las dependencias entre las fases. Las etapas privadas están marcadas con un icono de clave.

El diagrama flota, lo que significa que permanecerá visible incluso si se desplaza hacia abajo por la página.

Si no necesita ver el diagrama, puede ocultarlo (1).

![Diagrama.png](assets/diagram-350x93.png)

## Añadir una fase

Puede añadir una fase adicional a un flujo de trabajo que esté creando o modificando.

1. Si está agregando una fase a una revisión existente, vaya a la página de detalles de revisión, como se describe en [Administrar detalles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. En la sección **[!UICONTROL Flujo de trabajo]**, haga clic en **[!UICONTROL Nueva etapa]**.

1. Especifique información para la fase como en el paso 4 en la sección [!UICONTROL Creación de una prueba con un flujo de trabajo automatizado] de este artículo.
1. Haga clic en **[!UICONTROL Agregar fase]** y luego haga clic en **[!UICONTROL Listo]**.

## Eliminación de una fase

1. Haga clic en el icono de papelera disponible en la esquina superior derecha del escenario (1).\
   El icono aparece cuando pasa el ratón por encima del escenario.\
   ![eliminando_a_stage.png](assets/deleting-a-stage-350x250.png)

## Configuración del escenario

* **[!UICONTROL Nombre de fase]**: aparece en el diagrama de flujo de trabajo y se incluye en las notificaciones por correo electrónico enviadas a los revisores.
* **[!UICONTROL Activar fase]**: Para cada fase del flujo de trabajo, puede decidir cuándo se debe activar. Para su primera etapa, estarán disponibles las siguientes opciones:

   * Al crear la prueba
   * En una fecha y hora específicas
   * Manualmente
   * Solo estas tres opciones están disponibles para la primera etapa. Las demás opciones estarán disponibles cuando añada una segunda fase; requieren que seleccione una fase principal.
   * Una vez alcanzada la fecha límite anterior (requiere la selección de una fase principal)
   * Todas las decisiones son Aprobadas o [!UICONTROL Aprobadas con cambios] (requiere la selección de una etapa principal)
   * Todas las decisiones son Aprobadas (requiere seleccionar una etapa principal)
   * Todas las decisiones se toman (requiere elegir una etapa principal)

* **[!UICONTROL Plazo]:** Puede decidir cómo se debe calcular el plazo en cada fase de un flujo de trabajo. Las opciones son:

   * Desde la creación de la prueba: en el campo [!UICONTROL deadline] (9) puede seleccionar la fecha límite para la prueba.
   * Desde la activación de la fase: en el menú desplegable [!UICONTROL deadline], seleccione el número de días hábiles que se agregarán a la fecha de activación de la fase para establecer automáticamente una fecha límite en la prueba.

* **[!UICONTROL Bloquear]:** Hay varias opciones que determinan cuándo se puede bloquear una fase. Las opciones incluyen:

   * Bloqueo manual
   * Nunca
   * Cuando comience la siguiente etapa
   * Cuando se toman todas las decisiones

**[!UICONTROL Responsable principal de la toma de decisiones]**: Usted establece el Responsable principal de la toma de decisiones en el escenario. Los responsables de la toma de decisiones disponibles aparecen en la lista solo después de agregar los revisores a la fase.

>[!NOTE]
>
>Si elige un responsable principal de la toma de decisiones, solo una opción de decisión requerida dejará de estar disponible en esta fase.

* **[!UICONTROL Solo se requiere una decisión]**: puede habilitar esta opción en un escenario. Esto significa que la revisión se completará una vez que uno de los responsables de la toma de decisiones tome su decisión.
* **[!UICONTROL Privacidad]:** Cada etapa puede hacerse privada. Si una fase es privada, los comentarios y las decisiones no serán visibles para las personas que no se hayan añadido a esta fase o que no sean supervisores, administradores o administradores de facturación en la cuenta. Para obtener más información, consulte [Resumen del flujo de trabajo automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Adición de revisores a una fase

1. Introduzca un nombre de contacto o una dirección de correo electrónico en el campo de la parte inferior de cada fase.
1. Haga clic en el icono de signo más verde para añadirlos.
1. Establezca la función en la prueba.
1. Configure la alerta de correo electrónico.
1. Al configurar la primera fase, también tiene la opción de cambiar el Propietario de la prueba.

   >[!NOTE]
   >
   >* Un revisor solo se puede agregar a una prueba una vez. No se puede agregar a la misma persona a más de una etapa de la prueba.
   >* Los revisores que no se agregan a una fase privada no pueden ver la fase en la prueba ni en los comentarios realizados en esa fase.


## Conversión de una prueba en un flujo de trabajo automatizado

Puede convertir una prueba básica en Flujo de trabajo automatizado.

1. Haga clic en **[!UICONTROL Convertir a flujo de trabajo automatizado]** en la página [!UICONTROL Detalles de la revisión].
Una vez que la revisión se haya vuelto a procesar en Flujo de trabajo automatizado, todas las etapas estarán activas, serán públicas y su opción [!UICONTROL Bloquear etapa] se establecerá en Manual de manera predeterminada. Todas las fases permanecen asignadas a los usuarios y a su configuración.

   * Activar fase se establece en Al crear la prueba en cada fase.
   * La opción Deadline calculated from se establece en Proof creation en cada fase.
   * Si solo se seleccionó una opción de decisión en la prueba básica, se seleccionará en todas las etapas.
   * Si se seleccionó en la prueba básica [!UICONTROL toma de decisiones principal], las etapas con ese destinatario se establecen en ellas y todas las demás lo tienen en Ninguno.
   * El nombre del escenario sigue siendo el mismo.

## Añadir una plantilla adicional a un flujo de trabajo automatizado existente

Después de convertir una prueba básica en un flujo de trabajo automatizado, puede agregarle una plantilla adicional.

1. En la página Detalles de la revisión, en la sección Flujo de trabajo, haga clic en **[!UICONTROL Agregar plantilla].**

   * La configuración de la plantilla determina qué se puede hacer con una prueba a la que se agregó esta plantilla. Por ejemplo, si la plantilla tiene deshabilitadas las opciones [!UICONTROL Agregar una etapa y Agregar personas a las etapas], los botones para [!UICONTROL agregar etapa] y [!UICONTROL compartir prueba] no estarán visibles.
   * Si la opción [!UICONTROL Agregar una etapa] está deshabilitada en la plantilla determinada, después de agregarla el botón [!UICONTROL Agregar plantilla] no estará visible.
   * Cuando se añade una persona a un escenario en una plantilla de flujo de trabajo automatizado, pero también ya está presente en la prueba, si se aplica esta plantilla, el sistema la elimina del escenario automáticamente. Si no se añade ninguna otra persona a esta fase en particular, se muestra el siguiente error, ya que el sistema no permite añadir una fase vacía al flujo de trabajo.

     ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
