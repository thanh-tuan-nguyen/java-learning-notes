# Methoden in Java

Methoden werden verwendet, um bestimmte Aufgaben in einem Programm auszuführen.

Sie helfen dabei, Code übersichtlicher zu machen und mehrfach zu verwenden.

## Einfache Methode

```java
public static void sayHello() {
    System.out.println("Hallo Tuan!");
}
```

Aufruf:

```java
sayHello();
```

## Aufbau einer Methode

```java
public static void methodName() {
    // Code
}
```

Dabei bedeutet:

- `public`: Die Methode kann von anderen Bereichen verwendet werden.
- `static`: Die Methode gehört direkt zur Klasse.
- `void`: Die Methode gibt keinen Wert zurück.
- `methodName`: Der Name der Methode.
- `()`: Hier können später Werte übergeben werden.

## Methode mit Parameter

Mit einem Parameter kann einer Methode ein Wert mitgegeben werden.

```java
public static void showProduct(String productName) {
    System.out.println("Produkt: " + productName);
}
```

Aufruf:

```java
showProduct("Jasminreis");
showProduct("Kokosmilch");
```

Ausgabe:

```text
Produkt: Jasminreis
Produkt: Kokosmilch
```

## Methode mit mehreren Parametern

```java
public static void showProduct(String productName, int stock) {
    System.out.println("Produkt: " + productName);
    System.out.println("Bestand: " + stock);
}
```

Aufruf:

```java
showProduct("Jasminreis", 12);
```

## Methode mit Rückgabewert

Eine Methode kann auch ein Ergebnis zurückgeben.

```java
public static int calculateNewStock(int stock, int soldQuantity) {
    return stock - soldQuantity;
}
```

Aufruf:

```java
int currentStock = 10;
int newStock = calculateNewStock(currentStock, 3);

System.out.println(newStock);
```

Ergebnis:

```text
7
```

`return` gibt das Ergebnis der Methode zurück.

## Beispiel: Mindestbestand prüfen

```java
public static boolean isBelowMinimumStock(int stock, int minimumStock) {
    return stock < minimumStock;
}
```

Aufruf:

```java
boolean needsRestock = isBelowMinimumStock(4, 5);

if (needsRestock) {
    System.out.println("Nachbestellung erforderlich.");
}
```

## Warum Methoden wichtig sind

Ohne Methoden wird ein Programm schnell unübersichtlich.

Statt alles in die `main`-Methode zu schreiben, können einzelne Aufgaben getrennt werden.

Zum Beispiel:

```java
addProduct();
showProducts();
searchProduct();
deleteProduct();
checkStock();
```

Solche Methoden können später auch in einer Produktverwaltung verwendet werden.

## Merksätze

- Methoden fassen zusammengehörigen Code zusammen.
- Methoden können mehrfach verwendet werden.
- Parameter übergeben Werte an eine Methode.
- `void` bedeutet, dass kein Wert zurückgegeben wird.
- `return` gibt ein Ergebnis zurück.
- Methodennamen sollten klar beschreiben, was die Methode macht.

## Status

Die Beispiele wurden zunächst als Lernnotizen erstellt und werden später lokal mit Java getestet.
