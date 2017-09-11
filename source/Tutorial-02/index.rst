T-02 Values
===========

Ausdrücke können Werten mit einem Namen zugewiesen werden, dabei braucht man den Befehl ``val``:

::

  scala> val x = 1 + 1
  x: Int = 2
  
Diese gespeicherten Werte sind *unveränderbar* und können nicht neue Werte aufnehmen.

Diese Werte kann man anschliessend wieder im Code verwendet werden:

::

  scala>println(x)
  // 2
  
Jeder Wert kann auch explizit einen bestimmten *Typ* erhalten:

:: 

  scala> val x: Int = 1 + 1
  scala> val y: Double = 2.11 + 3.2
  scala> val name: String = "Mein Name"
  
