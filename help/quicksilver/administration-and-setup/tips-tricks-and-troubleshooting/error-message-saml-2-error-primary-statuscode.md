---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensaje de error: error de SAML 2.0: Primary StatusCode"
description: No puede establecer correctamente una conexión con ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---

# Mensaje de error: Error de SAML 2.0: Primary StatusCode

## Problema

No puede establecer correctamente una conexión con ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>Si establece correctamente una conexión de prueba y sigue teniendo problemas, es posible que tenga asignaciones de atributos incorrectas o problemas con los Federation ID. Póngase en contacto con Atención al cliente si tiene alguna pregunta.

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
   <td>[!UICONTROL Administrador del sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Causa 1: el algoritmo hash seguro está establecido en SHA-256

### Solución

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Aparece el cuadro de diálogo Administración de ADFS 2.0.

1. Seleccione **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confianzas de usuario de confianza]** en el panel izquierdo.

1. Haga clic con el botón secundario en la confianza de usuario autenticado relacionada con [!DNL Adobe Workfront] y, a continuación, seleccione **[!UICONTROL Propiedades]**.
1. Haga clic en la ficha **[!UICONTROL Avanzado]** y, a continuación, seleccione **[!UICONTROL SHA-1]** en el menú desplegable **[!UICONTROL Algoritmo hash seguro]**.\
   ![](assets/1-350x287.png)

## Causa 2: el certificado de firma de ADFS está a punto de caducar y se ha reemplazado por un nuevo certificado con fechas superpuestas

### Solución

La página de configuración de SSO [!DNL Workfront] indica la fecha de caducidad del certificado. Si el certificado está a punto de caducar, debe extraer manualmente el nuevo certificado de firma del servidor ADFS:

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Aparece el cuadro de diálogo Administración de ADFS 2.0.

1. Seleccione **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confianzas de usuario de confianza]** en el panel izquierdo.

1. Haga clic con el botón secundario en la confianza de usuario autenticado relacionada con [!DNL Workfront] y seleccione **[!UICONTROL Propiedades]**.
1. Haga clic en la ficha **[!UICONTROL Firma]**.
1. Haga clic en el nombre del certificado de firma y luego haga clic en **[!UICONTROL Ver]**.
1. Haga clic en Copiar a **[!UICONTROL archivo]**... y seleccione **[!UICONTROL Siguiente]**.

1. Seleccione **[!UICONTROL Base-64 codificado x.509 (CER)]** y haga clic en **[!UICONTROL Siguiente]**.

1. Especifique el nombre de archivo y haga clic en **[!UICONTROL Siguiente]**.
1. Haga clic en **[!UICONTROL Finalizar]**.
1. En [!DNL Workfront], vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Sistema]** > **[!UICONTROL Inicio de sesión único (SSO)]** y cargue manualmente el certificado de firma.

## Causa 3: la comprobación de revocación de certificados está fallando

La solución para esto depende de la versión de [!DNL Microsoft] ADFS que esté usando. Consulte la documentación de [!DNL Microsoft] para obtener los comandos apropiados para su versión.
