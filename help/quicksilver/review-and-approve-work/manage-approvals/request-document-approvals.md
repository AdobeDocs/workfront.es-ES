---
product-area: documents
navigation-topic: approvals
title: Solicitar aprobaciones de documentos
description: Puede solicitar la aprobación de los administradores u otros usuarios de un documento en Adobe Workfront. También puede solicitar aprobaciones de documentos a usuarios sin cuentas de Workfront si el administrador de Workfront ha habilitado esta capacidad, tal como se describe en Configuración de las preferencias de seguridad del sistema.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 99%

---

# Solicitar aprobaciones de documentos

Puede solicitar la aprobación de los administradores u otros usuarios de un documento en Adobe Workfront. También puede solicitar aprobaciones de documentos a personas sin cuentas de Workfront si el administrador de Workfront ha habilitado esta capacidad, tal como se describe en [Configurar las preferencias de seguridad del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización o superior a Proyectos, Tareas, Problemas, Plantillas, Portafolios, Programas, Informes, Tableros y Calendarios, Documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de administración al objeto asociado con el acceso de solicitud o la aprobación </p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Solicitar la aprobación de un documento

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del Resumen y empiece a escribir en el cuadro de texto **Añadir aprobador**. Puede añadir usuarios de Workfront por nombre o usuarios externos por correo electrónico.

1. Si el administrador de Adobe Workfront ha habilitado la capacidad de colaborar con personas que no usan Workfront, tal como se describe en [Configurar las preferencias de seguridad del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), puede escribir sus direcciones de correo electrónico para incluirlas.

   No se puede solicitar la aprobación de equipos o grupos.

1. Repita el paso anterior para añadir otros aprobadores.

## Volver a enviar una aprobación para una nueva versión

Las decisiones de aprobación de documentos no se restablecen automáticamente al cargar una nueva versión. Por ejemplo, si el documento se aprueba con cambios, la decisión mostrará “cambios” como la decisión, aunque cargue una nueva versión con los cambios especificados. Puede borrar la decisión sobre una nueva versión si vuelve a enviar manualmente la aprobación.

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del Resumen, haga clic en el icono Más y, a continuación, haga clic en Volver a enviar.

   ![Volver a enviar aprobación](assets/nwe-resubmit-approval-350x149.png)

## Eliminar una solicitud de aprobación de un documento

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del resumen y, a continuación, haga clic en el menú **Más**, en línea con el nombre del aprobador, y seleccione **Eliminar**.

   La solicitud de aprobación se elimina y el aprobador recibe una notificación que le informa de que ya no necesita su aprobación. También se elimina su acceso compartido relacionado con la aprobación.

## Enviar un recordatorio a un aprobador

Puede enviar un mensaje a un aprobador para recordarle que el documento espera sus comentarios.

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del resumen y, a continuación, haga clic en el menú **Más** en línea con el nombre del aprobador y seleccione **Recordar**.

   El aprobador recibe una notificación que le informa de que la aprobación sigue pendiente. También pueden recibir un recordatorio por correo electrónico si está habilitado.
