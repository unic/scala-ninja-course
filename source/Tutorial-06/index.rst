T-06 Bedingungen - Entscheidungen treffen
=========================================

Der ``if..then..else..`` Befehl hilft dir im Programm Entscheidungen zu treffen.

Beispiel:

::

  val n = 10
  val t = 23
  if (t > n) {
    println("t ist grösser")
  } else {
    println("t ist kleiner")
  }
  

Da ``t`` grösser ist als ``n`` wird auch ``t ist grösser`` im Bildschirm ausgegeben.

Wenn du jetzt z.B. ``t = 8`` schreibst, dann kriegst du die Meldung ``t ist kleiner``.

Man kann ein ``if`` Befehl auch kurz auf einer Zeile schreiben:

::

  if (10 > 1) println("yes grösser")
  if (10 > 11) println("yes grösser") else println("nope kleiner")
  
Aber meistens wird die längere Schreibweise oben mit den geschweiften Klammern bevorzugt, weil diese meist leserlicher ist.

Du kannst auch Bedingungen mit *Und* (mit doppeltem Ampersand-Zeichen) oder *Oder* (mit doppeltem Hochstrich) verknüpfen:

Beispiel mit Und-Verknüpfung:

::

  if (t > n && t > 1000) {
    // TODO code...
  }
  
  
Beispiel mit Oder-Verknüpfung:

::

  if (t > n || t > 1000) {
    // TODO code...
  }

  