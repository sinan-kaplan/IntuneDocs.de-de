---
title: Einrichten der Android-Verwaltung
description: "Aktivieren Sie die Verwaltung mobiler Geräte (Mobile Device Management, MDM) für Android- und KNOX Standard-Geräte mit Microsoft Intune."
keywords: 
author: nathbarn
ms.author: nathbarn
manager: angrobe
ms.date: 03/20/2017
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: dbe5cad1-3e0d-41a9-966b-738156089700
ROBOTS: NOINDEX,NOFOLLOW
ms.reviewer: lacranda
ms.suite: ems
ms.custom: intune-classic
ms.openlocfilehash: 5826cd29bf07a3f1cf9b91ec75f0e0bb46050d60
ms.sourcegitcommit: 1a54bdf22786aea1cf1b497d54024470e1024aeb
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/10/2017
---
# <a name="set-up-android-device-management"></a>Einrichten der Android-Geräteverwaltung

[!INCLUDE[classic-portal](../includes/classic-portal.md)]

Als Intune-Administrator können Sie die Verwaltung von Android-Geräten, einschließlich Samsung KNOX Standard-Geräten, über das Unternehmensportal aktivieren. Benutzer können ihre Geräte anschließend über die Unternehmensportal-App registrieren, die in Google Play zur Verfügung steht.

Standardmäßig können Android-Geräte in Intune registriert werden. Um Android-Geräte für die Registrierung zu blockieren, melden Sie sich mit Ihren Administratoranmeldeinformationen im [Microsoft Intune-Verwaltungsportal](https://manage.microsoft.com) an. Wählen Sie **Admin** (Administrator) > **Verwaltung mobiler Geräte** > **Registrierungsregeln** aus, und deaktivieren Sie das Kontrollkästchen **Android-Geräte zulassen**.

1.  **Einrichten von Intune**<br>
    Wenn nicht bereits geschehen, bereiten Sie die Verwaltung mobiler Geräte durch [Festlegen der Autorität für die Verwaltung mobiler Geräte](prerequisites-for-enrollment.md#step-2-set-mdm-authority) auf **Microsoft Intune** und Einrichten von MDM vor.

2.  **Android-Registrierung aktiviert**<br>
    Um die Registrierung mobiler Android-Geräte zu ermöglichen, sind keine weiteren Konfigurationen in der Intune-Konsole erforderlich.

3.  **Benutzern erklären, wie sie ihre Geräte registrieren, um auf Unternehmensressourcen zugreifen zu können**

    Registrierungsanleitungen für Endbenutzer finden Sie unter [Registrieren Ihres Android-Geräts bei Intune](https://docs.microsoft.com/intune-user-help/enroll-your-device-in-intune-android). Im Laufe des Registrierungsprozesses werden Benutzer darüber informiert, was sie erwarten können und was IT-Administratoren auf ihren Geräten sehen können und was nicht.

    Informationen zu anderen Endbenutzeraufgaben finden Sie in den folgenden Artikeln:
  - [Ressourcen zu Endbenutzerszenarios in Microsoft Intune](/intune/end-user-educate)
  - [Endbenutzer-Leitfaden für Android-Geräte](https://docs.microsoft.com/intune-user-help/using-your-android-device-with-intune)

Da der Google Play Store in China nicht verfügbar ist, müssen Android-Geräte das Unternehmensportal von chinesischen App-Marktplätzen beziehen. Die Unternehmensportal-App für Android wird in den folgenden Stores zum Download zur Verfügung stehen:
* [Baidu](https://go.microsoft.com/fwlink/?linkid=836946)
* [Huawei](https://go.microsoft.com/fwlink/?linkid=836948)
* [Tencent](https://go.microsoft.com/fwlink/?linkid=836949)
* [Wandoujia](https://go.microsoft.com/fwlink/?linkid=836950)
* [Xiaomi](https://go.microsoft.com/fwlink/?linkid=836947)

Die Unternehmensportal-App für Android verwendet Google Play Services für die Kommunikation mit dem Microsoft Intune-Dienst. Da Google Play Services in China noch nicht verfügbar sind, kann die Ausführung der folgenden Aufgaben bis zu 8 Stunden dauern. 

|Intune-Administratorkonsole| Intune-Unternehmensportal-App für Android |Intune Unternehmensportalwebsite|   
|---|---|---|
|Vollständiges Zurücksetzen| Entfernen eines Remotegeräts| Entfernen eines Geräts (lokal und remote)|
|Selektives Zurücksetzen| Zurücksetzen eines Geräts| Zurücksetzen eines Geräts|
|Bereitstellung neuer oder aktualisierter Apps| Installieren von verfügbaren Branchen-Apps| Zurücksetzen der Gerätekennung|
|Remotesperre|||
|Zurücksetzen der Kennung|||

### <a name="see-also"></a>Weitere Informationen:
[Voraussetzungen für die Registrierung von Geräten in Microsoft Intune](prerequisites-for-enrollment.md)
