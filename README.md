# Containervirtualisierung und Orchestrierung
Mein Bericht für das erste und zweite Semester.

## Bauen der PDF

Zum Erstellen des Berichts habe ich unter Windows 

- [Texmaker](https://www.xm1math.net/texmaker/) als Editor
- [MiKTeX LaTeX](https://miktex.org/) als LaTeX Implementierung 
- [Perl](https://strawberryperl.com/) zum bauen des Glossars

benutzt.


Zum Bauen mit Texmaker, kann folgender Befehl bei _Schnell Übersetzen_ verwendet werden:  
```
pdflatex -synctex=1 -interaction=nonstopmode %.tex|biber %|pdflatex -synctex=1 -interaction=nonstopmode %.tex|makeglossaries %.glo|pdflatex -synctex=1 -interaction=nonstopmode %.tex|pdflatex -synctex=1 -interaction=nonstopmode %.tex|"C:/Program Files (x86)/Adobe/Acrobat Reader DC/Reader/AcroRd32.exe" %.pdf
```
