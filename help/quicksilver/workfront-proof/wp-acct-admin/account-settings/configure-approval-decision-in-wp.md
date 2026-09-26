---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configuración de las opciones de decisión de aprobación en [!DNL Workfront Proof]
description: Puede configurar las opciones de decisión de aprobación para todas las pruebas creadas por [!DNL Workfront Proof] usuarios de su organización.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
TQID: 'https://experienceleague.adobe.com/byd7VyLV7IkwQ1YSHoQMHQNXOPAeJvP8-ENhHBvo01A'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 95%
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

1. Abra la pestaña **[!UICONTROL Decisiones]**.
De forma predeterminada, los motivos están disponibles para todos los responsables de la toma de decisiones en las pruebas, pero es posible restringir esto a solamente los responsables principales de la toma de decisiones.
Según las necesidades, es posible permitir que se seleccionen varios motivos o que haya una lista de selección única. También puede hacer que los motivos sean obligatorios, lo que significa que los revisores tendrán que elegir un motivo antes de que se les permita guardar la decisión sobre una prueba.
   ![Reasons_setup.png](assets/reasons-setup-350x121.png)

1. En la sección **[!UICONTROL Motivos]**, haga clic en **[!UICONTROL Nuevo motivo]**.
   ![New_reason.png](assets/new-reason-350x135.png)

1. Escriba un título para la sección de motivos en el cuadro que aparece en **[!UICONTROL Motivo]**.
1. Si desea incluir un cuadro de texto, seleccione **[!UICONTROL Incluir cuadro de texto]**.
1. Haga clic en **[!UICONTROL Guardar]**.
   ![reason_setup_2.png](assets/reasons-setup-2-350x146.png)
   El paso más importante es seleccionar las decisiones por las que los motivos deben mostrarse. Si se olvida de hacerlo, los motivos no aparecerán en las pruebas.

1. Marque las casillas en la columna **[!UICONTROL Motivos de visualización]** de la lista de decisiones en la parte superior de la página. Seleccione una o más decisiones para los motivos.
   ![reasons_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## Creación de un mensaje posterior a la decisión

Es posible crear un mensaje posterior a la decisión para que se muestre después de que un revisor guarde su decisión sobre la prueba.

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]**.

1. Abra la pestaña **[!UICONTROL Decisiones]**.
1. En la sección **[!UICONTROL Mensaje posterior a la decisión]**, haga clic en **[!UICONTROL Editar]**, al final de la fila **[!UICONTROL Mensaje]**.
También se puede decidir si se desea que el mensaje se muestre a todos los responsables de la toma de decisiones o limitarlo al responsable principal de la toma de decisiones.
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. En la columna **[!UICONTROL Mostrar mensaje]**, especifique las decisiones en las que se mostrará este mensaje.
Si no se selecciona al menos una decisión, el mensaje no se mostrará en las pruebas. Asegúrese de marcar al menos una casilla en esta columna.
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
