---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Conversión de portafolios heredados al almacenamiento en la nube de Adobe
description: Convierta los portafolios de almacenamiento de Workfront heredados existentes al almacenamiento en la nube de Adobe desde el área Preferencias de almacenamiento en Preferencias del sistema.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 9d28f52ace4d443bdffc475baf79d482152d4157
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 11%

---

# Conversión de portafolios heredados al almacenamiento en la nube de Adobe

Como administrador de Workfront, puede convertir portafolios de almacenamiento de Workfront heredados existentes a almacenamiento en la nube de Adobe desde el área Preferencias de almacenamiento en Preferencias del sistema. Después de convertir un portafolio, se comporta como cualquier otro portafolio de almacenamiento en la nube de Adobe.

Para obtener más información sobre cómo se comportan los portafolios convertidos y cómo se ven afectados sus objetos secundarios, consulte [Portabilidad de objetos](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability) en [Mover a Workfront en el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p>Cualquier paquete de flujo de trabajo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Antes de convertir un portafolio

Antes de convertir una cartera de soluciones de almacenamiento de Workfront heredadas, tenga en cuenta lo siguiente:

* La conversión solo afecta al propio portafolio. Los proyectos y programas secundarios que utilizan el almacenamiento heredado de Workfront permanecen en el almacenamiento heredado.
  >[!NOTE]
  >
  >Un programa secundario heredado se convierte automáticamente en almacenamiento en la nube de Adobe solo cuando alguien le agrega manualmente un proyecto de almacenamiento en la nube de Adobe.
* Los documentos y las carpetas de documentos del portafolios permanecen en el almacenamiento heredado de Workfront después de la conversión.
* Después de la conversión, no puede agregar proyectos de almacenamiento de Workfront heredados al portafolio.

## Conversión de portafolios heredados al almacenamiento en la nube de Adobe

Para convertir uno o más portafolios de almacenamiento de Workfront heredados al almacenamiento en la nube de Adobe:

{{step-1-to-setup}}

1. Seleccione **Sistema** en el panel de navegación izquierdo, luego seleccione **Preferencias**.

1. Desplácese hacia abajo hasta la sección **Preferencias de almacenamiento**.

1. En el campo **Seleccionar portafolios para convertirlos al almacenamiento en la nube de Adobe**, seleccione uno o más portafolios de almacenamiento de Workfront heredados.

1. Haga clic en **Guardar**.

   Aparece un mensaje de confirmación que describe lo que sucede cuando se convierte un portafolio:

   * Ya no puede mover proyectos de almacenamiento de Workfront heredados al portafolio.
   * Todos los proyectos nuevos creados en la cartera utilizan el almacenamiento en la nube de Adobe.
   * Frame.io es el visor de documentos en los proyectos de almacenamiento en la nube de Adobe del portafolio.
   * Los proyectos secundarios que utilizan almacenamiento de Workfront heredado permanecen en el almacenamiento heredado.
   * Los programas secundarios permanecen en el almacenamiento heredado.

1. Haga clic en **Convertir** para confirmar.

   Los portafolios seleccionados se convierten al almacenamiento en la nube de Adobe.
