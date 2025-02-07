---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Comparar objetos entre entornos
description: Puede comparar objetos entre entornos para asegurarse de que los paquetes de promoción de entornos contengan los objetos que necesita.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 085b0f04-5a9c-49b9-86d7-2363731ee067
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 22%

---

# Comparar objetos entre entornos

Puede comparar objetos entre entornos para asegurarse de que los paquetes de promoción de entornos contengan los objetos que necesita.

Se seleccionan los entornos y los tipos de objetos que se van a comparar. Workfront compara todos los objetos de los tipos seleccionados en ambos entornos y presenta datos sobre las diferencias entre objetos.

## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td>Plan de <strong>[!DNL Adobe Workfront] </strong>
   </td>
   <td> Prime o Ultimate (solo planes nuevos)
   </td>
  </tr>
  <tr>
   <td>Licencias de <strong>[!DNL Adobe Workfront] </strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Su organización debe estar en Adobe Business Platform para comparar objetos entre entornos.

## Generación de una comparación de objetos

1. Vaya a un entorno en el que desee comparar un objeto.
1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configuración]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccione **Sistema** en la navegación izquierda y, a continuación, **Promoción del entorno**.
1. Haga clic en **Comparar entornos** cerca de la esquina superior derecha de la pantalla.
1. En el campo **Entorno de Source**, seleccione el entorno en el que desea crear el paquete. Es el entorno **desde el que** está copiando objetos.
1. En el campo **Entorno de destino**, seleccione el entorno en el que desea instalar el paquete. Este es el entorno en el que está copiando los objetos **a**.
1. En el área **Objetos para comparar**, seleccione los tipos de objetos que desea comparar entre entornos.
1. Haga clic en **Generar comparación** cerca de la esquina superior derecha de la pantalla.

   La comparación puede tardar algún tiempo en generarse, según el número y el tamaño de los objetos comparados.

## Ver comparación de objetos

Una vez completada la generación de la comparación, se muestra la comparación.

La lista incluye objetos de los tipos seleccionados que existen en el entorno de origen, si esos objetos faltan en el entorno de destino y si hay diferencias de campo entre los dos.

>[!BEGINSHADEBOX]

![Ejemplo de comparación](assets/environment-promotion-comparison.png)

En este ejemplo:

* La primera línea muestra un objeto que está presente en el entorno de destino, pero que es diferente del entorno de origen.
* La segunda línea muestra un objeto que está presente en el entorno de destino y es el mismo que en el entorno de origen.
* La tercera línea muestra un objeto que no está presente en el entorno de destino.

>[!ENDSHADEBOX]

Para ver diferencias de objeto específicas:

1. Haga clic en el icono de lupa ![Comparar icono](assets/compare-icon.png) en la línea de ese objeto.

   Se abre una ventana con todos los campos de ese objeto. las diferencias se marcan en rojo.

## Creación de un paquete a partir de una comparación de objetos

Puede crear un paquete directamente a partir de una comparación de objetos.

Para obtener instrucciones, consulte [Crear un paquete a partir de una comparación de objetos](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison) en el artículo Crear o editar un paquete de promoción de entorno.
