---
title: "Benutzerdefinierte Intune-Einstellungen für iOS-Geräte"
titleSuffix: Intune Azure preview
description: "Intune in Azure (Vorschau): Erfahren Sie etwas über die Einstellungen, die Sie in einem benutzerdefinierten iOS-Profil verwenden können."
keywords: 
author: robstackmsft
ms.author: robstack
manager: angrobe
ms.date: 02/15/2017
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 6da8caa8-65c2-4f47-842f-9570dcb1ac22
ms.reviewer: heenamac
ms.suite: ems
ms.custom: intune-azure
translationtype: Human Translation
ms.sourcegitcommit: b4d095506215b775d56d172e9aabae1737757310
ms.openlocfilehash: d8e6d0d641dd55c79442f68e7e97d21efcdad7fa
ms.lasthandoff: 02/16/2017


---

# <a name="microsoft-intune-custom-settings-for-ios-devices"></a>Benutzerdefinierte Microsoft Intune-Einstellungen für iOS-Geräte

[!INCLUDE[azure_preview](../includes/azure_preview.md)]

Verwenden Sie das benutzerdefinierte iOS-Profil von Microsoft Intune, um Einstellungen, die Sie mit dem [Apple Configurator-Tool](https://itunes.apple.com/app/apple-configurator-2/id1037126344?mt=12) erstellt haben, auf iOS-Geräten bereitzustellen. Mit diesem Tool können Sie zahlreiche Einstellungen zur Betriebssteuerung dieser Geräte erstellen und in ein Konfigurationsprofil exportieren. Sie können dieses Konfigurationsprofil anschließend in ein benutzerdefiniertes iOS-Profil von Intune importieren und die Einstellungen Benutzern und Geräten in Ihrer Organisation zuweisen.

Diese Funktion ermöglicht die Bereitstellung von iOS-Einstellungen, die nicht mit anderen Intune-Profiltypen konfigurierbar sind.


1. Anweisungen zu den ersten Schritten finden Sie unter [Konfigurieren von benutzerdefinierten Geräteeinstellungen in Microsoft Intune](how-to-configure-custom-settings.md).
2. Geben Sie auf dem Blatt **Profil erstellen** Folgendes an:

- **Name des benutzerdefinierten Konfigurationsprofils:** Geben Sie einen Namen für die Richtlinie an, der auf dem Gerät und in Intune-Status angezeigt wird.
- **Konfigurationsprofildatei:** Suchen Sie das mit Apple Configurator erstellte Konfigurationsprofil.
Stellen Sie sicher, dass die Einstellungen, die Sie aus dem Apple Configurator-Tool exportieren, mit der iOS-Version auf den Geräten kompatibel sind, für die Sie die benutzerdefinierte iOS-Richtlinie bereitstellen. Um Informationen zum Korrigieren inkompatibler Einstellungen zu erhalten, suchen Sie auf der [Apple Developer-Website](https://developer.apple.com/) nach der **Referenz zu Konfigurationsprofilen** und der **Referenz zum Protokoll für die Verwaltung mobiler Geräte**.

Die importierte Datei wird im Bereich **Dateiinhalt** des Blatts angezeigt.
