T-10 Dateien lesen
==================

In Scala kann man mit der ``scala.io.Source`` Klasse einfach Text-Dateien lesen.

Beispiel:

:: 

  val myFile = Source.fromFile("C:\DEIN_PFAD\example.txt")
  for (line <- myFile.getLines) {
    println(line.toUpperCase)
  }

  myFile.close

Hierfür erstellst du irgendwo auf deinem Computer eine *example.txt* Datei und gibst deinen Pfad oben an.

Wenn du z.B. Zeilen mit bestimmten Texten entfernen willst, kannst du das z.B. mit *filter* machen, wie du bereits im Tutorial-08 gelernt hast:

:: 

  val meineZeilen = myFile.getLines().filter(a => a.equals("MeinText"))
  
  for (zeile <- meineZeilen) {
    println(zeile)
  }


