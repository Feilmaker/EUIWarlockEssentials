# EUI Warlock Essentials

Für Hexenmeister in WoW Forever (Interface 16001). Benötigt aktivierte EllesmereUI Aura & Buff Reminders und EllesmereUI mit der öffentlichen Plugin-API, z. B. die als Referenz verwendete Version 9.8.9.

## Installation

1. WoW schließen und den Ordner EUIWarlockEssentials nach Interface/AddOns/ kopieren. Die alten Addons EllesmereUISoulShards und EllesmereUIWarlockBuffs deaktivieren. 
2. In EllesmereUI unter **Warlock Essentials** zuerst **Soul Shard Bag** und dann **Aura Reminder** konfigurieren. `/euishards` öffnet weiterhin die Splitterverwaltung.

Die Drei-Punkte-Menüs neben den Hauptoptionen öffnen weitere Einstellungen für Pause, Taschenzähler, Makros und Steine. Die Warnschwelle für wenige Splitter steht direkt unter der Pausenoption.

## Aura Reminder

Die Schalter für Dämonenhaut / Dämonenrüstung, Dämonische Opferung und Seelenverbindung verwenden dieselben Einstellungen wie die EUI-Klassenbuffs. Seelenstein und Zauberstein / Feuerstein haben eigene Schalter. Die Hilfetexte neben den Einstellungen erklären die zusammengefassten Auren und die Klickaktion.

Der Seelenstein-Zielmodus startet auf **Smart**. **Nur auf mich selbst** prüft und belegt deinen Charakter auch in Gruppen und Schlachtzügen. In beiden Modi stellt der erste Klick einen Seelenstein her, wenn keiner in der Tasche liegt.

## Cooldown Manager

Unter **Warlock Essentials → Cooldown Manager** stehen die Zauber nach den aktiven EUI-Cooldown- und Utility-Leisten gruppiert. Wähle pro Zauber **Primär**, **Sekundär**, **Beide** oder **Keine**. Die Leistenbelegung und Zauberreihenfolge stammen aus EUI.

## Seelentasche

Auf eine ausgerüstete Seelentasche in der Taschenleiste rechtsklicken. Ein Klick entfernt einen überschüssigen Seelensplitter, ohne die Tasche zu öffnen. Weitere Klicks entfernen jeweils einen weiteren, bis der Gesamtbestand der Kapazität aller ausgerüsteten Seelentaschen entspricht. Beispiel: 25 Splitter und eine 20er-Seelentasche ergeben fünf Löschklicks. Die Aktion berücksichtigt Pause, Drain Soul und gesperrte Splitter. Ein Linksklick öffnet die Tasche. Das manuell eingestellte Limit gilt weiterhin für `/ssb delete` und die Löschtaste.

Sinkt der Seelensplitterbestand unter den eingestellten Grenzwert, pulsiert **Low Soul Shards** auch im Kampf. Die Warnung blendet sich aus, sobald der Grenzwert wieder erreicht ist oder du SSB pausierst. Im **EUI Unlock Mode** kannst du die Warnung unter **Warlock Essentials** verschieben. Standardmäßig steht sie in der Bildschirmmitte.

Der separate **Soul Shard Counter** zeigt das Splittersymbol und die Gesamtzahl. Unter **Soul Shard Bag → Soul Shard Counter** kannst du Symbol, Text und Warnleuchten anpassen. Im **EUI Unlock Mode → Warlock Essentials → Soul Shard Counter** lässt sich der Zähler verschieben, verankern und skalieren.

## Pause und Tastenbelegung

Unter **Warlock Essentials → Soul Shard Bag** stehen die Pause-Taste und gleich darunter die Löschtaste. Linksklick erfasst die gewünschte Taste, Rechtsklick entfernt die Belegung. Während der Pause trägt die Seelentasche ein gelbes Pausensymbol. Der Chat zeigt den Status beim Pausieren und Fortsetzen an.

Erstelle die empfohlenen SSB-Makros in EUI und ziehe sie auf deine Aktionsleiste. Eigene Makros verwenden `/ssb delete` oder `/click SSBDelete`.

## Dämonenleiste

Die Dämonenleiste zeigt die bedienbaren Fähigkeiten von Wichtel, Leerwandler, Sukkubus, Inkubus und Teufelsjäger aus den aktiven Pet-Slots. Linksklick wirkt die Fähigkeit. Rechtsklick schaltet Autocast bei unterstützten Fähigkeiten um. Ein goldener Punkt unten rechts zeigt aktiven Autocast.

Im **EUI Unlock Mode → Warlock Essentials → Dämonenleiste** kannst du die Leiste verschieben, verankern und ihre Größe ändern. Die EUI-Einstellungen der Dämonenleiste enthalten die Position und Farben der Haltungsanzeige.

Unter **Dämonenleiste → Einstellungen → Tooltips** kannst du Tooltips ein- oder ausschalten oder sie beim Halten von Strg, Umschalt oder Alt anzeigen lassen.

Unter **Dämonenleiste → Pet-Aktionen** kannst du jede Fähigkeit einzeln ein- oder ausblenden. Die Liste zeigt die Zaubersymbole und gruppiert die Fähigkeiten nach Dämon. Sukkubus und Inkubus teilen sich die Auswahl.

Unter **Dämonenleiste → Darstellung** stellst du Symbolgröße, Abstand, Zoom und Rahmen ein. Die Leiste passt sich an die sichtbaren Symbole an. Farbe, Größe, Anker und Versatz des Autocast-Punkts lassen sich dort ebenfalls einstellen.

## Herkunft

Spiellogik und Übersetzungen basieren auf [SoulShardForever 1.17.0](https://github.com/msromike/SoulShardForever) von msromike (MIT). Die Einstellungsseite nutzt die [EllesmereUI-Plugin-API](https://github.com/EllesmereGaming/EllesmereUI/blob/main/PLUGINS_API.md).
