---
title: Konfigurieren der Unternehmensportal-App
titleSuffix: Intune Azure preview
description: "Intune in Azure (Vorschau): Erfahren Sie, wie Sie unternehmensspezifisches Branding auf die Intune-Unternehmensportal-App anwenden können. "
keywords: 
author: robstackmsft
ms.author: robstack
manager: angrobe
ms.date: 02/15/2017
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: dec6f258-ee1b-4824-bf66-29053051a1ae
ms.reviewer: mghadial
ms.suite: ems
ms.custom: intune-azure
translationtype: Human Translation
ms.sourcegitcommit: 153cce3809e24303b8f88a833e2fc7bdd9428a4a
ms.openlocfilehash: 9ebfadd945916b6be8225b9e07d67100e3f91222
ms.lasthandoff: 02/18/2017

---

# <a name="how-to-configure-the-microsoft-intune-company-portal-app"></a>Konfigurieren der Microsoft Intune-Unternehmensportal-App

[!INCLUDE[azure_preview](../includes/azure_preview.md)]

Im Microsoft Intune-Unternehmensportal können Benutzer auf Unternehmensdaten zugreifen, häufige Aufgaben wie das Registrieren von Geräten und das Installieren von Apps ausführen und sich über Unterstützungsmöglichkeiten durch Ihre IT-Abteilung informieren.

> [!Tip]
> Wenn Sie das Unternehmensportal anpassen, gelten die Konfigurationen sowohl für die Unternehmensportal-Website als auch für die Unternehmensportal-Apps.

Durch Anpassen des Unternehmensportals können Sie Ihren Endbenutzern eine vertraute und sinnvolle Benutzeroberfläche bereitstellen. Dazu wählen Sie in der Workload **Apps verwalten** die Option **Setup** > **Unternehmensportalbranding** aus und konfigurieren die erforderlichen Einstellungen.

## <a name="company-contact-information-and-privacy-statement"></a>Kontaktdaten und Datenschutzerklärung des Unternehmens
Der Unternehmensname wird als Titel des Unternehmensportals angezeigt. Die Kontaktinformationen werden Benutzern im Unternehmensportal auf dem Bildschirm **An IT-Abteilung wenden** angezeigt. Die Datenschutzerklärung wird angezeigt, wenn ein Benutzer auf den Datenschutzlink klickt.


|Feldname|Max. Länge|Weitere Informationen|
|-|-|-|
|**Firmenname**|40|Dieser Name wird als Titel des Unternehmensportals angezeigt.|
|**Kontaktname für IT-Abteilung**|40|Dieser Name wird auf der Seite **An IT-Abteilung wenden** angezeigt.|
|**Telefonnummer der IT-Abteilung**|20|Diese Telefonnummer wird auf der Seite **An IT-Abteilung wenden** angezeigt.|
|E-Mail-Adresse der IT-Abteilung|40|Diese Kontaktadresse wird auf der Seite **An IT-Abteilung** wenden angezeigt. Sie müssen eine gültige E-Mail-Adresse im Format **alias@domainname.com** eingeben.|
|**Weitere Informationen**|120|Dies wird auf der Seite **An IT-Abteilung wenden** angezeigt.|
|**URL der Datenschutzrichtlinie des Unternehmens**|79|Sie können eine eigene Datenschutzerklärung für Ihr Unternehmen angeben. Diese wird angezeigt, wenn die Benutzer im Unternehmensportal auf die Datenschutzlinks klicken. Sie müssen eine gültige URL im Format **http://www.contoso.com** eingeben.|

## <a name="support-contacts"></a>Supportkontakte
Die Supportwebsite wird Benutzern im Unternehmensportal angezeigt, um ihnen Zugriff auf Onlinesupport zu ermöglichen.



|Feldname|Max. Länge|Weitere Informationen|
|-|-|-|
|**URL der Supportwebsite**|150|Wenn Sie über eine Supportwebsite verfügen, die Ihre Benutzer verwenden sollen, geben Sie hier die URL an. Die URL muss das Format **http://www.contoso.com** aufweisen. Wenn Sie keine URL angeben, wird im Unternehmensportal auf der Seite **An IT-Abteilung wenden** keine Supportwebsite angezeigt.|
|**Name der Supportwebsite**|40|Dies ist der Anzeigename der URL für die Supportwebsite. Wenn Sie für die Supportwebsite eine URL, aber keinen Anzeigenamen angeben, wird im Unternehmensportal auf der Seite **An IT-Abteilung wenden** der Text „Zur IT-Website wechseln“ angezeigt.

## <a name="company-branding-customization"></a>Anpassen des Unternehmensbrandings
Sie können Ihr Unternehmensportal mit Ihrem Firmenlogo, Firmennamen, Farbdesign und Hintergrund anpassen.



|Feldname|Weitere Informationen|
|-|-|
|**Farbdesign**|Wählen Sie ein Farbdesign aus, das auf das Unternehmensportal angewendet werden soll.|
|**Firmenlogo anzeigen**|Wenn Sie diese Option aktivieren, können Sie Ihr Firmenlogo hochladen. Dieses wird dann im Unternehmensportal angezeigt. Sie können zwei Logos hochladen: ein Logo, das angezeigt wird, wenn der Hintergrund des Unternehmensportals weiß ist, und eines, das angezeigt wird, wenn für den Hintergrund des Unternehmensportals das von Ihnen ausgewählte Farbdesign verwendet wird. Die Logodateien müssen PNG- oder JPG-Dateien sein. Ihre Auflösung darf maximal 400 x 100 Pixel betragen, und die Größe darf 750 KB nicht überschreiten.<br>Sie können auch den eingegebenen Firmennamen neben dem hochgeladenen Logo anzeigen.|

Nachdem Sie Ihre Änderungen gespeichert haben, können Sie **eine Vorschau der Einstellungen im Intune-Webportal anzeigen**, um Ihre Konfiguration zu überprüfen.
