---
# required metadata

title: Verwalten von Einstellungen und Features auf Ihren Geräten mit Microsoft Intune-Richtlinien | Microsoft Intune
description:
keywords:
author: robstackmsft
manager: jeffgilb
ms.date: 04/28/2016
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 09bae0b9-4f79-4658-8ca1-a71ab992c1b2

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: jeffgilb
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Verwalten von Einstellungen und Features auf Ihren Geräten mit Microsoft Intune-Richtlinien
Microsoft Intune-**Richtlinien** sind Gruppen von Einstellungen zur Steuerung der Features auf mobilen Geräten und Computern. Sie erstellen Richtlinien mithilfe von Vorlagen, in denen empfohlene oder angepasste Einstellungen enthalten sind, und stellen diese dann für Geräte- oder Benutzergruppen bereit.

## Welche Arten von Richtlinien können Sie verwenden?

Intune-Richtlinien lassen sich in die folgenden Kategorien einteilen: Welche Kategorie Sie verwenden, bestimmt, wie Sie die Richtlinie erstellen und bereitstellen können.


- **Konfigurationsrichtlinien:** Diese werden häufig zum Verwalten von Sicherheitseinstellungen und -features auf Ihren Geräten verwendet. Verwenden Sie die Informationen in diesem Thema, um mehr über das Erstellen und Bereitstellen dieser Richtlinien und die verfügbaren Einstellungen zu erfahren.
- **Gerätekompatibilitätsrichtlinien:** Diese definieren die Regeln und Einstellungen, die ein Gerät erfüllen muss, damit es als kompatibel mit Richtlinien für bedingten Zugriff eingestuft wird. Kompatibilitätsrichtlinien ermöglichen Ihnen auch, die Kompatibilität von Geräten unabhängig von bedingten Zugriffsrechten zu überwachen und zu beheben.
Weitere Informationen finden Sie unter [Gerätekompatibilitätsrichtlinien in Microsoft Intune](introduction-to-device-compliance-policies-in-microsoft-intune.md)..
- **Richtlinien für bedingten Zugriff:** Mit diesen Richtlinien können Sie E-Mail- und andere Dienste basierend auf Bedingungen schützen, die Sie festlegen.
Weitere Informationen finden Sie unter [Beschränken des Zugriffs auf E-Mail- und Office 365-Dienste mit Microsoft Intune](restrict-access-to-email-and-o365-services-with-microsoft-intune.md)..
- **Richtlinien zum Registrieren von firmeneigenen Geräten:** Informationen zu Richtlinien zum Registrieren von firmeneigenen Geräten finden Sie unter [Einrichten der iOS- und Mac-Verwaltung mit Microsoft Intune](set-up-ios-and-mac-management-with-microsoft-intune.md)..
- **Ressourcenzugriffsrichtlinien:** Diese Gruppe von Richtlinien ermöglicht Benutzern den Zugriff auf die Dateien und Ressourcen, die sie für ihre Arbeit benötigen, und zwar unabhängig davon, wo sie gespeichert sind.
Weitere Informationen finden Sie unter [Aktivieren des Zugriffs auf Unternehmensressourcen mit Microsoft Intune](enable-access-to-company-resources-with-microsoft-intune.md)..


Eine vollständige Liste der Intune-Richtlinien finden Sie unter [Referenz zu Microsoft Intune-Richtlinien](microsoft-intune-policy-reference.md)..




## Erstellen einer Konfigurationsrichtlinie

