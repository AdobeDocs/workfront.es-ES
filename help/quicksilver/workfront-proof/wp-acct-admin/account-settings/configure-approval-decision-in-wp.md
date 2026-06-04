---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configuración de las opciones de decisión de aprobación en  [!DNL Workfront Proof]
description: Es posible configurar las opciones de decisión de aprobación de todas las pruebas creadas por los usuarios de  [!DNL Workfront Proof]  de la organización.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
TQID: https://experienceleague.adobe.com/byd7VyLV7IkwQ1YSHoQMHQNXOPAeJvP8-ENhHBvo01A
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 462
ht-degree: 85%

---

# Configuración de las opciones de decisión de aprobación en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Como administrador de [!DNL Workfront Proof] que usa un plan de edición Select o Premium, puede configurar las opciones de decisión de aprobación de las siguientes maneras para todas las pruebas creadas por los usuarios de [!DNL Workfront Proof] de la organización:

* Cambiar el nombre de la decisión
* Cambiar el orden de las decisiones que se muestran en el visor de revisión
* Decidir qué decisiones se mostrarán

En este artículo se explica lo siguiente:

## Establecimiento de las decisiones de configuración

1. Haga clic en **[!UICONTROL Configuración de la cuenta]**.
1. Abra la pestaña **[!UICONTROL Decisiones]**.
1. Realice cualquiera de los siguientes cambios:

   * Para ocultar una decisión, haga clic en **[!UICONTROL Ocultar]**, a la derecha de la decisión que no necesite.
   * Para cambiar el nombre de una decisión, haga clic en el nombre de la decisión, edítela y, a continuación, haga clic fuera del cuadro (o presione Entrar). [!DNL Workfront Proof] actualizará el nombre de la decisión en todas las pruebas existentes del sistema.

     >[!IMPORTANT]
     >
     >Conserve la lógica de una decisión cuando le cambie el nombre. Por ejemplo, la decisión predeterminada “Rechazado” podría cambiarse por “Se requiere una nueva versión”, pero no debería cambiarse por “Enviar a impresoras”).

     En caso de querer volver a los valores predeterminados de [!DNL Workfront Proof], haga clic en Restaurar decisiones predeterminadas.

>[!NOTE]
>
>* La lógica que hay detrás de las decisiones se usa para calcular el estado general de un flujo de trabajo de prueba en caso de haber varias decisiones de varios niveles.
>* Las decisiones “Aprobado” y “Aprobado con cambios” activan la siguiente fase de un flujo de trabajo automático.
>* Al cambiar el nombre de una decisión y querer verificar la lógica, es posible hacer clic en **[!UICONTROL Actividad]**, en el panel de navegación izquierdo, y comprobar el registro de actividad donde se muestran las decisiones originales entre corchetes.
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## Creación de motivos de decisión

Los motivos de decisión son una buena manera de recopilar información adicional de decisiones sobre una prueba.

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]**.

1. Abra la ficha **[!UICONTROL Decisiones]**.
De forma predeterminada, los motivos están disponibles para todos los responsables de la toma de decisiones en sus pruebas, pero solo puede restringirlos a los responsables de la toma de decisiones principales.
Según sus necesidades, puede permitir que se seleccionen varios motivos o puede convertirla en una sola lista de selección. También puede hacer que los motivos sean obligatorios, lo que significa que los revisores tendrán que elegir un motivo antes de que se les permita guardar su decisión en una prueba.
   ![Reasons_setup.png](assets/reasons-setup-350x121.png)

1. En la sección **[!UICONTROL Motivos]**, haga clic en **[!UICONTROL Nuevo motivo]**.
   ![New_reason.png](assets/new-reason-350x135.png)

1. Escriba un título para la sección de motivos en el cuadro que aparece en **[!UICONTROL Motivo]**.
1. Si desea incluir un cuadro de texto, seleccione **[!UICONTROL Incluir cuadro de texto]**.
1. Haga clic en **[!UICONTROL Guardar]**.
   ![reason_setup_2.png](assets/reasons-setup-2-350x146.png)
El paso más importante es seleccionar las decisiones por las que los motivos deben mostrarse. Si se olvida de hacerlo, los motivos no aparecerán en las pruebas.

1. Marque las casillas en la columna **[!UICONTROL Motivos de visualización]** de la lista de decisiones en la parte superior de la página. Puede seleccionar una o más decisiones por los motivos que desee.
   ![reasons_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## Creación de un mensaje posterior a la decisión

Es posible crear un mensaje posterior a la decisión para que se muestre después de que un revisor guarde su decisión sobre la prueba.

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]**.

1. Abra la pestaña **[!UICONTROL Decisiones]**.
1. En la sección **[!UICONTROL Mensaje de decisión posterior]**, haga clic en **[!UICONTROL Editar]** al final de la fila **[!UICONTROL Mensaje]**.
También puede decidir si desea que el mensaje se muestre a todos los responsables de la toma de decisiones o si desea limitarlo al responsable de la toma de decisiones principal.
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. En la columna **[!UICONTROL Mostrar mensaje]**, especifique las decisiones en las que se debe mostrar este mensaje.
Si no selecciona al menos una decisión, el mensaje no se mostrará en las pruebas. Asegúrese de marcar al menos una casilla en esta columna.
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
