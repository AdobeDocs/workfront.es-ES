---
product-area: documents
navigation-topic: approvals
title: Solicitar aprobaciones de documentos
description: Puede solicitar la aprobación de los administradores u otros usuarios para un documento en Adobe Workfront. También puede solicitar aprobaciones de documentos a personas que no tengan cuentas de Workfront si el administrador de Workfront ha habilitado esta capacidad, tal como se describe en Configuración de preferencias de seguridad del sistema.
author: Courtney
feature: Work Management
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Solicitar aprobaciones de documentos

Puede solicitar la aprobación de los administradores u otros usuarios para un documento en Adobe Workfront. También puede solicitar aprobaciones de documentos a personas que no tengan cuentas de Workfront si el administrador de Workfront ha habilitado esta capacidad, tal como se describe en [Configuración de las preferencias de seguridad del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver o acceder más a Proyectos, Tareas, Problemas, Plantillas, Portfolio, Programas, Informes, Tableros y Calendarios, Documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o acceder más al objeto asociado con el acceso o la aprobación de la solicitud </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Solicitar la aprobación de un documento

1. Vaya al proyecto, la tarea o el problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.

1. Desplácese hacia abajo hasta el **Aprobaciones** del Resumen y comience a escribir en la sección **Agregar aprobador** cuadro de texto. Puede agregar usuarios de Workfront por nombre o usuarios externos por correo electrónico.

1. Si el administrador de Adobe Workfront ha habilitado la capacidad de colaborar con personas que no usan Workfront, tal como se describe en [Configuración de las preferencias de seguridad del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), puede escribir sus direcciones de correo electrónico para incluirlas.

   No se puede solicitar la aprobación de equipos o grupos.

1. Repita el paso anterior para añadir otros aprobadores.

## Volver a enviar una aprobación en una nueva versión

Las decisiones de aprobación de documentos no se restablecen automáticamente al cargar una nueva versión. Por ejemplo, si el documento está aprobado con cambios, la decisión mostrará &quot;cambios&quot; como decisión, incluso si carga una nueva versión con los cambios especificados. Puede borrar la decisión sobre una nueva versión si vuelve a enviar la aprobación manualmente.

1. Vaya al proyecto, la tarea o el problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.

1. Desplácese hacia abajo hasta el **Aprobaciones** en Resumen, haga clic en el icono Más y, a continuación, haga clic en Volver a enviar .

   ![](assets/nwe-resubmit-approval-350x149.png)

## Eliminar una solicitud de aprobación de documento

1. Vaya al proyecto, la tarea o el problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.

1. Desplácese hacia abajo hasta el **Aprobaciones** en el Resumen y, a continuación, haga clic en la **Más** en línea con el nombre del aprobador y seleccione **Eliminar**.

   La solicitud de aprobación se elimina y el aprobador recibe una notificación de que ya no es necesaria su aprobación. También se elimina su acceso compartido relacionado con la aprobación.

## Enviar un recordatorio a un aprobador

Puede enviar un mensaje para recordar a un aprobador que está esperando sus comentarios.

1. Vaya al proyecto, la tarea o el problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.

1. Desplácese hacia abajo hasta el **Aprobaciones** en el Resumen y, a continuación, haga clic en la **Más** en línea con el nombre del aprobador y seleccione **Recordar**.

   El aprobador recibe una notificación que le informa de que la aprobación sigue pendiente. También pueden recibir un recordatorio por correo electrónico si lo tienen habilitado.
