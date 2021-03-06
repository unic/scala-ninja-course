T-04 Scala-Dateien erstellen und kompilieren
============================================

Den Vorgang, wo man den geschriebenen *Code* in eine ausführbare Einheit *übersetzt*, nennt man **Kompilieren**.
D.h. man kompiliert eine *Sourcecode-Datei* in eine ausführbare Einheit, damit man das Programm auch ausführen kann.

Erstelle eine neue Datei mit Hilfe eines einfachen Text-Editors *HelloWorld.scala* und schreibe folgendes Programm:

::

   object HelloWorld {
     def main(args: Array[String]): Unit = {
       println("Hello, world!")
     }
   }

Kompiliere *HelloWorld.scala* :

::

   cmd> scalac HelloWorld.scala
   
Im selben Verzeichnis wirst du dann eine neue Datei finden *HelloWorld.class*.

Du kannst anschliessend dein Programm laufen lassen mit folgendem Befehl:

::

   cmd> scala HelloWorld
   
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