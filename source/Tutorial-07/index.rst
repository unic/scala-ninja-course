T-07 Schleifen - Befehle mehrmals auführen
==========================================

Schleifen oder *Loops* in Englisch, sind Programmier-Befehle, die dir erlauben, andere Befehle mehrmals auszuführen.

Zum Beispiel: Du möchtest alle Zahlen von 1 bis 10 ausgeben:

:: 

  for ( a <- 1 to 10) {
    println("Zahl: " + a)
  }
  

Eine andere Art Schleifen zu programmieren ist mit dem ``while`` Befehl. Dabei läuft die Schleife solange bis eine definierte Bedingung wahr ist.

Das gleiche Beispiel mit den Zahlen 1 bis 10 als ``while`` Schleife:

:: 

  var a = 1
  while (a <= 10) {
    println(a)
    a += 1
  }
  
