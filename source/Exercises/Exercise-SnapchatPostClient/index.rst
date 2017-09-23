Exercise: "SnapchatPostClient"
==============================

Es soll ein Programm geschrieben werden, dass aus einer Textdatei mehrere Snapchat-Posts automatisch auflisten und posten kann.

Die externe Textdatei, die die Snapchat-Posts enthält ist wie folgt aufgebaut: ``DATUM %%% TEXT %%% BILD_NAME``

Eine solche ``posts.txt`` Datei könnte wie folgt aussehen:

:: 

  12.07.2017 %%% Mein neues Zuhause %%% zuhause.jpg
  13.07.2017 %%% Yeah endlich Ferien %%% ferien.jpg
  14.07.2017 %%% Unsere neue Katze jault %%% katze-jaulen.jpg
  
**Aufgabe**

Schreibe nun ein Programm, das die Posts einliest und ausgeben kann.

Erweitere dein Programm dann wie folgt:

* Implementiere eine Funktion, die überprüft, ob ein Post keine bösen Wörter enthält, z.B. Posts die Texte haben mit *blöd*, *fuck*, etc. würden nicht ausgegeben resp. behandelt
* Erweitere die Ausgabe so, dass du die Anzahl Posts in der Datei ausgeben kannst
* Implementiere eine Funktion, die dir nur die Bilder ausgibt