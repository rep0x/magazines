# Was ist das Ternäre System?

TEXT SCHMUCKLOS

Was ist das Ternäre System und besteht dadurch ein Vorteil?
Die ternäre Logik, die bei IOTA eingesetzt wird, zieht sich durch das gesamte Projekt. Angefangen bei dem ternären Mikrocontroller JINN, der Hash-Funktion Troika, über den Seed, welcher nur aus Großbuchstaben von A-Z und der Zahl 9 besteht, bis hin zur Tatsache das genau 2.779.530.283.277.761 IOTA Token existieren.

## Die Grundlagen
Bevor wir klären, warum IOTA auf eine ternäre Logik setzt, müssen wir uns zuerst die beiden Systeme etwas genauer anschauen, die für diesen Artikel relevant sind.
Das binäre System: Ein Bit (binary digit) kann genau zwei Zustände (21 = 2) annehmen: 0 und 1. Acht Bits ergeben ein Byte (28 = 256) und können somit 256 Kombinationen abbilden.
Das ternäre System: Ein Trit (trinary digit) kann genau drei Zustände (31 = 3) annehmen: -1, 0 und 1. Drei Trits ergeben ein Tryte (33 = 27) und können somit 27 Kombinationen abbilden.

Die Gegenzahl jeder balancierten ternären Zahl, wird durch das Vertauschen jeder −1 durch 1 und umgekehrt ermittelt. Negative Zahlen können dadurch ebenso leicht dargestellt werden wie positive Zahlen, da im Gegensatz zum Dezimalsystem kein negatives Vorzeichen notiert werden muss. Dieser Umstand macht einige Berechnungen im ternären System effizienter als im binären System. Da Trytes noch komplexer als Bytes sind, ist es wichtig diese leserlicher zu machen. Dabei werden sie in eine Art andere Sprache umgewandelt. Hierfür hat das IOTA Development Team das Tryte-Alphabet erschaffen. Dieses besteht aus der Zahl 9 und den Großbuchstaben A-Z. Das macht insgesamt 27 verschiedene Ziffern, also genau die Anzahl der Kombinationen eines Trytes. Somit kann jede Kombination eines Trytes durch eine Ziffer dargestellt werden. IOTA nutzt genau dieses Alphabet für den Seed, Adressen, Hashes etc. Der Seed selbst besteht aus 81 Ziffern, also 81 Trytes.

Ein Beispiel
CIIXLALQIZSAYXTYLOGYHMY9MSCDGCRXQFOHTZRXFRSFBQJJFFXRMVOJQWZJAILCKFSYEFWNLFWIHISEF

Jedes Tryte hat 27 Kombinationen. Damit hat IOTAs Seed 27^81 Kombinationen. Das sind ~8.71 * 10 Kombinationen. Also deutlich mehr als es Atome im gesamten sichtbaren Universum gibt. Die Wahrscheinlichkeit einen Seed zu erraten, liegt praktisch bei 0 Prozent. Zum Vergleich: Bitcoins private keys sind praktisch ebenfalls nicht zu erraten und das bei nur 2256 = ~1.1577 Kombinationen. Bei Quantencomputern und der Rückrechnung von Adressen auf Seeds bzw. private Schlüssel hat IOTA, durch die deutlich gesteigerte Anzahl an Möglichkeiten, im Vergleich zu Bitcoin die Nase vorn.

## Warum gibt es genau 2.779.530.283.277.761 IOTA Token?
Diese Zahl hat ebenfalls etwas mit den Trytes zu tun. Trytes „balancieren“ sich um den Wert 0 und das von -13 bis +13. Daher auch der Begriff balanced trinary system. Als Beispiel haben wir 27 Kombinationen und den maximalen Wert 13. Dieser kann auch mathematisch berechnet werden:
(33 - 1) / 2 = 13 Kombinationen mit einem positiven Wert
33 Trits ergeben das maximale Supply: (333 - 1) / 2 = 2.779.530.283.277.761 IOTA
Anmerkung: Es war wichtig eine hohe Anzahl an Token zu erschaffen, da sie für Mikrozahlungen zwischen Maschinen genutzt werden sollen und dabei sind hohe Preise pro Token sehr hinderlich. Sollte es in ferner Zukunft, durch eine sehr hohe Nachfrage, nötig sein, die maximale Anzahl der Token zu erhöhen, so ist dies möglich.

## Warum ergeben genau 33 Trits das maximalen Supply?
Das Wertefeld in einer Transaktion ist 81 Trits lang, von denen 33 Trits aktuell verwendet werden. Damit sind es genau (333 - 1) / 2 oder 2.779.530.283.277.761 IOTA, was eine Zahl ist, die noch mit einem 64-bit Integer (Datentyp für ganze Zahlen) dargestellt werden kann.
Da 81 Trits für das Wertfeld reserviert wurden, kann bei Bedarf das max. Supply auf (381 - 1) / 2 erhöht werden. In diesem Fall würde jeder derzeitige Eigentümer immer noch den gleichen Anteil am Gesamtwert besitzen, aber diese Beträge können nun in kleinere Einheiten aufgeteilt werden. Beispiel: Wer vor der Erhöhung 1 MIOTA in der Wallet hatte, der hat nach der Erhöhung 1 GI in der Wallet, nichts ändert sich am Gesamtwert, jedoch stehen nun kleinere Einheiten zur Verfügung als vorher.

