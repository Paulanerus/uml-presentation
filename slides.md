---
theme: academic
coverAuthor: Paul Fröhlich
coverDate: 1/6/2022
themeConfig:
  paginationX: r
  paginationY: b
  paginationPagesDisabled: [1, 2, 16]
---

# UML in der Softwareentwicklung

---

# Gliederung

- Was ist UML?
- Diagrammtypen
  - Use-Case
  - Klassendiagramm
- UML in der Softwareentwicklung

---

# Probleme bei der Entwicklung von Software und Systemen

<img width="500" src="/images/group.jpg" alt="group">

---

# Was ist UML?

**UML** steht für **U**nified **M**odeling **L**anguage und ist eine grafische Modellierungssprache für:
<div class="pl-4 -mt-4">

- Architektur
- Design
- Implementierung von komplexen Softwaresystemen
</div>

Verschidene Typen um verschiedene Aspekte eines Systems zu visualisieren oder analysieren.

Wurde an die OMG (Object Management Group) übergeben, welche diese am 19. November 1997 als Standard akzeptierte.

---

# Diagrammtypen

13 Diagrammtypen die in 2 Obergruppen aufgeteilt werden:

- Verhaltensdiagramme
- Strukturdiagramme

---

# Use-Case Diagramm

- hilft zur Analyse eines Systems
- keine vollständige beschreibung des Systems

**Notation:**

_Use-Case_

<div class="columns-2">
  <div class="pl-4 -mt-4">
  
  - Menge von Aktionen die schrittweise ausgeführt werden
  - wird von einem Akteur ausgelöst und gesehen
  - darf gleichzeitig mehrfach ausgelöst werden
  </div>
  <img src="/images/use-case.jpg" alt="use-case">
</div>

---

# Use-Case Diagramm - Notation

_System (Betrachtungsgegenstand)_

<div class="columns-2">
  <div class="pl-4 -mt-4">
  
  - umfasst alle Use-Cases
  - kann geschachtelt werden
  </div>

  <img width="350" src="/images/system.jpg" alt="system">
</div>

_Akteur_

<div class="columns-2">
  <div class="pl-4 -mt-4">

- ist außerhalb des Systems
- kann erben
- Muss keine Person sein, kann auch Sensor, Zeitergebnis oder ein anderes Gerät sein
</div>

  <img width="150" src="/images/act.jpg" alt="act">
</div>

---

# Use-Case Diagramm - Notation

_<\<include>>-Beziehung_

<div class="columns-2">
  <div class="pl-4 -mt-4">
  
  - visualisiert, dass ein Use-Case das Verhalten eines anderen importiert
  - Darf mehrfach importiert werden, nicht sich selbst
  </div>

  <img src="/images/include.jpg" alt="include">
</div>

_<\<extend>>-Beziehung_

<div class="columns-2">
  <div class="pl-4 -mt-4">

- visualisiert, dass das Verhalten eines Use-Cases durch einen anderen erweitert werden kann, aber nicht muss
</div>

  <img src="/images/extend.jpg" alt="extend">
</div>

---

# Use-Case Diagramm - Notation

_<\<extend>>-Beziehung Zusatz_
  <div class="pl-4 -mt-4">

- extension point(s): Zeitpunkt der Erweiterung
- Bedingung: sind optional
</div>

<div class="columns-2">
<img src="/images/extension.jpg" alt="extension">
<img src="/images/condition.jpg" alt="condition">
</div>
---

<img src="/images/all.jpg" alt="all">

---

# Klassendiagramm

Das Klassendiagramm ist eine Darstellung um Klassen und deren Zusammenhänge zu visualisieren. <u>Keine</u> Möglichkeit Algorithmen zu modellieren

Was ist eine Klasse? -> Name, Attribute und Methoden

**Notation:**

<div class="columns-2">

<img width="260" src="/images/notation-class.png" alt="notation-class.png">

**Weitere Beschreibungsmöglichkeiten:**

<div class="pl-4 text-sm">

- <u>unterstrich</u> -> static
- \# -> protected
- {readOnly} -> final
- ± Datenstruktur : Datentyp <span class="text-amber-500">[1..n]</span> | <span class="text-purple-500">[*]</span> -> Datenstruktur mit einer <span class="text-amber-500">festen</span> Länge | <span class="text-purple-500">beliebig viele</span> Elemente
- {order} -> geordnete Datenstruktur
- {unique} -> jedes Element ist einzigartig

</div>
</div>

---

# Klassendiagramm - Beziehungen

**<\<use>>**

<div class="columns-2">
<div class="pl-4 -mt-4">

- schwache Beziehung
- wird nur so lange "benutzt", bis eine Methode agbearbeitet ist
</div>
<img src="/images/use-class.png" alt="use-class">
</div>

**Assoziation**

<div class="pl-4 -mt-4">

- einfache Verbindung
- stehen in irgendeiner Verbindung zueinander
</div>

**Vererbung**
<img width="360" src="/images/inh.png" alt="inh">

---

# Klassendiagramm - Aggregation/Komposition

**Aggregation**

<div class="text-sm">

<div class="columns-2">
<div class="pl-4 -mt-4">

- nicht ausgefüllter Diamanten an stärkeren Seite
- können beide ohne den anderen existieren
</div>
<div>
<img src="/images/aggr.png" alt="aggr-class">

```js
Person p;
EntwicklerTeam team(p);
```

</div>
</div>

**Komposition**

<div class="columns-2">
<div class="pl-4 -mt-4">

- ausgefüllter Diamanten an stärkeren Seite
- ohne instanziierende Seite existieren beide nicht
</div>
<div>
<img src="/images/komp.png" alt="aggr-class">

```js
Gewächshaus haus(PflanzenSlot);
```

</div>
</div>
</div>
---

# Weitere Diagrammtypen

<div class="text-sm">

- **Verhaltensdiagramme**

  - Use Case Diagramm
  - Aktivitätsdiagramm
  - Zustandsdiagramm
  - Sequenzdiagramm
  - Kommunikationsdiagramm
  - Timingdiagramm
  - Interaktionsübersichtdiagramm

- **Strukturdiagramme**
  - Klassendiagramm
  - Paketdiagramm
  - Objektdiagramm
  - Kompositionsstrukturdiagramm
  - Komponentendiagramm
  - Verteilungsdiagramm

</div>

---

# UML in der Softwareentwicklung

- **Wann wird es verwendet**
  - Am Anfang kann aber schnell während des Projekts erweitert werden

- **Warum wird es verwendet?**

  - Systemanalyse/ -architektur
  - Softwareanalyse/ -architektur
  - bessere Abschätzung für den Kunden (eine Art Schnittstelle)

- **Tools**
  - Papier und Stift
  - Zahlreiche online und offline Tools

---
layout: center
---

# Danke für Eure Aufmerksamkeit!
Noch Fragen?