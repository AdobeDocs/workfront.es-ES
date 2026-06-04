---
title: Habilitar o deshabilitar el Asistente de IA
content-type: reference
description: Puede controlar qué niveles de acceso de su organización tienen acceso al asistente de IA.
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/h1895B7LDBKIhpJPrMROBoi-85LqrBUS1Rmw-m2n2Bo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 289
ht-degree: 33%

---

# Habilitar o deshabilitar el Asistente de IA

Como administrador de Workfront, puede controlar qué usuarios de su organización tienen habilitado el asistente de IA. Esto se administra mediante niveles de acceso.

Debe habilitar el asistente de IA para su organización para poder habilitarlo para un nivel de acceso.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Habilitar o deshabilitar el Asistente de IA para su organización

Para habilitar el Asistente de IA para su organización:

{{step-1-to-setup}}

1. Seleccione **Sistema** en el panel de navegación izquierdo, luego seleccione **Preferencias**.
1. Desplácese hacia abajo hasta la sección **Preferencias de IA**.
1. Active la opción **Habilitar IA**.

>[!IMPORTANT]
>
>Debe tener un acuerdo de IA general firmado con Adobe para poder utilizar el Asistente de IA.
>Para obtener más información sobre el Contrato de IA general, consulte [Firmar el Contrato de IA general de Adobe](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) en el artículo Asistente de IA en Workfront.

## Habilitar o deshabilitar el Asistente de IA para un nivel de acceso

Para habilitar el asistente de IA para un nivel de acceso determinado:

{{step-1-to-setup}}

1. Seleccione **Niveles de acceso** en el panel de navegación izquierdo.
1. Seleccione el nivel de acceso deseado y luego haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) situado encima de la lista.
1. En el área **Establecer restricciones adicionales...** del cuadro **Editar nivel de acceso**, desmarque la casilla de verificación **Deshabilitar el Asistente de IA de Workfront**.
1. Haga clic en **Guardar**.
1. Repita los pasos del 3 al 5 para cada nivel de acceso para el que desee habilitar el Asistente de IA.



>[!NOTE]
>
>* El Asistente de IA está desactivado de forma predeterminada para los usuarios que no son administradores.
>* Si un usuario que no es administrador interactúa con el icono del asistente de IA en Workfront, aparece el acuerdo del asistente de IA en el que se solicita al usuario que no es administrador que acepte los términos y condiciones. Si aceptan el acuerdo, pueden utilizar el Asistente de IA aunque esté deshabilitado en su plantilla de diseño.