## Warum verwenden derzeitige Computer das binäre Zahlensystem?
Zu den Anfangszeiten der Computertechnik wurden mechanische Rechenmaschinen durch elektrische Rechenmaschinen abgelöst, diese ersten Computer funktionierten mit Relais, die auch nur die Zustände „an“ oder „aus“ annehmen konnten. Weil Relais aber mit einem hohen Anteil an mechanischen Bauteilen sehr störanfällig, sind wurden diese durch Transistoren ersetzt, die ebenfalls nur die Zustände „an“ oder „aus“ annehmen (Spannung ein, Spannung aus). Da Transistoren ohne mechanische Bauteile auskommen, können sie in ihren Abmaßen sehr klein gefertigt werden.

Heutige Computer besteht aus vielen Verbindungen und Komponenten, die zur Übertragung und Speicherung von Daten, sowie zur Kommunikation mit anderen Komponenten verwendet werden. Der größte Teil der Speicherung, Übertragung und Kommunikation geschieht heute mit digitaler Elektronik. Diese nutzen immer noch das Binärsystem mit den zwei klar voneinander getrennte Zuständen an = 1 und aus = 0.

Binärsysteme werden immer noch wegen ihrer hohen Geschwindigkeit bei der Veränderung von Schaltungszuständen eingesetzt. Transistoren sind sehr schnelle und wirksame Schalter. Im Zusammenspiel der Menge an Transistoren und der Art ihrer Zustände lassen sich schnell unterschiedliche Zeichen abbilden und Rechenoperationen durchführen. Der Nachteil ist: Um die Geschwindigkeit eines, auf elektrischen Transistoren basierendem Chip zu erhöhen, muss man mehr Transistoren in diesen Chip verbauen. Dazu muss man entweder den Chip größer oder die einzelnen Transistoren kleiner herstellen. Derzeit tendiert man zu kleineren Transistoren, was aber den Nachteil der höheren Hitzeentwicklung, sowie höhere Fehleranfälligkeit mit sich bringt.

## Vorteile eines ternären Systems
Ein System mit drei Zuständen, hätte insofern Vorteile, dass man auf andere Grundelemente statt Transistoren setzen könnte, um effizientere ICs (integrierter Schaltkreise) herzustellen. Ternär ist effizienter, da es die höchste Dichte an Informationsdarstellung unter ganzzahligen Basen (2,4...) aufweist. Im ternären System lassen sich also größere Zahlen in weniger Speicher unterbringen. So wäre die Dezimalzahl 6 im Binärsystem die Zahl 110 (benötigt 3 Bits), im ternären System nur noch 20 (eine Stelle weniger). Der Wirkungsgrad eines Nummernsystems zur Basis von 3 ist effizienter als zu 2 (etwa 1,58-fach effizienter). Man spart also Speicher und Berechnungen würden schneller ablaufen, bei geringerer Takt Zahl des Chips.

Der für ein ternäres System erforderliche Aufwand, um eine komplexe logische Schaltung innerhalb der CPU aufzubauen, kann auf etwa 36% gegenüber einem gleichwertigen binären System reduziert werden. Das führt neben einer platzsparenden kleineren Bauform des Mikrocontrollers zu einer entsprechenden Energieeinsparung. Ternäre Baugruppen wurden in der Computerbranche bisher nicht verwendet, da die Umsetzung der Hardware viel komplexer ist. Zudem fehlt die breite Unterstützung des Massenmarkts. Ist
diese Hardware Umsetzung aber einmal gelungen so sind diese Mikrocontroller deutlich energiesparender und viel leistungsstärker als ihr binäres Pendant.

Mit dem Aufkommen, der in Massenproduktion gefertigten binären Bauteile für Computer, wurden ternäre Rechner (die es zu der Zeit schon gab) leider zu einer kleinen Fußnote der Computergeschichte, obwohl das balancierte ternär System eine effizientere Zahldarstellung in der Mathematik darstellt als das Binäre. In den Siebziger Jahren wurde die Entwicklung ternärer Computer weitestgehend eingestellt, weil binäre Systeme sich schneller und billiger weiterentwickeln ließen. Wie des Öfteren in der Vergangenheit, hat sich im Laufe der Zeit nicht das technisch überlegende Konzept durchgesetzt, sondern das Konzept, welches von der Hardware her am einfachsten und billigsten für den damaligen Massenmarkt umzusetzen war. Es stellt sich die Frage, wo die ternäre Computertechnik heute wäre, wenn diese ebenfalls ständig weiterentwickelt worden wäre.

In Anbetracht der Eleganz und Effizienz der ternären Logik, wird von dem Experten Donald E. Knuth, ein Wiederaufkommen von ternären Computern in der Zukunft prognostiziert. Mögliche Wege, wie sich die Weiterentwicklung ternärer Computer in Zukunft gestalten könnte, ist auch die Kombination eines optischen Computers mit dem ternär System. Ein ternärer Computer unter Verwendung von Lichtwellenleitern könnte dunkel als 0 und zwei orthogonale Polarisationen von Licht als 1 und −1 verwenden.