---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Desinstalar el conector mejorado de Workfront para Adobe Experience Manager
description: Debe desinstalar el conector mejorado de Workfront con Adobe Experience Manager con la última integración nativa que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
TQID: https://experienceleague.adobe.com/CeCyF8zbwp4tVcxQebq0EdaJqagDyppVuCL6ilqEvJA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 260
ht-degree: 92%

---

# Desinstalar Workfront con el conector mejorado de Adobe Experience Manager

Debe desinstalar el conector mejorado de Workfront con Adobe Experience Manager con la última integración nativa que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.

## Requisitos previos

* (Opcional) Si es necesario, revierta los cambios realizados en la configuración del cortafuegos de Workfront y en la configuración de Dispatcher de AEM.

## Desinstalar el conector mejorado

1. Acceda y clone su repositorio de AEM as a Cloud Service desde Cloud Manager.

1. Abra el repositorio de Git clonado en el IDE que desee.

1. Compruebe la rama en la que está instalado el conector mejorado.

1. Vaya a la siguiente ruta y elimine el archivo zip del conector mejorado:

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. Elimine la siguiente dependencia del archivo pom.xml de la raíz del proyecto.

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >Asegúrese de que la versión a la que se hace referencia en el bloque de código anterior, es decir, 1.8.0, refleje la versión que se está desinstalando del código.

1. Elimine la siguiente dependencia del archivo pom.xml del submódulo del proyecto denominado **all**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. Elimine lo siguiente incrustado del archivo pom.xml del submódulo del proyecto denominado &quot;all&quot;.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (Condicional) Quite la configuración del repositorio del archivo pom.xml de la raíz del proyecto.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (Condicional) Quite la configuración del servidor del archivo settings.xml, presente en la siguiente ruta ./cloudmanager/maven/settings.xml en la raíz del proyecto.&#39;

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. Confirme los cambios y envíe el código al repositorio de Cloud Manager

1. Ejecute la canalización de Cloud Manager para implementar los cambios en la instancia de Cloud Services
