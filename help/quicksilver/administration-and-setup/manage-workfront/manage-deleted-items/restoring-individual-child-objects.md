---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restauración de objetos secundarios individuales
description: En este documento se describe cómo obtener ayuda para recuperar objetos secundarios individuales que se han eliminado de los entornos de producción o vista previa de Adobe Workfront menos de 30 días antes.
feature: System Setup and Administration
role: Admin
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# Restauración de objetos secundarios individuales

En este documento se describe cómo obtener ayuda para recuperar objetos secundarios individuales que se han eliminado de los entornos de producción o vista previa de Adobe Workfront menos de 30 días antes.

Un administrador de Workfront puede restaurar proyectos, tareas, problemas y documentos en cada instancia de Workfront, tal como se describe en [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Sin embargo, solo el equipo de la base de datos de Workfront puede restaurar objetos como tareas, problemas, documentos, formularios personalizados, horas y notas independientemente de su objeto principal.

Los datos de su entorno en directo están disponibles en el Simulador para pruebas de vista previa durante un máximo de 7 días. Esto significa que puede exportar los datos independientes desde el entorno de la zona de pruebas de vista previa mediante los siguientes métodos:

* Kick-Starts
* Creación de un informe y exportación de los resultados

Para obtener más información sobre la exportación de datos desde Workfront, consulte [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Puede importar los datos exportados de las siguientes maneras:

* Manualmente, si utiliza informes exportados
* De forma masiva, si está usando Kick-Starts

   Para obtener más información sobre la importación de datos en Workfront mediante Kick-Starts, consulte [Importar datos en Adobe Workfront mediante una plantilla de inicio rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

El entorno de espacio aislado de vista previa se actualiza durante nuestras ventanas de mantenimiento durante el fin de semana.

Para obtener más información sobre las ventanas de mantenimiento para el entorno de espacio aislado de vista previa, consulte [trust.workfront.com](https://trust.workfront.com/).

>[!IMPORTANT]
>
>Los documentos son una excepción a estos métodos de restauración. Puede descargarlos manualmente desde el entorno de vista previa y volver a cargarlos en el entorno de producción. Si desea descargar y cargar documentos de forma masiva, deberá solicitar una restauración de datos de Workfront.

## Información necesaria para una restauración de datos

Una vez que haya determinado que un objeto eliminado necesita ser restaurado por nuestro equipo de base de datos, recopile toda la información que tenga sobre él. Los administradores de nuestra base de datos necesitan la siguiente información para encontrar el objeto e iniciar una restauración:

* Nombre del objeto
* Tipo de objeto (tarea, problema, proyecto, etc.)
* Fecha y hora estimadas de eliminación
* GUID de objeto (si es posible)

   Consulte la siguiente información al localizar el GUID de un objeto:

   * El GUID se puede encontrar haciendo referencia a las notificaciones de correo electrónico activadas al interactuar con el objeto (asignaciones, comentarios, etc.)
   * Ejemplo de un GUID encontrado al final de una URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Una vez que haya recopilado esta información o si necesita ayuda, llame a nuestro equipo de asistencia al cliente al 844-306-HELP(4357) o envíe un ticket en línea.

## Proceso de restauración de datos

1. Una vez que nuestro equipo de asistencia al cliente reciba su información, la pasará a nuestro equipo de asistencia al cliente.
1. Nuestro equipo de asistencia al cliente se pondrá en contacto con nuestro equipo de bases de datos.
1. Una vez que el equipo de la base de datos ha tenido la oportunidad de revisar los datos que se están restaurando, se puede proporcionar una estimación más precisa para el ETA. Una restauración generalmente tarda tres días, pero puede tardar más en función del tipo y el volumen de los datos que se restauran.
1. El equipo de base de datos restaurará la información en el entorno de espacio aislado de vista previa, donde tendrá la oportunidad de revisar los datos restaurados. Nuestro equipo de asistencia al cliente le informará de cuándo se pueden encontrar los datos en el Simulador para pruebas de vista previa.
1. Una vez que esté satisfecho con la restauración en el simulador de pruebas, informe a nuestro equipo de asistencia al cliente y se pondrá en contacto con nuestro equipo de bases de datos para notificarles que pueden restaurar los datos en su entorno de producción.
1. Tendrá la oportunidad de revisar los datos restaurados antes de que se cierre la solicitud.
