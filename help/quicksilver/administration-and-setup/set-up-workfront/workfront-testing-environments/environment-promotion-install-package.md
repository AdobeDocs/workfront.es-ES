---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Instalación de un paquete de promoción de entorno
description: La capacidad de promoción de entornos está diseñada para proporcionar la capacidad de mover objetos relacionados con la configuración de un entorno a otro. Obtenga información sobre cómo instalar un paquete de promoción de entorno en un entorno de destino.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 5d84d50b8984bbff7bbc02ffc0ce86ec1f486742
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Instalación de un paquete de promoción de entorno

>[!NOTE]
>
>Para instalar un paquete, debe haber iniciado sesión en el entorno en el que desea instalarlo. Este es el entorno en el que está copiando objetos **hasta**.

1. Vaya al entorno en el que desea instalar el paquete.
1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccionar **Sistema** en el panel de navegación izquierdo, seleccione **Promoción de entorno**.
1. Seleccione el paquete en la lista mostrada.
1. Para instalar el paquete, haga clic en **Instalar** en la parte superior derecha de la pantalla.
1. Asigne cada objeto del paquete al objeto correspondiente en el entorno de destino.

   Para obtener más información, consulte [Asignación](#mapping) en este artículo


## Asignación

Cada tipo de objeto aparece en la lista de navegación izquierda y en una tarjeta. La tarjeta muestra objetos de ese tipo y si existen en el entorno de destino. Puede determinar cómo se moverán estos objetos al entorno de destino.

* Crear nuevo: crea un nuevo objeto en el entorno de destino. Si el objeto existe en el entorno de destino, puede crear un nuevo objeto con un nombre nuevo. Si no existe en el entorno de destino, puede crear el objeto con un nombre nuevo o con el nombre que tiene el objeto en el paquete.
* Usar existente: el objeto del paquete no está instalado y el objeto que ya existía en el entorno de destino no se modifica.
* Sobrescribir existente: (no disponible actualmente) el objeto del paquete reemplaza al objeto existente en el entorno de destino.
* No utilizar: el objeto del paquete no está instalado en el entorno de destino. Si selecciona No utilizar, aparecerá un mensaje de error que detalla cómo esta opción afectará a otros objetos o campos.

Los valores predeterminados son `Create new` si el objeto no existe en el entorno de destino, y `Use existing` si el objeto no existe en el entorno de destino. Para volver a la asignación predeterminada, haga clic en **Restablecer asignación predeterminada**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
