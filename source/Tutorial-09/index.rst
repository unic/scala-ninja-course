T-09 String Operationen
=======================

Variablen oder Werte mit dem ``String`` Typ bieten verschiedene Funktionen an um z.B. String-Werte zu vergleichen, zu suchen, zuzuschneiden und mehr.

Mittels *String Interpolation* ist es auch möglich andere Variable in Strings einzubetten:

::

  val n = 12
  val anzahl = s"Ich habe $n Paar Schuhe"
  

Mit Hilfe der ``contains`` Methode kannst du überprüfen, ob einen gesuchten Text enthalten ist:

:: 

  val myPosts = "Hello World, you enter the powerful world of nature"
  myPosts.contains("nature") // Ergibt den Boolean Wert "true", also wahr
  

Wenn du zwei Strings auf Gleichheit überprüfen möchtest, dann kannst du ``equals`` benutzen:

::

  val name1 = "Hans"
  val name2 = "Hans"
  name1.equals(name2) // Ergibt "true", da der Name gleich ist
  

Mit ``equalsIgnoreCase`` kannst du auch auf Gleichheit überprüfen mit dem Unterschied, dass Gross-Klein-Schreibung nicht beachtet wird.

::

  val name1 = "Hans"
  val name2 = "hans"
  name1.equals(name2) // Ergibt "false", da der Name zwar gleich ist, aber ein Name ist mit Kleinbuchstaben geschrieben
  name1.equalsIgnoreCase(name2) // Ergibt aber nun "true", da Gross-/Kleinschreibung nicht beachtet wird
  

Wenn du bestimmte Text-Vorkommnisse in einem String mit einem anderen Text ersetzen möchtest, kannst du ``replace`` benutzen:

:: 

  val myStory = "Das Wandern in den Bergen ist wunderschön"
  val neueStory = myStory.replace("Bergen", "Wäldern") 
  // Würde den Text "Das Wandern in den Wäldern ist wunderschön" erzeugen
  
Wenn du einen Text mit einem bestimmten Zeichen aufsplitten möchtest, dann kannst du ``split`` benutzen:

::

  val meinText = "Foo&Bla&Doo"
  meinText.split("&").foreach(x => println(x))
  

