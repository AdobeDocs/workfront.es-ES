---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Habilitar el almacenamiento empresarial de Adobe para su organización
description: Puede habilitar el almacenamiento empresarial de Adobe para que su organización utilice una solución de almacenamiento unificado para todos los productos de Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b3c8559ddac934cc41461f88503b2fa71abaf452
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 11%

---

# Habilitar el almacenamiento empresarial de Adobe para su organización

El almacenamiento empresarial de Adobe es una solución de almacenamiento unificado para todos los productos de Adobe. Es una solución de almacenamiento basada en la nube que sirve como repositorio central para los recursos de los productos empresariales de Adobe.

El almacenamiento empresarial de Adobe está habilitado de forma predeterminada para los clientes nuevos y se puede habilitar para los clientes existentes tras la renovación del contrato.

Para obtener más información sobre el almacenamiento empresarial de Adobe, consulte [Información general sobre el almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p>Cualquier paquete de flujo de trabajo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Habilitar el almacenamiento empresarial de Adobe para su organización

Para habilitar el almacenamiento empresarial de Adobe para su organización:

{{step-1-to-setup}}

1. Seleccione **Sistema** en el panel de navegación izquierdo, luego seleccione **Preferencias**.
1. Desplácese hacia abajo hasta la sección **Preferencias de almacenamiento**.
1. En el menú desplegable Predeterminado, seleccione **Almacenamiento empresarial de Adobe**.
1. (Opcional) Si desea utilizar una combinación de almacenamiento empresarial de Adobe y almacenamiento de Workfront heredado, active la casilla de verificación **Permitir al usuario seleccionar el proveedor de almacenamiento**.

   >[!NOTE]
   >
   >Al habilitar esta opción, los usuarios pueden seleccionar el proveedor de almacenamiento cuando creen un nuevo proyecto. almacenamiento empresarial está etiquetado como &quot;Nuevo proyecto&quot; ya que es el proveedor de almacenamiento predeterminado. El almacenamiento heredado de Workfront está etiquetado como &quot;Proyecto heredado&quot;.
   >
   >![nuevas opciones de proyecto y de proyecto heredado](assets/new-esm-project.png)

1. En el menú desplegable Se aplica a, elija una de las siguientes opciones:

   - **Organización completa**: esta opción aplica el proveedor de almacenamiento predeterminado a todo el entorno de Workfront. Cada vez que un usuario cree un nuevo proyecto, se utilizará el proveedor de almacenamiento predeterminado.
   - **Grupos específicos**: esta opción aplica el proveedor de almacenamiento predeterminado solamente a grupos específicos dentro de su organización. Cada vez que un usuario de los grupos especificados cree un nuevo proyecto, se utilizará el proveedor de almacenamiento predeterminado

1. Haga clic en **Guardar**.

   >[!NOTE]
   >
   >Los proyectos existentes mantienen el modelo de almacenamiento con el que se crearon. Por ejemplo, los proyectos que utilizan el almacenamiento empresarial de Adobe siguen utilizando el almacenamiento empresarial de Adobe después de cambiar la preferencia de almacenamiento predeterminada.
