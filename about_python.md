# über Python

Python ist eine dieser seltenen Programmiersprachen die sowohl _einfach_ als auch _mächtig_ sind. Wenn Sie mit Python arbeiten werden Sie angenehm überrascht sein davon wie einfach es ist sich bloß auf das Programmierproblem konzentrieren zu müssen anstatt auf die Programmiersprache. 

Die offizielle Einführung in Python lautet:

> Python ist eine einfach zu erlerndende, mächtige Programmiersprache. Sie hat effiziente hochrangige Datastrukturen und einen sehr einfachen aber effizienten Zugang zur objektorientierten Programmierung. Python's eleganter Syntax und "dynamic typing", zusammen mit ihrer Natur als interpretersprache, macht sie zu einer idealen Programmiersprache für Scripting und "rapid application development" in vielen Anwendungsgebieten auf den meisten Plattformen.

Ich werde diese Eigenschaften in den folgenden Absätzen im Detail erläutern. 

## Die Geschichte hinter dem Namen "Python"

Guido van Rossum, der Erfinder der Programmiersprache Python, hat die Sprache nach der BBC show "Monty Python's Flying Circus" benannt. Er ist kein besonderer Freund von Würgeschlagen. 

## Eigenschaften von Python

### Einfach

Python ist eine einfache (unkomplizierte) und minimalistische Programmiersprache. Ein Python-Programm zu lesen fühlt sich an wie (sehr striktes) Englisch. Dises "pseudo-code"-Natur von Python ist eine ihrer großen Stärken: Sie erlaubt die Konzentrations auf Problemlösungen anstatt auf die Programmiersprache.

### Einfach zu erlenen 

Wie Sie sehen werden ist es mit Python extrem einfach zu starten. Python hat, wie erwähnt, eine sehr einfache Syntax. 

### Free and Open Source

Python ist ein Beispiel für _FLOSS_ (Free/Libre and Open Source Software: freie und quelloffene Software). Einfach ausgedrückt, jeder darf Python kopieren und verteilen, jeder darf Python's "Source Code" lesen, jeder darf den "Source Code" verändern, jeder darf Teile davon in anderen freien Programmen verwenden. FLOSS basiert auf dem Konzept einer Gemeinschaft welche ihr Wissen teilt. Das ist einer der Gründe warum Python so gut ist - es wurde erschaffen und wird ständig verbessert von einer Gemeinschaft welche ein besseres Python Python haben will. 

### höhere Programmiersprache

Wer in Python programmiert braucht sich nicht um low-level Details wie Memory-Management etc. kümmern. 

### Portierbar

Durch die Open-Source Natur von Python wurde es auf zahlreiche Betriebsystemen portiert (so verändert das es überall läuft). Alle Python Programme laufen auf allen Betriebsystemen ohne daß man etwas ändern muss wenn man sorgfältig programmiert und auf Betriebsystem-spezifische Befehle verzichtet. 

Python läuft auf  GNU/Linux, Windows, FreeBSD, Macintosh, Solaris, OS/2, Amiga, AROS, AS/400, BeOS, OS/390, z/OS, Palm OS, QNX, VMS, Psion, Acorn RISC OS, VxWorks, PlayStation, Sharp Zaurus, Windows CE und auf PocketPC!

