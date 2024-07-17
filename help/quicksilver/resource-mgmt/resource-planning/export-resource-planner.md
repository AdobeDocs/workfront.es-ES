---
product-area: resource-management
navigation-topic: resource-planning
title: Exportar información del Planificador de recursos
description: Puede exportar información desde cualquier vista del Planificador de recursos a un archivo de Excel (.xlsx) que se guarde en el equipo.
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# Exportar información del Planificador de recursos

Puede exportar información desde cualquier vista del Planificador de recursos a un archivo de Excel (.xlsx) que se guarde en el equipo.

>[!IMPORTANT]
>
>Existen limitaciones en la información que se muestra y en la información que se puede exportar desde el Planificador de recursos. Para obtener información sobre estas limitaciones, consulte [Limitaciones de visualización del Planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Pro y superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización o superior a Proyectos, Usuarios y Administración de recursos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos o superiores para proyectos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Exportar información del Planificador de recursos

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recursos**. Se muestra **Planificador** de forma predeterminada.

1. Seleccione la vista del Planificador. Puede seleccionar una de las siguientes opciones:

   * Ver por usuario
   * Ver por proyecto
   * Ver por rol

1. Haga clic en **Exportar**.

   Aparece el cuadro de diálogo Opciones de exportación.

   ![](assets/rp-export-options-box-350x421.png)

1. Especifique la siguiente información:\
   **Fecha de inicio**: La fecha de inicio de la exportación. El archivo exportado contiene información de asignación y disponibilidad a partir del primer día de la semana que contiene el día especificado aquí.\
   **Número de períodos**: El número de períodos que desea incluir en el archivo. El valor predeterminado es 4 periodos.\
   **Tipo**: Tipo de períodos de tiempo durante los cuales desea mostrar la información en el archivo exportado (semanas, meses o trimestres).\
   Los siguientes son los períodos de tiempo máximos que puede exportar:

   * 52 semanas
   * 36 meses
   * 12 trimestres

   **Seleccionar para exportar**: en función de la vista que haya seleccionado, puede seleccionar exportar la información de disponibilidad y presupuesto de todos los objetos enumerados en la pantalla o de los específicos.
Puede seleccionar exportar la siguiente información:

   * En la vista de proyecto, seleccione para exportar:

      * Proyectos
      * Proyectos y roles
      * Todo (esta es la opción predeterminada)

   * En la vista de usuario, seleccione para exportar:

      * Usuarios
      * Usuarios y proyectos
      * Todo (esta es la opción predeterminada)

   * En la vista de rol, seleccione para exportar:

      * Funciones
      * Roles y proyectos
      * Todo (esta es la opción predeterminada)

   **Formato de datos**: En función de cómo desee que se muestre el archivo de Excel, seleccione las siguientes opciones:

   * **Sin procesar**: seleccione esta opción para mostrar la información de disponibilidad y asignación desagrupada por los objetos a los que pertenece en el archivo de Excel. (esta es la opción predeterminada)
   * **Agrupado**: seleccione esta opción para mostrar la información de disponibilidad y asignación agrupada por los objetos a los que pertenece. Muestra la información exportada tal como aparece en la pantalla.

   En el cuadro de diálogo Opciones de exportación se muestra un ejemplo del aspecto que tendrá la información en el archivo exportado.

1. Haga clic en **Exportar** para exportar la información desde el Planificador de recursos.\
   Solo se exporta la información que ha guardado.

1. (Condicional) Si tiene horas presupuestadas sin guardar en las vistas Rol o Proyecto, haga clic en **Guardar y continuar.**
Se descargará un archivo de Excel (.xlsx) en el equipo.\
   La exportación desde el Planificador de recursos no está disponible mientras el archivo esté preparado para la descarga.\
   (Condicional) Si exporta una gran cantidad de datos, recibe un correo electrónico con un vínculo donde puede descargar el archivo.\
   ![RP_email_with_export_planner_attachment.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Condicional) Cuando reciba el correo electrónico con el archivo exportado, haga clic en **Descargar** para descargar el archivo.\
   Esto le lleva de nuevo a Workfront, donde puede descargar el archivo.\
   Debe iniciar sesión en Workfront para que se complete la descarga.\
   Si no descarga el archivo cuando se envía, el vínculo de descarga permanece activo durante 7 días después de iniciar la exportación.
