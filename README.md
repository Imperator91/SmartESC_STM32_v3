Für die letzte funktionierende "stancecoke"-Version wechsle zum v0.5-Branch!
https://github.com/Koxx3/SmartESC_STM32_v3/tree/v0.5

Achtung: Neue Logik zur Aktivierung des Autodetektionsverfahrens:
Ziehe den Bremshebel und drücke die Dashboard-Taste für 5 Sekunden!

Fork der EBiCS-Firmware für Lishui-Geräte. Portiert auf den Xiaomi M365-Controller.
Verwende JST PA-Steckverbinder mit 2mm Pitch (muss noch bestätigt werden).

Dieser Branch funktioniert mit dem originalen M365-Dashboard.
Anleitung zur Nutzung:
Methode 1 (GitHub-Account erforderlich):

    Forke das Projekt-Repository auf deinen GitHub-Account, indem du auf das „Fork“-Symbol klickst.
    Bearbeite die Datei config.h in deinem Repository online und committe die Änderungen.
    Klicke auf die Schaltfläche „Actions“ in der Menüleiste der GitHub-Seite. Dort siehst du die „Workflows“.
    Warte, bis der laufende Workflow abgeschlossen ist, dann klicke auf die Überschrift des Workflows.
    Lade die generierte ZIP-Datei herunter, indem du auf das Würfelsymbol unten auf der Seite klickst.
    Ein Tutorial findest du auf YouTube.

Methode 2 (Lokale Installation):

    Installiere die STM Cube IDE.
    Starte die IDE und installiere egit aus dem Eclipse Marketplace (Help → Eclipse Marketplace...).
    Importiere dieses Repository von GitHub (File → Import → Git → Projects from Git).
    Bearbeite die Datei config.h (im Ordner Core/Inc) nach deinen Wünschen.
        Funktionierende Einstellungen für das originale M365 sind in den Kommentaren enthalten – nutze sie als bewährte Ausgangskonfiguration.
    Klicke auf „Build“ (das Symbol mit dem Hammer).
    Die fertige ZIP-Datei wird im Ordner /tools/zip-output generiert.
    Kopiere die Datei auf dein Smartphone und flashe sie mit der App downG auf deinen Scooter.

Nach dem Flashen:

    Hebe das Hinterrad an, sodass der Motor frei drehen kann.
    Drücke die Dashboard-Taste für 5 Sekunden – die Autodetektion beginnt.
    Der Motor dreht sich langsam. Sobald er stoppt, ist der Scooter einsatzbereit.

Dashboard-Tastenbelegung:

    Kurzer Druck: Licht ein-/ausschalten
    Doppelklick: Fahrmodus wechseln
    Langer Druck: Ausschalten
    Sehr langer Druck: Autodetektion starten

![PCB Layout M365](https://github.com/Koxx3/SmartESC_STM32_v3/blob/master/Documentation/PCB%20Layout%20M365.PNG)
