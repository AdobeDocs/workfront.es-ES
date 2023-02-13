---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: La URL de cierre de sesión de ADFS no funciona
description: El procedimiento descrito en esta página solo se aplica a organizaciones que aún no están integradas en Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# La URL de cierre de sesión de ADFS no funciona

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a las organizaciones que aún no están integradas en la variable [!UICONTROL Adobe Admin Console].
>
>Si su organización se ha incorporado a la variable [!UICONTROL Adobe Admin Console], consulte [Diferencias de administración basadas en plataformas ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problema

Al utilizar la URL de cierre de sesión de ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), recibe una página de mensaje con el error: &quot;Hubo un problema al acceder al sitio. Intenta volver a navegar al sitio&quot;.

Si el problema persiste, póngase en contacto con el administrador de este sitio y proporcione el siguiente número de referencia para identificar el problema: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] licencia</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

1. En el servidor de ADFS manager, vaya a **[!UICONTROL Relaciones de confianza]** > **[!UICONTROL Confiar en las confianzas del partido]** > `<your party trust>` propiedades.

1. En el **[!UICONTROL Puntos finales]** , haga clic en **[!UICONTROL Agregar]**.

1. **[!UICONTROL Tipo de extremo]** = cierre de sesión SAML, enlace = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Puede establecer una URL de respuesta si desea que se redirija a otra página. Pero recomendamos el sitio de ADFS porque advierte que está desconectado, pero aun así debería cerrar el explorador.
