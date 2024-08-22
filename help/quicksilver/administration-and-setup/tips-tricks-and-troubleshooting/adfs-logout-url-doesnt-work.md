---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: La URL de cierre de sesión de ADFS no funciona
description: El procedimiento descrito en esta página se aplica solo a las organizaciones que aún no se han incorporado a Adobe Admin Console.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# La URL de cierre de sesión de ADFS no funciona

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica solo a las organizaciones que aún no se han incorporado a [!UICONTROL Adobe Admin Console].
>
>Si su organización se ha incorporado a [!UICONTROL Adobe Admin Console], vea [Diferencias de administración basadas en la plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problema

Al utilizar la URL de cierre de sesión de ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), recibe un mensaje de página con el error: &quot;Se ha producido un problema al acceder al sitio. Intente volver a navegar al sitio&quot;.

Si el problema persiste, póngase en contacto con el administrador de este sitio y proporcione el siguiente número de referencia para identificar el problema: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td role="rowheader">Licencia de Adobe [!DNL Workfront]</td> 
   <td> 
   <p>Nuevo: estándar</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

1. En el servidor del administrador de ADFS, vaya a **[!UICONTROL Relaciones de confianza]** > **[!UICONTROL Confianzas de usuario de confianza]** > `<your party trust>` propiedades.

1. En la ficha **[!UICONTROL Puntos finales]**, haga clic en **[!UICONTROL Agregar]**.

1. **[!UICONTROL Tipo de extremo]** = Cierre de sesión SAML, Enlace = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Puede establecer una dirección URL de respuesta si desea que se redirija a otra página. Pero recomendamos el sitio ADFS porque advierte que ha cerrado la sesión, pero que debe cerrar el explorador.
