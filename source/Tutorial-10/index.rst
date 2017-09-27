T-10 Blöcke, Funktionen und Methoden
====================================

Blöcke
------

:: 

   println({
     val x = 1 + 1
     x + 1
   })

Es wird jeweils der letzte Ausdruck zurückgegeben. Im obigen Beispiel also *3*.


Funktionen
----------

::

   (x: Int) => x + 1 
   
Obige Funktion trägt keinen Namen, man nennt solche Funktionen auch *anonyme Funktionen*.

Funktionen können aber auch Namen haben, z.B. *addOne*:

:: 

   val addOne = (x: Int) => x + 1
   println(addOne(1)) // 2
   
und mehrere Parameter aufnehmen:

:: 

   val add = (x: Int, y: Int) => x + y
   println(add(1, 2)) // 3
   
oder auch keine Parameter:

::

   val getTheAnswer = () => 42
   println(getTheAnswer()) // 42


Methoden
--------

Methoden sind ähnlich wie Funktionen, mit einigen Unterschieden.

z.B. eine Methode wird über den Befehl *def* definiert.

:: 

   def add(x: Int, y: Int): Int = x + y
   println(add(1, 2)) // 3
   
Eine Methode enthält einen Namen, eine Paramter-Liste, Rückgabe-Typ und einen Code-Teil (Body):

:: 

   def getSquareString(input: Double): String = {
     val square = input * input
     square.toString
   }

Das Resultat einer Methode ist jeweils der letzte Ausdruck in der Methode. Es gibt aber auch den Befehl *return*, mit dem man ein Resultat zurückgeben kann, wird aber in Scala
selten eingesetzt.
   
Auch Operatoren sind Methoden:

z.B.:

::

   1 + 1

ist dasselbe wie:

:: 

   1.+(1)

Es gibt dann auch noch die spezielle *main* Methode, die als Startpunkt eines Scala-Programmes gilt:

:: 

   object MeineApp {
     def main(args: Array[String]): Unit =
       println("Hello, Scala developer!")
   } 