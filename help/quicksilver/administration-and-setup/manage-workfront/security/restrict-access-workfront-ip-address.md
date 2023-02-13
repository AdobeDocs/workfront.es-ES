---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Restringir el acceso a Adobe Workfront por dirección IP
description: Puede configurar una lista de permitidos IP de Adobe Workfront que limite el acceso a Workfront a 45 direcciones IP o intervalos de direcciones IP que especifique. Esto proporciona una capa adicional de seguridad para la aplicación Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 1%

---

# Restringir el acceso a Adobe Workfront por dirección IP

Puede configurar una lista de permitidos IP de Adobe Workfront que limite el acceso a Workfront a 45 direcciones IP o intervalos de direcciones IP que especifique. Esto proporciona una capa adicional de seguridad para la aplicación Workfront.

El administrador de la red debe proporcionar estas direcciones IP o intervalos de direcciones IP.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Empresa</p> </td> 
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

## Otras listas de permitidos

Si el servidor de firewall o de correo está configurado para permitir el acceso solo a determinados proveedores, debe añadir ciertas direcciones IP a su lista de permitidos. Esto abre la comunicación entre su entorno y los servidores de Adobe Workfront. Para obtener información al respecto, consulte [Configurar la lista de permitidos del cortafuegos](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Además, si su organización utiliza el plan de Enterprise, puede configurar la lista de permitidos de correo electrónico de Workfront para controlar qué dominios de correo electrónico pueden aceptar correos electrónicos de Workfront y qué dominios de correo electrónico pueden estar en la dirección de correo electrónico que especifican los usuarios en su perfil de usuario de Workfront. Para obtener más información, consulte [Configurar la lista de permitidos de correo electrónico](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Adición de direcciones IP a la lista de permitidos

Después de agregar direcciones IP a la lista de permitidos de Workfront, solo se pueden usar esas direcciones IP para acceder a Workfront. Los usuarios que intentan acceder a Workfront desde otra dirección IP reciben un mensaje de error que indica que su dirección IP está bloqueada.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Información del cliente.**

1. En el **LISTA DE PERMITIDOS IP** , seleccione **Habilitar la lista de permitidos IP.**

   Esta opción está desactivada de forma predeterminada.

1. Especifique la dirección IP que está utilizando para acceder al sistema de Workfront.

   O

   Especifique un rango de direcciones IP que incluya la que está utilizando actualmente para acceder al sistema Workfront.

   La dirección IP que utiliza para acceder a Workfront debe agregarse a la lista de permitidos antes de habilitar la lista de permitidos.

1. Haga clic en **Añadir rango de IP,** a continuación, especifique la dirección IP o el rango de direcciones IP a las que desea poder acceder a Workfront.
1. (Opcional) Repita el paso anterior para agregar direcciones IP o intervalos de direcciones IP adicionales.

   Se pueden agregar hasta 45 direcciones o rangos.

1. Haga clic en **Guardar.**
