opal-examples
=============

Eine Sammlung von kommentierten Beispielquelltexten für die an der TU Berlin entwickelten und im Kurs MPGI1 verwendeten funktionalen Programmiersprache OPAL.

A collection of code examples for the functional programming language OPAL created and used at the Technical University of Berlin. - Since this project mainly targets a german-speaking audience all comments and also function names in the examples are in German.

Die Beispiele können direkt im Repository per HTTP gebrowsed oder per Git gecloned werden.

Die einzelnen Strukturen entsprechen ungefähr immer einem zusammenfassbaren Thema. Einige Beispiele (wie Medienliste) kombinieren verschiedene Aspekte.

Es wird davon ausgegangen, dass die Beispiele immer im Kontext der .impl-Datei ausgeführt werden (siehe Beispielaufruf in Funktionen.impl). Die .sign-Dateien sind daher meistens leer oder nur so minimal wie für die Beispiele nötig befüllt.

Beispielstrukturen
------------------

* Funktionen (TODO: Overloading Beispiel)
* Bedingungen
* LetInWhere
* Rekursion
* HOF (TODO: Currying)
* Medium (Datenstrukturen)
* Listen
* Listenfunktionale (TODO)
* Sortieren (Insertionsort, Selectionsort, Quicksort, Mergesort, Listenfunktionale filter und reduce)
* PatternMatching (TODO)
* Fehlerbehandlung (Behandlung von Fehlerfällen mit "Option"-Datentyp)
* Medienliste (Zusammenfassung verschiedener Themen: Datenstrukturen, Listen, Rekursion, Listenfunktionale)
* Baum (Suchbaum, AVL-Baum)
* Plotter (Spielerei - Funktionen als ASCII-Darstellung im Terminal plotten)

OPAL-Installation auf Ubuntu
----------------------------

Die offizielle Installationsanleitung für OPAL gibt es hier: http://projects.uebb.tu-berlin.de/opal/trac/wiki/InstallationGerman

Hier eine Kurzfassung, für die Kompilierung/Installation unter Ubuntu:

System updaten und benötigte Pakete installieren:

	sudo apt-get update
	sudo apt-get upgrade
	sudo apt-get dist-upgrade
	sudo apt-get install flex libreadline-gplv2-dev tcl8.5-dev libx11-dev tk8.5-dev

Paket herunterladen und entpacken:

	cd
	wget https://projects.uebb.tu-berlin.de/opal/trac/raw-attachment/wiki/OCS/ocs-2.4b.tar.gz
	tar -zxvf ocs-2.4b.tar.gz
	cd ocs-2.4b

Kompilieren:

	./configure --prefix=/home/ubuntu/ocs
	make install

Der Prefix kann weggelassen und sudo make install benutzt werden, wenn es global installiert werden soll. Statt "ubuntu" müsste der Username angegeben werden.

Beispiele mittels Git herunterladen und ausprobieren:

	cd
	sudo apt-get install git
	git clone https://github.com/stefanschramm/opal-examples.git
	cd opal-examples
	~/ocs/bin/oasys
	a Funktionen
	f Funktionen.impl
	e ersterTest(3,5)

Links
-----

* OPAL-Projektseite: http://projects.uebb.tu-berlin.de/opal/trac
* Bibliotheca Opalica: https://projects.uebb.tu-berlin.de/opal/dosfop/2.4/bibopalicaman/
* Freitagsrunde zu OPAL mit FAQ und Installationshinweisen: https://wiki.freitagsrunde.org/Opal


Korrektur- und Erweiterungsvorschläge zur Beispielsammlung bitte gerne an: mail AT stefanschramm PUNKT net. 


Die aktuelle Fassung dieser Sammlung findet sich im Repository auf: https://github.com/stefanschramm/opal-examples

