---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Evite la suplantación y añada [!DNL Adobe Workfront] Registros de SPF
description: Si los usuarios no reciben [!DNL Adobe Workfront] notificaciones por correo electrónico, debe añadir [!DNL Workfront] Registros de SPF en el cortafuegos. Debe trabajar con su equipo de TI para añadir registros SPF.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Evite la suplantación y añada [!DNL Adobe Workfront] Registros de SPF

## Problema

Si los usuarios no reciben [!DNL Adobe Workfront] notificaciones por correo electrónico, debe añadir [!DNL Workfront] Registros de SPF en el cortafuegos. Debe trabajar con su equipo de TI para añadir registros SPF.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser un [!DNL Workfront] administrador. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

Si ya agregó las direcciones IP a la lista de permitidos para el entorno de producción como se describe en [Configuración de la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) y los usuarios de siguen sin recibir correos electrónicos:

1. Añada el siguiente registro SPF al cortafuegos:

   *spf.workfront.com*

   Esto agrega automáticamente todo [!DNL Workfront] Direcciones IP a su lista de permitidos en su cortafuegos y permite que todos los filtros de spam (que utilizan registros SPF) validen [!DNL Workfront] como remitentes válidos para su dominio.

   >[!NOTE]
   >
   > Un registro SPF es un registro TXT que forma parte de un archivo de zona DNS. No admitimos la modificación del archivo de zona DNS.

1. Debe especificar qué tipo de registro SPF se debe configurar. Estos son los tipos válidos de registros SPF:

   * todo (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * existe (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   Por ejemplo, &quot;v=spf1 a mx include: spf.workfront.com -all&quot;

Si no puede añadir registros SPF al cortafuegos debido a la directiva de la empresa, colabore con su [!DNL Workfront] Representante de asistencia.
