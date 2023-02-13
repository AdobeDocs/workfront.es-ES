---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensaje de error: No se pudo validar la firma digital XML"
description: No puede establecer una conexión correcta con ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Mensaje de error: No se pudo validar la firma digital XML

## Problema

No puede establecer una conexión correcta con ADFS.

![error_message.png](assets/error-message.png)

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

## Causa 1: El certificado es incorrecto

### Solución

Recupere manualmente el certificado de firma del servidor ADFS:

1. En [!DNL Windows], haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Se muestra el cuadro de diálogo Administración de ADFS 2.0 .

1. Select **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confiar en las confianzas del partido]** en el panel izquierdo.

1. Haga clic con el botón derecho en **[!UICONTROL Confiar en la confianza de las partes]** y seleccione **[!UICONTROL Propiedades]**.

1. Haga clic en el **[!UICONTROL Firma]** pestaña .
1. Haga clic en el nombre del certificado de firma y, a continuación, haga clic en **[!UICONTROL Ver]**.
1. Haga clic en Copiar para **[!UICONTROL Archivo]**... y seleccione **[!UICONTROL Siguiente]**.

1. Select **[!UICONTROL x.509 (CER) con codificación base-64]** y haga clic en **[!UICONTROL Siguiente]**.

1. Especifique el nombre del archivo y haga clic en **[!UICONTROL Siguiente]**.
1. Haga clic en **[!UICONTROL Finalizar]**.
1. En [!DNL Adobe Workfront], vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Sistema]** > **[!UICONTROL Inicio de sesión único (SSO)]** y cargar manualmente el certificado de firma.

## Causa 2: El certificado se firma mediante DSA cuando [!DNL Workfront] espera una firma RSA

### Solución

Vuelva a crear el certificado y utilice la firma RSA en lugar del DSA.

## Causa 3: Los datos XML son incorrectos

### Solución

Vuelva a exportar y vuelva a importar los metadatos XML desde el sistema de administración de ADFS.

## Causa 4: No se pudo realizar la solicitud debido a un error en el lado SAML

### Solución

Póngase en contacto con su proveedor de SAML.
