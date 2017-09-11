T-01 Kommandozeile und Expressions
==================================

#. Starte deine Kommandozeile und tippe "scala" ein

::

  $ scala
  scala>
  
Es ist nun möglich einfache *Ausdrücke* oder *Expressions* direkt einzutippen und "Enter" zu drücken.

Diese Ausdrücke werden direkt vom Scala-Interpreter ausgeführt.

Hier einige Beispiele zum Selberausprobieren:

::

  scala> 2 + 2
  res0: Int = 4
  
  scala> res0 + 2
  res1: Int = 6
  
  scala> 20 / (3 + 7)
  res2: Int = 2
  
  scala> 2.1 + 3.45
  res3: Double = 5.550000000000001
  
  scala> 2 * 2
  res4: Int = 4
  
  scala> "Hello " + "World"
  res5: String = Hello World
  
  
Ausdrücke können z.B. mit dem *Befehl* ``println`` im Kommandozeilen-Fenster ausgegeben werden:

::

  scala> println("Hello world!")
  // Hello world!
  
  scala>println(2+3)
  // 5
  
  
  