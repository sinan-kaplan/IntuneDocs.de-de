---
title: Aktivieren von Lookout MTP in Intune | Microsoft-Dokumentation
description: Aktivieren von Lookout Mobile Threat Protection in der Intune-Verwaltungskonsole.
keywords: 
author: andredm7
ms.author: andredm
manager: angrobe
ms.date: 12/19/2016
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 2f835fd0-4e62-42f3-b7ca-ce8b7ddd40e4
ms.reviewer: sandera
ms.suite: ems
ms.custom: intune-classic
translationtype: Human Translation
ms.sourcegitcommit: 53862e49c922b75b414fd5aceec3bba2b10299a6
ms.openlocfilehash: 1297522d0f7b52ebe14eb7b938f3458e7308ae27


---

# <a name="enable-lookout-mtp-connection-in-the-intune-admin-console"></a>Aktivieren der Lookout MTP-Verbindung in der Intune-Verwaltungskonsole

[!INCLUDE[classic-portal](../includes/classic-portal.md)]

Um die Verbindung mit Lookout Mobile Threat Protection (MTP) in Intune zu aktivieren, muss der Intune-Connector in der Lookout-Konsole bereits konfiguriert sein.  Wenn dies noch nicht erfolgt ist, führen Sie die in [Einrichten Ihres Abonnements für Lookout Mobile Threat Protection](set-up-your-subscription-with-lookout-mtp.md) beschriebenen Schritte aus.

Um die Lookout MTP-Verbindung in Intune zu aktivieren, wählen Sie auf der Seite **Verwaltung** der [Microsoft Intune-Verwaltungskonsole](https://manage.microsoft.com) die Option **Integration von Drittanbieterdiensten** aus. Wählen Sie **Lookout-Status** aus, und aktivieren Sie **Synchronisierung mit MTP** mithilfe der Umschaltfläche.

![Screenshot der Lookout-Synchronisierungsseite mit hervorgehobener Umschaltfläche „Aktivieren“](../media/mtp/lookout-intune-synchronization.png)

>[!IMPORTANT]
> Sie **müssen** die Lookout for Work-App konfigurieren, bevor Sie die Regeln der Kompatibilitätsrichtlinie erstellen und den bedingten Zugriff konfigurieren. Dadurch wird sichergestellt, dass die App für die Installation durch Endbenutzer bereit und verfügbar ist, bevor sie Zugriff auf E-Mail oder andere Unternehmensressourcen erhalten.

Damit wird das Setup der Lookout- und Intune-Integration in der Intune-Administratorkonsole abgeschlossen.  Die nächsten Schritte zum Implementieren dieser Lösung umfassen die Bereitstellung der [Lookout for Work-Apps](configure-and-deploy-lookout-for-work-apps.md) und das Einrichten der [Kompatibilitätsrichtlinie](enable-device-threat-protection-rule-in-compliance-policy.md).


## <a name="next-steps"></a>Nächste Schritte
[Konfigurieren der Lookout for Work-App](configure-and-deploy-lookout-for-work-apps.md)



<!--HONumber=Jan17_HO2-->

