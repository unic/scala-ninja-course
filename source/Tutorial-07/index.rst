T-07 Listen
===========

Listen sind wie Behälter um mehrere Werte oder Variable zu speichern.

Du kannst eine Liste mit Zahlen z.B. wie folgt definieren:

::

   val a = List(1, 2, 3)
   println(a)

oder eine Liste mit Namen (String-Werten):

:: 

   val names = List("Hans", "Fred", "Caroline")

Um auf ein Listen-Element zuzugreifen kannst du folgenden Befehl brauchen:

:: 

   names(0)
   // Hans

**Beachte**: Die Listen-Elemente starten immer bei *0*, also das erste Element ist an der Position *0*.

Die Grösse einer Liste kannst du mit *length* herausfinden:

::
   
   names.length
   // 3
   
Mit dem *foreach*-Befehl kannst du z.B. die einzelnen Listen-Elemente ausgeben:

:: 

   names.foreach(element => println(element))

Mit der Methode *filter* kann man bestimmte Listen-Elemente rausfiltern.

Beispiel: Du willst nur die geraden Zahlen ausgeben:

:: 

   val zahlen = List(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
   val geradeZahlen = zahlen.filter(x => x % 2 == 0)
   // List(2, 4, 6, 8, 10)

Mit der *map* Methode kannst du eine Funktion auf die einzelnen Listen-Elemente anwenden.

Beispiel: Du möchtest eine neue Liste haben mit der Quadrat Zahl von jedem einzelnen Element.

:: 

   val zahlen = List(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
   val quadratZahlen = zahlen.map(x => x * x)
   // List(1, 4, 9, 16, 25, 36, 49, 64, 81, 100)
   

Weitere Links:

- https://www.scala-exercises.org/std_lib/lists
