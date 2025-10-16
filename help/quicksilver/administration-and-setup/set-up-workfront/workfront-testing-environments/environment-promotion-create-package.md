---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Crear o editar un paquete de promoción de entorno
description: La capacidad de promoción del entorno está pensada para ofrecer la posibilidad de mover objetos relacionados con la configuración de un entorno a otro. Aprenda a crear un paquete de promoción del entorno que luego puede instalar en un entorno diferente.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 71%

---

# Crear o editar un paquete de promoción de entorno

Debe crear un paquete en el entorno **desde el que** desea copiar objetos. Por ejemplo, si va a configurar un proyecto en el entorno de zona protegida de actualización personalizada y lo va a promocionar al entorno de producción, debe crear el paquete en el entorno de zona protegida de actualización personalizada.

>[!IMPORTANT]
>
>Si la zona protegida de actualización personalizada se actualiza mientras configura un objeto para la promoción del entorno, dicha configuración se perderá durante la actualización. Le recomendamos que no actualice la zona protegida de actualización personalizada a menos que todos los objetos y paquetes de promoción del entorno pendientes se hayan promocionado correctamente.

## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td>paquete de Adobe Workfront
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

## Crear un paquete

1. Vaya al entorno en el que desea crear el paquete. Es el entorno **desde el que** está copiando objetos.
1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configuración]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccione **Sistema** en la navegación izquierda y, a continuación, **Promoción del entorno**.
1. Haga clic en **Crear paquete**.

   Se abre la página Nuevo paquete de promociones.

1. En el campo **Nombre**, introduzca un nombre para el paquete. 
1. En el campo **Descripción**, escriba una descripción para este paquete.
1. Para añadir un objeto al paquete, en el panel de navegación izquierdo, seleccione el tipo de objeto que desea añadir.
1. Seleccione uno o varios objetos de la lista que aparece, o escriba el nombre en la barra de búsqueda y seleccione el objeto cuando aparezca en la lista. Puede seleccionar más de un objeto en la lista.

   La lista incluye hasta 500 objetos del tipo de objeto seleccionado. Para localizar un objeto que no esté en la lista, utilice la barra de búsqueda.
1. Haga clic en **Añadir (X objetos)** para añadir los objetos seleccionados al paquete.

   >[!INFO]
   >
   >**Ejemplo**
   >
   >Si ha seleccionado tres proyectos para añadirlos al proyecto, el botón indica **Añadir 3 proyectos**.

   Los objetos que ha añadido aparecen en el área Contenido del paquete a la derecha de la página.

1. Para añadir otro tipo de objeto, repita los pasos 7 a 9.
1. (Opcional) Para eliminar un objeto del paquete, pase el puntero por encima del objeto en el área Contenido del paquete y, a continuación, haga clic en la X junto al objeto.
1. Cuando haya añadido todos los objetos deseados al paquete, haga clic en **Guardar y cerrar** para guardar el paquete sin ensamblarlo.

   O

   Haga clic en **Guardar y ensamblar** para guardar y ensamblar el paquete.

   >[!NOTE]
   >
   >* Los botones Guardar y cerrar, y Guardar y ensamblar están disponibles si un paquete tiene un nombre con cinco o más caracteres y al menos un objeto añadido.
   >* No puede montar un paquete que esté en un estado instalable como, por ejemplo, en prueba o activo.

## Editar o montar un paquete existente

Un paquete debe estar en estado `DRAFT` para poder editarse.

1. Vaya al entorno en el que desea editar el paquete. Este es el entorno en el que se creó originalmente el paquete.
1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configuración]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccione **Sistema** en la navegación izquierda y, a continuación, **Promoción del entorno**.
1. Seleccione el paquete en la lista mostrada.
1. (Condicional) Para ver los paquetes deshabilitados, habilite la opción **Mostrar paquetes retirados**.
1. (Opcional) Para ver el contenido, incluidos todos los objetos y sus subobjetos, haga clic en la flecha desplegable situada junto al tipo de objeto en la sección **Contenido**.
1. (Opcional) Para ver instalaciones e intentos de instalación anteriores de este paquete, haga clic en **Implementaciones**.
1. (Opcional) Para editar el paquete, haga clic en **Editar paquete** en la parte superior derecha de la pantalla.
Un paquete debe estar en estado `DRAFT` para poder editarse. Para mover el paquete al estado `DRAFT`, en el campo **Estado**, seleccione `Draft`. A continuación, puede seguir editando el paquete.
1. Para instalar el paquete, haga clic en **Instalar**, en la parte superior derecha de la pantalla.

   Para obtener instrucciones sobre cómo instalar un paquete, consulte [Instalar un paquete de promoción de entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).

## Creación de un paquete a partir de una comparación de objetos

Puede crear un paquete directamente a partir de una comparación de objetos.

1. Cree una comparación de objetos, tal como se describe en [Comparar objetos entre entornos](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).
1. En la comparación generada, seleccione los objetos que desea incluir en el paquete.
1. Haga clic en **Crear paquete** en la esquina superior derecha de la pantalla.
1. Introduzca un nombre y una descripción para el paquete.
1. Haga clic en **Crear paquete** en la ventana Crear paquete.

   Se genera el paquete.
