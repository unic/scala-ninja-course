T-03 Variablen
==============

Variablen sind veränderbar und können im Gegensatz zu *Values/Werten* neue Werte annehmen.

D.h. es können neue Werte einer entsprechenden Variablen zugewiesen werden.

Beispiel:

:: 

   scala> var y = 1 + 1
   scala> y = 3
   scala> println(y * y) // 9

Beim obigen Beispiel sehen wir, dass die Variable *x* von 2 auf die Zahl 3 verändert wird.
Dies ist möglich für Variablen.

Schauen wir uns ein Beispiel an mit dem Befehl *val*:

::

   scala> val z = 1 + 1
   scala> z = 3

Nach dem Ausführen der letzten Zeile, wird folgende Fehlermeldung von Scala ausgegeben:

::
   error: reassignment to val


Auch bei Variablen kann man den Typ explizit definieren wenn nötig:

:: 

   var x: Int = 1 + 1