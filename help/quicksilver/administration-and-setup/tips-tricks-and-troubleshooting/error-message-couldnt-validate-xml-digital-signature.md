---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensaje de error: No se ha podido validar la firma digital XML"
description: No puede establecer correctamente una conexión con ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 1%

---

# Mensaje de error: No se pudo validar la firma digital XML

## Problema

No puede establecer correctamente una conexión con ADFS.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>Si establece correctamente una conexión de prueba y sigue teniendo problemas, es posible que tenga asignaciones de atributos incorrectas o problemas con los Federation ID. Póngase en contacto con Atención al cliente si tiene alguna pregunta.

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
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Causa 1: el certificado es incorrecto

### Solución

Recupere manualmente el certificado de firma del servidor ADFS:

1. En [!DNL Windows], haga clic en **[!UICONTROL Inicio]** > **[!UICONTROL Administración]** > **[!UICONTROL Administración de ADFS 2.0]**.\
   Aparece el cuadro de diálogo Administración de ADFS 2.0.

1. Seleccione **[!UICONTROL Relación de confianza]** > **[!UICONTROL Confianzas de usuario de confianza]** en el panel izquierdo.

1. Haga clic con el botón derecho en **[!UICONTROL Confianza del usuario de confianza]** y seleccione **[!UICONTROL Propiedades]**.

1. Haga clic en la ficha **[!UICONTROL Firma]**.
1. Haga clic en el nombre del certificado de firma y luego haga clic en **[!UICONTROL Ver]**.
1. Haga clic en Copiar a **[!UICONTROL archivo]**... y seleccione **[!UICONTROL Siguiente]**.

1. Seleccione **[!UICONTROL Base-64 codificado x.509 (CER)]** y haga clic en **[!UICONTROL Siguiente]**.

1. Especifique el nombre de archivo y haga clic en **[!UICONTROL Siguiente]**.
1. Haga clic en **[!UICONTROL Finalizar]**.
1. En [!DNL Adobe Workfront], vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Sistema]** > **[!UICONTROL Inicio de sesión único (SSO)]** y cargue manualmente el certificado de firma.

## Causa 2: el certificado se firma mediante DSA cuando [!DNL Workfront] espera una firma RSA

### Solución

Vuelva a crear el certificado y utilice la firma RSA en lugar del DSA.

## Causa 3: los datos XML son incorrectos

### Solución

Volver a exportar y volver a importar los metadatos XML desde el sistema de administración de ADFS.

## Causa 4: no se pudo realizar la solicitud debido a un error del lado de SAML

### Solución

Póngase en contacto con su proveedor de SAML.
