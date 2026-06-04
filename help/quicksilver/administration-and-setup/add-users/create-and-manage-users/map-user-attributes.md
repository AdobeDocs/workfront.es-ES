---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Asignar atributos de usuario
description: Mediante el inicio de sesión único (SSO), puede pasar atributos del Active Directory de su proveedor de identidades a los usuarios de Adobe Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
TQID: https://experienceleague.adobe.com/nuU1cn2BDPN7k-gr7a3t5JFR54zD9gHaxBeESEL53p0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 595
ht-degree: 95%

---

# Asignar atributos de usuario

<!--Audited 2/2024-->

Mediante el inicio de sesión único (SSO), puede pasar atributos del Active Directory de su proveedor de identidades a los usuarios de Adobe Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>Debe ser administrador de Workfront</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sugerencias para asignar atributos

Tenga en cuenta lo siguiente al asignar atributos:

* Realice siempre pruebas en una zona protegida de vista previa o una zona protegida de actualización del cliente (CR).
* Realice pruebas con cuentas de administrador y de otro tipo para confirmar que está asignando los atributos correctamente.
* Los atributos asignados se aplican cada vez que un usuario inicia sesión con el inicio de sesión único.

  Ejemplo: si asigna “apellidos” y actualiza su nombre en Workfront sin actualizar el valor en su proveedor de identidad, los apellidos se sobrescribirán para que coincidan con el valor del proveedor de identidad la próxima vez que el usuario inicie sesión.

## Asignar atributos de usuario para su organización

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-left.png) en la esquina superior izquierda de Adobe Workfront y, a continuación, haga clic en **Configurar** ![Icono de configuración de engranajes](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Inicio de sesión único (SSO)**.

1. Seleccione la ficha **Adobe**.

1. (Opcional y condicional) Si su organización tenía la asignación de atributos configurada en la experiencia clásica y desea copiar esa asignación de atributos en la experiencia unificada de Adobe, haga clic en **Migrar asignaciones**. A continuación, puede descartar, eliminar o editar estas asignaciones.

   >[!NOTE]
   >
   >Se recomienda migrar las asignaciones la primera vez que se configuren en la experiencia unificada de Adobe. No pasa nada por migrarlos de nuevo más adelante, pero hacerlo más de una vez es innecesario.

1. Para crear una nueva asignación de atributos, haga clic en **Añadir asignación**.

1. Haga clic en la flecha situada junto al nombre del campo Workfront y seleccione el campo de [!DNL Workfront] al que desee asignar.

1. (Opcional) Si desea crear más de una regla para un campo determinado, haga clic en la flecha situada junto a **Siempre** y seleccione el operador que desea que utilice la regla.

1. (Condicional) Si ha seleccionado un operador además de Siempre, seleccione el campo Workfront y el valor a los que se aplica el operador.

   >[!NOTE]
   >
   >Los operadores `Is Truthy` y `Is Falsy` no requieren valores.

1. Seleccione si desea aplicar el valor de un atributo en el administrador de identidades al campo Workfront o si desea aplicar un valor constante específico.

1. Introduzca el nombre del campo del administrador de identidades que desea aplicar o el texto del valor de constante que desea aplicar.

1. (Opcional) Para añadir más reglas para el mismo campo de Workfront, haga clic en **Añadir nueva regla** y siga los pasos 4-9.

   >[!IMPORTANT]
   >
   > * Se ignorará cualquier regla que se encuentre por debajo de la regla Siempre. Si tiene una regla Siempre, debe moverla al final de la lista de reglas. Para mover reglas en la lista, haga clic en el menú de tres puntos situado a la derecha de la regla y mueva la regla hacia arriba o hacia abajo.
   > * Para crear una regla en medio de la lista, haga clic en el menú de tres puntos situado junto a la regla que desea que esté por encima o por debajo de la nueva regla y seleccione **Añadir regla por encima** o **Añadir regla por debajo**.

1. Para eliminar una regla, haga clic en el menú de tres puntos situado junto a la regla que desea eliminar y seleccione **Eliminar**.
1. Para eliminar una asignación, haga clic en el icono **Eliminar** que se encuentra en la tarjeta de esa asignación.

1. Para guardar, desplácese hasta la parte superior de la página y haga clic en **Guardar**.


