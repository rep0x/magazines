# IOTA Apps in unter 5 Minuten entwickeln

Das IOTA Payment Modul bringt eine IOTA Wallet in deine Javascript Anwendung.

TEXT SEBASTIAN HEUSSER

Du hast eine Idee oder schon eine Applikation und möchtest IOTA Zahlungsmöglichkeiten einbauen? Kein Problem! Das IOTA Payment Modul bringt eine IOTA Wallet für Javascript Apps mit und kümmert sich um alles IOTA relevante. Das Modul kommt mit einem eigenen Webserver mit, kommuniziert mit dem Browser oder anderen Applikationen via HTTP und Websockets und bietet vielerlei Einstellungsmöglichkeiten.

Mit einer einfachen Installation und Einbindung ist das ganze Modul nach nur wenigen Minuten einsatzbereit. Man muss nur noch im eigenen Code definieren, was passieren soll. So kann der Entwickler genau definieren, was passieren soll, wenn eine IOTA Transaktion einging und bestätigt wurde. Mit dem Websocket Server ist es möglich, dem Benutzer wichtiges Feedback zu geben, wie zum Beispiel “Die Transaktion ist eingegangen” oder “Die Zahlung wurde bestätigt”.

Der Unterschied zwischen dem IOTA Hub und dem Payment Modul ist ein ganz einfach. Der IOTA hub wurde für Anwendungen wie Kryptobörsen entwickelt, also Anwendungen mit mehreren Benutzern die ein Wallet besitzen. Bei dem Payment Modul gibt es nur ein Wallet, welches auch durch ein mitgeliefertes Frontend benutzt und konfiguriert werden kann.

Das Payment Modul ist noch in einer sehr frühen Entwicklungsphase, wurde aber schon von einigen Entwicklern erfolgreich eingebaut. So wurde zum Beispiel die Bezahlfunktion des einfachIOTA Magazin Onlineshops mit dem Payment Modul umgesetzt. Der Button wurde als Extra Frontend Modul als weiteres Paket ausgelagert, so das Frontendentwickler mit einer Zeile Code ihre Applikation mit einem IOTA Pay Button erweitern können. Ein Artikel auf Hackster. io beschreibt, wie man das Payment Modul auf einem Raspberry Pi in betrieb nimmt und die Adressen als QR-Code auf einem E-Ink Display anzeigt.

Das Projekt befindet sich, wie IOTA auch, immer noch in de Entwicklungsphase. Tägliche Updates sind an der Tagesordnung. Wenn dir Fehler oder Verbesserungen auffallen, kannst Du gerne ein Issue auf GitHub anlegen. Wir suchen auch immer nach Unterstützung, um das Payment Modul noch sicherer und schneller zu machen.

- [Payment Modul](https://github.com/iota-pay/iota-payment)
- [VueJS Pay Button](https://github.com/iota-pay/vue-iota-payment)
- [Raspberry Pi Tutorial auf Hackster.io](https://www.hackster.io/huhn/raspberry-pi-as-iota-payment-provider-8f1e0f)