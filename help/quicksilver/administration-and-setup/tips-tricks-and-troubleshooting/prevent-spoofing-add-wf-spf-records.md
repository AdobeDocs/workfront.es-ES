---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Impedir la suplantación y agregar  [!DNL Adobe Workfront] registros SPF
description: Si los usuarios no reciben notificaciones por correo electrónico de  [!DNL Adobe Workfront] , debe añadir registros SPF de  [!DNL Workfront]  al cortafuegos. Debe trabajar con su equipo de TI para añadir registros SPF.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 97%

---

# Impedir la suplantación de identidad y añadir registros SPF de [!DNL Adobe Workfront]

## Problema

Si los usuarios no reciben notificaciones por correo electrónico de [!DNL Adobe Workfront], debe añadir registros SPF de [!DNL Workfront] al cortafuegos. Debe trabajar con su equipo de TI para añadir registros SPF.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

Si ya añadió las direcciones IP a su lista de permitidos para su entorno de producción como se describe en [Configuración de la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) y los usuarios siguen sin recibir correos electrónicos:

1. Añada el siguiente registro SPF al cortafuegos:

   *spf.workfront.com*

   Se añadirán automáticamente todas las direcciones IP de [!DNL Workfront] a la lista de permitidos en el cortafuegos y esto permitirá que todos los filtros de correo no deseado (que usan registros SPF) validen los servidores de [!DNL Workfront] como remitentes válidos para su dominio.

   >[!NOTE]
   >
   > Un registro SPF es un registro TXT que forma parte de un archivo de la zona DNS. No es posible modificar el archivo de la zona DNS.

1. Debe especificar qué tipo de registro SPF se tiene que configurar. Estos son los tipos de registros SPF válidos:

   * all (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * exists (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   Por ejemplo, &quot;v=spf1 a mx include: spf.workfront.com -all&quot;

Si no puede añadir registros SPF al cortafuegos debido a la directiva de la compañía, póngase en contacto con el representante de asistencia técnica de [!DNL Workfront].
