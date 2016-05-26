---
# required metadata

title: Erstellen von Richtlinien und Veröffentlichen einer App für Benutzer der Evaluierungsversion | Microsoft Intune
description:
keywords:
author: Staciebarker
manager: jeffgilb
ms.date: 04/28/2016
ms.topic: get-started-article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: c3a17884-442a-44f5-bc81-4589e823f65e

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: jeffgilb
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---


# Erstellen von Richtlinien und Veröffentlichen einer App für Benutzer der Evaluierungsversion
Mit Intune-Richtlinien stehen Einstellungen bereit, mit deren Hilfe Sie die Sicherheitseinstellungen auf mobilen Geräten steuern, die Windows-Firewall- und Endpoint Protection-Einstellungen für Computer warten und Anwendungen bereitstellen können. Wenn Sie planen, Intune nach Ablauf der Evaluierungsversion auf Geräten zu verwenden, die für die Produktion konfiguriert werden, müssen Sie unbedingt die Anweisungen unter [Verwalten von Einstellungen und Features auf Ihren Geräten mit Microsoft Intune-Richtlinien](/intune/deploy-use/manage-settings-and-features-on-your-devices-with-microsoft-intune-policies) und [Schützen von Windows-PCs mit Endpoint Protection für Microsoft Intune](/intune/deploy-use/help-secure-windows-pcs-with-endpoint-protection-for-microsoft-intune) beachten..

Sie können zwei Arten von App-Installationen mithilfe von Intune ausführen: Die erste ist eine **erforderliche Installation**, bei der die App automatisch auf verwalteten Computern bereitgestellt wird. Die andere ist eine **verfügbare Installation**, bei der die App oder ein Link auf die App über das Intune-Unternehmensportal bereitgestellt wird, damit Benutzer auswählen können, ob die App auf ihren Computern oder mobilen Geräten installiert werden soll.

Bevor Sie Intune zum Bereitstellen von Apps verwenden, stellen Sie sicher, dass Sie über die erforderlichen Lizenzen zum Veröffentlichen, Verteilen und Verwenden der App verfügen. Im Arbeitsbereich **Lizenzen** können Sie Lizenzvertragsinformationen für Apps oder Software, die im Rahmen von Microsoft-Volumenlizenzverträgen gekauft wurden, und für Microsoft- oder Nicht-Microsoft-Apps oder -Software, die auf anderem Wege gekauft wurde, hinzufügen und verwalten. Sie können dann Lizenzberichte erstellen, die dann Informationen zur Verwendung verwalteter Lizenzen im gesamten Unternehmen anzeigen, damit Sie über Aktivitäten zur Nutzung von Lizenzen auf dem Laufenden bleiben.

In den folgenden Schritten werden Sie eine Konfigurationsrichtlinie für mobile Geräte und eine Firewallrichtlinie für Windows-Computer einrichten und Skype als verfügbare Installation für mobile Geräte konfigurieren, nachdem diese registriert wurden. Nachdem Sie eine neue Richtlinie hinzugefügt und bereitgestellt haben, erben alle Benutzer oder Geräte in der Gruppe, für die Sie die Richtlinie bereitgestellt haben, die Einstellungen als Basisrichtlinie. Sie können die Details dieser Richtlinien später jederzeit über den Arbeitsbereich **Richtlinie** in der Verwaltungskonsole überprüfen und bearbeiten.

## Erstellen und Bereitstellen einer Konfigurationsrichtlinie für mobile Geräte

