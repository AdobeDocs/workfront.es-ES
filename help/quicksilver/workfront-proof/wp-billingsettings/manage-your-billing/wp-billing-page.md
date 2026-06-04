---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: 'La página de facturación de revisión de  [!DNL Workfront] '
description: Para acceder a la página [!UICONTROL Facturación], abra el menú Configuración en la parte superior derecha de la pantalla y elija Facturación en el menú desplegable.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
TQID: https://experienceleague.adobe.com/o1VGrecH-BIItFQ0fvzpFYPILQ555TOhgOstI2ek9eo
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
source-wordcount: 610
ht-degree: 100%

---

# La página de facturación de [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión en [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

## La página de facturación

Para acceder a la página [!UICONTROL Facturación], abra el menú **[!UICONTROL Configuración]** en la parte superior derecha de la pantalla y elija **[!UICONTROL Facturación]** en el menú desplegable.

La página [!UICONTROL Facturación] contiene lo siguiente:

* Nombre de la cuenta (1)
* Lista de cuentas (por ejemplo, si tiene cuentas satélite)(2)
* Cambiar plan (3)
* Cambiar datos de pago (4)
* Nueva cuenta satélite (5)
* Cerrar cuenta (6)
* Información del plan actual (7)
* Contacto y dirección de facturación (8)
* Estadísticas de uso (9)
* Historial de facturación (10)
* Actividad de facturación (11)

  ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL Plan actual]

Esta sección (7) muestra los detalles de su plan actual, incluidos los siguientes:

* El nombre del plan
* Método de pago actual
* Fechas de inicio y finalización del plan actual
* Siguiente tipo de plan
* Método de pago del siguiente plan

  Para obtener más información, consulte [Elección de la forma de pago en  [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL Contacto y dirección de facturación]

Esta sección (8) muestra los detalles principales de contacto de facturación principal y de dirección de su cuenta.

El contacto de facturación solo se puede seleccionar entre los usuarios configurados como Administradores de facturación en su cuenta. En las cuentas satélite, solo se pueden definir en este campo los administradores de facturación de la cuenta principal.

![Billing_Contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> Puede tener varios administradores de facturación en su cuenta, pero solo uno de ellos, seleccionado en el campo [!UICONTROL Contacto de facturación], recibirá todas las notificaciones de facturación y alertas de uso de la cuenta.

Esto incluye los siguientes correos electrónicos de notificación:

* Uso de revisión
* Facturas
* Bajar de categoría
* Alerta de pago atrasado/suspensión de cuenta
* Error de tarjeta de crédito

  ![Billin_CC.png](assets/billin-cc-350x103.png)

El campo [!UICONTROL Facturación CC] también le permite añadir una dirección de correo electrónico para que se copie en todos los correos electrónicos relacionados con la facturación. Haga clic en el campo para activar la edición en línea e introduzca una dirección de correo electrónico de su elección (puede ser también la dirección de correo electrónico de un usuario existente).

## [!UICONTROL Dirección de facturación]

Esta sección utiliza la edición en línea, por lo que solo tiene que hacer clic en los campos para introducir o editar el texto.

>[!NOTE]
>
> Incluimos esta dirección en sus facturas de suscripción para asegurarse de que estos datos estén siempre actualizados.

![Billing_Address.png](assets/billing-address-350x199.png)

## [!UICONTROL Estadísticas de uso]

Esta sección muestra las estadísticas de uso de su cuenta dentro del período de facturación actual, incluidas las siguientes:

* Almacenamiento utilizado
* Pruebas utilizadas
* Límite de usuarios utilizado

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL Advertencias de uso]

Los [[!UICONTROL perfiles de permisos de prueba] en [!DNL Workfront] Prueba](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) establecidos como contacto de facturación (1) en su cuenta recibirán una notificación por correo electrónico cuando esta llegue a:

* Un 75 % y, posteriormente, un 98 % de la capacidad de almacenamiento
* Un 75% y, posteriormente, un 100 % del límite de pruebas

![Billing_Contact__1_.png](assets/billing-contact--1--350x74.png)

Una vez que se alcancen los límites de pruebas o de almacenamiento, aparecerán las alertas en la parte superior de la página [!UICONTROL Facturación]:

* Para el límite de pruebas alcanzado

  ![Proofs_limit_reached.png](assets/proofs-limit-reached-350x65.png)

* Para el límite de almacenamiento alcanzado

![Storage_limit_reached.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>El recuento de pruebas se termina cuando se crean pruebas en su cuenta y no se puede restaurar eliminándolas.

Se puede liberar espacio de almacenamiento eliminando las pruebas y los archivos y vaciando la [!UICONTROL Papelera] posteriormente.

Recuerde que, si necesita más pruebas, almacenamiento o usuarios, puede actualizar su cuenta en cualquier momento y con efecto inmediato.

## [!UICONTROL Historial de facturación]

Esta sección muestra la actividad de los períodos de facturación recientes. También puede descargar sus facturas desde esta sección.

Para obtener más información, consulte “[Descargar [!DNL Workfront Proof] factura](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md)”.

## [!UICONTROL Actividad de facturación]

Esta sección muestra los cambios recientes en su configuración de facturación, como suscripciones, actualizaciones, reducciones y renovaciones de plan [!DNL Workfront Proof].

Si se cambia el plan a uno con un límite de usuarios inferior (1), se desactivará automáticamente a quienes excedan el nuevo límite cuando comience el nuevo plan. Esta actividad también se guarda en los Registros de la cuenta (2).

![Billing_Downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
