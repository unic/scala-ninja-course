T-04 Scala-Dateien erstellen und kompilieren
============================================

Erstelle eine neue Datei mit Hilfe eines einfachen Text-Editors *HelloWorld.scala* und schreibe folgendes Programm:

::

   object HelloWorld {
     def main(args: Array[String]): Unit = {
       println("Hello, world!")
     }
   }

Kompiliere *HelloWorld.scala*:

::

   > scalac HelloWorld.scala
   
Im selben Verzeichnis wirst du dann eine neue Datei finden *HelloWorld.class*.

Du kannst anschliessend dein Programm laufen lassen mit folgendem Befehl:

::

   > scala HelloWorld
   
Du kannst dein Programm noch vereinfachen in dem du das *Trait* *App* verwendest. 
Du musst aktuell nicht wissen was ein *Trait* ist, wird später noch erklärt.

Passe deinen Code wie folgt an:

:: 

   object HelloWorld extends App {
     println("Hello, world!")
   }
  
Der Einsatz vom Trait *App* macht der Einsatz der *main* Methode überflüssig, 
da dies im Hintergrund automatisch für dich generiert wird mit deinem Code zwischen den geschweiften Klammern.

Kompiliere jetzt nochmals dein Programm und führe es aus.


Weitere Links:

- https://www.scala-lang.org/documentation/your-first-lines-of-scala.html