---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restaurar objetos secundarios individuales
description: En este artículo se describe cómo puede obtener ayuda para recuperar objetos secundarios individuales que se hayan eliminado de los entornos de producción o vista previa de Adobe Workfront menos de 30 días antes.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 88%

---

# Restaurar objetos secundarios individuales

En este artículo se describe cómo puede obtener ayuda para recuperar objetos secundarios individuales que se hayan eliminado de los entornos de producción o vista previa de Adobe Workfront menos de 30 días antes.

Un administrador de Workfront puede restaurar proyectos, tareas, problemas y documentos en cada instancia de Workfront, tal como se describe en [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Pero solo el equipo de la base de datos de Workfront puede restaurar objetos como tareas, problemas, documentos, formularios personalizados, horas y notas, independientemente de su objeto principal.

Los datos de su entorno en directo están disponibles en la vista previa de zona protegida durante un máximo de 7 días. Esto significa que puede exportar los datos independientes del entorno de vista previa de zona protegida mediante los siguientes métodos:

* Kick-Starts
* Creación de informes y exportación de resultados

Para obtener más información acerca de cómo exportar datos desde Workfront, consulte [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Puede importar los datos exportados de las siguientes maneras:

* Manualmente, si utiliza informes exportados
* De forma masiva, si utiliza Kick-Starts

  Para obtener más información sobre cómo importar datos en Workfront mediante Kick-Starts, consulte [Importar datos en Adobe Workfront mediante una plantilla de Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

El entorno de vista previa de zona protegida se actualiza durante nuestras ventanas de mantenimiento del fin de semana.

Para obtener más información acerca de las ventanas de mantenimiento del entorno de vista previa de zona protegida, consulte [el estado de página web de Adobe](https://status.adobe.com/es).

>[!IMPORTANT]
>
>Los documentos son una excepción a estos métodos de restauración. Puede descargarlos manualmente desde el entorno de vista previa y volver a cargarlos en el entorno de producción. Si desea descargar y cargar documentos por lotes, deberá solicitar una restauración de datos de Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información necesaria para una restauración de datos

Una vez que haya determinado que nuestro equipo de base de datos debe restaurar un objeto eliminado, recopile toda la información que tenga sobre él. Se requiere la siguiente información para que los administradores de la base de datos encuentren el objeto e inicien una restauración:

* Nombre de objeto
* Tipo de objeto (tarea, problema, proyecto, etc.)
* Fecha y hora estimadas de la eliminación
* GUID de objeto (si es posible)

  Consulte la siguiente información cuando busque el GUID de un objeto:

   * El GUID se puede encontrar haciendo referencia a las notificaciones de correo electrónico activadas por la interacción con el objeto (asignaciones a, comentarios en, etc.)
   * Ejemplo de GUID encontrado al final de una dirección URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Una vez que haya recopilado esta información o si necesita ayuda, llame a nuestro Equipo de Atención al cliente al 844-306-HELP(4357) o envíe un ticket en línea.

## Proceso de restauración de datos

1. Una vez que nuestro Equipo de Atención al cliente reciba su información, la remitirá a nuestro Equipo de Atención al cliente.
1. Nuestro Equipo de Atención al cliente se pondrá en contacto con nuestro Equipo de Base de datos.
1. Una vez que el Equipo de Base de datos haya tenido la oportunidad de revisar los datos que se están restaurando, se puede proporcionar una estimación más precisa para la ETA. Una restauración suele tardar tres días, pero puede tardar más según el tipo y el volumen de datos que se estén restaurando.
1. El Equipo de Base de datos restaurará la información en el entorno de vista previa de zona protegida, donde tendrá la oportunidad de revisar los datos restaurados. Nuestro Equipo de Asistencia al cliente le informará cuando los datos se puedan encontrar en la vista previa de zona protegida.
1. Una vez que esté satisfecho con la restauración en la zona protegida, informe a nuestro Equipo de Atención al cliente, que se pondrá en contacto con nuestro Equipo de Base de datos para notificarles que pueden restaurar los datos en su entorno de producción.
1. Tendrá la oportunidad de revisar los datos restaurados antes de que se cierre la solicitud.
