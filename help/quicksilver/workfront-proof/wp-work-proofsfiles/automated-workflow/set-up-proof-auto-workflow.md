---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Configure una prueba con un flujo de trabajo automatizado en [!DNL Workfront Proof]
description: Esto repite la información que se encuentra en Configuración de pruebas en Workfront. Consolidar aquí o allá. Quizás mejor aquí.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1637'
ht-degree: 0%

---

# Configure una prueba con un flujo de trabajo automatizado en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Flujo de trabajo automatizado le facilita la administración de la revisión y aprobación del contenido cuando tiene procesos de revisión complejos o si envía contenido para su revisión a los mismos grupos de personas regularmente.

La prueba se crea y luego se mueve de una etapa a otra hasta la aprobación final. Se notifica a los usuarios relevantes en cualquier momento para solicitar su aprobación.

![stage_chart.png](assets/stages-diagram-350x81.png)

Puede añadir un flujo de trabajo automatizado a una prueba al cargar el documento o después de cargar el documento.

## Crear una prueba con el flujo de trabajo automatizado

1. Comience a crear la prueba.
1. En el **[!UICONTROL Compartir]** , haga clic en **[!UICONTROL Uso del flujo de trabajo automatizado]**.

   Puede desmarcar esta opción para volver a un flujo de trabajo estándar.

1. (Opcional) Si desea utilizar una plantilla de flujo de trabajo automatizado que su [!DNL Workfront] administrador configurado y compartido con usted, selecciónelo en el **[!UICONTROL Seleccionar una plantilla de flujo de trabajo]** menú desplegable.

   >[!NOTE]
   >
   >Su capacidad para modificar la plantilla depende de la configuración de la plantilla configurada por el [!DNL Workfront] administrador. Si la capacidad de modificar la plantilla está deshabilitada, solo el propietario de la plantilla puede modificarla.

1. Especifique la siguiente información para configurar la primera etapa del flujo de trabajo automatizado:

   * **[!UICONTROL Nombre]:** El nombre del escenario aparece en el diagrama de flujo de trabajo y se incluye en las notificaciones por correo electrónico enviadas a los revisores.
   * **[!UICONTROL Fecha límite]:** La funcionalidad de este campo difiere según la opción seleccionada en la variable **[!UICONTROL Fecha límite calculada a partir de]** lista desplegable.

   * **[!UICONTROL Desde la creación de pruebas]:** Seleccione la fecha límite para la prueba.
   * **[!UICONTROL Desde la activación del paso]:** Seleccione el número de días laborables que se agregarán a la fecha de activación del escenario para establecer automáticamente una fecha límite en la prueba.
   * **[!UICONTROL Activar etapa]:** Para cada etapa del flujo de trabajo, puede decidir cuándo se debe activar. Para la primera etapa, están disponibles las siguientes opciones.

      * Creación de pruebas
      * En una fecha y hora específicas
      * Manualmente\

         Hay opciones adicionales disponibles para etapas posteriores. Estas opciones requieren una etapa principal. Son:
      * Después de alcanzar la fecha límite anterior
      * Todas las decisiones son aprobadas o aprobadas con cambios
      * Todas las decisiones son aprobadas
      * Todas las decisiones se toman
   * **[!UICONTROL Fecha límite calculada a partir de]:** La opción seleccionada en esta lista desplegable afecta a las opciones disponibles en la **[!UICONTROL Fecha límite]** campo .

   * **[!UICONTROL Creación de prueba]:** En el **[!UICONTROL Fecha límite]** , seleccione la fecha límite para la prueba.

   * **[!UICONTROL Activación del escenario]:** En el **[!UICONTROL Fecha límite]** , seleccione el número de días hábiles que se agregarán a la fecha de activación del escenario para establecer automáticamente una fecha límite en la prueba.

   * **[!UICONTROL Bloqueo del escenario]:** Seleccione cuándo se puede bloquear el escenario.
   * **[!UICONTROL Creador de decisiones principal]:** Seleccione el responsable de la toma de decisiones principal en el escenario. Los responsables de la toma de decisiones solo están disponibles en la lista desplegable después de agregar revisores a la etapa.
   * **[!UICONTROL Solo se requiere una decisión]:** Seleccione esta opción para que la revisión se complete después de que uno de los responsables de la toma de decisiones tome su decisión.\

      Esta opción no está disponible si ha designado un usuario en la variable **[!UICONTROL Creador de decisiones principal]** menú desplegable.

   * **[!UICONTROL Fase privada]:** Cuando se selecciona esta opción, los comentarios y las decisiones no son visibles para las personas que no se agregan a esta etapa o que no son supervisores, administradores ni administradores de facturación en la cuenta


