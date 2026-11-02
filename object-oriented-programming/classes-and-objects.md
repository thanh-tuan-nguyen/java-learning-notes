# Klassen und Objekte in Java

Java ist eine objektorientierte Programmiersprache.

Mit Klassen können eigene Datentypen erstellt werden. Eine Klasse beschreibt, welche Eigenschaften und Funktionen ein Objekt besitzen soll.

## Klasse als Bauplan

Eine Klasse kann man sich wie einen Bauplan vorstellen.

Zum Beispiel beschreibt die Klasse `Product`, welche Informationen ein Produkt besitzen soll.

```java
public class Product {

    String name;
    double price;
    int stock;
}
```

Die Klasse besitzt drei Eigenschaften:

- `name` für den Produktnamen
- `price` für den Verkaufspreis
- `stock` für den Lagerbestand

## Objekt erstellen

Aus einer Klasse können konkrete Objekte erstellt werden.

```java
Product product1 = new Product();
```

`Product` ist die Klasse.

`product1` ist der Name der Variable.

`new Product()` erstellt ein neues Objekt der Klasse `Product`.

## Eigenschaften eines Objekts setzen

```java
Product product1 = new Product();

product1.name = "Jasminreis";
product1.price = 14.99;
product1.stock = 12;
```

Das Objekt `product1` besitzt jetzt eigene Werte.

## Zweites Objekt erstellen

Aus derselben Klasse können mehrere verschiedene Objekte erstellt werden.

```java
Product product1 = new Product();

product1.name = "Jasminreis";
product1.price = 14.99;
product1.stock = 12;

Product product2 = new Product();

product2.name = "Kokosmilch";
product2.price = 2.49;
product2.stock = 20;
```

Beide Objekte gehören zur Klasse `Product`, besitzen aber unterschiedliche Werte.

## Werte ausgeben

```java
System.out.println(product1.name);
System.out.println(product1.price);
System.out.println(product1.stock);
```

Mögliche Ausgabe:

```text
Jasminreis
14.99
12
```

## Methoden in einer Klasse

Eine Klasse kann neben Eigenschaften auch Methoden besitzen.

```java
public class Product {

    String name;
    double price;
    int stock;

    public void showProduct() {
        System.out.println("Produkt: " + name);
        System.out.println("Preis: " + price);
        System.out.println("Bestand: " + stock);
    }
}
```

Die Methode kann über das Objekt aufgerufen werden:

```java
product1.showProduct();
```

## Beispiel für eine Bestandsprüfung

```java
public class Product {

    String name;
    int stock;
    int minimumStock;

    public boolean isBelowMinimumStock() {
        return stock < minimumStock;
    }
}
```

Der Aufruf könnte so aussehen:

```java
if (product1.isBelowMinimumStock()) {
    System.out.println("Nachbestellung erforderlich.");
}
```

## Klasse und Objekt unterscheiden

Klasse:

```text
Product
```

Sie beschreibt, wie Produkte grundsätzlich aufgebaut sind.

Objekt:

```text
product1
```

Es ist ein konkretes Produkt mit eigenen Werten.

Beispiel:

```text
Klasse: Product

Objekt 1:
Jasminreis
14,99 €
12 Stück

Objekt 2:
Kokosmilch
2,49 €
20 Stück
```

## Merksätze

- Eine Klasse ist ein Bauplan für Objekte.
- Ein Objekt ist eine konkrete Instanz einer Klasse.
- Eine Klasse kann Eigenschaften und Methoden besitzen.
- Mit `new` wird ein neues Objekt erstellt.
- Von einer Klasse können beliebig viele Objekte erstellt werden.
- Jedes Objekt kann eigene Werte besitzen.

## Bezug zu meiner Produktverwaltung

Für meine spätere Produktverwaltung kann jedes Produkt als eigenes Objekt dargestellt werden.

Die Klasse `Product` könnte später beispielsweise folgende Eigenschaften enthalten:

- Artikelnummer
- Produktname
- Barcode
- Verkaufspreis
- aktueller Lagerbestand
- Mindestbestand

Weitere Informationen wie Wareneingänge, MHD-Chargen und Verkäufe sollen später in eigenen Klassen abgebildet werden.

## Status

Die Beispiele wurden zunächst als Lernnotizen erstellt und werden später lokal mit Java getestet.
