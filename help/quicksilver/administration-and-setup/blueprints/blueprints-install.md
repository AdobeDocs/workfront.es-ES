---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Instalar un modelo
description: Puede instalar un modelo en el entorno de producción o un entorno de zona protegida.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Instalar un modelo

Puede instalar un modelo en el entorno de producción o un entorno de zona protegida.

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
   <td role="rowheader"><strong>Licencia de Adobe [!DNL Workfront]</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL Administrador del sistema]</p> </td> 
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
        <td><strong>Vista previa de zona protegida</strong></td>
        <td>La vista previa de zona protegida es un entorno de prueba que sirve como réplica del entorno en directo y Workfront la actualiza cada fin de semana. Todos los paquetes de asistencia tienen acceso a la vista previa de espacio aislado. Para obtener más información, vea <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">El entorno de espacio aislado de vista previa [!DNL Adobe Workfront]</a>.</td>
    </tr>
    <tr>
        <td><strong>Espacio aislado 1 y 2</strong></td>
        <td>La zona protegida de actualización personalizada es un entorno de prueba independiente que actualiza manualmente. Hay un coste adicional para obtener la zona protegida de actualización personalizada. Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">El entorno de espacio aislado de actualización personalizado de [!DNL Adobe Workfront]</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Se recomienda instalar primero el modelo en un entorno de zona protegida. De este modo, puede probar el contenido del modelo y asegurarse de que sea adecuado para su organización sin realizar cambios en los datos activos.

>[!NOTE]
>
>Algunos modelos solo están disponibles para su instalación en el entorno de vista previa con fines de prueba. Si accede al contenido de solo vista previa en el entorno de producción, en la zona protegida 1 o en la zona protegida 2, el botón de instalación no estará activo y podría ver un mensaje de advertencia.\
>Además, la capacidad de cambiar de entorno es limitada al acceder a contenido de solo vista previa, incluso cuando se encuentra en el entorno de vista previa.

## Instalar el modelo

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y luego haga clic en **[!UICONTROL Modelos]**.
1. Busque el modelo que desee instalar. Puede filtrar por caso de uso, nivel de madurez, estado de instalación y tipo en el lado derecho.
1. (Opcional) Haga clic en **[!UICONTROL Detalles]** para conocer el funcionamiento del modelo.
1. Haga clic en **[!UICONTROL Instalar]**.
1. Elija instalar en el entorno de producción o en un entorno de zona protegida.\
   Para obtener más información, consulte [¿Dónde debo instalar un modelo?](#where-should-i-install-a-blueprint) sección de este artículo.
1. En la página [!UICONTROL Configurar], puede elegir realizar una de las siguientes acciones:

   * Instale el modelo tal cual. Para los tipos de modelo que no requieren ninguna configuración, esta es la única opción. Para los tipos de modelo que necesitan configuración, puede elegir instalar el modelo ahora y configurarlo más adelante. Haga clic en **[!UICONTROL Instalar tal cual]**.
   * Configure el modelo antes de la instalación para los modelos que requieran configuración. Realice las selecciones de configuración y haga clic en **[!UICONTROL Instalar modelo]**.\

     Para obtener más información, consulte [Configurar un modelo](../../administration-and-setup/blueprints/configure-template-package.md).
Cuando finaliza la instalación, un mensaje muestra una lista de los objetos específicos (como roles, equipos o grupos) que se instalaron correctamente con el modelo y los objetos que no se instalaron.

Después de instalar el modelo, es posible que se necesiten algunas acciones adicionales para implementarlo por completo. Para obtener más información, consulte [Acciones que se deben realizar después de instalar un modelo](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
