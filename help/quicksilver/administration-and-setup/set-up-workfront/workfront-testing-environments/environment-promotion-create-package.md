---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Crear o editar un paquete de promoción de entorno
description: La capacidad de promoción de entornos está diseñada para proporcionar la capacidad de mover objetos relacionados con la configuración de un entorno a otro. Aprenda a crear un paquete de promoción de entorno que luego pueda instalar en un entorno diferente.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 6f5da5ede6bb8c98b26d7d37366670c89ded6c49
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Crear o editar un paquete de promoción de entorno

Debe crear un paquete en el entorno en el que desee copiar los objetos **de**. Por ejemplo, si está configurando un proyecto en el entorno de espacio aislado de actualización personalizado y lo está promocionando al entorno de producción, debe crear el paquete en el entorno de espacio aislado de actualización personalizado.

>[!IMPORTANT]
>
>Si la zona protegida de actualización personalizada se actualiza mientras configura un objeto para la promoción del entorno, esa configuración se perderá durante la actualización. Le recomendamos que no actualice la zona protegida de actualización personalizada a menos que todos los objetos y paquetes de promoción de entorno pendientes se hayan promocionado correctamente.

## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Prime o Ultimate (solo planes nuevos)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licencias</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser un [!DNL Workfront] administrador.
   </td>
  </tr>
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creación de un paquete

1. Vaya al entorno en el que desea crear el paquete. Este es el entorno en el que está copiando los objetos **de**.
1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccionar **Sistema** en el panel de navegación izquierdo, seleccione **Promoción de entorno**.
1. Clic **Crear paquete**.

   Se abre la página Nuevo paquete de promociones.

1. En el **Nombre del paquete** , introduzca un nombre para el paquete.
1. En el **Descripción** , introduzca una descripción para este paquete.
1. Para añadir un objeto al paquete, haga clic en **Agregar objetos** en el panel de navegación izquierdo, seleccione el tipo de objeto que desea añadir.
1. Seleccione uno o varios objetos de la lista o escriba el nombre en la barra de búsqueda y seleccione el objeto cuando aparezca en la lista. Puede seleccionar más de un objeto en la lista.
1. Clic **Agregar (objetos X)** para añadir los objetos seleccionados al paquete.

   >[!INFO]
   >
   >**Ejemplo**
   >
   >Si ha seleccionado tres proyectos para agregarlos al proyecto, el botón indica **Agregar 3 proyectos**.

   Los objetos que ha añadido aparecen en el área Contenido del paquete a la derecha de la página.

1. Para agregar otro tipo de objeto, repita los pasos 7-9.
1. (Opcional) Para eliminar un objeto del paquete, pase el ratón sobre el objeto en el área Contenido del paquete y, a continuación, haga clic en la X junto al objeto.
1. Una vez añadidos todos los objetos deseados al paquete, haga clic en **Guardar y cerrar** para guardar el paquete sin montarlo.

   O

   Clic **Guardar y montar** para guardar y montar el paquete.

   >[!NOTE]
   >
   >* Los botones Guardar y Cerrar y Guardar y Montar están disponibles si un paquete tiene un nombre con cinco o más caracteres y al menos un objeto añadido.
   >* No puede montar un paquete que esté en un estado instalable como Pruebas o Activo.

## Editar o montar un paquete existente

1. Vaya al entorno en el que desea crear el paquete. Este es el entorno en el que está copiando los objetos **de**.
1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccionar **Sistema** en el panel de navegación izquierdo, seleccione **Promoción de entorno**.
1. Seleccione el paquete en la lista mostrada.
1. (Condicional) Para ver los paquetes deshabilitados, habilite la variable **Mostrar paquetes retirados** opción.
1. (Opcional) Para ver el contenido, incluidos todos los objetos y sus subobjetos, haga clic en la flecha desplegable situada junto al tipo de objeto en la **Contenido** sección.
1. (Opcional) Para ver las instalaciones anteriores y los intentos de instalación de este paquete, haga clic en **Implementaciones**.
1. (Opcional) Para editar el paquete, haga clic en **Editar paquete** en la parte superior derecha de la pantalla.
1. Para instalar el paquete, haga clic en **Instalar** en la parte superior derecha de la pantalla.

   Para obtener instrucciones sobre la instalación de un paquete, consulte [Instalación de un paquete de promoción de entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
