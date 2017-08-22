dokuwa
======

Files
-----
- dokuwa.txt = Original dokuwa export of Dominik Klein from 2013
- dokuwa_examples.txt = Original dokuwa example export of Dominik Klein from 2013
- dokuwa.csv = dokuwa.txt convertet to CSV format (using VIM replacing: "/" to "," / "}" to ")" / "{" to " (" ) 
- AppleDictionary/dokuwa.dictionary.zip = zipped Apple dictionary file (createt with pyglossary from CSV file)


How I create the CSV from TXT in VIM
------------------------------------
1,$s/,/;/g
1,$s/\(^[A-Z|a-z|ä|ü|ö|Ä|Ü|Ö|á|é|ß|\-|.|!| ]*\)/\1,/g
1,$s/{/(/g
1,$s/}/)/g
1,$s/\// /g


HowTo create Apple dictionary from CSV
--------------------------------------
- Download pyglossary form here: https://github.com/ilius/pyglossary/archive/master.zip
- Install all extra files for creating Apple dictionary and Mac OSX according to https://github.com/ilius/pyglossary/blob/master/README.md
- Open a terminal and type: "python3 pyglossary-master/pyglossary.pyw --read-options=resPath=OtherResources --write-format=AppleDict dokuwa.csv dokuwa"
- "cd dokuwa" and "make" will create the file "dokuwa.dictionary"

Copyright
---------
Die Inhalte auf dokuwajiten.de stehen unter zwei Lizenzen. Ein Teil der ursprünglichen von wadoku.de lizensierten Daten steht unter

1.) der wadoku.de Lizenz

Neueinträge sowie Editierungen nach der Konvertierung von wadoku.de in die Richtung Deutsch-Japanisch stehen unter

2.) Der CC-BY-SA 3.0 Deutschland Lizenz

Die Daten auf dokuwajiten.de dürfen unter Einhaltung der Lizenzbestimmungen verwendet werden.

Namensnennungs-Klausel der CC-BY-SA 3.0 Deutschland

Die Erfüllung der Namensnennung-Klausel der CC-BY-SA 3.0 Deutschland kann hierbei auf eine der folgenden Arten eingehalten werden:

Durch einen Hyperlink auf www.dokuwajiten.de

durch Hyperlink (sofern möglich) oder URL auf eine andere, stabile Online-Kopie, die frei zugänglich ist, die Lizenz erfüllt und die die Namensnennung der Autoren auf eine Weise gewährleistet, die gleichwertig zu der auf den Projekt-Webseiten ist, oder

durch Verwendung des folgenden Textbausteins:

Verwendet das Deutsch-Japanische Wörterbuch DokuWa, erreichbar unter www.dokuwajiten.de

Im Falle einer Migration der Seite www.dokuwajiten.de auf eine neue URL sind obige Links durch die neue URL zu ersetzen.