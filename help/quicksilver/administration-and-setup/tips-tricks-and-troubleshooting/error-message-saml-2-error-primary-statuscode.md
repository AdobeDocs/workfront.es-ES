---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensaje de error: Error de SAML 2.0: Código de estado principal'
description: No puede establecer correctamente una conexión con ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 97%

---

# Mensaje de error: Error de SAML 2.0: Primary StatusCode

## Problema

No puede establecer correctamente una conexión con ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>Si establece una conexión de prueba satisfactoria y sigue teniendo problemas, es posible que tenga asignaciones de atributos incorrectas o problemas con los identificadores de federación. Póngase en contacto con el Servicio de atención al cliente si tiene alguna pregunta.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Causa 1: El Algoritmo hash seguro está configurado en SHA-256

### Solución

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Aparece el cuadro de diálogo Administración de ADFS 2.0.

1. Seleccione **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confianzas de terceros confiables]** en el panel izquierdo.

1. Haga clic derecho en la confianza de terceros confiables relacionada con [!DNL Adobe Workfront], luego seleccione **[!UICONTROL Propiedades]**.
1. Haga clic en la pestaña **[!UICONTROL Avanzado]** luego seleccione **[!UICONTROL SHA-1]** en el menú desplegable de **[!UICONTROL Algoritmo hash seguro]**.
   ![SHA-1](assets/1-350x287.png)

## Causa 2: El certificado de firma de ADFS está a punto de expirar y ha sido reemplazado por un nuevo certificado con fechas superpuestas

### Solución

La página de configuración de [!DNL Workfront] SSO muestra la fecha de vencimiento del certificado. Si el certificado está a punto de expirar, debes extraer manualmente el nuevo certificado de firma del servidor ADFS:

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Aparece el cuadro de diálogo Administración de ADFS 2.0.

1. Seleccione **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confianzas de terceros confiables]** en el panel izquierdo.

1. Haga clic derecho en la confianza de terceros confiables relacionada con [!DNL Workfront], y seleccione **[!UICONTROL Propiedades]**.
1. Haga clic en la pestaña **[!UICONTROL Firma]**.
1. Haga clic en el nombre del certificado de firma y luego haga clic en **[!UICONTROL Ver]**.
1. Haga clic en Copiar a **[!UICONTROL archivo]**... y seleccione **[!UICONTROL Siguiente]**.

1. Seleccione **[!UICONTROL Base-64 codificado x.509 (CER)]**, y haga clic en **[!UICONTROL Siguiente]**.

1. Especifique el nombre de archivo y haga clic en **[!UICONTROL Siguiente]**.
1. Haga clic en **[!UICONTROL Finalizar]**.
1. En [!DNL Workfront], navega a **[!UICONTROL Configuración]** > **[!UICONTROL Sistema]** > **[!UICONTROL Inicio de Sesión Único (SSO)]** y sube manualmente el certificado de firma.

## Causa 3: la comprobación de revocación de certificados está fallando

La solución para esto depende de la versión de [!DNL Microsoft] ADFS que esté usando. Consulte la documentación de [!DNL Microsoft] para obtener los comandos apropiados para tu versión.
