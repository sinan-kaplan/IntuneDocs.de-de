---
# required metadata

title: Erstellen von Gruppen zum Organisieren von Benutzern und Geräten | Microsoft Intune
description:
keywords:
author: Staciebarker
manager: jeffgilb
ms.date: 04/28/2016
ms.topic: get-started-article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 5fdf98c8-fe67-4d7a-9837-ed1234348014

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: jeffgilb
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---


# Erstellen von Gruppen zum Organisieren von Benutzern und Geräten
Mit Gruppen erhalten Sie in Intune maximale Flexibilität beim Verwalten Ihrer Geräte und Benutzer. Sie können Gruppen einrichten, die Ihren organisatorischen Anforderungen (z. B. nach geografischem Standort, nach Abteilung oder nach Hardwareeigenschaften) entsprechen und diese dazu verwenden, um eine Vielzahl von Verwaltungsaufgaben ausführen, die von der Bereitstellung von Richtlinien für eine Gruppe von Benutzern bis zur Bereitstellung von Anwendungen auf einer Reihe von Geräten reichen.

Sowohl Geräte als auch Benutzergruppen werden im Arbeitsbereich „Gruppen“ der Intune-Verwaltungskonsole erstellt.

![Arbeitsbereich „Gruppen“ der Verwaltungskonsole](./media/groups.png)


> [!TIP]
> Weitere Informationen zum Verwenden von Gruppen finden Sie unter [Verwenden von Gruppen zum Verwalten von Benutzern und Geräten in Microsoft Intune](/intune/deploy-use/use-groups-to-manage-users-and-devices-with-microsoft-intune)..


## Erstellen einer Gerätegruppe
Verwenden Sie Gerätegruppen zum Bereitstellen von Apps und Updates sowie zum Konfigurieren anderer Features. Richten Sie z. B. die Gruppe „Meine Geräte“ mithilfe der folgenden Schritte ein:

1.  Klicken Sie in der [Intune-Verwaltungskonsole](https://manage.microsoft.com/) auf **Gruppen** > **Übersicht** > **Gruppe erstellen**..

2.  Geben Sie unter **Gruppenname** „Meine Testgeräte“ ein, wählen Sie in der übergeordneten Gruppenliste **Alle Geräte** aus, und klicken Sie dann auf **Weiter**..

3.  Wählen Sie **Alle Geräte** auf der Seite **Mitgliedschaftskriterien definieren** aus, um anzugeben, dass die Gruppe sowohl mobile Geräte als auch Computer enthält.

4.  Klicken Sie auf der Seite **Direkte Mitgliedschaft definieren** auf **Weiter**. Hätten Sie zuvor eine Gruppe erstellt, die nicht alle Geräte enthält, und wollten Sie dieser neuen Gruppe nun bestimmte Geräte hinzufügen, dann können Sie dies an dieser Stelle tun.

5.  Überprüfen Sie auf der Seite **Zusammenfassung** die Aktionen, die ausgeführt werden, und klicken Sie dann auf **Fertig stellen**..

Sie finden die neue Gruppe in der Liste **Gruppen** im Arbeitsbereich **Gruppen** unter **Alle Geräte**. Hier können Sie die Gruppe auch bearbeiten oder löschen.

## Erstellen einer Benutzergruppe
Verwenden Sie Benutzergruppen, um Software- und Geräterichtlinien bereitzustellen. Richten Sie z. B. die Gruppe „Intune-Benutzer“ mithilfe der folgenden Schritte ein:

1.  Klicken Sie in der [Intune-Verwaltungskonsole](https://manage.microsoft.com/) auf **Gruppen** > **Übersicht** > **Gruppe erstellen**..

2.  Geben Sie unter **Gruppenname** „Intune-Benutzer“ ein, wählen Sie aus der übergeordneten Gruppenliste **Alle Benutzer** aus, und klicken Sie dann auf **Weiter**..

3.  Legen Sie auf der Seite **Mitgliedschaftskriterien definieren** die Option **Gruppenmitgliedschaft starten mit** auf **Alle Benutzer in der übergeordneten Gruppe** fest..

4.  Klicken Sie neben **Mitglieder dieser Sicherheitsgruppen ausschließen** auf **Durchsuchen** und anschließend auf **Unternehmensadministrator**. Durch diesen Ausschluss können Sie die Gruppe „Intune-Benutzer“ verwalten, ohne dass das Konto „Unternehmensadministrator“ (auch als Mandantenadministrator bezeichnet) davon betroffen ist.

5.  Klicken Sie auf der Seite **Direkte Mitgliedschaft definieren** auf **Weiter**. Hier brauchen Sie nichts zu tun, denn die Gruppe „Intune-Benutzer“ soll alle Benutzer außer dem Unternehmensadministrator einschließen.

6.  Überprüfen Sie auf der Seite **Zusammenfassung** die Aktionen, die ausgeführt werden, und klicken Sie dann auf **Fertig stellen**..

Sie finden die neue Gruppe in der Liste **Gruppen** im Arbeitsbereich **Gruppen** unter **Alle Benutzer**. Hier können Sie die Gruppe auch bearbeiten oder löschen.



### Nächste Schritte
Gratulation! Sie haben Schritt 5 der Kurzanleitung *Erste Schritte mit Intune* abgeschlossen..

>[!div class="step-by-step"]

>[&larr; **Verwalten von Intune-Lizenzen**](.\start-with-a-paid-subscription-to-microsoft-intune-step-4.md)       [**Erstellen von Richtlinien und Apps** &rarr;](.\start-with-a-paid-subscription-to-microsoft-intune-step-6.md)  


<!--HONumber=May16_HO1-->

