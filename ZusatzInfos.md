# UML in der Softwareentwicklung

### Hinführung

==TODO==
Probleme bei der Entwicklung von Software und Systemen

### Was ist UML?

Ihre Anfänge hat die Sprache in den 1990er und wurde von den „drei Amigos“ **Grady Booch**, **Ivar Jacobson** und **James Rumbaugh** entwickelt, als Reaktion auf die vielen Vorschläge für Modellierungssprachen und -Methoden, welche das OOP unterstützen sollten. Die gemeinsame Idee für UML entstand bei der Arbeit (Rational Software) als man die verschiedenen Notationssysteme strukturiert zusammenführen wollte.
Einige andere Modellierungssprachen hatten einen direkten/indirekten Einfluss auf die Entstehung von UML (_OOSE, RDD, OMT, OBA, OODA, SOMA, MOSES und OPEN/OML_)

---

**Use Case Diagramm**
Zeigt das externe Verhalten eines Elements aus der Sicht der Nutzer, indem es die Nutzer (Aktuere) die Use-Cases und deren Beziehung darstellt.

dazu müssten die dahinterstehenden Abläufe genauer beschrieben werden mit Hilfe von einfachen Texten bis verschiedenen Diagrammen der UML

Elemente können:

- Systeme o. Subsysteme
- Klassen
- Schnittstellen
- Komponente
- Knoten

sein.

**Notation**

_Use-Case_

- (Datei Speicher -> umfasst alle nötigen Aktionen, die dazu nötig sind, eine Datei zu speichern)
- (Sicht: „Film ausleihen“, System: „Film verleihen“)
- Akteur sieht nur das Ergebnis, nicht die Aktionen dahinter
- Kommt zur „Ruhe“, wenn keine Kommunikation mehr mit dem Akteur zustande kommt
- Dürfen mit anderen Use-Cases in einer Beziehung zueinander stehen

_Akteur_

- Interagiert mit dem System über eine Assoziation

_include-Beziehung_

- Wenn A B inkludiert, darf B nich A inkludieren

[Beispiel] Kundendaten Use-Cases sehen nur das Ergebnis von Berechtigung prüfen

_Assoziation_

- Kann Informationen halten, wie oft damit interagiert werden kann

---

Klassendiagramm

± Methode(Parameterliste) : Rückgabewert

### UML in der Softwareentwicklung

Legt schon am Anfang übersichtlich fest, was zum System (Element) gehört und was nicht. Was man entwickelt (Kosten) und welche Schnittstellen man gerecht werden muss (Anforderung).
Hilft also zum planen eines neuen Systems oder Erweiterung eines bereits bestehenden.

---

https://www.lucidchart.com/pages/de/was-ist-ein-uml-diagramm
https://de.wikipedia.org/wiki/Unified_Modeling_Language
https://www.lucidchart.com/pages/de/was-ist-ein-uml-diagramm
https://de.ryte.com/wiki/Unified_Modeling_Language
http://www.codeadventurer.de/?p=2428

Rupp, Chris (2008), UML 2 glasklar, 3. Auflage, München
