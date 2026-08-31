# Schleifen in Java

Schleifen werden verwendet, wenn ein Programm bestimmte Anweisungen mehrfach ausführen soll.

Typische Beispiele:

- mehrere Produkte anzeigen
- eine Liste durchsuchen
- Zahlen mehrfach ausgeben
- eine Eingabe wiederholen
- mehrere Lagerbestände prüfen

## for-Schleife

Eine `for`-Schleife eignet sich besonders, wenn vorher bekannt ist, wie oft etwas ausgeführt werden soll.

```java
for (int i = 1; i <= 5; i++) {
    System.out.println(i);
}

Die Ausgabe wäre:
1
2
3
4
5

Aufbau einer for-Schleife
for (Startwert; Bedingung; Veränderung) {
    // auszuführender Code
}

Im Beispiel:

for (int i = 1; i <= 5; i++)

bedeutet:

int i = 1 → Die Variable i startet bei 1.
i <= 5 → Die Schleife läuft, solange i kleiner oder gleich 5 ist.
i++ → Nach jedem Durchlauf wird i um 1 erhöht.

i++ ist eine Kurzform für:
i = i + 1;

Beispiel mit Produkten
for (int i = 1; i <= 3; i++) {
    System.out.println("Produkt " + i);
}

Ausgabe:
Produkt 1
Produkt 2
Produkt 3

Später können auf diese Weise beispielsweise mehrere Produkte aus einer Liste ausgegeben werden.

while-Schleife

Eine while-Schleife läuft so lange, wie eine bestimmte Bedingung erfüllt ist.

int stock = 5;

while (stock > 0) {
    System.out.println("Noch " + stock + " Stück vorhanden.");
    stock--;
}

