# Was ist Proof of Work?

TEXT THORALF MÜLLER

PoW ist die Abkürzung von Proof of Work, also dem Nachweis einer Arbeit. Die Arbeit ist in unserem Falle eine Rechenaufgabe, die von einem Rechner gelöst werden muss. Bei den meisten Blockchains machen das die sogenannten “Miner”. Das Proof of Work wird bei IOTA als Spamschutz eingesetzt. Spam, wie man ihn von E-Mails kennt, will man natürlich auch in einem dezentralen System vermeiden. Damit das Netzwerk nicht mit Spam überflutet wird, setzt man nun dieses PoW ein. Somit muss man nun etwas Rechenleistung aufbringen, um Transaktionen in das System einzubringen. Im Endeffekt macht man das Spammen unprofitabel, da man durch viel Spam auch hohe Stromkosten erzeugt.

Der PoW bei IOTA dient nur als Spamschutz und wird nicht für den Konsensus benötigt. Der Schlüssel zum PoW ist, dass er schwierig zu produzieren, aber einfach zu überprüfen ist. Für jede Transaktion muss der PoW gemacht werden, damit sie von den Nodes akzeptiert wird.
Dabei wird die Nonce (die letzten 27 Trytes einer Transaktion) verändert und anschließend die Transaktion mit der geänderten Nonce gehasht. Wenn der Hash der Transaktion, in Trits umgewandelt, am Ende so viele Nullen hat, wie für das jeweilige Netzwerk benötigt werden, ist die Transaktion gültig. Falls nicht, wird der Prozess wiederholt, bis genug Nullen vorhanden sind.

Die Anzahl der mindestens benötigten Nullen wird in MWM (minimum weight magnitude) angegeben, beim Mainnet sind es 14, im Devnet 9. Je höher die Zahl ist, umso aufwendiger ist es. 3 Trits mit dem Wert 0 sind eine 9 in Trytes, deswegen sind am Ende von einem gültigen Hash in Trytes immer mehrere 9en zu sehen.

Beispielhash
  TRSJAIDFMDPA9DRRVMTQPSIKIWHJMEEUXTASVRKWGJCFASU
  99UFBVKFBJZSNQXMDXTL9YS9EvFBRMA9999

Die letzten 9 Trytes des Hashes in Trits umgewandelt, mit 14 Nullen am Ende:
0, -1, 1, -1, 1, 0, 0, 0, -1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
Der PoW kann entweder lokal auf dem Gerät ausgeführt werden, oder remote auf einem anderen Gerät. Der Vorteil von lokalem PoW ist, dass man von niemandem abhängig ist. Wenn man aber kein leistungsstarkes Gerät hat kann der PoW lange dauern, wodurch die Wahrscheinlichkeit einer Bestätigung der Transaktion sinken kann. In Trinity kannst du das in den Einstellungen selbst festlegen (remote PoW funktioniert nur bei Nodes, die das auch unterstützen). Wenn du remote PoW verwenden willst, kannst du dafür entweder
öffentliche Nodes oder z.B. einen Service wie https://powsrv.io/ oder https://tanglebay.org/ nutzen, welche FPGAs einsetzen und dadurch den PoW sehr schnell und effizient erledigen.

https://powsrv.io/ erledigt den PoW besonders schnell (ca. 50 ms/ Transaktion), ist aber kostenpflichtig. Hier kann man einfach den PoW für eine Anzahl an Transaktionen kaufen und so nutzen, wie man will. Zum Beispiel über mehrere Monate verteilt oder direkt alles auf einmal. Das geht zur Zeit mit ca. 90 Transaktionen pro Sekunde.
Wenn du den PoW lokal und sehr schnell erledigen willst, kannst du dafür einen Proxy Server installieren. Der übernimmt nur den PoW und leitet alle anderen Anfragen an einen IRI Node weiter. Eine Anleitung dazu findest du hier: https://docs.iota.org/docs/node- software/0.1/iri/how-to-guides/install-a-pow-proxy
Im Browser gibt es die Möglichkeit den PoW mit WebGL2 (GPU) zu erledigen, das wird aber nicht von allen Browsern unterstützt.
Dafür kannst du curl.lib.js und iota.js für den Browser importieren und dann attachToTangle (die Funktion für den PoW) überschreiben:

```code
var iota = core.composeAPI({
    provider: `https://nodes.thetangle.org:443`,
    attachToTangle: curl.localPoW })
```

Unter https://thoralf-m.github.io/Devbox/ kannst du es selbst ausprobieren, indem du einfach eine Transaktion mit einer Nachricht schickst. Klicke dazu auf den „localPoW“, danach auf den „message tx“ und dann den „Run“ Button. An der Auslastung der GPU kann man dann sehen, dass es auch wirklich lokal berechnet wird.
Es gibt auch Ideen den PoW in der Zukunft durch einen anderen Spamschutz zu ersetzen, dafür könnte man z.B. die Transaktionen pro Sekunde auf die physikalische Position limitieren, was vor allem für das IoT interessant ist.