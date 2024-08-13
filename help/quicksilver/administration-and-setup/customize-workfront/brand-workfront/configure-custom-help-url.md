---
title: Configurar una URL de ayuda personalizada
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: Si crea un sitio de ayuda interno personalizado que contiene información sobre cómo utiliza su organización Workfront, puede configurar el icono Ayuda del menú principal para ir a ese sitio. Esto no afecta al vínculo de Ayuda principal del menú principal ni a los vínculos de ayuda contextual de Workfront, que llevan a los usuarios al sitio de Ayuda de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d2b63508-1943-4f9e-888e-8f1bfb54c33e
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Configuración de una URL de ayuda personalizada

Si crea un sitio de ayuda interno personalizado que contiene información sobre cómo utiliza su organización Workfront, puede configurar el icono Ayuda del menú principal para ir a ese sitio.

![](assets/custom-help-button.png)

Esto no afecta al vínculo de Ayuda principal del menú principal ni a los vínculos de ayuda contextual de Workfront, que llevan a los usuarios al sitio de Ayuda de Workfront.

![](assets/custom-help-url.png)

Para obtener información sobre cómo los usuarios acceden a una dirección URL de ayuda personalizada que configuró en Workfront y al sitio de ayuda normal de Workfront, consulte [Acceso a la ayuda de Workfront en la nueva experiencia de Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/access-workfront-help.md).

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurar una dirección URL de ayuda personalizada

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Preferencias**.
1. En la sección **Preferencias generales**, en el campo **URL de ayuda personalizada**, escriba la URL donde se encuentra su sitio de ayuda personalizado.

   Si la ubicación de ayuda personalizada requiere credenciales de inicio de sesión, esas credenciales son necesarias para los usuarios cuando acceden al sitio desde Workfront. Puede que sea necesario administrar las credenciales del sitio de ayuda personalizado de forma independiente de las credenciales de Workfront si no utiliza el inicio de sesión único (SSO).

1. Haga clic en **Guardar**.