1. (Opcional) Agregue revisores al escenario.
1. Tenga en cuenta lo siguiente al agregar revisores:

   * Un revisor se puede agregar a una prueba solo una vez. (No se puede añadir la misma persona a más de un paso de la prueba).
   * Los revisores que se añaden a un escenario privado solo pueden ver la fase a la que se añaden en la prueba y los comentarios realizados en ese escenario.
   * De forma predeterminada, agregar un usuario a una etapa concede a ese usuario acceso para ver la prueba desde el momento en que se crea la prueba.\

      El administrador del sistema puede configurar el sistema de pruebas para restringir el acceso de los usuarios a la prueba hasta que el flujo de trabajo entre en la fase en la que se agregó el usuario. Para obtener más información, consulte

1. (Opcional) Haga clic en **[!UICONTROL Nueva etapa]** y, a continuación, repita los pasos 4 y 5 para añadir varias etapas al flujo de trabajo automatizado.
1. Continúe creando la prueba especificando la información necesaria en la [!UICONTROL Organizar] y [!UICONTROL Más configuración] secciones de [!UICONTROL Nueva prueba] como se describe en

## Diagramas de flujo de trabajo automatizados

Al configurar el flujo de trabajo para la prueba, verá que se está creando un diagrama. Cada etapa que agregue a la prueba aparecerá en el diagrama, indicando claramente las dependencias entre las etapas. Los escenarios privados se marcan con un icono clave.

El diagrama flota, lo que significa que permanecerá visible aunque se desplace hacia abajo por la página.

Si no necesita ver el diagrama, puede ocultarlo (1).

![Diagrama.png](assets/diagram-350x93.png)

## Añadir un escenario

Puede añadir un paso adicional a un flujo de trabajo que esté creando o modificando.

1. Si está agregando un escenario a una prueba existente, vaya a la página de detalles de la prueba , tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. En el **[!UICONTROL Flujo de trabajo]** , haga clic en **[!UICONTROL Nueva etapa]**.

1. Especifique la información para la fase, como en el paso 4 de la sección [!UICONTROL Creación de una prueba con un flujo de trabajo automatizado] en este artículo.
1. Haga clic en **[!UICONTROL Agregar etapa]** y haga clic en **[!UICONTROL Listo]**.

## Eliminar un escenario

1. Haga clic en el icono de papelera disponible en la esquina superior derecha del escenario (1).\
   El icono aparece cuando pasa el ratón por encima del escenario.\
   ![delete_a_stage.png](assets/deleting-a-stage-350x250.png)

## Configuración de escenario

* **[!UICONTROL Nombre del escenario]**: Aparece en el diagrama de flujo de trabajo y se incluye en las notificaciones por correo electrónico enviadas a los revisores.
* **[!UICONTROL Activar etapa]**: Para cada etapa del flujo de trabajo, puede decidir cuándo se debe activar. Para la primera etapa, estarán disponibles las siguientes opciones:

   * Creación de pruebas
   * En una fecha y hora específicas
   * Manualmente
   * Solo estas tres opciones están disponibles para la primera etapa. Las demás opciones estarán disponibles cuando agregue una segunda etapa; requieren que seleccione una etapa principal.
   * Después de alcanzar la fecha límite anterior (requiere la selección de una etapa principal)
   * Todas las decisiones son aprobadas o [!UICONTROL Aprobado con cambios] (requiere la selección de una etapa principal)
   * Todas las decisiones son aprobadas (requiere la selección de una etapa principal)
   * Todas las decisiones se toman (requiere la selección de una etapa principal)

* **[!UICONTROL Fecha límite]:** Puede decidir cómo se debe calcular la fecha límite en cada etapa de un flujo de trabajo. Las opciones son:

   * Desde la creación de pruebas: En el [!UICONTROL límite] campo (9) puede seleccionar la fecha límite para la prueba.
   * Desde la activación del paso: En el [!UICONTROL límite] menú desplegable selecciona el número de días laborables que se agregarán a la fecha de activación del escenario para establecer automáticamente una fecha límite en la prueba.

