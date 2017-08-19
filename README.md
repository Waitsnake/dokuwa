dokuwa
======

Files
-----
- dokuwa.txt = Original dokuwa export of Dominik Klein from 2013
- dokuwa_examples.txt = Original dokuwa example export of Dominik Klein from 2013
- dokuwa.csv = dokuwa.txt convertet to CSV format (using VIM replacing: "/" to "," / "}" to ")" / "{" to " (" ) 
- AppleDictionary/dokuwa.dictionary.zip = zipped Apple dictionary file (createt with pyglossary from CSV file)

HowTo create Apple dictionary from CSV
--------------------------------------
- Download pyglossary form here: https://github.com/ilius/pyglossary/archive/master.zip
- Install all extra files for creating Apple dictionary and Mac OSX according to https://github.com/ilius/pyglossary/blob/master/README.md
- Open a terminal and type: "python3 pyglossary-master/pyglossary.pyw --read-options=resPath=OtherResources --write-format=AppleDict dokuwa.csv dokuwa"
- "cd dokuwa" and "make" will create the file "dokuwa.dictionary"