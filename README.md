
# Übung 22 - Collections


## 1. Aufgabe

Setzen Sie folgendes Klassendiagramm um:

<p align="center">
  <img src="/assets/images/UML1.png" alt="Bildbeschreibung" />
</p>

**Beschreibung der `Fahrzeug`-Klasse:**

- Eigenschaften: 
	- Im Konstruktor müssen die `set`-Methoden aufgerufen werden. 
	- Prüfen Sie alle Eigenschaften auf sinnvolle Werte. 

- Methoden: 
	- `anzeigen()`: Gib alle Eigenschaften schön formatiert aus. 


**Beschreibung der `Auto`-Klasse:**

- Eigenschaften: 
	- Im Konstruktor müssen die `set`-Methoden aufgerufen werden. 
	- Prüfen Sie alle Eigenschaften auf sinnvolle Werte. 

- Methoden: 
	- `anzeigen()`: Gib alle Eigenschaften schön formatiert aus. 


**Beschreibung der `Motorrad`-Klasse:**

- Eigenschaften: 
	- Im Konstruktor müssen die `set`-Methoden aufgerufen werden. 

- Methoden: 
	- `anzeigen()`: Gib alle Eigenschaften schön formatiert aus. 

Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Testen Sie Ihr Programm, indem Sie die Methoden aufrufen. 

## 2. Aufgabe

Setzen Sie folgendes Klassendiagramm um:

<p align="center">
  <img src="/assets/images/UML2.png" alt="Bildbeschreibung" />
</p>

**Beschreibung der `Medium`-Klasse:**

- Eigenschaften: 
	- Im Konstruktor müssen die `set`-Methoden aufgerufen werden. 
	- Prüfen Sie alle Eigenschaften auf sinnvolle Werte. 

- Methoden: 
	- `getPrice()`: Soll nur 0 zurückgeben, da die Methode von anderen Klassen ohnehin noch überschrieben wird. 
	- `playingTime()`: Soll nur 0 zurückgeben, da die Methode von anderen Klassen ohnehin noch überschrieben wird. 
	- `showInfo()`: Gibt alle Eigenschaften des Mediums aus. **Hinweis:** Probieren Sie `System.out.println(this);` Warum funktioniert das?
	- `toString()`: Überschreiben Sie die `toString()`-Methode. Geben Sie einen String zurück, welcher alle Eigenschaften beinhaltet. 

**Beschreibung der `CD`-Klasse:**
- Eigenschaften: 
	- Im Konstruktor müssen die `set`-Methoden aufgerufen werden. 
	- Prüfen Sie alle Eigenschaften auf sinnvolle Werte. 
- Methoden:
	- `playingTime()`: Gibt die Laufzeit der `CD` an.
	- `showInfo()`: Gibt alle Eigenschaften der `CD` aus. 
	- `toString()`: Überschreiben Sie die `toString()`-Methode. Geben Sie einen String zurück, welcher alle Eigenschaften beinhaltet. 

**Beschreibung der `DVD`-Klasse:**
- Eigenschaften: 
	- Im Konstruktor müssen die `set`-Methoden aufgerufen werden. 
	- Prüfen Sie alle Eigenschaften auf sinnvolle Werte. 
- Methoden:
	- `playingTime()`: Gibt die Laufzeit der `DVD` an.
	- `showInfo()`: Gibt alle Eigenschaften der `DVD` aus. 
	- `toString()`: Überschreiben Sie die `toString()`-Methode. Geben Sie einen String zurück, welcher alle Eigenschaften beinhaltet. 

**Beschreibung der `MediaLibrary`-Klasse:**
- Eigenschaften: 
	- Im Konstruktor wird die `ArrayList` erzeugt.
- Methoden:
	- `addMedium(Medium medium)`: Fügt der Liste das angegebene `medium` hinzu, wenn es noch nicht vorhanden ist. **Achtung:** Es könnte auch `null` übergeben werden. In diesem Fall soll das Medium nicht hinzugefügt werden.
	- `removeMedium(Medium medium)`: Das angegebene `medium` soll aus der Liste entfernt werden. Dies darf jedoch nur geschehen, wenn das `medium` auch in der Liste vorhanden ist. **Achtung:** Es könnte auch `null` übergeben werden. In diesem Fall soll das Medium nicht hinzugefügt werden.
	- `removeMedia(ArrayList<Medium> media)`: Löscht die Medien aus dem Attribut media, die auch im Parameter media enthalten sind. Die Medien, die im Attribut media nicht enthalten sind, sollen in einer neuen Liste gespeichert werden. Geben Sie diese zurück.
	- `showInfo()`:  Gibt für jedes Medium der Liste alle Eigenschaften aus.
	- `playingTime()`: Gibt die Laufzeit aller Medien der Liste als Summe aus.
	- `moneyValue()`: Gibt den Preis aller Medien der Liste als Summe aus.

Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Testen Sie Ihr Programm, indem Sie die Methoden aufrufen. 
