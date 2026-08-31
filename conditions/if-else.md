# Bedingungen mit if und else in Java

Mit Bedingungen kann ein Programm Entscheidungen treffen.

Ein Programm kann beispielsweise prüfen:

- Ist ein Produkt noch auf Lager?
- Wurde der Mindestbestand unterschritten?
- Ist ein Benutzer angemeldet?
- Ist eine Zahl größer als eine andere?

## Grundaufbau

```java
if (Bedingung) {
    // Wird ausgeführt, wenn die Bedingung wahr ist
}

Beispiel:
int stock = 10;

if (stock > 0) {
    System.out.println("Produkt ist verfügbar.");
}

Die Bedingung stock > 0 prüft, ob der Lagerbestand größer als 0 ist.


if und else

Mit else kann festgelegt werden, was passieren soll, wenn die Bedingung nicht erfüllt ist.

int stock = 0;

if (stock > 0) {
    System.out.println("Produkt ist verfügbar.");
} else {
    System.out.println("Produkt ist nicht verfügbar.");
}

Mindestbestand prüfen

Für eine Produktverwaltung kann beispielsweise geprüft werden, ob Ware nachbestellt werden sollte.

int stock = 4;
int minimumStock = 5;

if (stock < minimumStock) {
    System.out.println("Warnung: Mindestbestand unterschritten.");
} else {
    System.out.println("Lagerbestand ausreichend.");
}


else if

Mit else if können mehrere Bedingungen geprüft werden.

int stock = 3;

if (stock == 0) {
    System.out.println("Produkt ausverkauft.");
} else if (stock < 5) {
    System.out.println("Produkt sollte nachbestellt werden.");
} else {
    System.out.println("Lagerbestand ausreichend.");
}

Vergleichsoperatoren
| Operator | Bedeutung           |
| -------- | ------------------- |
| `==`     | gleich              |
| `!=`     | ungleich            |
| `>`      | größer als          |
| `<`      | kleiner als         |
| `>=`     | größer oder gleich  |
| `<=`     | kleiner oder gleich |


Wichtig

Ein einzelnes = weist einer Variable einen Wert zu:
int stock = 10;


Zwei Gleichheitszeichen == vergleichen zwei Werte:
if (stock == 10) {
    System.out.println("Der Bestand beträgt genau 10.");
}


Eigene Übung

Ein Produkt besitzt einen Bestand von 7 Stück und einen Mindestbestand von 10 Stück.

int stock = 7;
int minimumStock = 10;

if (stock < minimumStock) {
    System.out.println("Nachbestellung erforderlich.");
} else {
    System.out.println("Keine Nachbestellung erforderlich.");
}


Merksätze
if prüft eine Bedingung.
else wird ausgeführt, wenn die Bedingung nicht erfüllt ist.
else if ermöglicht weitere Bedingungen.
= weist einen Wert zu.
== vergleicht zwei Werte.
Status

Die Beispiele wurden zunächst als Lernnotizen erstellt und werden später lokal mit Java getestet.
