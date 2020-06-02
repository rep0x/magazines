# Hardware Wallet mit ESP32

Bau dein eigenes Hardware Wallet mit dem du IOTA Transaktionen versenden kannst! 

TEXT SEBASTIAN HEUSSER

Der ESP32 ist, anders als der Raspberry Pi, nur ein Mikrocontroller und ist in etwa vergleichbar mit einem Arduino - nur hat der ESP32 viel mehr Power und Funktionalität. Beispielsweise hat letzterer einen integrierten WLAN und Bluetooth Chip und kann auf diese Weise einfach mit dem Heimnetz kommunizieren. An die GPIO Pins könnt ihr, ähnlich wie beim Raspberry Pi, Sensoren, Schalter und andere Teile anschließen. Der ESP32 kostet rund 10 Euro und kann mit verschiedenen Komponenten gekauft werden. Zum Beispiel einer Kamera oder einem kleinen Display. Aber Achtung der ESP32 mit Cam hat keinen USB Anschluss. Ihr müsst also ein passendes USB Modul haben, um ihn beschreiben zu können. Mit der Veröffentlichung von CClient v1.0.0-beta kann man auf dem ESP32 eine Hardware-Wallet implementieren. Wir benutzen hier die Version von TIm Rappe, die auf den Code der IOTA Foundation aufbaut, aber die Erstinstallation für uns noch viel einfacher macht. Viel Spaß beim Basteln!

## Dein Machine Wallet

Im Grunde geht das ganz einfach:
    1. Alle benötigten Programme installieren
    2. Machine Wallet Software herunterladen
    3. Die Software auf den ESP hochladen (flashen)
    4. Seed eingeben und Transaktionen versenden
Natürlich ist das nur die Theorie. In der Praxis geht das leider nicht immer ganz so reibungslos. Falls bei dir Fehler auftreten und du nicht mehr weiter kommst, kannst du dich gerne bei uns im Discord anmelden und im #hardware Channel nach Hilfe fragen!


## Schritt für Schritt Anleitung
Befolge die Schritt für Schritt Anleitung auf einfachIOTA.de und du kannst schon bald dein eigenes Hardware Wallet benutzen. Wir raten dir jedoch das Devnet dafür zu nutzen, da die Bibliothek noch einen sehr frühen Entwicklungsstand hat.

- [Schritt für Schritt Anleitung](https://www.einfachiota.de/#/post/iota-machine-wallet-auf-einem-esp32)
- [ESPIntegration](https://github.com/magnisinfo/IOTA_ESP32_integration)
- [CCLibrary](https://github.com/iotaledger/entangled/tree/develop/cclient)