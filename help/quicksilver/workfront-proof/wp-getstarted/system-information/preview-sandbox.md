---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Entorno de prueba de espacio aislado de vista previa [!DNL Workfront Proof]
description: El espacio aislado de vista previa es un entorno de prueba que sirve como réplica del entorno en directo y se actualiza cada fin de semana antes de [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Entorno de prueba de espacio aislado de vista previa [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

El espacio aislado de vista previa es un entorno de prueba que sirve como réplica del entorno en directo y se actualiza cada fin de semana antes de [!DNL Workfront Proof].

## El simulador para pruebas de vista previa

El Simulador para pruebas de vista previa sirve como entorno en el que los usuarios de su organización pueden probar y trabajar de forma segura con los datos del entorno de producción sin afectar al entorno de producción. Es ideal para ejecutar sesiones de capacitación, probar nuevas funciones y determinar la funcionalidad de configuración.

Además, las nuevas funciones de producto se cargan en el entorno de espacio aislado de vista previa antes de entregarse al entorno de producción. Los usuarios pueden probar nuevas funciones sin afectar a su flujo de trabajo habitual en el entorno de producción.

El Simulador para pruebas de vista previa contiene los datos de producción reales. Los datos fluyen de Producción a Vista previa y no a la inversa. Se actualiza todos los fines de semana, por lo que los datos pueden estar hasta una semana después del entorno de producción. Los elementos creados desde la última actualización se encuentran en el entorno de espacio aislado de vista previa hasta la siguiente actualización.

## Acceso al Simulador para pruebas de vista previa

De forma predeterminada, como administrador del sistema, tiene acceso al entorno limitado de vista previa. Si no puede acceder al entorno de espacio aislado de vista previa como se describe en esta sección, póngase en contacto con su [!DNL Workfront] o nuestro equipo de asistencia.

* [Acceso al Simulador para pruebas de vista previa como independiente [!DNL Workfront Proof] Cliente](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Acceso al Simulador para pruebas de vista previa como un [!DNL Workfront]+[!DNL Workfront Proof] Cliente](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Acceso al Simulador para pruebas de vista previa como independiente [!DNL Workfront Proof] Cliente

1. Vaya a esta URL:  `https://preview.proofhq.com`.
1. Inicie sesión con sus credenciales de vista previa.\
   Las credenciales de Vista previa deben ser las mismas que las credenciales de producción a menos que las haya cambiado en Producción después de que se actualizara la Vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización, que se realiza cada fin de semana. No se sincronizan automáticamente.

### Acceso al Simulador para pruebas de vista previa como un [!DNL Workfront+Workfront] Cliente de prueba

Como administrador del sistema, puede acceder al [!DNL Workfront Proof] Vista previa del Simulador para pruebas mediante el [!DNL Workfront] interfaz.

Para acceder a la [!DNL Workfront Proof] Espacio aislado de vista previa:

1. Inicie sesión en su [!DNL Workfront] entorno.
1. Haga clic en **[!UICONTROL Configuración]** en la barra de navegación global.
1. Haga clic en **[!UICONTROL Sistema]** >**[!UICONTROL Preferencias]**.

1. En el **[!UICONTROL Entornos de prueba]** , haga clic en **[!UICONTROL Vista previa de Simulador para pruebas]**.

1. Inicie sesión con sus credenciales de vista previa.\
   Las credenciales de vista previa deben ser las mismas que las credenciales de producción a menos que las haya cambiado en Producción después de que se actualizara la vista previa. Los inicios de sesión solo se sincronizan cuando se produce una actualización. No se sincronizan automáticamente.
1. Haga clic en el [!DNL Workfront Proof] en la barra de navegación global.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   La variable [!DNL Workfront Proof] Se muestra el entorno de vista previa.

## Recibir correos electrónicos del Simulador para pruebas de vista previa

Las notificaciones por correo electrónico nunca se activan desde la variable [!DNL Workfront Proof] Entorno de vista previa.
