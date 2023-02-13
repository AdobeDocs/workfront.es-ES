---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Instalación de un modelo
description: Puede instalar un modelo en el entorno de producción o un entorno de espacio aislado.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Instalación de un modelo

Puede instalar un modelo en el entorno de producción o un entorno de espacio aislado.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licencia</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## ¿Dónde debo instalar un modelo? {#where-should-i-install-a-blueprint}

Puede instalar el paquete en cualquiera de los siguientes entornos:

<table style="table-layout:auto">
        <tr>
        <td><strong>Producción</strong></td>
        <td>La producción es su entorno en directo.</td>
    </tr>
    <tr>
        <td><strong>Vista previa de espacio aislado</strong></td>
        <td>La vista previa de espacio aislado es un entorno de prueba que sirve como réplica del entorno en directo y Workfront la actualiza todos los fines de semana. Todos los paquetes de soporte tienen acceso a la vista previa de Sandbox. Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">La variable [!DNL Adobe Workfront] Entorno de espacio aislado de vista previa</a>.</td>
    </tr>
    <tr>
        <td><strong>Simulador para pruebas 1 y 2</strong></td>
        <td>El Simulador para pruebas de actualización personalizado es un entorno de prueba independiente que usted actualiza manualmente. Hay un coste adicional para obtener el Simulador para pruebas de actualización personalizado. Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">La variable [!DNL Adobe Workfront] Entorno de espacio aislado de actualización personalizada</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Se recomienda instalar primero el modelo en un entorno de entorno limitado. De este modo, puede probar el contenido del modelo y asegurarse de que es adecuado para su organización sin realizar cambios en los datos activos.

>[!NOTE]
>
>Ciertos modelos solo están disponibles para instalarse en el entorno de Vista previa para realizar pruebas. Si accede al contenido de solo vista previa en el entorno de producción, el Simulador para pruebas 1 o el Simulador para pruebas 2, el botón de instalación no está activo y puede que aparezca un mensaje de advertencia.\
>Además, la capacidad de conmutación de entorno es limitada al acceder al contenido solo de vista previa, incluso cuando se encuentra en el entorno de vista previa.

## Instalación del modelo

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Planes]**.
1. Busque el modelo que desea instalar. Puede filtrar por caso de uso, nivel de vencimiento, estado de instalación y escribir a la derecha.
1. (Opcional) Haga clic en **[!UICONTROL Detalles]** para aprender cómo funciona el modelo.
1. Haga clic en **[!UICONTROL Instalar]**.
1. Elija instalar en el entorno de producción o en un entorno de simulación de pruebas.\
   Para obtener más información, consulte la [¿Dónde debo instalar un modelo?](#where-should-i-install-a-blueprint) en este artículo.
1. En el [!UICONTROL Configurar] , puede elegir realizar una de las siguientes acciones:

   * Instale el modelo tal cual. Para los tipos de modelo que no requieren ninguna configuración, esta es la única opción. Para los tipos de modelo que necesitan configuración, puede optar por instalar el modelo ahora y configurarlo más tarde. Haga clic en **[!UICONTROL Instalar tal cual]**.
   * Configure el modelo antes de la instalación, para los modelos que requieren configuración. Realice las selecciones de configuración y haga clic en **[!UICONTROL Instalar modelo]**.\

      Para obtener más información, consulte [Configuración de un modelo](../../administration-and-setup/blueprints/configure-template-package.md).
Cuando se completa la instalación, un mensaje muestra una lista de los objetos específicos (como roles, equipos o grupos) que se instalaron correctamente con el modelo y cualquier objeto que no se instaló.

Después de instalar el modelo, es posible que se necesiten algunas acciones adicionales para implementarlo completamente. Para obtener más información, consulte [Acciones que deben realizarse después de instalar un modelo](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
