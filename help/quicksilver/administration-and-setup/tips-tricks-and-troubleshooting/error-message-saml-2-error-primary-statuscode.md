---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensaje de error: Error de SAML 2.0: Código de estado primario'
description: No puede establecer una conexión correcta con ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Mensaje de error: Error de SAML 2.0: Código de estado principal

## Problema

No puede establecer una conexión correcta con ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>Si establece una conexión de prueba correcta y sigue teniendo problemas, es posible que tenga asignaciones de atributos incorrectas o problemas con los ID de federación. Póngase en contacto con el servicio de atención al cliente si tiene alguna pregunta.

## Requisitos de acceso

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Causa 1: El algoritmo hash seguro está establecido en SHA-256

### Solución

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Se muestra el cuadro de diálogo Administración de ADFS 2.0 .

1. Select **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confiar en las confianzas del partido]** en el panel izquierdo.

1. Haga clic con el botón derecho en la confianza de la parte que confía relacionada con [!DNL Adobe Workfront]y, a continuación, seleccione **[!UICONTROL Propiedades]**.
1. Haga clic en el **[!UICONTROL Avanzadas]** y, a continuación, seleccione **[!UICONTROL SHA-1]** de la variable **[!UICONTROL Algoritmo hash seguro]** menú desplegable.\
   ![](assets/1-350x287.png)

## Causa 2: El certificado de firma de ADFS está a punto de caducar y ha sido reemplazado por un nuevo certificado con fechas superpuestas

### Solución

La variable [!DNL Workfront] La página Configuración de SSO enumera la fecha de caducidad del certificado. Si el certificado está a punto de caducar, debe extraer manualmente el nuevo certificado de firma del servidor ADFS:

1. En Windows, haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Se muestra el cuadro de diálogo Administración de ADFS 2.0 .

1. Select **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confiar en las confianzas del partido]** en el panel izquierdo.

1. Haga clic con el botón derecho en la confianza de la parte que confía relacionada con [!DNL Workfront]y seleccione **[!UICONTROL Propiedades]**.
1. Haga clic en el **[!UICONTROL Firma]** pestaña .
1. Haga clic en el nombre del certificado de firma y, a continuación, haga clic en **[!UICONTROL Ver]**.
1. Haga clic en Copiar para **[!UICONTROL Archivo]**... y seleccione **[!UICONTROL Siguiente]**.

1. Select **[!UICONTROL x.509 (CER) con codificación base-64]** y haga clic en **[!UICONTROL Siguiente]**.

1. Especifique el nombre del archivo y haga clic en **[!UICONTROL Siguiente]**.
1. Haga clic en **[!UICONTROL Finalizar]**.
1. En [!DNL Workfront], vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Sistema]** > **[!UICONTROL Inicio de sesión único (SSO)]** y cargar manualmente el certificado de firma.

## Causa 3: La comprobación de revocación de certificados está fallando

La solución para esto depende de la versión de [!DNL Microsoft] ADFS que está utilizando. Consultar [!DNL Microsoft]para obtener los comandos adecuados para su versión.
