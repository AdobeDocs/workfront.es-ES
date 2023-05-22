---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Previsualizar entorno de prueba de zona protegida - [!DNL Workfront Proof]
description: La zona protegida de vista previa es un entorno de prueba que sirve como réplica del entorno en directo y se actualiza cada fin de semana con [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Previsualizar entorno de prueba de zona protegida - [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

La zona protegida de vista previa es un entorno de prueba que sirve como réplica del entorno en directo y se actualiza cada fin de semana con [!DNL Workfront Proof].

## Explicación de la zona protegida de previsualización

La zona protegida de vista previa sirve como entorno en el que los usuarios de su organización pueden probar y trabajar con seguridad con datos del entorno de producción sin afectar al entorno de producción. Es ideal para ejecutar sesiones de formación, probar nuevas funciones y determinar la funcionalidad de la configuración.

Además, las nuevas funciones del producto se cargan en el entorno de vista previa de espacio aislado antes de enviarse al entorno de producción. Los usuarios pueden probar las nuevas funciones allí sin afectar al flujo de trabajo habitual en el entorno de producción.

La zona protegida de vista previa contiene los datos de producción reales. Los datos fluyen de Producción a Vista previa y no a la inversa. Se actualiza cada fin de semana, por lo que los datos pueden retrasarse hasta una semana respecto al entorno de producción. Los elementos creados desde la última actualización se encuentran en el entorno de vista previa de espacio aislado hasta la siguiente actualización.

## Acceso a la zona protegida de previsualización

De forma predeterminada, como administrador del sistema, tiene acceso al entorno de vista previa de espacio aislado. Si no puede acceder al entorno de vista previa de espacio aislado como se describe en esta sección, póngase en contacto con su [!DNL Workfront] o a nuestro equipo de asistencia.

* [Acceso a la zona protegida de vista previa como independiente [!DNL Workfront Proof] Cliente](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Acceso a la vista previa de espacio aislado como [!DNL Workfront]+[!DNL Workfront Proof] Cliente](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Acceso a la zona protegida de vista previa como independiente [!DNL Workfront Proof] Cliente

1. Vaya a esta dirección URL:  `https://preview.proofhq.com`.
1. Inicie sesión con sus credenciales de vista previa.\
   Las credenciales de vista previa deben ser las mismas que las de producción, a menos que las haya cambiado en Producción después de la actualización de la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización, que tiene lugar cada fin de semana. No se sincronizan automáticamente.

### Acceso a la vista previa de espacio aislado como [!DNL Workfront+Workfront] Cliente de revisión

Como administrador del sistema, puede acceder a las [!DNL Workfront Proof] Vista previa de zona protegida mediante [!DNL Workfront] interfaz.

Para acceder a [!DNL Workfront Proof] Previsualizar zona protegida:

1. Inicie sesión en su [!DNL Workfront] entorno.
1. Clic **[!UICONTROL Configurar]** en la barra de navegación global.
1. Clic **[!UICONTROL Sistema]** >**[!UICONTROL Preferencias]**.

1. En el **[!UICONTROL Entornos de prueba]** , haga clic en **[!UICONTROL Previsualización de zona protegida]**.

1. Inicie sesión con sus credenciales de vista previa.\
   Las credenciales de vista previa deben ser las mismas que las de producción, a menos que las haya cambiado en Producción después de actualizar la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.
1. Haga clic en [!DNL Workfront Proof] en la barra de navegación global.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   El [!DNL Workfront Proof] Muestra el entorno de vista previa.

## Recepción de correos electrónicos desde la zona protegida de previsualización

Las notificaciones por correo electrónico nunca se activan desde [!DNL Workfront Proof] Entorno de vista previa.
