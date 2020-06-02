# Was ist MAM?

MAM, Masked Authenticated Messaging, sind verschlüsselte Nachrichten im Tangle, deren Quelle nachgewiesen werden kann.

TEXT SEBASTIAN HEUSSER


OTA wurde für das Internet der Dinge und Maschinen zu Maschinen Kommunikation erschaffen. Mit Masked Authenticated Messaging können Sensoren und andere Geräte ganze Datenströme verschlüsseln und diese quantensicher im IOTA Tangle sichern. Nur autorisierte Personen können den gesamten Datenstrom lesen oder neue Daten anhängen. Im Wesentlichen funktioniert MAM wie ein Radio, bei dem nur diejenigen einem Sender zuhören können, die die richtige Frequenz kennen. Die Kanäle können öffentlich oder verschlüsselt sein, und nur der Sender kann neue Daten in den Kanel einbringen. Es gibt drei Optionen, aus denen Sender auswählen können, wenn sie eine neue Nachricht in dem Kanal veröffentlichen. -

- Public: Jeder kann den Inhalt der Nachricht lesen. 
- Privat: Nur der Sender (dh. der Seed Besitzer) kann die Nachrichten lesen.
- Restricted: Man kann einen Schlüssel angeben, welcher weitergeben werden kann.

Mit diesem Schlüssel kann man den Inhalt einer Nachricht lesen, jedoch ausschließlich mit dem Seed auch neue Nachrichten im Kanal veröffentlichen. Dieser Schlüssel wird im Quellcode als sideKey bezeichnet. Bibliotheken für MAM stehen für Javascript und C zur Verfügung. Hierbei sollte man allerdings sehr auf die Anweisungen im Code Repository achten, da sich das Projekt noch in einer sehr frühen Entwicklungsphase befindet. Eine gute Möglichkeit für Informationen, Diskussion und Fragen ist hierfür der #mam-dev und #mam-discussion Kanal im IOTA Discord.