1.  Öffnen Sie die [Intune-Verwaltungskonsole](https://manage.microsoft.com/)..

2.  Klicken Sie im linken Bereich auf das Symbol **Richtlinie**.

3.  Klicken Sie auf der Seite **Richtlinienübersicht** in der Liste **Aufgaben** auf **Richtlinie hinzufügen**..

4.  Erweitern Sie in der Richtlinienliste die Plattform, für die Sie eine Richtlinie erstellen möchten, wählen Sie **Allgemeine Konfiguration** sowie **Richtlinie mit den empfohlenen Einstellungen erstellen und bereitstellen** aus, und klicken Sie dann auf **Richtlinie erstellen**..

5.  Wählen Sie nach Aufforderung in **Gruppen auswählen, die Sie diese Richtlinie bereitstellen möchten** in der Liste **Meine Testbenutzer** aus, und klicken Sie auf **Hinzufügen** &gt; **OK**..

Die Richtlinie wird in der Liste der Konfigurationsrichtlinien angezeigt und wurde für die Gruppe **Meine Testbenutzer** bereitgestellt. Doppelklicken Sie auf die Richtlinie, um die Einstellungen anzuzeigen.

## Veröffentlichen der Skype-App für mobile Geräte

1.  Klicken Sie in der [Intune-Verwaltungskonsole](https://manage.microsoft.com/) auf das Symbol **Apps** und dann auf **Apps** &gt; **App hinzufügen**. Geben Sie Ihre Intune-Anmeldeinformationen ein, wenn Sie dazu aufgefordert werden.

    > [!NOTE]
    > Wenn Sie den **Intune-Softwareherausgeber** erstmals ausführen, kommt es zu einer kurzen Verzögerung, während die Anwendung installiert wird.

2.  Überprüfen Sie die Sicherheitswarnung, und klicken Sie auf **Ausführen**..

3.  Klicken Sie auf der Seite **Vorbereitung** auf **Weiter**..

4.  Wählen Sie auf der Seite **Softwaresetup** unter **Wählen Sie aus, wie diese Software für Geräte bereitgestellt werden soll** die Option **Externer Link** aus..

5.  Geben Sie unter **Geben Sie die URL an** den externen Link für die Software ein, und klicken Sie dann auf **Weiter**. Achten Sie darauf, der URL **https://** voranzustellen. Verwenden Sie für die Skype-App den nachfolgenden Link, der der Plattform für mobile Geräte entspricht, die Sie verwenden:

    -   **iOS:** [https://itunes.apple.com/us/app/skype-for-iphone/id304878510?mt%3D8](https://itunes.apple.com/us/app/skype-for-iphone/id304878510?mt%3D8)

    -   **Android:** [https://play.google.com/store/apps/details?id=com.skype.raider](https://play.google.com/store/apps/details?id=com.skype.raider)

    -   **Windows Phone 8 oder Windows Phone 8.1:** [http://www.windowsphone.com/en-us/store/app/skype/c3f8e570-68b3-4d6a-bdbb-c0a3f4360a51](http://www.windowsphone.com/en-us/store/app/skype/c3f8e570-68b3-4d6a-bdbb-c0a3f4360a51)

6.  Geben Sie auf der Seite **Softwarebeschreibung** die Informationen ein, die den Benutzern im Unternehmensportal zu der Software angezeigt werden sollen. Klicken Sie dann auf **Weiter**. Die folgenden Einstellungen stehen zur Verfügung (dieses Beispiel bezieht sich auf Skype):

    -   **Herausgeber:** Geben Sie den Namen des Herausgebers ein, **Microsoft**.

    -   **Name:** Geben Sie **Skype**

    -   **Beschreibung:** Geben Sie eine Beschreibung für die Software ein, z. B. **Skype-Kommunikations-App**

    -   **Kategorie:** Wählen Sie die Kategorie aus, die dieser Software am ehesten entspricht, z. B. **Zusammenarbeit**

    -   **Als ausgewählte App anzeigen und im Unternehmensportal hervorheben:** Wählen Sie diese Option aus, um die App im Unternehmensportal auf mobilen Geräten an hervorgehobener Stelle zu präsentieren.

    -   **Symbol:** (Optional) Wählen Sie aus, ob der Software ein Symbol zugeordnet werden soll. Die maximale Symbolgröße beträgt 250 x 250 Pixel, empfohlen wird allerdings 32 x 32 Pixel.

7.  Überprüfen Sie auf der Seite **Zusammenfassung** die Softwareinformationen, und klicken Sie dann auf **Hochladen**. Klicken Sie auf **Schließen**, um den Assistenten zu beenden.

8.  Klicken Sie in der [Intune-Verwaltungskonsole](https://manage.microsoft.com/) auf **Apps** &gt; **Apps** &gt; **Skype** &gt; **Bereitstellung verwalten**..

9. Wählen Sie auf der Seite **Gruppen auswählen** die Option **Testbenutzer** aus, um die Software für diese Benutzergruppe bereitzustellen, und klicken Sie auf **Hinzufügen** &gt; **Weiter**..

10. Wählen Sie auf der Seite **Bereitstellungsaktion** in der Spalte **Genehmigung** bei jeder Gruppe **Verfügbare Installation** aus.

11. Klicken Sie auf **Fertig stellen**..

Die Skype-App kann jetzt über das Unternehmensportal auf mobilen Geräten installiert werden. Doch zunächst müssen Sie Intune-Software auf PCs und mobilen Geräten installieren.

### Nächste Schritte
Gratulation! Sie habe soeben Schritt 4 der exemplarischen Vorgehensweise *Microsoft Intune-Evaluierung* ausgeführt.

>[!div class="step-by-step"]

>[&larr; **Erstellen von Gruppen**](.\get-started-with-a-30-day-trial-of-microsoft-intune-step-3.md)     [**Registrieren von Geräten** &rarr;](.\get-started-with-a-30-day-trial-of-microsoft-intune-step-5.md)  


<!--HONumber=May16_HO1-->

