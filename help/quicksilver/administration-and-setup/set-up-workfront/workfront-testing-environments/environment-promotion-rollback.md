---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Restablecer un paquete de promoción de entorno
description: La capacidad de promoción del entorno está pensada para ofrecer la posibilidad de mover objetos relacionados con la configuración de un entorno a otro. Obtenga información sobre cómo revertir un paquete de promoción instalado desde un entorno de destino.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
TQID: https://experienceleague.adobe.com/EPjuu-mWZH31cMvN-4tdzD8X-YFoW-DJ6YhfnJ0u06k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 389
ht-degree: 24%

---

# Restablecer un paquete de promoción de entorno



Una vez instalado un paquete, puede revertirlo. Esto elimina los cambios que el paquete realizó en el entorno de destino y restaura los objetos afectados a sus configuraciones anteriores.

Puede revertir un paquete de promoción en un plazo de 24 horas después de su instalación. Después de 24 horas, la funcionalidad de reversión ya no está disponible para esa instalación.

## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td>Paquete de Adobe Workfront
   </td>
   <td> <p>PRIME o ULTIMATE</p>
   </td>
  </tr>
  <tr>
   <td><strong>licencias de Workfront</strong>
   </td>
   <td> <p>Estándar</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td><p>Debe ser administrador de Workfront.</p>
   </td>
  </tr>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

* Se debe instalar un paquete de promoción de entorno para poder revertirlo.

  Para obtener instrucciones, consulte [Instalar un paquete de promoción de entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


## Determine si se puede revertir una implementación de paquete específica

Para saber si se puede revertir una implementación de paquete específica, tenga en cuenta lo siguiente:

* Deben haber transcurrido menos de 24 horas desde que se instaló el paquete.
* Solo se puede revertir la implementación del paquete más reciente.
* Se puede revertir una implementación fallida.
* Las reversiones no se pueden revertir.


## Revertir un paquete de promoción de entorno instalado

1. Vaya al entorno en el que se instaló el paquete.
1. Haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o, si está disponible, haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Setup]** ![Icono de Configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccione **Promoción de entorno** en el panel de navegación izquierdo.
1. Seleccione el paquete que desea revertir y haga clic en **Implementaciones**.
1. Pase el ratón sobre la implementación (instalación) que desee revertir y, a continuación, haga clic en Revertir cuando aparezca a la derecha de la línea de esa implementación.

   O

   Haga clic en la implementación que desea revertir y luego haga clic en **Revertir paquete** en la esquina superior derecha de la pantalla.

   >[!IMPORTANT]
   >
   >La implementación debe haber tenido lugar menos de 24 horas antes de revertirla. Las instalaciones con más de 24 horas de antigüedad no se pueden revertir.

1. (Opcional) En el área Vista previa de reversión, vea los cambios que se producirán cuando se revierta la implementación.
1. Haga clic en **Retroceder** en la esquina superior derecha de la pantalla.
