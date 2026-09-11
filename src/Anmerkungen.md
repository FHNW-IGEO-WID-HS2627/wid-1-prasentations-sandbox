# WID 1 - Sandbox

### Diese Datei...
...ist in Markdown (.md) geschrieben und sozusagen eine "ReadMe". Sie ist nicht Teil von HTML und auch keine "React" Projektdatei. Für Übungen und Hausaufgaben heisst sie meistens "Aufgabe.md" und enthält den Aufgabentext sowie Hinweise und Tips.


Forke immer zunächst die Aufgabe in deinen eigenen Sandbox Account, damit du eine eigene Kopie hast. In Moodle gibt es für Sandbox eine Anleitung ("Anleitung Sandbox.pdf"). 



### Tipps:
Wir werden JavaScript und "JSX" erst nächste Woche (in "WID2") kennenlernen. Bis dahin schreibe deine Code ausschliesslich in der "App.js"-Datei und innerhalb des `return` Blocks - also dort wo aktuell "Hallo Welt" steht.

Achte darauf, dass es immer genau ein (1) äusseres Eltern-Element gibt, z.B. ein `<div>` oder ein `<>  </>` ("Fragment"), andernfalls bekommst du diese Fehlermeldung:

```
Cannot assign to read only property 'message' of object 'SyntaxError: /src/App.js: Adjacent JSX elements must be wrapped in an enclosing tag. Did you want a JSX fragment <>...</>? (4:20)
```
Was bedeutet die?
- "Adjacent Elements" bedeutet, dass du mehrere Elemente auf der gleichen Hierachiestufe (d.h. ohne ein eindeutiges Elternelement) geschrieben hast.

- "Enclosing Tags" - damit ist das umgebende, und hier fehlende, Elternelement gemeint. Dieses setzt sich aus einem Start- und einem Endtag zusammen (z.B. `<div>  </div>`). Zwischen beiden kannst du beliebig weitere Elemente definieren, auch auf der gleichen Hierarchiestufe.

- "JSX Fragment" - in JSX (React Syntax) kann man auch "leere Tags" ("Fragemente") anstelle eines divs schreiben `<> </>` und als "enclosing tags" verwenden, um die Elemente zu umrahmen. Du kannst aber stattdessen auch einfach ein "div" benutzen.

Du kannst beliebig viele Kind-Elemente (und weitere Kindeskinder) hinzufügen, solange es ein umfassendes Eltern-Element gibt. Manchmal entfernt der Editor automatisch die runde Klammer im return Block (meist, wenn es darin nur eine Zeile hat.) Ggf. musst du diese wieder hinzufügen.

