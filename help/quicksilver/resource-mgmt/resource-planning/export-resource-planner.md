---
product-area: resource-management
navigation-topic: resource-planning
title: Exportar información del Planificador de recursos
description: Puede exportar información desde cualquier vista del Planificador de recursos a un archivo de Excel (.xlsx) que se guarda en el equipo.
author: Lisa
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
TQID: https://experienceleague.adobe.com/f1tAWm7-QiEGbN-ENKTlJumMK29mqdiZ5PgY-27gzc4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 582
ht-degree: 85%

---

# Exportar información del Planificador de recursos

Puede exportar información desde cualquier vista del Planificador de recursos a un archivo de Excel (.xlsx) que se guarda en el equipo.

>[!IMPORTANT]
>
>Existen limitaciones en la información que se muestra y en la que se puede exportar desde el Planificador de recursos. Para obtener información sobre estas limitaciones, consulte [Limitaciones de visualización del Planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td>
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Ligero o superior</p>
       <p>Revisión o superior</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Ver el acceso o superior a Proyectos, Usuarios y Administración de recursos</p></td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores para proyectos</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exportar información del Planificador de recursos

{{step1-to-resourcing}}

Se muestra el **Planificador** de forma predeterminada.

1. Seleccione la vista del Planificador. Puede seleccionar una de las siguientes opciones:

   * Ver por usuario
   * Ver por proyecto
   * Ver por rol

1. Haga clic en **Exportar**.

   Aparece el cuadro de diálogo Opciones de exportación.

   ![Opciones de exportación](assets/rp-export-options-box-350x421.png)

1. Especifique la siguiente información:\
   **Fecha de inicio**: la fecha de inicio de la exportación. El archivo exportado contiene información de asignación y disponibilidad a partir del primer día de la semana que contiene el día que especifique aquí.\
   **Número de períodos**: el número de períodos que desea incluir en el archivo. El predeterminado son cuatro períodos.\
   **Tipo**: tipo de períodos de tiempo durante los cuales desea mostrar la información en el archivo exportado (semanas, meses o trimestres).\
   Los siguientes son los períodos de tiempo máximos que puede exportar:

   * 52 semanas
   * 36 meses
   * 12 trimestres

   **Seleccionar para exportar**: en función de la vista que haya seleccionado, puede seleccionar exportar la información de disponibilidad y presupuesto de todos los objetos enumerados en la pantalla o de los específicos.
Puede seleccionar exportar la siguiente información:

   * En la vista del proyecto, seleccione exportar:

      * Proyectos
      * Proyectos y roles
      * Todo (esta es la opción predeterminada)

   * En la vista de usuario, seleccione exportar:

      * Usuarios
      * Usuarios y proyectos
      * Todo (esta es la opción predeterminada)

   * En la vista de función, seleccione exportar:

      * Funciones
      * Roles y proyectos
      * Todo (esta es la opción predeterminada)

   **Formato de datos**: en función de cómo desee que se muestre el archivo de Excel, seleccione las siguientes opciones:

   * **Básicos**: seleccione esta opción para mostrar la información de disponibilidad y asignación desagrupada por los objetos a los que pertenece en el archivo de Excel. (esta es la opción predeterminada)
   * **Agrupado**: seleccione esta opción para mostrar la información de disponibilidad y asignación agrupada por los objetos a los que pertenece. Muestra la información exportada tal como aparece en la pantalla.

   En el cuadro de diálogo Opciones de exportación se muestra un ejemplo del aspecto que tendrá la información en el archivo exportado.

1. Haga clic en **Exportar** para exportar la información desde el Planificador de recursos.\
   Solo se exporta la información que ha guardado.

1. (Condicional) Si tiene horas presupuestadas sin guardar en las vistas Rol o Proyecto, haga clic en **Guardar y continuar.**
Se descargará un archivo de Excel (.xlsx) en el equipo.\
   La exportación desde el Planificador de recursos no está disponible mientras el archivo esté preparado para la descarga.\
   (Condicional) Si exporta una gran cantidad de datos, recibe un correo electrónico con un vínculo donde puede descargar el archivo.\
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Condicional) Cuando reciba el correo electrónico con el archivo exportado, haga clic en **Descargar** para descargarlo.\
   Esto le lleva de nuevo a Workfront, donde puede descargar el archivo.\
   Debe iniciar sesión en Workfront para que se complete la descarga.\
   Si no descarga el archivo cuando se envía, el vínculo de descarga permanece activo durante siete días después de iniciar la exportación.
