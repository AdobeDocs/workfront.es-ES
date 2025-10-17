---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Instalar un modelo
description: Instale un modelo en el entorno de producción o un entorno de zona protegida.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 74%

---

# Instalar un modelo

<!-- Audited: 5/2025 -->

Instale un modelo en el entorno de producción o un entorno de zona protegida.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Administrador de Workfront</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## ¿Dónde se debería instalar un modelo? {#where-should-i-install-a-blueprint}

Instale el paquete en cualquiera de los siguientes entornos:

<table style="table-layout:auto">
        <tr>
        <td><strong>Producción</strong></td>
        <td>La producción es el entorno en directo.</td>
    </tr>
    <tr>
        <td><strong>Vista previa de zona protegida</strong></td>
        <td>La vista previa de zona protegida es un entorno de prueba que sirve como réplica del entorno en directo y Adobe Workfront la actualiza cada fin de semana. Todos los paquetes de asistencia tienen acceso a la vista previa de la zona protegida. Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">La [!DNL Adobe Workfront]vista previa del entorno de zona protegida</a>.</td>
    </tr>
    <tr>
        <td><strong>Zonas protegidas 1 y 2</strong></td>
        <td>La zona protegida de actualización personalizada es un entorno de prueba independiente que se actualiza manualmente por usted. La zona protegida de actualización personalizada tiene un coste adicional. Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">El [!DNL Adobe Workfront]entorno de zona protegida de actualización personalizado</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Se recomienda instalar primero el modelo en un entorno de espacio aislado. De este modo, es posible probar el contenido del modelo y asegurarse de que sea adecuado para la organización sin realizar cambios en los datos activos.

>[!NOTE]
>
>Algunos modelos solo están disponibles para su instalación en el entorno de vista previa con fines de prueba. Al acceder al contenido de solo vista previa en el entorno de producción, en la zona protegida 1 o en la zona protegida 2, el botón de instalación no estará activo y podría ver un mensaje de advertencia.\
>Además, la capacidad de cambiar de entorno es limitada al acceder a contenido de solo vista previa, incluso cuando se encuentra en el entorno de vista previa.

## Instalación del modelo

{{step1-to-blueprints}}

1. Busque el modelo que desee instalar. Puede filtrar por caso de uso, nivel de madurez, estado de instalación y tipo en la parte derecha de la página.
1. (Opcional) Haga clic en **[!UICONTROL Detalles]** para conocer el funcionamiento del modelo.
1. Haga clic en **[!UICONTROL Instalar]**.
1. Elija instalar en el entorno de producción o en un entorno de zona protegida.\
   Para obtener más información, consulte la sección [¿Dónde se instalan los modelos?](#where-should-i-install-a-blueprint) de este artículo.
1. En la página **Configurar**, realice una de las siguientes acciones:

   * Instalar el modelo tal cual. Para aquellos tipos de modelo que no requieran ninguna configuración, esta es la única opción. Para aquellos tipos de modelo que necesiten configuración, es posible instalar el modelo ahora y configurarlo más adelante. Haga clic en **[!UICONTROL Instalar tal cual]**.
   * Es necesario configurar el modelo antes de la instalación para aquellos modelos que requieran configuración. Realice las selecciones de configuración y haga clic en **[!UICONTROL Instalar modelo]**.

     Para obtener más información, consulte [Configurar un modelo](../../administration-and-setup/blueprints/configure-template-package.md).

   La instalación finaliza y un mensaje muestra una lista de los objetos específicos (como roles, equipos o grupos) que se instalaron correctamente con el modelo y los objetos que no se instalaron.

Después de instalar el modelo, es posible que se necesiten algunas acciones adicionales para implementarlo por completo. Para obtener más información, consulte [Acciones que se deben realizar después de instalar un modelo](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
