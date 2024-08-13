---
title: Desactivar la opción de actualización automática para usuarios no pagados en el nuevo plan de licencias
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso, nivel, sistema, administrador, estándar, ligero, colaborador
navigation-topic: access-levels
description: Todos los usuarios deben tener un nivel de acceso para iniciar sesión y trabajar en Workfront. El nivel de acceso se utiliza para controlar lo que un usuario puede ver y hacer con determinados objetos y áreas de Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 1%

---

# Desactive la opción de actualización automática para usuarios no pagados en el nuevo plan de licencias

Las decisiones sobre pruebas y documentos son limitadas para todas las licencias Workfront no pagadas en los nuevos planes. Cuando los usuarios alcanzan el número asignado de decisiones, se actualizan a una licencia básica de forma predeterminada.

Puede desactivar la opción de actualización automática desde el área de configuración. Para obtener más información sobre cómo funcionan las actualizaciones automáticas, consulte [Información general sobre documentos y pruebas limitados para usuarios sin pago](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>Una vez desactivado, cualquier usuario no remunerado que pase el número asignado de decisiones no se actualizará automáticamente.

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
   <td>Nuevo plan: Estándar
   <p>o</p>
   <p>Plan actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Deshabilitar las actualizaciones automáticas para usuarios no pagados

{{step-1-to-setup}}

1. Expanda [!UICONTROL **Sistema**] en el panel de navegación izquierdo y luego haga clic en [!UICONTROL **Preferencias**].
1. En la sección [!UICONTROL **Preferencias generales**], marque la casilla [!UICONTROL **Deshabilitar la actualización automática dentro de los niveles de acceso**].
1. Haga clic en [!UICONTROL **Guardar**].
