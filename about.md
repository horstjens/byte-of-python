# Appendix: Colophon {#colophon}

Falst alle Software die zur Erstellung dieses Buches verwendet wurde ist free/libre open source Software [FLOSS](./floss.md#floss).

## Die Geburt dieses Buches

Beim ersten Entwurf dieses Buchs verwendete ich Red Hat 9.0 Linux. In der 6. Revision des Buchs verwende ich Fedora Core 3 Linux.

Anfangs schrieb ich das Buch mit der Textverarbeitung KWord (siehe [history lesson](./revision_history.md#history-lesson)).

## Die Teenager Jahre des Buches

Später wechselte ich zu DocBook XML und dem Texteditor Kate aber fand dies ermüdend. Deshalb wechselte ich zu OpenOffice. OpenOffice war excellent für Formatierung und PDF-Erzeugung, aber das damit generierte HTML war schlampig.

Schlussendlich endeckte ich XEmacs für mich und schrieb das ganze Buch nochmal von vorne in DocBook XML nachdem ich entschieden hatte das dieses Format für mich langfristig passt.

In der 6. Revision entschied ich mich für dafür, Quanta+ als Editor zu verwenden. Ich benutzte die Standard XSL-Stylesheets welche mit Fedora Core 3 Linux installiert wurden. Allerdings hatte ich ein CSS Dokument geschreiben um Farbe und Style meiner HTML-Seiten zu ändern. Ich hatte auch einen primitven lexical Analyzer geschrieben (natürlich in Python), um automatisch Syntax Highlighting für alle Code-Blöcke zu erzeugen.

In der 7. Revision verwendete ich I was using [MediaWiki](http://www.mediawiki.org) als Basis. Ich editierte alles online und meine Leser konnten direkt im Wiki lesen / ändern / disskutieren. Das Resultat war daß ich mehr Zeit damit verbrachte Spam zu löschen als am Buch zu schreiben.

In der 8. Revision verwendete ich den Texteditor [Vim]({{ book.vimBookUrl }}), sowie zum konvertieren [Pandoc](http://johnmacfarlane.net/pandoc/README.html), als Betriebssystem Mac OS X.

In der 9. Revision wechselte ich zu [AsciiDoc format](http://asciidoctor.org/docs/what-is-asciidoc/) and schrieb mit [Emacs 24.3](http://www.masteringemacs.org/articles/2013/03/11/whats-new-emacs-24-3/),
[tomorrow theme](https://github.com/chriskempson/tomorrow-theme),
[Fira Mono font](https://www.mozilla.org/en-US/styleguide/products/firefox-os/typeface/#download-primary) und [adoc-mode](https://github.com/sensorflo/adoc-mode/wiki).

## Gegenwart

2016: Ich hatte genug von mehreren kleinen Render-Problemen mit AsciiDoctor (z.B. verschwand das `++` in `C/C++` wenn ich nicht aufpasste). Außerdem war das Asciidoc format so komplex daß ich immer weniger Lust hatte Text zu editieren.

Für die 10. Revision wechselte ich zu Markdown und [GitBook](https://www.gitbook.com) und schrieb mit dem [Spacemacs editor](http://spacemacs.org).

Nov 2020: Gitbook ist nicht miehr open source software, deshalb wechselte ich zu [Honkit](https://github.com/honkit/honkit), einem Open-Source fork von Gitbook.

## Über den Autor

Siehe {{ book.authorUrl }}
