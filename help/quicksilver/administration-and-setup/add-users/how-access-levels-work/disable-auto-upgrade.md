---
title: Desactive la opción de actualización automática para usuarios no pagados en el nuevo plan de licencias
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acceso, nivel, sistema, administrador, estándar, ligero, colaborador
navigation-topic: access-levels
description: Todos los usuarios deben tener un nivel de acceso para iniciar sesión y trabajar en Workfront. El nivel de acceso se utiliza para controlar lo que un usuario puede ver y hacer con determinados objetos y áreas de Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 1ff727f1-bc26-4ffe-a510-615bebfe5b96
source-git-commit: 8807636d2309435cb5f4e08d6a7d27246342200d
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 1%

---

# Desactive la opción de actualización automática para usuarios no pagados en el nuevo plan de licencias

Las decisiones sobre pruebas y documentos son limitadas para todas las licencias Workfront no pagadas en los nuevos planes. Cuando los usuarios alcanzan el número asignado de decisiones, se actualizan a una licencia básica de forma predeterminada.

Puede desactivar la opción de actualización automática desde el área de configuración. Para obtener más información sobre cómo funcionan las actualizaciones automáticas, consulte [Información general sobre la decisión limitada de documentos y pruebas para usuarios no pagados](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>Una vez desactivado, cualquier usuario no remunerado que pase el número asignado de decisiones no se actualizará automáticamente.


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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan actual: Estándar
   <p>o</p>
   <p>Plan heredado: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

## Deshabilitar las actualizaciones automáticas para usuarios no pagados

{{step-1-to-setup}}

1. Expandir [!UICONTROL **Sistema**] en el panel de navegación izquierdo, haga clic en [!UICONTROL **Preferencias**].
1. En el [!UICONTROL **Preferencias generales**] , marque la [!UICONTROL **Deshabilitar la actualización automática en los niveles de acceso**] cuadro.
1. Haga clic en [!UICONTROL **Guardar**].
