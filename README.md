# Java-Tutorial

---

# Java - Tutorial

## Reihenfolge:

- warum java
  - vorteile
  - nachteile
  - wie funktionier java
- kommentare
  - einzeilug
    ```java
    // dies ist ein kommenstar
    int x = 3; // x steht für ...
    ```
  - mehrzeilig
    ```java
    /* mehrere Zeilen
     * als Kommentar
     * ideal für längere
     * Beschreibungen
     */
    ```
- variable
  - short
    ```java
    short min = -32768;
    short max = 32767;
    ```
  - int
    ```java
    int min = -2147483648;
    int max = 2147483647;
    ```
  - long
    ```java
    long min = -9223372036854775808;
    long max = 9223372036854775807;
    ```
  - float
    ```java
    float min = 1.4E-45;
    float max = 3.4028235E38;
    ```
  - double
    ```java
    double min = 4.9E-324;
    double max = 1.7976931348623157E308;
    ```
  - char
    ```java
    // UTF-16 Codec
    char hashtag = '#';
    ```
  - string
    ```java
    // ACTUNG: String groß geschrieben
    // String ist keine Variable sondern eine Klasse, genau genommen
    String name = "Maxi";
    ```
- ausgabe
    ```java
    // println: Ausgabe plus Zeilenumbruch
    System.out.println("Hallo User");
    
    // pritn: Ausgabe ohne Zeilenumbruch
    System.out.print("Hallo Welt");
    
    // Variable ausgeben
    String name = "Max";
    int alter = "23";
    System.out.println("Hallo " + name + ", du bist " + alter + " Jahre jung.");
    ```
    **Escape-Zeichen:**
    \\n new line - neue Zeile
    \\t tabulator
    \" das " ausgaben
	```java
    System.out.println("\n---\n");
	//Ausgabe: 
    //	Zeilenumbruch
    //	---
    //    Zeilenumbruch
    ```
- eingabe
    ```java
    // Bibliothek "java.util.Scanner" wird zur EIngabe benötigt
    import java.util.Scanner;
   
	public class Program {
	  public static void main(String[] args) {
        // Klasse Scanner deklarieren (anlegen) und initalisieren (zuweisen)
		Scanner scan = new Scanner(System.in);
        // Zum Namen einlesen
		System.out.print("Ihr Name: ");
		String name = scan.nextLine();
        // Zum Alter einlesen
		System.out.print("Ihr Alter: ");
		int alter = scan.nextInt();
        // Scanner schließen, wenn dieser nicht mehr benötigt wird
		scan.close();
        // Ausgabe:
		System.out.println("Hallo " + name + ", du bist " + alter + " Jahre jung.");
	  }
    }
    ```
- convertierung
    ```java
    // int zu String
    int i = 23;
	String s = String.valueOf(i);

	// String to int
	String s2 = "123";
	int i2 = Integer.parseInt(s2);
    ```
- verzeigung
  - if
     **Vergleichsoperatoren:**
     < kleiner
     \> größer
     <= kleiner gleich
     \>= größer gleich
     == gleich
     != ungleich

    **logische Operatoren:**
    && und
    || oder
    ! nicht
    ```java
    int alter = 23;
    
    if (alter < 12){
      System.out.println("Kind");
    } else if (alter < 18){
      System.out.println("Jugendlicher/Teenager");
    } else {
      System.out.println("Erwachsener");
    }
    
    // === === ===
    
    String name = "Max";
    int plz = 1010;

	if (name.equalt("Max") && plz == 1010){
      System.out.println("Max lebt in 1010.");
    } else if (name.equals("Max") && plz != 1010){
      System.out.println("Max lebt nicht in 1010.");
    } else if (!name.equals("Max") && plz == 1010){
      System.out.println("Nicht Max lebt in 1010.");
    } else {
      System.out.println("Nicht Max lebt nicht in 1010.");
    }
    ```
  - switch
    ```java
    int eingabe = 3;
    
    switch (eingabe){
      case 0:
      	System.out.println("Eingabe war 0");
        break;
      case 1:
      	System.out.println("Eingabe war 1");
        break;
      case 2:
      	System.out.println("Eingabe war 2");
        break;
      default:
      	System.out.println("Eingabe war ungültig.");
    }
    ```
- schleifen
  - while
    ```java
    int i = 0;
    while (i < 10){
      System.out.println(i);
      i++;
    }
    ```
  - do while
    ```java
    import java.util.Scanner;
	// ...
	int eingabe = -1;
    do {
      // Menü anzeigen
      System.out.println("[1] Calc");
      System.out.println("[2] Editor");
      System.out.println("[3] ...");
      System.out.println("[0] Ende");
      // Usereingabe
      System.out.print("Ihre Eingabe: ");
      Scanner scan = new Scanner(System.in);
      eingabe = scan.nextInt();
      scan.close();
      // Logik
	  if(eingabe == 1){
        System.out.println("\"Calc\" gewählt");
      } else if(eingabe == 2){
        System.out.println("\"Editor\" gewählt");
      } else if(eingabe == 3){
        System.out.println("\"...\" gewählt");
      } else if(eingabe == 0){
        System.out.println("Programm wird beendet");
      } else {
        System.out.println("Ungültige Eingabe");
      }
    } while(einagbe != 0);
    ```
  - for
    ```java
    for(int i = 0; i < 10; i++){
      System.out.println(i);
    }
    ```
  - foreach
    ```java
    String name = "Max Mustermann";
    for(char item : name.toCharArray()){
      System.out.println(item);
    }
    ```
- array
  - 1 dimension (liste)
    ```java
    
    ```
  - 2 dimensionen (schach)
    ```java
    
    ```
  - 3 dimensionen (minecraft)
    ```java
    
    ```
- liste
    ```java
    
    ```
- funktion
  - parameter
    ```java
    
    ```
  - rückgabewert
    ```java
    
    ```
  - rekursion
    ```java
    
    ```
- exception
  - vordefinierte
  - eigene
- klasse
  - getter
  - setter
  - constructor
  - public
  - private
  - static
- polymorphy
  - interface
  - vererbung
- dateien
  - txt
    ```java
    
    ```
  - csv
    ```java
    
    ```
- gui
  - label
  - textbox
  - button
  - radiobutton
  - checkbox
- sql
  - sqlite
  - mysql
  - ms sql
  - access