1.  Klicken Sie in der [Microsoft Intune-Verwaltungskonsole](https://manage.microsoft.com/) auf **Richtlinie** &gt; **Konfigurationsrichtlinien** &gt; **Hinzufügen**..

2.  Wählen Sie die gewünschte Richtlinie aus, und wählen Sie, ob Sie die empfohlenen Einstellungen für die Richtlinie verwenden (sofern verfügbar, Sie können diese Einstellungen später ändern) oder eine benutzerdefinierte Richtlinie mit Ihren eigenen Einstellungen erstellen möchten.

    > [!TIP]
    > Hilfe zur Auswahl der richtigen Richtlinie finden Sie in der [Referenz zu Microsoft Intune-Richtlinien](microsoft-intune-policy-reference.md).

3.  Wenn Sie bereit sind, klicken Sie auf **Richtlinie erstellen**..

4.  Konfigurieren Sie im Bildschirm **Richtlinie erstellen** einen Namen und optional eine Beschreibung für die Richtlinie.

5.  Konfigurieren Sie die erforderlichen Richtlinieneinstellungen, und klicken Sie dann auf **Richtlinie speichern**..

    Wenn Sie Hilfe zu Richtlinieneinstellungen benötigen, wählen Sie Ihren Richtlinientyp aus der folgenden Liste aus:

    - [Einstellungen für iOS-Geräte](ios-policy-settings-in-microsoft-intune.md)
    - [Einstellungen für Android-Geräte](android-policy-settings-in-microsoft-intune.md)
    - [Einstellungen für Geräte mit Windows 8 und Windows 8.1](windows-configuration-policy-settings-in-microsoft-intune.md)
    - [Einstellungen für Geräte mit Windows Phone 8.1](windows-phone-8-1-policy-settings-in-microsoft-intune.md)
    - [Einstellungen für Desktop- und mobile Geräte mit Windows 10](windows-10-policy-settings-in-microsoft-intune.md)
    - [Einstellungen für Windows Team-Geräte](windows-team-configuration-policy-settings-in-microsoft-intune.md)
    - [Upgradeeinstellungen für die Windows-Edition](edition-upgrade-policy-settings-in-microsoft-intune.md)
    - [Einstellungen für Mac OS X-Geräte](mac-os-x-policy-settings-in-microsoft-intune.md)
    - [Einstellungen für Exchange ActiveSync](exchange-activesync-policy-settings-in-microsoft-intune.md)
    - [Einstellungen für Nutzungsbedingungsrichtlinien](terms-and-condition-policy-settings-in-microsoft-intune.md)
    - [Allgemeine Einstellungen für mobile Geräte (Legacy)](mobile-device-security-policy-settings-in-microsoft-intune.md)

4.  Klicken Sie im Bestätigungsdialogfeld auf **Ja** , um die Richtlinie jetzt bereitzustellen, oder auf **Nein** , um die Richtlinie zu erstellen, ohne sie bereitzustellen.

Sie können die neue Richtlinie anzeigen und bearbeiten, indem Sie durch die Abschnitte für die einzelnen Richtlinientypen im Arbeitsbereich **Richtlinie** navigieren.

Wenn sie eine Richtlinie erstellen, bei der die empfohlenen Einstellungen verwendet werden, setzt sich der Name der neuen Richtlinie aus dem Vorlagennamen, dem Datum und der Uhrzeit zusammen. Bearbeiten Sie die Richtlinie, dann werden Datum und Uhrzeit im Namen entsprechend dem Zeitpunkt der Bearbeitung angepasst.

Nachdem Sie nun eine Richtlinie erstellt haben, werden Sie sie in der Regel für eine oder mehrere Gruppen von Benutzern oder Geräten bereitstellen.

> [!TIP]
> Sie stellen nicht alle Richtlinientypen bereit. Beispielsweise wird die mobile Anwendungsverwaltungsrichtlinie nicht bereitgestellt. Diese Richtlinie wird stattdessen einer App zugeordnet, die Sie dann bereitstellen.

## Bereitstellen einer Konfigurationsrichtlinie

1.  Wählen Sie im Arbeitsbereich **Richtlinie** die Richtlinie aus, die Sie bereitstellen möchten, und klicken Sie dann auf **Bereitstellung verwalten**..

2.  Führen Sie im Dialogfeld **Bereitstellung verwalten** folgende Schritte aus:

    -   **Wenn Sie die Richtlinie bereitstellen möchten:** Wählen Sie mindestens eine Gruppe aus, für die Sie die Richtlinie bereitstellen möchten, und klicken Sie auf **Hinzufügen** &gt; **OK**..

    -   **Wenn Sie das Dialogfeld schließen möchten, ohne die Richtlinie bereitzustellen:** Klicken Sie auf **Abbrechen**..

Wenn Sie eine bereitgestellte Richtlinie auswählen, können Sie weitere Informationen zur Bereitstellung im unteren Teil der Richtlinienliste anzeigen.

## Verwalten von Richtlinien

1.  Klicken Sie in der [Microsoft Intune-Verwaltungskonsole](https://manage.microsoft.com/)auf **Richtlinie**, navigieren Sie zu der Richtlinie, die Sie verwalten möchten, und wählen Sie sie aus.

2.  Wählen Sie eine der folgenden Aktionen aus:

- **Bearbeiten:** Hiermit werden die Eigenschaften für die ausgewählte Richtlinie geöffnet, und Sie können Änderungen daran vornehmen.
- **Löschen:** Hiermit wird die ausgewählte Richtlinie gelöscht.<br>Wenn Sie eine Richtlinie löschen, wird sie aus allen Gruppen entfernt, für die sie bereitgestellt worden war.
- **Bereitstellung verwalten:** Wählen Sie die Gruppe aus, für die Sie die Richtlinie bereitstellen möchten, und klicken Sie dann auf **Hinzufügen**..

## Für Intune-Richtlinien auszuführende Aufgaben

### Wenn Sie die Richtlinien auf einem Gerät aktualisieren und so sicherstellen möchten, dass sie aktuell sind (gilt nur für Windows-PCs, auf denen nur die Intune-Clientsoftware ausgeführt wird)

1.  Klicken Sie in der [Microsoft Intune-Verwaltungskonsole](https://manage.microsoft.com/)auf **Gruppen**, und wählen Sie dann eine Gerätegruppe aus.

2.  Wählen Sie die Geräte aus, auf denen die Richtlinien aktualisiert werden sollen, und klicken Sie dann auf **Remoteaufgaben** &gt; **Richtlinien aktualisieren**..

3.  Klicken Sie in der Intune-Verwaltungskonsole unten rechts auf **Remoteaufgaben**.

## Referenzinformationen zu den Intune-Richtlinien

### Wie lange dauert es für mobile Geräte, bis Richtlinien oder Apps nach ihrer Bereitstellung abgerufen werden?
Wenn eine Richtlinie oder Anwendung bereitgestellt wird, beginnt Intune sofort mit dem Versuch, das Gerät zu benachrichtigen und zum Einchecken beim Intune-Dienst zu veranlassen. Dies dauert normalerweise weniger als 5 Minuten.

Wenn ein Gerät sich nach der ersten Benachrichtigung nicht zum Abrufen der Richtlinie eincheckt, werden drei weitere Versuche unternommen.  Wenn das Gerät offline ist (z. B. abgeschaltet oder nicht mit einem Netzwerk verbunden), erhält es die Benachrichtigungen möglicherweise nicht.

In diesem Fall erhält das Gerät die Richtlinie beim nächsten geplanten Einchecken beim Intune-Dienst wie folgt:

- iOS: alle 6 Stunden
- Android: alle 8 Stunden
- Windows Phone: alle 8 Stunden
- Windows-PCs, die als Geräte registriert sind: alle 24 Stunden

Wenn das Gerät gerade registriert wurde, ist die Eincheckfrequenz höher:

- iOS: 6 Stunden lang alle 15 Minuten, danach alle 6 Stunden
- Android: 15 Minuten lang alle 3 Minuten, danach 2 Stunden lang alle 15 Minuten, anschließend alle 8 Stunden
- Windows Phone: 15 Minuten lang alle 5 Minuten, danach 2 Stunden lang alle 15 Minuten, anschließend alle 8 Stunden
- Windows-PCs, die als Geräte registriert sind: 30 Minuten lang alle 3 Minuten, danach alle 24 Stunden

Benutzer können auch jederzeit die Unternehmensportal-App starten und das Gerät synchronisieren, um sofort auf Richtlinien zu prüfen.

### Bei welchen Aktionen sendet Intune sofort eine Benachrichtigung an ein Gerät?
Geräte checken bei Intune entweder beim Erhalt einer Benachrichtigung ein, die sie dazu auffordert, oder während ihres regelmäßigen geplanten Eincheckvorgangs, wie in den obigen Tabellen beschrieben.  Wenn Sie für ein Gerät oder einen Benutzer ausdrücklich eine Aktion durchführen wie Zurücksetzen, Sperren, Zurücksetzen der Kennung, App-Bereitstellung, Profilbereitstellung (WLAN, VPN, E-Mail usw.) oder Bereitstellung der Richtlinie, beginnt Intune sofort mit dem Versuch, das Gerät darauf hinzuweisen, dass es sich zum Erhalten dieser Updates beim Intune-Dienst einchecken soll.

Andere Änderungen, wie z. B. die Überarbeitung der Kontaktinformationen im Unternehmensportal, führen nicht zu einer sofortigen Benachrichtigung von Geräten.

> [!TIP]
> Wenn eine Richtlinie mit Einstellungen auf einem Android-Gerät bereitgestellt wird, wird der Benutzer aufgefordert, die entsprechende Maßnahme zu ergreifen, um der Richtlinie zu entsprechen. Bis der Benutzer diese Aktion durchgeführt hat oder das Gerät neu gestartet wird, werden die neuen Richtlinieneinstellungen nicht wirksam.

### Wie finde ich heraus, welche Einstellungen angewendet werden, wenn für denselben Benutzer oder dasselbe Gerät mehrere Richtlinien bereitgestellt werden?
Bei Bereitstellung mehrerer Richtlinien für denselben Benutzer oder dasselbe Gerät ist es wichtig zu wissen, dass die Bewertung für die jeweils anwendbare Einstellung auf der Ebene einzelner Einstellungen erfolgt.

-   Kompatibilitätsrichtlinieneinstellungen haben immer Vorrang vor Konfigurationsrichtlinieneinstellungen

-   Die restriktivste Kompatibilitätsrichtlinie wird angewendet, wenn sie gegen dieselbe Einstellung in einer anderen Kompatibilitätsrichtlinie ausgewertet wird

-   Die restriktivste Konfigurationsrichtlinie wird angewendet, wenn sie gegen dieselbe Einstellung in einer anderen Konfigurationsrichtlinie ausgewertet wird

### Was geschieht, wenn MAM-Richtlinien (mobile Anwendungsverwaltung) miteinander in Konflikt stehen? Welche wird auf die App angewendet?
Konfliktwerte sind die restriktivsten Einstellungen, die in einer mobilen Anwendungsverwaltungsrichtlinie zur Verfügung stehen, außer für die Zahleneingabefelder (z. B. PIN-Versuche vor dem Zurücksetzen).  Die Zahleneingabefelder werden auf dieselben Werte gesetzt, die auch verwendet werden, wenn Sie eine MAM-Richtlinie in der Konsole mit der Option der empfohlenen Einstellungen erstellen.

Konflikte treten auf, wenn zwei Richtlinieneinstellungen identisch sind.  Beispielsweise haben Sie zwei MAM-Richtlinien konfiguriert, die mit Ausnahme der Einstellung für Kopieren/Einfügen identisch sind.  In diesem Szenario wird die Einstellung für Kopieren und Einfügen auf den restriktivsten Wert festgelegt, die übrigen Einstellungen werden jedoch wie konfiguriert angewendet.

Wenn eine Richtlinie für die Anwendung bereitgestellt wird und in Kraft tritt und anschließend eine weitere bereitgestellt wird, erhält die zuerst bereitgestellte Richtlinie Vorrang und bleibt wirksam, während die zweite als in Konflikt stehend angezeigt wird. Wenn sie jedoch beide gleichzeitig angewendet werden, sodass es keine vorhergehende Richtlinie gibt, befinden sich beide im Konflikt, und alle in Konflikt stehenden Einstellungen werden auf die restriktivsten Werte festgelegt.

### Was geschieht, wenn Sie benutzerdefinierte iOS-Richtlinien in Konflikt stehen?
Intune bewertet nicht die Nutzlast von Apple-Konfigurationsdateien oder der benutzerdefinierten OMA-URI-Richtlinie, es dient lediglich als Übermittlungsmechanismus.

Wenn Sie daher eine benutzerdefinierte Richtlinie bereitstellen, stellen Sie sicher, dass die konfigurierten Einstellungen nicht mit Kompatibilitäts-, Konfigurations- oder anderen benutzerdefinierten Richtlinien in Konflikt stehen. Bei einer benutzerdefinierten Richtlinie mit Einstellungskonflikten werden die Einstellungen in zufälliger Reihenfolge angewendet.

### Was geschieht, wenn eine Richtlinie gelöscht wird oder nicht mehr anwendbar ist
Wenn Sie eine Richtlinie löschen oder ein Gerät aus einer Gruppe entfernen, für die eine Richtlinie bereitgestellt wurde, werden die Richtlinie und die Einstellungen entsprechend den folgenden Tabellen vom Gerät entfernt:

#### Angemeldete Geräte

- WLAN-, VPN-, Zertifikat- und E-Mail-Profile: Diese Profile werden von allen unterstützten registrierten Geräten entfernt.
- Alle anderen Richtlinientypen
    - **Windows- und Android-Geräte**: Einstellungen werden nicht vom Gerät entfernt.
    - **Windows Phone 8.1-Geräte**: Die folgenden Einstellungen werden entfernt:
        - Anfordern eines Kennworts zum Entsperren mobiler Geräte
        - Einfache Kennwörter zulassen
        - Minimale Kennwortlänge
        - Erforderlicher Kennworttyp
        - Kennwortablauf (Tage)
        - Kennwortverlauf speichern
        - Anzahl zulässiger wiederholter Anmeldefehler, bevor das Gerät zurückgesetzt wird
        - Minuten der Inaktivität, bevor ein Kennwort erforderlich ist
        - Erforderlicher Kennworttyp – Mindestanzahl von Zeichensätzen
        - Kamera zulassen
        - Verschlüsselung auf mobilem Gerät anfordern
        - Wechselspeichermedien zulassen
        - Webbrowser zulassen
        - App Store zulassen
        - Bildschirmaufnahme zulassen
        - Geolocation zulassen
        - Microsoft-Konto zulassen
        - Kopieren und Einfügen zulassen
        - WLAN-Tethering zulassen
        - Automatische Verbindung mit unverschlüsselten WLAN-Hotspots zulassen
        - Berichterstellung für WLAN-Hotspots zulassen
        - Zurücksetzen auf Werkseinstellungen zulassen
        - Bluetooth zulassen
        - NFC zulassen
        - WLAN zulassen
    
    - **iOS**: Alle Einstellungen werden entfernt, außer:
        - Sprachroaming zulassen
        - Datenroaming zulassen
        - Automatische Synchronisierung beim Roaming zulassen

#### Windows-PCs, auf denen die Intune-Clientsoftware ausgeführt wird

- **Endpoint Protection-Einstellungen:** Die Einstellungen werden auf die empfohlenen Werte zurückgesetzt. Die einzige Ausnahme ist die Einstellung **Microsoft Active Protection Service beitreten** , deren Standardwert **Nein**lautet. Weitere Informationen finden Sie unter [Schützen von Windows-PCs mit Endpoint Protection für Microsoft Intune](help-secure-windows-pcs-with-endpoint-protection-for-microsoft-intune.md)..
- **Einstellungen für Softwareupdates:** Die Einstellungen werden auf die Standardwerte des Betriebssystems zurückgesetzt. Weitere Informationen finden Sie unter [Aktualisieren Ihrer Windows-PCs mit Softwareupdates in Microsoft Intune](keep-windows-pcs-up-to-date-with-software-updates-in-microsoft-intune.md)..
- **Microsoft Intune Center-Einstellungen:** Alle den Supportvertrag betreffenden Informationen, die durch die Richtlinie definiert waren, werden von den Computern gelöscht.
- **Einstellungen für die Windows-Firewall:** Die Einstellungen werden auf die Standardwerte des Computerbetriebssystems zurückgesetzt. Weitere Informationen finden Sie unter [Schützen von Windows-PCs mit Endpoint Protection für Microsoft Intune](help-secure-windows-pcs-with-endpoint-protection-for-microsoft-intune.md)..





<!--HONumber=May16_HO1-->