Sie können sogar Python-Module wie [Kivy](http://kivy.org) verwenden um Apps oder Spiele zu erschaffen die auf Ihrem Computer _und_ auf iPhone, iPad und auf Android Geräten laufen.

### Interpretiert

Dies bedarf einer Erklärung:

Man unterscheidet zwischen 'compiled' und 'interpreted' Programmiersprachen. Compiled Programme (zb. C, C\++, Java) werden vom 'Source Code' (Quellcode) in eine dem Computer verständliche Maschinensprache (Binary Code, im Prinzip lauter Nullen und Eineser) übersetzt von einem Compiler. Dieses kompilierte Programm wird dann von einem Linker/Loader von der Festplatte in den Arbeitsspeicher gelanden und gestartet. 

Im Unterschied dazu benötigen Interpretierte Programmiersprachen (wie z.B. Python, JavaScript etc) keinen Compiler, man kann das Programm direkt vom Source-Code starten. Intern konvertiert Python den Source Code in ein Zwischenform ('ByteCode' genannt) welche dann in Maschinencode übersetzt wird. 

Python vereinfact das Programmieren dadurch daß man keinen Complier braucht und durch seine gute Portierbarkeit - Python Programme laufen auf fast jedem Betriebssystem!

### Objekt-orientiert 

Python unterstützt sowohl prozedurales Programmieren als auch objekt-orientiertes Programmieren ('OOP - object oriented programming'). In _prozeduralen_ Programmiersprachen dreht sich alles um wiederverwertbare Code-Teile: Prozeduren und Funktionen. In _objekt-orientierten_ Programmiersprachen liegt der Fokus auf Objekten welche Daten und Funktionalität verbinden. 

Python hat einen sehr mächtigen aber einfachen Zugang zu OOP, speziell im Vergleich zu anderen Programmiersprachen wie C++ oder Java.

Python supports procedure-oriented programming as well as object-oriented programming (OOP). In _procedure-oriented_ languages, the program is built around procedures or functions which are nothing but reusable pieces of programs. In _object-oriented_ languages, the program is built around objects which combine data and functionality. Python has a very powerful but simplistic way of doing OOP, especially when compared to big languages like C\++ or Java.

### Erweiterbar

Python ist erweiterbar - Soll ein Teil ihres Python-Codes z.B. sehr schnell sein oder für andere nicht lesbar, dann können Sie diesen Programmteil in einer anderen Programmiersprache wie z.B. C oder C\++ schreiben und von ihrem Python-Programm aus aufrufen.

### Einbettbar (Embeddable)

Wenn Sie Programme mit einer anderen Programmiersprache wie z.B. C oder C\++ schreiben können Sie Python in ihr Programm inkludieren (einbetten). Dies gibt den Benutzern ihres Programms die Möglichkeit, kleine Python-Programme (sogenannte Skripte) zu schreiben um z.B. Arbeitsvorgänge innerhalb ihres Programms zu automatisieren. 

### große Bibliothek

Die 'Python Standard Library' ist wirklich groß und besteht aus vielen Modulen. Sie hilft bei unterschiedlichsten Programmierthemen, wie z.B. regex (Regular Expressions),  Domkumentationsgenerierung, Threading, Datenbanken, webbrowser, CGI, FTP, Email, XML, XML-RPC, HTML, Sounddateien, Kryptographie, grafische Benutzeroberflächen (GUI) und vielem mehr. All diese Module werden mit Python mitinstalliert und sind überall verfügbar wo Python installiert ist. '_Batteries Included_' (Batterien sind schon dabei) ist das Motto von Python.

Neben der Python Standard Library gibt es noch unzählige andere hochwertige Bibliotheken welche man im [Python Package Index](http://pypi.python.org/pypi) finden kann.

### Zusammenfassung

Python ist eine eine wahrhaft aufregende und mächtige Programmiersprache. Python hat die richtige Kombination von Performanz (Geschwindigkeit) und Features und das weshalb Programmieren mit Python sehr einfach ist und viel Spaß macht.

## Python Version 3 versus Version 2

Sie können diesen Absatz getrost ignorieren wenn Sie sich nicht für die Unterschiede zwischen Python2 und Python3 interessieren. Merken Sie sich nur mit welcher von beiden Versionen Sie arbeiten. Dieses Buch ist für Python Version 3 geschreiben. 

Für Details zu den Unterschieden zwischen Python Version 2 und Python Version 3, siehe folgende Links:

- [The future of Python 2](http://lwn.net/Articles/547191/)
- [Porting Python 2 Code to Python 3](https://docs.python.org/3/howto/pyporting.html)
- [Writing code that runs under both Python2 and 3](https://wiki.python.org/moin/PortingToPy3k/BilingualQuickRef)
- [Supporting Python 3: An in-depth guide](http://python3porting.com)

## Was Programmierer sagen

Falls es Sie interessiert was großartige Hacker wie Erci S. Raymond über Python zu sagen haben:

- _Eric S. Raymond_ ist der Autor von "The Cathedral and the Bazaar" (Die Kathedrale und der Bazaar) und hat den Begriff  _Open Source_ (quelloffen) populär gemacht. Er sagt das [Python seine Lieblings-Programmiersprache ist](http://www.python.org/about/success/esr/). Sein Artikel war die Inspiration für meinen ersten Kontakt mit Python.

- _Bruce Eckel_ ist der Autor von berühmten Büchern wie 'Thinking in Java' und 'Thinking in C++'. Er sagt das ihn keine andere Programmiersprache so produktiv macht wie Python. Er sagt außerdem das Python möglicherweise die einzige Programmiersprache ist welche sich darauf fokusiert Dinge für die Programmierer einfacher zu machen. Siehe sein [Interview](http://www.artima.com/intv/aboutme.html) für mehr Details.

- _Peter Norvig_ ist ein bekannter Lisp Autor und der Direktor von "Search Quality" bei Google (Vielen Dank an dieser Stelle an Guido van Rossum für diesen Hinweis). Er sagt das [Programmieren in Python ist wie das Schreiben von Pseudocode](https://news.ycombinator.com/item?id=1803815). Er sagt auch  Python war immer ein integraler Bestandteil von Google. Sie können dies verifizieren durch einen Blick auf die [Google Jobs](http://www.google.com/jobs/index.html) Website welche Python-Kenntnisse voraussetzt für Software engineers bei Google. 