* **[!UICONTROL Bloqueo]:** Hay varias opciones que determinan cuándo se puede bloquear un escenario. Las opciones incluyen:

   * Bloqueo manual
   * Nunca
   * Inicio de la siguiente etapa
   * Cuando se toman todas las decisiones

**[!UICONTROL Creador de decisiones principal]**: El responsable de la toma de decisiones principal se coloca en el escenario. Los responsables de la toma de decisiones disponibles aparecen en la lista solo después de agregar los revisores a la fase.

>[!NOTE]
>
>Si elige un responsable principal de la toma de decisiones, solo una opción requerida para la decisión dejará de estar disponible en esta fase.

* **[!UICONTROL Solo se requiere una decisión]**: Puede activar esta opción en un escenario. Esto significa que el examen se completará una vez que uno de los encargados de adoptar decisiones tome una decisión.
* **[!UICONTROL Privacidad]:** Cada etapa se puede convertir en privada. Si un escenario es privado, los comentarios y las decisiones no serán visibles para las personas que no se agreguen a este paso o que no sean supervisores, administradores o administradores de facturación en la cuenta. Para obtener más información, consulte [Resumen del flujo de trabajo automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Agregar revisores a una etapa

1. Introduzca un nombre de contacto o una dirección de correo electrónico en el campo situado en la parte inferior de cada etapa.
1. Haga clic en el icono verde más para añadirlos.
1. Establezca la función en la prueba.
1. Establezca la alerta de correo electrónico.
1. Al configurar la primera etapa, también tiene la opción de cambiar el propietario de la prueba.

   >[!NOTE]
   >
   >* Un revisor se puede agregar a una prueba solo una vez. No se puede añadir la misma persona a más de un paso de la prueba.
   >* Los revisores que no se agregan a un escenario privado no pueden ver el escenario de la prueba o los comentarios realizados en ese escenario.



## Conversión de una prueba en un flujo de trabajo automatizado

Puede convertir una prueba básica en Flujo de trabajo automatizado.

1. Haga clic en **[!UICONTROL Convertir en flujo de trabajo automatizado]** en el [!UICONTROL Detalles de la prueba] página.
Una vez que la prueba se ha modificado en Flujo de trabajo automatizado, todas las etapas son activas, públicas y [!UICONTROL Bloqueo del escenario] se establece en Manual de forma predeterminada. Todas las etapas permanecen con los usuarios y su configuración.

   * El paso Activar se establece en Al crear la prueba en cada etapa.
   * La fecha límite calculada a partir de la opción se establece en Proof creation in every stage.
   * Si solo se seleccionó una opción de decisión en la prueba básica, todas las etapas la tienen seleccionada.
   * Si en una prueba básica [!UICONTROL Creador de decisiones principal] se ha seleccionado, las etapas con ese destinatario se establecen en ellas y todas las demás tienen configurado como Ninguno.
   * El nombre del escenario sigue siendo el mismo.

## Añadir una plantilla adicional a un flujo de trabajo automatizado existente

Después de convertir una prueba básica en Flujo de trabajo automatizado, puede añadir una plantilla adicional.

1. En la página Detalles de la prueba , en la sección Flujo de trabajo , haga clic en **[!UICONTROL Agregar plantilla].**

   * La configuración de la plantilla determina lo que se puede hacer con una prueba a la que se agregó esta plantilla. Por ejemplo, si la plantilla tiene la variable [!UICONTROL Agregar un escenario y agregar personas a escenarios] opciones desactivadas, botones para [!UICONTROL añadir etapa] y [!UICONTROL compartir prueba] no será visible.
   * If [!UICONTROL Opción Añadir etapa] está desactivado en la plantilla dada, después de agregarla a la plantilla [!UICONTROL Agregar plantilla] no están visibles.
   * Cuando se añade una persona a una etapa de una plantilla de flujo de trabajo automatizado, pero también está presente en la prueba, si esta plantilla se aplica, el sistema elimina a esta persona de la fase automáticamente. Si no hay nadie más agregado a esta etapa en particular, se mostrará el siguiente error, ya que el sistema no permitirá añadir una etapa vacía al flujo de trabajo.

      ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
