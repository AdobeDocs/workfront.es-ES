---
title: Desactivar la opción de actualización automática para usuarios sin pago
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso, nivel, sistema, administrador, estándar, light, colaborador
navigation-topic: access-levels
description: Todos los usuarios deben tener un nivel de acceso para iniciar sesión y trabajar en Workfront. El nivel de acceso se utiliza para controlar lo que un usuario puede ver y hacer con determinados objetos y áreas de Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 92%

---

# Desactivar la opción de actualización automática para usuarios sin pago

Las decisiones sobre revisiones y documentos son limitadas para todas las licencias de Workfront sin pago en los nuevos planes. Cuando los usuarios alcanzan el número asignado de decisiones, pasan a una licencia Light de forma predeterminada.

Puede deshabilitar la opción de actualización automática desde el área de configuración. Para obtener más información sobre cómo funcionan las actualizaciones automáticas, consulte [Información general sobre documentos y decisión de la revisión limitados para usuarios sin pago](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>Una vez desactivadas, cualquier usuario sin pago que supere el número asignado de decisiones no se actualizará de forma automática.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Estándar
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Deshabilitación de las actualizaciones automáticas para usuarios sin pago

{{step-1-to-setup}}

1. Expanda [!UICONTROL **Sistema**] en el panel de navegación izquierdo y luego haga clic en [!UICONTROL **Preferencias**].
1. En la sección [!UICONTROL **Preferencias generales**], marque la casilla [!UICONTROL **Deshabilitar la actualización automática dentro de los niveles de acceso**].
1. Haga clic en [!UICONTROL **Guardar**].
