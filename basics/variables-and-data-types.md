# Variablen und Datentypen in Java

Variablen werden verwendet, um Informationen während der Ausführung eines Programms zu speichern.

Eine Variable besitzt:

* einen Datentyp
* einen selbst gewählten Namen
* einen gespeicherten Wert

## Grundlegender Aufbau

```java
Datentyp variablenName = Wert;
```

Beispiel:

```java
String productName = "Jasminreis";
```

Dabei bedeutet:

* `String`: Der Datentyp der Variable
* `productName`: Der Name der Variable
* `"Jasminreis"`: Der gespeicherte Wert
* `=`: Weist der Variable einen Wert zu
* `;`: Beendet die Java-Anweisung

## String

Mit `String` wird Text gespeichert.

```java
String productName = "Jasminreis";
String barcode = "1234567890123";
```

Texte stehen in Java zwischen doppelten Anführungszeichen.

Auch ein Barcode kann als `String` gespeichert werden. Er wird normalerweise nicht zum Rechnen verwendet und kann mit einer Null beginnen.

## int

Mit `int` werden ganze Zahlen gespeichert.

```java
int stock = 25;
int minimumStock = 5;
```

Mögliche Werte sind beispielsweise:

```text
0
10
25
-3
```

Eine Zahl vom Typ `int` besitzt keine Nachkommastellen.

## double

Mit `double` können Zahlen mit Nachkommastellen gespeichert werden.

```java
double salesPrice = 3.49;
double purchasePrice = 2.15;
```

In Java wird bei Dezimalzahlen ein Punkt statt eines Kommas verwendet.

Für echte Geldberechnungen wird später häufig `BigDecimal` verwendet. Für meine ersten Übungen nutze ich zunächst `double`.

## boolean

Mit `boolean` wird gespeichert, ob eine Aussage wahr oder falsch ist.

```java
boolean available = true;
boolean expired = false;
```

Ein `boolean` kann nur einen der folgenden Werte besitzen:

```text
true
false
```

## char

Mit `char` wird ein einzelnes Zeichen gespeichert.

```java
char categoryCode = 'A';
```

Ein einzelnes Zeichen steht zwischen einfachen Anführungszeichen.

## Mehrere Variablen gemeinsam

```java
String productName = "Jasminreis";
String barcode = "1234567890123";
int stock = 25;
int minimumStock = 5;
double salesPrice = 3.49;
boolean available = true;
```

Diese Variablen könnten später zu einem Produkt in einer Produktverwaltung gehören.

## Werte ausgeben

Mit `System.out.println()` können Werte in der Konsole ausgegeben werden.

```java
System.out.println(productName);
System.out.println(stock);
System.out.println(salesPrice);
```

Text und Variablen können mit dem Pluszeichen verbunden werden:

```java
System.out.println("Produkt: " + productName);
System.out.println("Bestand: " + stock);
System.out.println("Verkaufspreis: " + salesPrice + " Euro");
```

## Eigene Übung

Für ein Produkt sollen folgende Variablen erstellt werden:

* Produktname
* Barcode
* Lagerbestand
* Mindestbestand
* Verkaufspreis
* Verfügbarkeit

```java
String productName = "Kokosmilch";
String barcode = "8851234567890";
int stock = 12;
int minimumStock = 5;
double salesPrice = 2.49;
boolean available = true;
```

## Merksätze

* `String` speichert Text.
* `int` speichert ganze Zahlen.
* `double` speichert Zahlen mit Nachkommastellen.
* `boolean` speichert `true` oder `false`.
* `char` speichert ein einzelnes Zeichen.
* Java-Anweisungen enden meistens mit einem Semikolon.
* Variablennamen sollten verständlich beschreiben, was gespeichert wird.

## Status

Die Beispiele wurden zunächst als Lernnotizen auf GitHub erstellt. Sie werden später lokal in einer Java-Entwicklungsumgebung getestet.
