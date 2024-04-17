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
source-git-commit: f65fbe7ceab19cee75aa0346c389907707c47c8b
workflow-type: tm+mt
source-wordcount: '401'
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
1. Para cada objeto que tenga un conflicto, seleccione cómo resolver el conflicto.

   Para resolver un conflicto, haga clic en la flecha desplegable situada junto al tipo de objeto y seleccione la acción que desee realizar.

   Para obtener más información, consulte [Conflictos](#collisions) en este artículo
1. Para implementar el paquete en el nuevo entorno, haga clic en **Implementar** en la parte superior derecha de la pantalla.

## Conflictos

Los conflictos se producen cuando ya existe un objeto que forma parte del paquete de instalación en el entorno de destino. Cuando esto sucede, puede seleccionar cómo resolver el conflicto. Los conflictos se resuelven en el nivel de objeto.

Para ver los conflictos, haga clic en el menú desplegable situado junto a cada tipo de objeto. Los conflictos se muestran en la columna Conflicto.

Para resolver un conflicto, seleccione una acción en la columna Acción de implementación o utilice la acción predeterminada que ya se muestra.

* **Crear con nombre nuevo**: cree un nuevo objeto en el entorno de destino. Si el objeto existe en el entorno de destino, puede crear un nuevo objeto con un nombre nuevo. Si no existe en el entorno de destino, puede crear el objeto con un nombre nuevo o con el nombre que tiene el objeto en el paquete.
* **Usar los existentes**: el objeto del paquete no está instalado y el objeto que ya existía en el entorno de destino no cambia.
* **Sobrescribir**: el objeto del paquete reemplaza al objeto existente en el entorno de destino.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Los valores predeterminados son `Create new` si el objeto no existe en el entorno de destino, y `Use existing` si el objeto no existe en el entorno de destino. Para volver a la asignación predeterminada, haga clic en **Restablecer asignación predeterminada**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
