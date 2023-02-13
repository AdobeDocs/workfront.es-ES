---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Asignación de atributos de usuario y provisión automática de nuevos usuarios
description: Mediante el inicio de sesión único (SSO), puede pasar atributos de Active Directory del proveedor de identidad a los usuarios de Adobe Workfront. También puede agregar nuevos usuarios a Workfront mediante la opción de aprovisionamiento automático (también denominada Aprovisionamiento justo a tiempo o JIT).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 2%

---

# Asignación de atributos de usuario y provisión automática de nuevos usuarios

Mediante el inicio de sesión único (SSO), puede pasar atributos de Active Directory del proveedor de identidad a los usuarios de Adobe Workfront. También puede agregar nuevos usuarios a Workfront mediante la opción de aprovisionamiento automático (también denominada Aprovisionamiento justo a tiempo o JIT).

>[!NOTE]
>
>Esto no está disponible si su organización se ha incorporado a Adobe Admin Console. Si necesita más información, consulte con su administrador de red o TI.


## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Sugerencias para asignar atributos

Tenga en cuenta lo siguiente al asignar atributos:

* Realice pruebas siempre en un simulador para pruebas de vista previa o en un simulador para pruebas de actualización del cliente (CR).
* Pruebe con cuentas de administrador y de no administrador para confirmar que está asignando atributos correctamente.
* Los atributos se asignan cada vez que un usuario inicia sesión en Workfront mediante SSO, no solo durante el aprovisionamiento automático.

## Asignación de atributos de usuario y provisión automática de nuevos usuarios

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Inicio de sesión único (SSO)**.

1. En el **Tipo** desplegable, haga clic en **SAML 2.0**.

1. Haga clic en **Asignar atributos de usuario**.

   ![](assets/map-user-attributes.png)

1. (Opcional) Si desea que Workfront cree nuevos usuarios a partir de Active Directory automáticamente, haga clic en **Aprovisionamiento automático de usuarios**.

   Esta función requiere la asignación de atributos.

1. En la fila de opciones que aparece, asigne los atributos que necesite para sus usuarios de Workfront.

   Puede asignar atributos como Dirección, Administrador, Función de trabajo, Grupo en el hogar, etc.

   Las asignaciones de atributos funcionan en una proporción 1:1. Por ejemplo, no se pueden establecer todos los grupos a los que pertenece un usuario; solo puede configurar uno por usuario.

   >[!IMPORTANT]
   >
   >Se requieren los siguientes atributos para cada usuario:
   >      
   >* Nombre
   >* Apellido
   >* Dirección de correo electrónico

   >      
   >No se recomienda asignar niveles de acceso en las asignaciones de atributos. Si lo hace, tenga cuidado al configurar el valor predeterminado para asegurarse de no eliminar el acceso de administrador de forma involuntaria.

   La tabla siguiente explica los campos que puede utilizar para asignar atributos:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Atributo de usuario de Workfront</td> 
      <td>Elija el nombre del atributo que está asignando</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atributo de directorio</td> 
      <td>Escriba la etiqueta de atributo SSO que desee utilizar./td&gt; 
     </tr> 
     <tr> 
      <td role="rowheader">Valor predeterminado</td> 
      <td> <p>Después de elegir un atributo de usuario de Workfront, si el valor es NULL durante la conexión, este campo se rellena con el valor predeterminado correspondiente en el sistema. Escriba un valor aquí solo si planea aplicar reglas de asignación de atributos (consulte el paso 7). El valor predeterminado actúa como excepción a esas reglas.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Haga clic en **Reglas** para agregar una regla al atributo .

   1. En la lista desplegable , elija el modificador de atributos que desee utilizar.
   1. En los 2 campos a la derecha, escriba el valor del atributo de directorio y el valor por el que desea reemplazarlo.

      ![](assets/rule-fields.png)
   Puede hacer clic en **Agregar regla** para agregar más reglas al atributo.

1. (Opcional) Para asignar más atributos de usuario, haga clic en **Agregar asignación** y repita los pasos 6-7.
1. Haga clic en **Guardar**.
