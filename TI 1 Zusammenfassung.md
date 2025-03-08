# Logik und Beweistechniken 1
Die Logik befasst sich mit eindeutigen Eigenschaften von Objekten und deren Zusammenhängen. Damit ist sie eine universelle Wissenschaft, die sowohl auf natürliche Zusammenhänge als auch für rein theoretische Überlegungen angewendet werden kann.
- Technischen Informatik: Schaltungen und zentralen Ausführungseinheiten
- Softwareentwicklung beschreibt Programmausführung durch logische Ausdrücke
- Abstrakte Aussagen können ebenso nur mit korrekter Logik bewiesen werden
- Theoretische Algorithmen werden durch logische Ausdrücke erst
Wichtig: Übersetzung von menschlicher Sprache in die Logik und umgekehrt, sowohl um Informationen verarbeiten zu können, als sie auch verständlich machen zu können.

## Definitionen
**Aussage**: Ein feststellender Satz, mit der Eigenschaft, eindeutig wahr oder falsch zu sein, unabhängig davon, ob die Einstufung in dem Moment erfolgen kann.
**Junktor**: Logischer Operator, der eine oder mehrere Aussagen miteinander verknüpft, um komplexere Aussagen zu bilden (z. B. $⊤$, $⊥$, $¬A$, $∧$, $∨$, $↔$...)
**Zusammengesetzte Aussagen**: Können äquivalent in zwei mit einem Junktor verbundene Aussagen zerlegt werden.
**Elementare Aussagen**: Können nicht sinnvoll weiter zerlegt werden.
**Logische Negation**: Die Negation einer Aussage wird als die Verneinung dieser Aussage definiert.
**Dualität der Aussagenlogik**: Eine Aussagenäquivalenz der Aussagenlogik bleibt korrekt, wenn alle Konjunktionen und Disjunktionen sowie Tautologie und Kontradiktion zur dualen Äquivalenz vertauscht werden.
**Beweis**: Eine formale Argumentationskette, die von angenommenen wahren Prämissen ausgeht und durch logische Ableitungsregeln zu einer Konklusionen führt, die die Wahrheit einer Aussage demonstriert.
**Kalkül (Rechnung)**: In einem Kalkül oder logischem System werden logische Axiome, das sind grundlegende und nicht bewiesene Aussagen, vorausgesetzt.
**Präpositionen (Verhältnis)**: Präpositionen sind eine Menge von Aussagen, die Voraussetzungen, die zusammen mit den Aussagen des Kalküls nachvollziehbar verwendet werden können.
**Konklusionen (Schlussfolgerung)**: Logische Schlüsse bestehen aus Präpositionen, um die gewünschte Konklusion zu belegen.
**Prädikate**: Ein Prädikat P ist eine Funktion einer logischen Aussage $P(x)$ oder $P(x_1, ..., x_n)$, dessen Subjekt x oder Subjekte $x_1, ..., x_n$ variabel sind.
**Quantoren**: Quantoren sind Operatoren für Prädikate, die den Umfang einer Aussage über die Elemente eines bestimmten Bereichs spezifizieren (z. B. $∀$, $∃$...)

## Symbole
**Tautologie (wahr)**: $⊤$
**Kontradiktion (falsch)**: $⊥$
**Negation (Verneinung)**: $¬A$ oder $Ā$
**Konjunktion (logische Und)**: $∧$
**Disjunktion (logische Oder)**: $∨$
**Äquivalenz (Gleichwertigkeit)**:
	**$↔$ (Logische Äquivalenz)**: Zwei logische Ausdrücke haben denselben Wahrheitswert (für Wahrheitstabellen und Aussagenlogik)
	**$⇔$ (Logische oder metalogische Äquivalenz)**: Logik: $⇔$ und $↔$ sind austauschbar. Metalogik: $⇔$ zeigt die Herleitung einer Äquivalenz oder die Gleichwertigkeit von logischen Systemen oder Theorien (hauptsächlich für Beweise)
	**$=$ (Mathematische oder logische Gleichheit)**: Mathematik: Drückt aus, dass zwei Objekte (Zahlen, Variablen, Mengen etc.) identisch oder gleichwertig sind; Logik: Kann gleiche Wahrheitswerte darstellen, verwende aber lieber $↔$ oder $⇔$
	**$:=$ ("wird definiert als" oder "ist gleich per Definition")**
**Implikation (Zusammenhang)**:
	**$→$ (Logische Implikation)**: Eine Aussage folgt aus einer anderen (Teil des Objektbereichs, also formalen Struktur einer Aussage oder eines logischen Systems) Bsp.: $P(x) → Q(x)$
	**$⇒$ (Metalogische Implikation)**: Beschreibt eine Beziehung zwischen Aussagen durch Aussagen (für Beweistheorie oder formalen Argumenten) Bsp.: $∃x : ∀y : P(x, y) ⇒ ∀y : ∃x : P(x, y)$
**Allquantor / Universeller Quantor($B(x)$ gilt für alle Parameter $x$ bzw. $A(x)$)**: $∀x: B(x)$ oder $∀A(x) : B(x)$
**Existenzquantor (Es gibt mindestens ein Parameter $x$ bzw. $A(x)$, sodass $B(x)$ gilt)**: $∃x : B(x)$ oder $∃A(x) : B(x)$
**Element von (Objekt ist Mitglied einer Menge)**: $∈$
**Kein Element von (Objekt ist nicht in einer Menge enthalten)**: $∉$

## Bedeutung von Wörtern
| Mögliche Sätze                                                                                      | Bedeutung |
|-----------------------------------------------------------------------------------------------------|-----------|
| A und B                                                                                             | A ∧ B     |
| A oder B                                                                                            | A ∨ B     |
| Nicht A; Die Aussage A ist falsch                                                                   | ¬A        |
| A genau dann, wenn B; A ist äquivalent B; A gilt dann, und nur dann, wenn B gilt                    | A ↔/⇔ B   |
| Aus A folgt B; A impliziert B; Wenn A wahr ist, dann ist auch B wahr; Wenn A gilt, dann gilt auch B | A →/⇒ B   |
| Alle; jeder, jede, jeden                                                                            | ∀         |
| Nicht alle (Es gibt mindestens ein Element, das die gegebene Eigenschaft nicht erfüllt)             | ¬∀        |
| Es existiert; es gibt; (mindestens) ein, einer, eine, jemand                                        | ∃         |
| Es existiert nicht; niemand; keine (Es existiert kein Element, das die gegebene Eigenschaft erfüllt | ¬∃        |

### Unterschied zwischen $∃$ und $¬∀$
- $∃$ bedeutet, dass von 1 bis alle Ergebnisse gültig sind
- $¬∀$ bedeutet, dass von 1 bis alle Ergebnisse ungültig sind

## Aussagenlogik 1.2
### Wahrheitstabelle und Negation
| A | B | A ∧ B | A ∨ B | A ↔ B | A → B |
|---|---|-------|-------|--|--|
| ⊥ | ⊥ | ⊥     | ⊤     | ⊤ | ⊤ |
| ⊥ | ⊤ | ⊥     | ⊤     | ⊥ | ⊤ |
| ⊤ | ⊥ | ⊥     | ⊤     | ⊥ | ⊥ |
| ⊤ | ⊤ | ⊤     | ⊥     | ⊤ | ⊤ |

#### Beispiel
![Negation.png](./Anhang/Negation.png)

### Axiomensystem nach Peano
![Peano.png](./Anhang/Peano.png)

## Logisches Schließen 1.3
Tool zum Visualisieren: [The Incredible Proof Maschine](https://incredible.pm)

Die einfachsten Beweise können ohne Aussagen aus einem Kalkül geführt werden:

![Beweis Beispiel.png](./Anhang/Beweis Beispiel.png)
![Beweis Beispiel IPM.png](./Anhang/Beweis Beispiel IPM.png)

Hier ist die zu zeigende **Konklusion** (unten) direkt aus der gegebenen **Prämisse** (oben) belegbar und könnte lauten:
	Beweis: Die Konklusion $A$ ergibt sich aus der Prämisse $A$.

### Regeln
#### Konjunktion
![Konjunktion.png](./Anhang/Konjunktion.png)
![Konjunktion IPM.png](./Anhang/Konjunktion IPM.png)

**Konjunktion ist kommutativ**:

![Konjunktion kommutativ.png](./Anhang/Konjunktion kommutativ.png)

#### Implikation / Modus Ponens
![Implikation.png](./Anhang/Implikation.png)
![Implikation IPM.png](./Anhang/Implikation IPM.png)

**Implikation ist transitiv**:
![Implikation transitiv.png](./Anhang/Implikation transitiv.png)

#### Disjunktion
![Disjunktion.png](./Anhang/Disjunktion.png)
![Disjunktion IPM.png](./Anhang/Disjunktion IPM.png)
![Disjunktion IPM 2.png](./Anhang/Disjunktion IPM 2.png)
[Auch transitiv oder so?]

#### Allquantor
![Allquantor.png](./Anhang/Allquantor.png)
![Allquantor IPM.png](./Anhang/Allquantor IPM.png)

#### Existenzquantor
![Existenzquantor.png](./Anhang/Existenzquantor.png)
![Existenzquantor IPM.png](./Anhang/Existenzquantor IPM.png)

### Schritte darstellen
Beispiel anhand Konjuktion:

![Schritte.png](./Anhang/Schritte.png)

#### Baumdarstellung
![Baumdarstellung.png](./Anhang/Baumdarstellung.png)

### Beispiel
Auf Basis dieser Regeln können Assoziativität und Kommutativität der Disjunktion bewiesen werden, wie auch die Distributivität der Konjunktion:

![Satz 1.23.png](./Anhang/Satz 1.23.png)

Beweis: Aus der Prämisse $A ∧ (B ∨ C)$ folgt nach $KL$ und $KR$, dass $A$ und $B ∨ C$ erfüllt sind.

Aus den Aussagen $A$ und $B ∨ C$ ist nun mit Regel D die Konklusion $(A ∧ B) ∨ ( A ∧ C)$ zu zeigen:
1. Fall: Ist $B$ erfüllt, so gilt nach $K$ mit $A$ und $B$, dass $A ∧ B$ gilt. Wegen $DL$ ist mit $A ∧ B$ auch $(A ∧ B) ∨ (A ∧ C)$ erfüllt.
2. Fall: Ist $C$ erfüllt, so gilt nach $K$ mit $A$ und $C$, dass $A ∧ C$ gilt. Wegen $DR$ ist mit $A ∧ C$ auch $(A ∧ B) ∨ (A ∧ C)$ erfüllt.

Da mit der Aussage $B ∨ C$ und in beiden Fällen $B$ und $C$ die Aussage $(A ∧ B) ∨ (A ∧ C)$ erfüllt ist, gilt diese nach Regel $D$ allgemein und die Konklusion ist bewiesen.

#### Tabellarischer Beweis
![Tabellarischer Beweis.png](./Anhang/Tabellarischer Beweis.png)

### Schlussprinzipien
#### Ex falso quodlibet
Alles kann aus einer falschen Aussage gefolgert werden.

![ex falso quodlibet.png](./Anhang/ex falso quodlibet.png)

#### Modus Tollens
Durch Aufheben aufhebende Schlussweise.

![Modus Tollens.png](./Anhang/Modus Tollens.png)
[Es gibt auch einen Modus ponens]

#### Tertium Non Datur
Diese Regel ist immer wahr und besitzt daher keine Prämissen. Somit kann man beliebige Aussagen „erzeugen“, wodurch die konstruktive Logik verlassen wird.

![Tertium Non Datur.png](./Anhang/Tertium Non Datur.png)

#### Indirekter Beweis
Aus $¬B→¬A$ folgt $A→B$, es gilt also:

![Indirekter Beweis.png](./Anhang/Indirekter Beweis.png)

## Prädikatenlogik
Hier zunächst nur vorausgesetzt, dass der logische Ausdruck für jeden Parameter x oder Parameterliste $x_1, ..., x_n$ eindeutig ausgewertet werden
kann. Wenn im Folgenden nur von einstelligen Prädikaten $P(x)$ geschrieben wird, so sind damit immer auch mehrstellige Prädikate wie $P(x, y)$, $P(x, y, z)$ oder $P(x_1, ..., x_n)$ gemeint.

| Aussagen | Prädikat | Prädikatenaussage |
|--|--|--|
| Die Zahl 5 ist gerade. | G(x): Die Zahl x ist gerade. | G(5) |
| Deutschland liegt nicht in Europa. | E(x): x liegt in Europa. | ¬E(Deutschland) |
| 11 ist ungerade und eine Primzahl. | G wie oben, P(x): x ist eine Primzahl | ¬G(x) ∧P(x) |
| Alle Enten sind blau. | B(x): x ist Blau, D(x): ist eine Ente | ∀D(x) : B(x) |

## Prädikatenlogik 1.4
### Allquantor und Existenzquantor
[Einstieg?]
Die vereinfachenden Schreibweisen der Ausdrücke $∀A(x) : B(x)$ und $∃A(x) : B(x)$, die oft mithilfe von später eingeführten Mengen mit $A(x) : x ∈ M$ als $∀x ∈ M : B(x)$ oder $∃x ∈ M : B(x)$ verwendet werden, können so in die elementare Form umgeschrieben werden:

$$
∀A(x) : B(x) ⇔ ∀x: ¬A(x) ∨ B(x)\\
∃A(x) : B(x) ⇔ ∃x: A(x) ∧ B(x)
$$

Bei einer begrenzten Anzahl von möglichen Parametern können die Quantoren durch Konjunktion und Disjunktion beschrieben werden:

$$
∀x : A(x) ⇔ A(1) ∧ A(2) ∧ A(3) \\
∃x : A(x) ⇔ A(1) ∨ A(2) ∨ A(3)
$$

### Prädikate
Für **symmetrische oder austauschbare** Prädikate $P$ mit Parameter $x$ und $y$ ergeben sich folgende Äquivalenzen:

$$
∀x : ∀y : P(x, y) ⇔ ∀y : ∀x : P(x, y) \\
∃x : ∃y : P(x, y) ⇔ ∃y : ∃x : P(x, y)
$$

**Bsp.**: $P(x, y)$: "$x$ ist mit $y$ befreundet."
Freundschaft ist symmetrisch ($P(x, y) ⇔ P(y, x)$), daher sind sie logisch gleichwertig.

Weißt das Prädikat **asymmetrischen Eigenschaften** auf, kann man nur eine Richtung zeigen bzw. implizieren:

$$
∀x : ∀y : P(x, y) ⇒ ∀y : ∀x : P(x, y) \\
∃x : ∃y : P(x, y) ⇒ ∃y : ∃x : P(x, y)
$$

**Bsp.**: $P(x, y)$: "$x$ ist der Vater von $y$."
"Vater von" ist keine symmetrische Beziehung (man kann nicht gegenseitig Vater sein), deswegen kann nur impliziert werden.

Unterschiedliche Quantoren sind immer nur in eine Richtung vertauschbar:

$$
∃x : ∀y : P(x, y) ⇒ ∀y : ∃x: P(x, y)
$$

Negationen wandeln den Typ des Quantors:

$$
¬∀x : P(x) ⇔ ∃x : ¬P(x) \\
¬∃x : P(x) ⇔ ∀x : ¬P(x)
$$

Daraus lassen sich vier Aussagen schließen:

$$
1. ¬∀x: P(x) ⇒ ∃x: ¬P(x) \\
2. ∃x: ¬P(x) ⇒ ¬∀x: P(x) \\
3. ¬∃x: P(x) ⇒ ∀x: ¬P(x) \\
4. ∀x: ¬P(x) ⇒¬∃x: P(x) \\
$$

### Beispiel
$L(x, y) : x\text{ liebt }y$

![Quantoren Prädikat Beispiel.png](./Anhang/Quantoren Prädikat Beispiel.png)

- Aus Aussage (3) „Alle lieben eine(n)“ folgt Aussage (2) „Jede(r) liebt jemanden“, aber die Gegenrichtung wird nicht allgemein gelten.
- Existenzaussagen bedeuten nicht, dass es jeweils nur genau einen Fall gäbe: Alle Allquantoren können durch schwächere [?] Existenzquantoren ersetzt werden. Die Rückrichtung ist jedoch nicht allgemein gültig.

## Beweistechniken 1.5
- Mit „Gegeben ist: *Prämissen*“ und „Zu zeigen ist: *Konklusion*“ beginnen
- Beim Gebrauch von Hilfsaussagen ($D$, $AI$, $EE$…) im Beweis einer Teilaussage ebenso die lokalen Prämissen und die gewünschte Konklusion definieren
- Kennzeichnen, wann die Konklusion erreicht und alle benötigten Zwischenaussagen bewiesen wurden
- Beweise wie $A ⇔ B$ in zwei Teile $A ⇒ B$ und $B ⇒ A$ aufzuteilen, ist sicherer und verständlicher
- Sind beiden Richtungen bewiesen, so ist die Äquivalenz bewiesen

### Beweise
#### Direkter Beweis
Ein direkter Beweis einer Implikation $A ⇒ B$ ist eine Abfolge von Implikationen zu Zwischenschritten, die am Ende zur Konklusion B führen ($A ⇒ A_1 ⇒ A_2 ⇒ … ⇒ A_n ⇒ B$).

#### Indirekter Beweis
Macht sich die Äquivalenz $(A ⇒ B) ⇔ (¬B ⇒ ¬A)$ zu Nutze. Um also $A ⇒ B$ zu zeigen, wird die äquivalente Aussage $¬B ⇒ ¬A$ gezeigt.

#### Beweis durch Widerspruch
Nutzt die Äquivalenz $(A ⇒B) ⇔ ¬(A ∧ ¬B)$ und startet mit den Prämissen $A$ und $¬B$, um damit auf einen Widerspruch als auf Falsch zu schließen.

#### Beweis durch Gegenbeispiel
Kommt bei der Widerlegung von Aussagen mit Allquantor zum Einsatz. Um eine Aussage mit Allquantor zu widerlegen, reicht ein einziges Gegenbeispiel, welches nachvollziehbar der Aussage widerspricht.

#### Vollständige Induktion
Vollständige Induktion über den natürlichen Zahlen. Sei $P$ ein Prädikat über den natürlichen Zahlen. Mit den folgenden zwei Schritten wird $P(x)$ für alle natürlichen Zahlen $x$ bewiesen:

Induktionsanfang $n = 1: P(1)$ ist wahr.
Induktionsschritt $n → n + 1$: Sei $n$ eine natürliche Zahl und $P(n)$ sei wahr. Dann folgt $P(n + 1)$.

Dann gilt $P(x)$ für alle natürlichen Zahlen $x$. Der Beweis basiert auf der Definition der natürlichen Zahlen.
[Noch Rechenbeispiele für die einzelnen Beweise?]

### Beispiel
**Satz**: *Sei $n$ eine natürliche Zahl, also eine ganze positive Zahl. Dann ist $n^2$ genau dann eine gerade Zahl, wenn $n$ gerade ist.*

**Beweis vom Satz**:
Gegeben ist: $n$ ist eine ganze positive Zahl.
Zu zeigen ist: Genau dann, wenn $n^2$ gerade ist, ist $n$ gerade.

**Dafür werden im Folgenden zwei Aussagen gezeigt**:
⇒ Wenn $n^2$ eine gerade Zahl ist, so ist $n$ eine gerade Zahl.
⇐ Wenn $n$ eine gerade Zahl ist, so ist $n^2$ eine gerade Zahl.

- Eine Zahl $n$ ist genau dann gerade, wenn sie als das Doppelte einer anderen ganzen positiven Zahl $k$ geschrieben werden kann ($n = 2k$)
- D. h. positiven ganzen Zahlen sind ungerade wenn $n = 2k - 1$

**Direkter Beweis von n ist gerade $⇒ n^2$ ist gerade**:
Gegeben ist: $n$ ist gerade.
Zu zeigen ist: $n^2$ ist gerade.

1. Ist n gerade, so gibt es ein ganzes $k$, sodass $n = 2k$ ist.
2. Damit ist $n^2 = n * n = 2k * 2k = 2 * 2k^2$.
3. Damit ist $m = 2k^2$ wieder eine ganze Zahl.
4. Somit ist $n^2 = 2 * m$ eine gerade Zahl.

**Indirekter Beweis von $n^2$ ist gerade $⇒ n$ ist gerade**:
Gegeben ist: $n$ ist nicht gerade, also ungerade.
Zu zeigen ist: $n^2$ ist nicht gerade, also ungerade.

1. Wenn $n$ ungerade ist, so gibt es ein ganzes positives $k$ mit $n = 2k - 1$.
2. Dann ist

$$
n^2 = n * n \\
= (2k - 1) * (2k - 1) \\
= 4k^2 - 4k + 1 \\
= 2 * (2k^2 - 2k) + 2 - 2 + 1 \\
= 2 * (2 * (k^2 - k) + 1) - 1 \\
$$

4. Da k positive ganze Zahl, ist $k^2 - k = k * (k - 1)$ eine ganze Zahl, und größer oder gleich $0$.
5. Damit ist $m = 2(k^2 - k) + 1$ eine ganze positive Zahl.
6. Somit ist $n^2 = 2m - 1$ eine ungerade Zahl.

# Relationen und Funktionen 2
- Es ist möglich n-stellige Relationen zwischen Mengen $A_1,...,A_n$ als Teilmenge von $A_1 ×...× A_n$ zu betrachten. Hier werden aber nur zweistellige Relationen innerhalb einer Menge behandelt.
- Viele der Konzepte können auf Relationen zwischen unterschiedlichen Mengen und auch mehrstellige Relationen erweitert werden.

## Definitionen
**Natürliche Zahlen ($\mathbb{N}$)**: Positive, ganze Zahlen, die bei 1 beginnen und unendlich fortgesetzt werden:  $\mathbb{N}:\{1, 2, 3, 4,...\}$
**Ganze Zahlen ($\mathbb{Z}$)**: Erweitern die natürlichen Zahlen um die negativen ganzen Zahlen und die Null: $\mathbb{Z}:\{..., -2, -1, 0, 1, 2,...\}$
**Rationale Zahlen ($\mathbb{Q}$)**: Alle Zahlen, die als Bruch dargestellt werden können, wobei der Zähler und der Nenner ganze Zahlen sind und der Nenner nicht null ist: $\mathbb{Q}: \frac{1}{2}, \frac{-3}{4}, 5$ (5 kann als $\frac{5}{1}$ geschrieben werden)
**Reelle Zahlen ($\mathbb{R}$)**: Alle rationalen und irrationalen Zahlen. Sie decken die gesamte Zahlenlinie ab: $\mathbb{R}: 2, -3.5, \sqrt{2}, \pi$
**Komplexe Zahlen ($\mathbb{C}$)**: Erweitern die reellen Zahlen um eine zusätzliche Dimension, die auf der imaginäre Einheit $i$ ($i^2 = -1$) basiert, und umfassen Zahlen, die in der Form $a + bi$ geschrieben werden können: $\mathbb{C}: 3 + 4i, -2 - i, 0 + i$
**Relation $R$**: Eine Relation R zwischen zwei Mengen $A$ und $B$ ist eine Teilmenge ihres kartesischen Produkts $R ⊆ A × B$. Je zwei Elemente $a ∈ A$ und $b ∈ B$ stehen genau dann in Relation zueinander, geschrieben $aRb$, wenn $(a, b) ∈ R$.
**Menge $M$**: Eine Zusammenfassung von wohlbestimmten und wohl unterschiedenen Objekten unseres Denkens zu einem Ganzen [Klammer zeigen]
**Tupel / Paare, Tripel**: Elemente $(a,b)$ werden als zweistellige Tupel bezeichnet. Die Elemente des kartesischen Produkts über $n$ Mengen ($A_1 ×...× A_n = \{(a_1,...,a_n) |a_1 ∈ A_1 , ... , a_n ∈A_n \}$) werden als $n$-stellige Tupel bezeichnet. Dreistellige Tupel werden auch als Tripel bezeichnet
**Intervall**: Eine zusammenhängende Menge von Zahlen auf einer Zahlengeraden, die durch zwei Endpunkte $[a,b]$ definiert ist und alle Zahlen dazwischen (inklusive Endpunkte) umfasst. Offene $(a,b)$ und halboffene $[a,b)$, $(a,b]$ Intervalle schließen die Endpunkte der offenen Seiten nicht mit ein
**Äquivalenzrelation**: Relation, die reflexiv, symmetrisch und transitiv ist. Teilt Mengen in disjunkte Äquivalenzklassen ein
**Ordnungsrelation $R\subseteq M\times M$**: Eine zweistellige Relation ("kleiner-gleich"-Beziehung), die Elemente einer Menge $M$ miteinander vergleicht
**Quasiordnung / Präordnung**: Ordnungsrelation, wenn $R$ reflexiv und transitiv ist
**Halbordnung / teilweise Ordnung**: Ordnungsrelation, wenn $R$ reflexiv, transitiv und antisymmetrisch ist
**Vollordnung / lineare Ordnung / totale Ordnung**: Ordnungsrelation, wenn $R$ reflexiv, transitiv, antisymmetrisch und linear ist
**Infixsymbole**: Symbole, die zwischen den Operanden in einem Ausdruck stehen und normalerweise Operationen darstellen[VS Prefix]
**Abbildung / Funktion $f$**: Eine Regel, die jedem Element einer Ausgangsmenge (Elemente der Definitionsmenge $A$) genau ein Element der Zielmenge $B$ zuordnet $f: A \rightarrow B$
**Definitionsmenge oder -bereich $A$**: Die Menge aller möglichen Ausgangswerte, auf die die Abbildung angewendet wird
**Zielmenge oder -bereich $B$ / Kodomain**: Die Menge, in der alle potenziellen Ausgabewerte einer Abbildung liegen (unterschiedliche Eingabewerte können zum gleichen Ausgabewert führen)
**Ausgangs- oder Eingabewerte**: Die Werte, die in die Abbildung eingegeben werden
**Ausgabewerte**: Diese beziehen sich auf die konkreten Werte, die eine Abbildung liefert, wenn sie auf ein bestimmtes Element der Definitionsmenge angewendet wird
**Wertemenge / Bildmenge**: Die Menge aller Ausgabewerte, die eine Abbildung tatsächlich annimmt, wenn sie auf jedes Element der Definitionsmenge angewendet wird. Sie ist also eine Teilmenge der Zielmenge
**Identische Funktion / Identität $id$**: Spezielle Art von Funktion, die jedes Element der Definitionsmenge auf sich selbst abbildet
**Bild** $Bild(f)$: Die Menge aller Ausgabewerte (Elemente der Zielmenge $B$), welche durch die Anwendung der Abbildung auf Elemente der Ausgangsmenge (Elementen der Definitionsmenge $A$) entstehen
**Urbild**: Bezieht sich auf eine Teilmenge der Zielmenge $B$, und ist die Menge aller Elemente aus der Definitionsmenge $A$, welche von der Abbildung auf die gegebene Teilmenge abgebildet werden
**Permutationen**: Anordnungen oder Umordnungen einer gegebenen Menge von Objekten in einer spezifischen Reihenfolge
**Graph $G$ / Netzwerk $N$**: Eine strukturierte Menge von verbundenen Knoten (oder Punkten), oft dargestellt durch ein Graphenmodell, das die Beziehungen zwischen den Knoten beschreibt. Graphen sind entweder gerichtet (unidirektional = in eine Richtung) oder ungerichtet (bidirektional = keine Richtung)
**Knoten & Kanten**: Ein grundlegendes Element eines Netzwerks oder Graphen, das andere Knoten (z.B. Zustände oder Entitäten) durch Kanten (Verbindungen) miteinander verbindet
**Kardinalität / Mächtigkeit**: Anzahl der Elemente in dieser Menge (Endliche Mengen ($|M|$) oder unendliche Mengen). Sind $A$ und $B$ endliche Mengen mit $|A| = n$ und $|B| = m$ Elementen, so ist das kartesische Produkt ebenso endlich und hat $|A×B| = n·m$ Elemente. Unendliche Mengen können entweder abzählbar (Eins-zu-eins-Korrespondenz mit den natürlichen Zahlen) oder unabzählbar sein
**Mengensystem $Z$**: Ein Mengensystem ist eine Menge, deren Elemente selbst Mengen sind: $M=\{\{a,b\},\{c,d,e\}\}$
**Potenzmenge $P$**: Die Potenzmenge einer Menge $A$ ist die Menge aller möglichen Teilmengen von $A$, einschließlich der leeren Menge und $A$ selbst. Wenn $A$ eine endliche Menge ist, enthält die Potenzmenge $2^{|A|}$ Elemente, wo $|A|$ die Mächtigkeit der Menge $A$ ist.
**Disjunkt**: Jedes Element der Menge ist in genau einer Teilmenge enthalten und kann nicht zwischen den Teilmengen geteilt werden
**Äquivalenzklasse $[a]$**: Eine disjunkte Restklassen (Teilmengen einer Äquivalenzrelation), die durch eine Äquivalenzrelation innerhalb einer Menge definiert wird. Alle Elemente einer Äquivalenzklasse sind äquivalent zueinander, das heißt, sie stehen in der jeweils definierten Beziehung zueinander: $[a] = \{ x \in A \mid x \sim a \}$
**Partitionierung einer Menge**: Die Aufteilung in eine Sammlung disjunkter, nicht-leerer Teilmengen $P$, deren Vereinigung die ursprüngliche Menge $A$ ergibt: $P_i \subseteq A$
**Quotientenmenge / Faktormenge (von $M/R$)**: Enthält alle, bei der Partitionierung entstandenen, Äquivalenzklassen: $A\sim = \{ [a] \mid a \in A \}$
**Zusammenhangskomponenten**: In einem ungerichteten Graphen eine maximal zusammenhängende Teilmenge von Knoten, in der zwischen jedem Knotenpaar ein Pfad existiert.

Projektive Raum: [?]
homogene Koordinaten: [?]
Diskrete und kontinuierliche Optimierung: [?]
Hasse-Diagramm: [!]
Fehlt viel aus Permutationen

## Symbole
**Leere Menge**: $∅$ oder $\{\}$
**Vereinigungsmenge / Vereinigung (Alle Elemente, die entweder in $A$ oder $B$ sind)**: $\cup$
**Durchschnittsmenge / Schnitt (Alle Elemente, die sowie in $A$ als auch in $B$ sind)**: $\cap$
**Einseitige Mengendifferenz (Alle Elemente, die in $A$, aber nicht in $B$ enthalten sind)**: $\setminus$
**Symmetrische Mengendifferenz (Alle Elemente, die entweder in $A$ oder in $B$ enthalten sind, aber nicht in beiden)**: $\Delta$
**Teilmenge / inklusiv gleich (Jedes Element von $A$ ist auch ein Element von $B$ ($A$ liegt in $B$))**: $\subseteq$
**Echte Teilmenge (Es gibt mindestens ein Element in $B$, das nicht in $A$ ist ($A$ liegt in $B$))**: $\subset$
**Obermenge / inklusiv gleich (Jedes Element von $B$ ist auch ein Element von $A$ ($B$ liegt in $A$))**: $\supseteq$
**Echte Obermenge (Es gibt mindestens ein Element in $A$, das nicht in $B$ ist ($B$ liegt in $A$))**: $\supset$
**Teiler von ([!])**: $|$
**Parallel zu ([!])**: $\parallel$
**Kartesisches Produkt (Menge aller einzigartigen, geordneten Paare)**: $×$
**Äquivalenzrelation**: $∼$ oder $\sim_R$ (dieses Symbol ersetzt $R$ in Äquivalenzrelationen)
**Vorrangrelation / vorgeordnete Relation**: $\preceq$ (diese Symbole ersetzten $R$ in Ordnungen)[Definieren!]
↦, 
$M = \bigcup_{i=1}^{n} M_i$
| bei {x| x… }
≡
mod
◦
Wohin $N \backslash \{0\}$

## Mengen 2.1
[[LA 1 Zusammenfassung#Mengen und Mengenoperationen]]
[Trotzdem vergleichen!]

## Relationen 2.2
- Das $R$ wird durch Vergleichsperatoren ersetzt (z.B. $=$, $>$, $≥$, $"\text{ist älter als}"$, …)
- Eine Relation kann symmetrisch und antisymmetrisch sein, wenn nur ein Element enthalten ist
- $(a,b)R(c,d) ⇔ a/b = c/d ⇔ a * d = b * c$

### Beispiel
Es seien $A = \{r, s, t\}$ und $B = \{u, v, w\}$. Dann ist
$R = \{(r, u),(r, w),(s, w)\} ⊆ A × B$

![Relationen.png](./Anhang/Relationen.png)

### Eigenschaften von Relationen
*Sei $M$ eine Menge und $R⊆ M × M$ eine Relation.*

Die Relation $R$ ist...
- **symmetrisch**, wenn für alle $(x, y) ∈ R$ auch $(y, x) ∈ R$ folgt
- **antisymmetrisch**, wenn aus $(x, y) ∈ R$ und $(y, x) ∈ R$ folgt, dass $x = y$
- **reflexiv**, wenn für alle $x ∈ M$ gilt, dass $(x, x) ∈ R$
- **transitiv**, wenn aus $(x, y) ∈ R$ und $(y, z) ∈ R$ folgt, dass $(x, z) ∈ R$.
- **linear**, wenn für jedes $x, y ∈ M$ gilt: $(x,y ) ∈ R$ oder $(y, x) ∈ R$.

#### Beispiele der Eigenschaften
**Symmetrie**: Beide Paarkombinationen müssen funktionieren, die Elemente sind aber nicht gleich (z.B. $xRy ⟺ x ist verwandt mit y$. Verwandtschaft ist gegenseitig, aber man kann nicht mit sich selbst verwandt sein)
**Antisymmetrie**: Elemente sind "identisch" (z.B. $xRy⟺ x\text{ ist älter oder gleich alt zu }y$. Da nicht beide gleichzeitig älter als der andere sein können, müssen sie gleich alt sein)
**Reflexivität**: Heißt alle Paare sind vorhanden (z.B. $xRx ⟺ x\text{ ist so groß wie }x$)
**Transitivität**: z.B. Suche nach bestimmten Paaren (z.B. $xRy⟺ x\text{ ist ein Geschwister von }y$. Sind Theo und Thilo Geschwister, sowie Thilo und ein Bananenbrot, müssen Theo und das Bananenbrot Geschwister sein)
**Linearität**: Jedes Paar ist vergleichbar (z.B. $xRy ⟺ x\text{ ist größer oder gleich groß zu }y$. Es muss irgendeine Aussage stimmen)
[Genauere Beschreibungen]
[Aus welchen Eigenschaften lassen sich andere (nicht) schließen?]
[Wenn kein Gegenbeispiel, dann richtig?]

#### Beispiel
Für die Menge $M = \{a,b,c,d\}$ ist die Relationen $R = \{(a,a),(a,b),(a,c),(a,d),(b,b),(b,c),(b,d),(c,c),(c,d),(d,d)\}$ definiert

Die Relation $R$ ist…
• nicht symmetrisch, denn aus $(a,b) ∈ R$ folgt nicht $(b,a) ∈ R$,
• antisymmetrisch, denn aus $(x,y) ∈ R$ und $(y,x) ∈ R$, folgt, dass $x = y$,
• reflexiv, da $\{(a,a),(b,b),(c,c),(d,d)\}$⊆R,
• transitiv, da z.B. mit $(a,b) ∈ R$, $(b,c) ∈ R$ auch $(a,c) ∈ R$ folgt,
• linear, da für alle $x ∈ M$ und $y ∈ M$ entweder $(x,y) ∈ R$ oder $(y,x) ∈ R$ gilt.

![Relation Beispiel.png](./Anhang/Relation Beispiel.png)

### Graphen
| Merkmal                              | Gerichtete Graphen                                                            | Ungerichtete Graphen                                         |
|--------------------------------------|-------------------------------------------------------------------------------|--------------------------------------------------------------|
| **Definition**                       | Kanten haben eine Richtung von einem Knoten zu einem anderen (unidirektional) | Kanten haben keine Richtung, Verbindungen sind bidirektional |
| **Darstellung der Kante**            | Geordnetes Paar $(u, v)$                                                      | Ungeordnetes Paar ${u, v}$                                   |
| **Grad (Anzahl verbundener Kanten)** | Knoten haben Eingangs- und Ausgangsgrade                                      | Jede verbunde Kante ist ein Grad                             |
| **Pfad**                             | Pfade folgen den Richtungen der Kanten                                        | Pfade sind in beide Richtungen möglich                       |

![Gerichtete und ungerichtete Graphen.png](./Anhang/Gerichtete und ungerichtete Graphen.png)

### Äquivalenzrelationen
#### Beispiel 1
1. **Menge**: Betrachten wir die Menge der ganzen Zahlen $\mathbb{Z}$.

2. **Äquivalenzrelation**: Wir definieren eine Äquivalenzrelation $\sim$ auf $\mathbb{Z}$ durch: Zwei Zahlen $a$ und $b$ sind äquivalent ($a \sim b$), wenn sie bei Division durch 3 denselben Rest haben. Dies nennt man "Kongruenz modulo 3".

3. **Äquivalenzklassen**:
	- Die Äquivalenzklasse von 0 wäre die Menge aller ganzen Zahlen, die bei Division durch 3 den Rest 0 ergeben: $[0] = \{\ldots, -6, -3, 0, 3, 6, \ldots\}$.
	- Die Äquivalenzklasse von 1 wäre die Menge aller ganzen Zahlen, die bei Division durch 3 den Rest 1 ergeben: $[1] = \{\ldots, -5, -2, 1, 4, 7, \ldots\}$.
	- Die Äquivalenzklasse von 2 wäre die Menge aller ganzen Zahlen, die bei Division durch 3 den Rest 2 ergeben: $[2] = \{\ldots, -4, -1, 2, 5, 8, \ldots\}$.

4. **Quotientenmenge**: Die Quotientenmenge $\mathbb{Z}/\sim$ ist die Menge der unterschiedlichen Äquivalenzklassen, also: $\mathbb{Z}\sim = \{[0], [1], [2]\}$

#### Beispiel 2
Sei $N$ ein ungerichteter Graph und sei darin $M$ eine Menge von Knoten und $K$ die Relation der Kanten zwischen den Punkten in einem Netzwerk, also mit $x K y$ gilt immer auch $y K x$.

![Netzwerk Äquivalenzrelation.png](./Anhang/Netzwerk Äquivalenzrelation.png)
*Graph zu Beispiel (Reflexive Kanten werden oft nicht eingezeichnet)*

Dann ist die Relation $K$ im Allgemeinen keine Äquivalenzrelation, aber die abgeleitete Relation $xRy$ für $x$ ist mit $y$ über Kanten verbunden, ist eine Äquivalenzrelation:

**Reflexivität**: Es gilt $xRx$, da jeder Punkt mit sich verbunden ist
**Symmetrie**: Ist $xRy$, so existiert eine Folge von Kanten $x\ K\ a_1\ K\ ...\ K\ a_n\ Ky$, die umgekehrt $y$ mit $x$ verbindet, also $yRx$ gilt
**Transitivität**: Ist $xRy$ und $yRz$, so existieren jeweils von $x$ nach $y$ nach $z$ eine Folge von Kanten, die zusammengehängt $x$ mit $z$ verbinden, also gilt $xRz$

Sei $M$ eine Menge und $R$ eine Äquivalenzrelation. Für ein $x∈M$ ist
$[x]_R = \{y∈M|xRy\}$

Sei R eine Äquivalenzrelation über einer Menge $M$ und $x,y∈M$ beliebig:
1. Es gilt $x∈[x]_R$
2. Gilt $xRy$, so ist $x∈[y]_R$
3. Ist $[x]_R ∩[y]_R ≠ ∅$, so ist $[x]_R = [y]_R$.

Sei $R$ Äquivalenzrelation der Menge $M$, dann ist das Mengensystem der Äquivalenzklassen
$K = \{[x]_R|x∈M \}$ eine Partition der Menge $M$.
[Beweis nicht verstanden!]

### Ordnungsrelationen
Ist $R$ über Menge $M$
- **reflexiv**, $∀x∈M : x⪯x$,
- **transitiv**, $∀x,y,z∈M : ( (x⪯y ∧y⪯z) ⇒ x⪯z )$
so ist die Relation **Quasiordnung**.

Ist die Relation zusätzlich
- **antisymmetrisch**, $∀x,y∈M : ( (x⪯y ∧y⪯x) ⇒ x= y )$,
so ist die Relation **Halbordnung**.

Ist die Relation zusätzlich
- **linear**, $∀x,y∈M : (x⪯y) ∨(y⪯x)$
so ist die Relation **Vollordnung**.

1. Die Ordnung $≤$ ist auf den ganzen Zahlen $\mathbb{Z}$ eine **Vollordnung**:
- Reflexivität: Für alle $x∈\mathbb{Z}$ gilt $x≤x$
- Transitivität: Für alle $x,y,z∈\mathbb{Z}$ mit $x≤y$ und $y≤z$ ist auch $x≤z$
- Antisymmetrie: Für alle $x,y∈\mathbb{Z}$ mit $x≤y$ und $y≤x$ ist $x = y$
- Linearität: Für alle $x,y∈\mathbb{Z}$ ist $(x≤y) ∨ (y≤x)$

2. Die Ordnung $⊆$ ist auf Mengen wie z.B. $P(\mathbb{Z})$ eine **Halbordnung**:
- Reflexivität: Für alle Mengen $A$ gilt $A⊆A$
- Transitivität: Für alle Mengen $A,B,C$ mit $A⊆B$ und $B⊆C$ ist auch $A⊆C$
- Antisymmetrie: Gilt für zwei Mengen $A,B$, dass $A⊆B$ und $B⊆A$, so ist $A=B$
Die Ordnung ist nicht linear, da nicht alle Mengen vergleichbar sind.

3. Die Ordnung $⪯$ nach Größe von Preisen von Produkten im Supermarkt ist eine **Quasiordnung**:
- Reflexivität: Für alle Artikel $x$ gilt $x⪯x$
- Transitivität: Für Artikel $x,y,z$ mit $x⪯y$ und $y⪯z$ ist natürlich auch $x⪯z$
- Die Ordnung ist nicht antisymmetrisch, da gleicher Preis nicht auf das gleiche Produkt führt
[Woher erkenne ich dass ⪯?]

Sei $⪯$ eine Halbordnung auf einer Menge $M$.
1. Ein Element $x∈M$ ist **minimal** bezüglich $⪯$, wenn es kein weiteres Element $y∈M$ mit $x ≠ y$ gibt mit $y⪯x$
2. Ein Element $x∈M$ ist **maximal** bezüglich ⪯, wenn es kein weiteres Element $y∈M$ mit $x ≠ y$ gibt mit $x⪯y$
3. Das Element $x∈M$ ist **kleinstes** Element bezüglich $⪯$, wenn $∀y:x⪯y$
4. Das Element $x∈M$ ist **größtes** Element bezüglich $⪯$, wenn $∀y:y⪯x$

*Für Halb- und Vollordnung: Existiert ein kleinstes Element, so ist es das einzige minimale Element (und umgekehrt). Das gleiche gilt für maximale und größte Elemente.*

#### Beispiel
![Gerichtete Graphen.png](../Theoretische Informatik/Anhang/Gerichtete Graphen.png)

1. Die Relation $R$ auf dem Graphen $G_1$:
	- Reflexiv, transitiv und antisymmetrisch (Halbordnung)
	- Nicht linear, da bspw. $d$ und $i$ nicht gegenseitig erreichbar und damit nicht vergleichbar sind
	- Elemente $a$ und $g$ sind minimal, Elemente $i$, $d$, $b$ und $c$ sind maximal
	- Der Graph hat kein größtes oder kleinstes Element

2. Die Relation $R$ auf dem Graphen $G_2$
	- Reflexiv, transitiv und antisymmetrisch (Halbordnung)
	- Nicht linear, da $d$ und $e$ nicht vergleichbar sind
	- $a$ ist minimal und kleinstes Element, $c$ ist maximal und größtes Element

3. Die Relation $R$ auf dem Graphen $G_3$
	- Reflexiv und transitiv (Quasiordnung)
	- Nicht antisymmetrisch, da es zwischen $a$, $d$, $g$, $h$, $e$, $b$ einen Zyklus gibt
	- Kein minimales oder kleinstes Element
	- $c$ ist maximales und größtes Element.

[S. 40]

## Abbildungen 2.3
- Eine Abbildung oder Funktion mit Notation $f : A→B$ ist eine Relation auf $A×B$ ($A,B≠∅$)
- Jedes Element $x∈A$ steht mit genau nur einem Element $f(x) = y ∈ B$ in Relation
- Die Menge $A$ ist die Definitionsmenge der Abbildung und $B$ ist die Wertemenge
- Teilmenge von $A×B$, die die Relation bestimmt, wird als Graph der Abbildung bezeichnet: $graph(f) = {(x,f(x)) |x∈A }⊆A×B$

$$
f: A→B \\
x↦f(x)=y
$$

### Bild und Urbild
#### Bild
**Definition**: Die Menge aller Ausgabewerte (Elemente der Zielmenge $B$), welche durch die Anwendung der Abbildung auf Elemente der Ausgangsmenge (Elementen der Definitionsmenge $A$) entstehen.

**Erklärung**: Wenn man sich eine Abbildung als Maschine vorstellen, die Eingabewerte verarbeitet, dann ist das Bild die Sammlung all der Ausgabewerte, die die Maschine tatsächlich produzieren kann.

**Mathematische Darstellung**: Für eine Abbildung $f: A \rightarrow B$ ist das Bild von $f$ die Menge: $\operatorname{Im}(f) = \{ f(x) \mid x \in A \}$ (Alternativ zu $Im(f)$ auch $Bild(f)$ oder $f(A)$)

#### Urbild
**Definition**: Bezieht sich auf eine Teilmenge der Zielmenge $B$, und ist die Menge aller Elemente aus der Definitionsmenge $A$, welche von der Abbildung auf die gegebene Teilmenge abgebildet werden.

**Erklärung**: Das Urbild sagt uns, welche Eingabewerte in die Maschine gesteckt werden müssen, um bestimmte Ausgabewerte zu erhalten.

**Mathematische Darstellung**: Für eine Abbildung $f: A \rightarrow B$ und eine Teilmenge $T \subseteq B$ ist das Urbild von $T$ die Menge: $f^{-1}(T) = \{ x \in A \mid f(x) \in T \}$

Falls $T$ ein einzelnes Element $b$ in $B$ ist, dann ist das Urbild von $b$ die Menge aller Elemente in $A$, die auf $b$ abgebildet werden:$f^{-1}(\{b\}) = \{ a \in A \mid f(a) = b \}$

*Das Urbild ist keine Inversfunktion, es sei denn, die Abbildung $f$ ist bijektiv. Dann existiert für $f : A → B$ die Funktion $f^{−1} : B → A$*

#### Beispiel
Quadratische Funktion $f(x) = x^2$:
- Das Bild der Funktion $f$ ist die Menge aller möglichen Werte, die die Funktion annehmen kann
- Da $f$ niemals einen negativen Wert annimmt, ist das Bild $[0, \infty)$
- Im Graphen entspricht dies der y-Achse
- Das Urbild eines Wertes $y$ der Funktion $f$ ist die Menge aller $x$
- Z.B. das Urbild $y=4$ ist die Menge der $x$-Werte, für die $x^2 = 4$ ($x=\sqrt4 = \pm2$)
- Im Graphen sind dies die $x$-Werte, die $y = 4$ schneiden

### Eigenschaften von Abbildungen
**Eindeutige Abbildungen heißen**:
|Name |Menge A| Menge B|
|-|-|-|
|Funktion| Körper| Körper|
|Funktional| Vektor| Körper|
|Operator| Vektor| Vektor|

Eine Abbildung $f : A→B$ ist...
- …**injektiv** (Eindeutigkeit der Zuordnung), wenn verschiedene Elemente in $A$ auf verschiedene Elemente in $B$ abgebildet werden: $x,y∈A$ mit $x≠y$ folgt $f(x)≠f(y)$
- …**surjektiv** (Vollständigkeit der Abbildung), wenn jedes Element in der Zielmenge $B$ zumindest einmal von einem Element in der Definitionsmenge $A$ getroffen wird.
- …**bijektiv** (Eindeutigkeit und Vollständigkeit), wenn sie sowohl injektiv als auch surjektiv ist.

**Injektivität**: Eine injektive Funktion vermeidet also, dass zwei verschiedene Elemente der Definitionsmenge denselben Wert in der Zielmenge annehmen.

**Surjektivität**: Eine surjektive Funktion ist "überdeckend", da sie jeden Punkt in der Zielmenge erreicht.

**Bijektivität**: Es gibt eine perfekte Eins-zu-eins-Korrespondenz zwischen den Elementen der Definitionsmenge $A$ und der Zielmenge $B$. Jede Abbildung von $A$ auf $B$ ist eindeutig und deckt die gesamte Zielmenge ab. Eine bijektive Funktion hat auch eine Umkehrfunktion $f^{-1}: B \to A$, die ebenfalls eine Funktion ist.

### Beispiel 1
![Injektivität und Surjektivität.png](./Anhang/Injektivität und Surjektivität.png)

- Die Abbildung $f$ in ist weder injektiv noch surjektiv
- Die Abbildung $g$ ist surjektiv, aber nicht injektiv
- Die Abbildung $h$ ist injektiv aber nicht surjektiv
- Die Abbildung $i$, ist sowohl injektiv als auch surjektiv, und damit eine bijektive Abbildung

### Beispiel 2
![Quadratfunktion.png](./Anhang/Quadratfunktion.png)

Für die Quadratfunktion $f : R → R, x → f(x) = x^2$ ist das Bild vom Intervall $[1,2]$ gerade $f([1,2]) = [1,4]$ und das Urbild des Intervalls $[1,4]$ ist $f^{−1}([1,4]) = [−2,−1]∪[1,2]$.

- Die Quadratfunktion ist als Funktion $\mathbb{R} → \mathbb{R}$ weder injektiv noch surjektiv
- Als Funktion $[0,∞) → ∞$ ist sie injektiv und als Funktion $[0,∞) → [0,∞)$ ist sie injektiv und surjektiv und damit bijektiv

### Beispiel 3
[Kp was hier abgeht]
$f : \mathbb{R} → \mathbb{R}$
$x↦f(x) = (x−1)^2−1$
![Abbildung Beispiel.png](./Anhang/Abbildung Beispiel.png)

Gilt $f(x_0) = y_0$, so heißt $y_0$ das Bild von $x_0$ und $x_0$ heißt das Urbild von $y_0$, $G_f := \{(x,f(x))|x∈A\}$ heißt Graph von $f$

Sei $f : A→B$ eine Abbildung und $A_1 ⊂A$ und $B_1 ⊂ B$

1. $f(A_1) := \{f(x)|x∈A_1\}$ Bildmenge von $A_1$
	$f^{−1}(B_1) := \{x|x∈A∧f(x) ∈B_1\}$ Urbildmenge von $B_1$
2. $f : A→B$ heißt surjektiv, falls $f(A) = B$. Kurzum $∀y∈B∃x∈A: f(x) = y$
3. $f : A→B$ heißt injektiv (linkseindeutig), falls zu jedem $y$ höchstens ein $x$ gehört $∀y∈B: (∃!x∈A: f(x) = y∧¬(∃x∈A: f(x) = y))$
	äquivalent:
	$∀x_1,x_2 ∈ A: f(x_1) = f(x_2) ⇒ x_1 = x_2$ (gleiche $y$ bedingen das gleiche $x$)
	$∀x_1,x_2 ∈A: x_1 ≠ x_2 ⇒ f(x_1) ≠ f(x_2)$ (ungleiche $x$ bilden auf ungleiche $y$ ab)
4. $f : A→B$ heißt bijektiv (umkehrbar eindeutig, eineindeutig), falls $f$ surjektiv und injektiv ist. Kurzum $∀y∈B∃!x∈A: f(x) = y$.
[Kurz Liste verstehen. Z.B. was ist "!"?]

### Permutationen
- Sei $M$ eine **endliche** Menge, dann heißen **bijektive** Abbildungen $p : M → M$ Permutationen
- Die Menge aller Permutationen über $M$ ist definiert als: $S_M = \{p: M→M|p\text{ ist bijektiv}\}$
- Für die Menge $M=\{1,2,...,n\}$ der Zahlen von $1$ bis $n$ ist $S_n$ die Menge deren Permutationen
- Da Elemente endlicher Mengen immer durchgezählt werden können, können wir generell $S_n$ stellvertretend für die Permutationen $S_M$ von Mengen mit $n$ Elementen, also $|M|= n$, betrachten
- Die Anzahl der möglichen Permutationen, die aus einer Menge von $n$ unterschiedlichen Objekten gebildet werden können, ist $n!$
[Umkehrpermutation?]

Die Menge $S$ hat 6 Elemente, die in ausführlicher Schreibweise von Urbild (meist $1,2,3,4...$) in der ersten Zeile und Abbild (von oben nach unten) in der zweiten Zeile geschrieben werden können:

![Permutationen.png](./Anhang/Permutationen.png)

- Beispielsweise ist $σ_3(1) = 2$ und $σ_4(3) = 1$.
- Es gibt $6! = 6 \times 5 \times 4 \times 3 \times 2 \times 1 = 720$ verschiedene Permutationen.

Permutationen können alternativ auch kürzer dargestellt werden mit der **Zykelschreibweise** bzw. -darstellung (oder Kurzschreibweise).

$$
σ_4 =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 3 & 1
\end{pmatrix}
: 1 \overset{σ_4}{↦} 2 \overset{σ_4}{↦} 3 \overset{σ_4}{↦} 1 \overset{σ_4}{↦}...
$$

Die Zahlen durchlaufen immer einen Zyklus $1, 2, 3$, weshablb man es auch als $σ_4 = (1\ 2\ 3)$ darstellen kann (Reihenfolge der Zahlen eigentlich egal).

**Einfacher gesagt**: Wenn $1$ (oben) sich auf $2$ (darunter) bildet bzw. zeigt, und $2$ (oben) auf $3$ (darunter) zeigt und $3$ (oben) wiederum auf $1$ (darunter), dann entsteht ein Zyklus, weil sich die Reihenfolge wiederholt.

**Merke**: Man fängt normalerweise oben links, bei $1$, an. Ziegt eine Zahl auf sich selbst, schreibt man sie nicht mit auf. Bsp.:

$$
σ_2 =
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 2
\end{pmatrix}
= (2\ 3)
$$

Wenn jedes Element auf sich selbst abbildet, spricht man von einer Identität $id$. Da es keinen Zyklus gibt, den man aufschreiben könnte, schreibt man einfach nur  $id$. Bsp.:

$$
σ_1 =
\begin{pmatrix}
1 & 2 & 3 \\
1 & 2 & 3
\end{pmatrix}
= id
$$

Zyklusschreibweise zu $S$: $σ_1 = id, σ_2 = (2\ 3), σ_3 = (1\ 2), σ_4 = (1\ 2\ 3), σ_5 = (1\ 3\ 2), σ_6 = (1\ 3)$

Permutationen können auch mehrere Zyklen haben, die hintereinander geschrieben werden [Was das für ein Zeichen?]:

$$
ϱ =
\begin{pmatrix}
1 & 2 & 3 & 4 \\
3 & 4 & 1 & 2
\end{pmatrix}
= (1\ 3)(2\ 4)
$$

$1$ und $3$ bilden sich gegenseitig ab, sowie $2$ und $4$. Es besteht keine Verbindung zwischen den beiden Zyklen, weshalb sie mit Klammern getrennt aufgeschrieben werden.

Sind $f : A → B$ und $g : B → C$ Abbildungen so ist deren Verkettung $g◦f$ definiert als Abbildung:

$$
g◦f : A→C \\
x↦g(f(x))
$$

$(σ_3 ◦σ_4)(1) = σ_3(σ_4(1)) = σ_3(2) = 1$
$(σ_3 ◦σ_4)(2) = σ_3(σ_4(2)) = σ_3(3) = 3$
$(σ_3 ◦σ_4)(3) = σ_3(σ_4(3)) = σ_3(1) = 2$
[Sieht vielleicht kompliziert aus, deswegen Beispiel anschauen]

Und damit ist $σ_3 ◦σ_4 = σ_2$. Da bei der Verkettung von Permutationen wieder neue Permutationen entstehen, ergibt sich durch Verkettung immer wieder ein Element aus $S$.

$σ_1 = id$, und es gilt $σ_1 ◦ σ_k = σ_k = σ_k ◦ σ_1$ für alle $k = 1,...,6$.

Da alle Funktionen in $S$ bijektiv sind, haben alle eine Inverse, die ebenfalls als Permutation in $S$ ist: $σ_1^{−1} = σ_1, σ_2^{−1} = σ_2, σ_3^{−1} = σ_3, σ_4^{−1} = σ_5, σ_5^{−1} = σ_4, σ_6^{−1} = σ_6$

#### Beispiel 1
Gegebe die folgenden Permutationen $(146)(23)$ und $(17)(23)(45)$ in Zyklusschreibweise an und bestimme die Verkettung $(\ (146)(23)\ )\ ◦\ (\ (17)(23)(45)\ )$.

1. Schreibe einfach die Zyklen ab. Wenn $1 ↦ 4$, dann $\begin{matrix}1 \\ 4\end{matrix}$, und $4 ↦ 6$, dann $\begin{matrix}4 \\ 6\end{matrix}$. Da in der Zyklusschreibweise keine $5$ und $7$ vorhanden sind, bilden sie sich selbst ab.

$$
(146)(23) =
\begin{matrix}
1 & 2 & 3 & 4 & 5 & 6 & 7 \\
4 & 3 & 2 & 6 & 5 & 1 & 7
\end{matrix}
$$

2. Das gleiche für $(17)(23)(45)$ machen:

$$
(17)(23)(45) =
\begin{matrix}
1 & 2 & 3 & 4 & 5 & 6 & 7 \\
7 & 3 & 2 & 5 & 4 & 6 & 1
\end{matrix}
$$

3. Bei dem Verketten ist wichtig darauf zu achten, dass man auf der **rechten Seite** beginnt. Zuerst sucht man $\begin{matrix}1 \\ ?\end{matrix}$. Man erkennt, dass $\begin{matrix}1 \\ 7\end{matrix}$ (rechts) zu $\begin{matrix}7 \\ 7\end{matrix}$ (links) führt, wodurch das Ergebnis $\begin{matrix}1 \\ 7\end{matrix}$ ist.

$$
\begin{matrix}
1 & 2 & 3 & 4 & 5 & 6 & 7 \\
4 & 3 & 2 & 6 & 5 & 1 & 7
\end{matrix}\;◦\;
\begin{matrix}
1 & 2 & 3 & 4 & 5 & 6 & 7 \\
7 & 3 & 2 & 5 & 4 & 6 & 1
\end{matrix}\;=\;
\begin{matrix}
1 & 2 & 3 & 4 & 5 & 6 & 7 \\
7 & 2 & 3 & 5 & 6 & 1 & 4
\end{matrix}
$$

4. Nachdem alle Elemente verkettet sind, muss man in die Zyklusschreibweise zurückrechnen. $1$ bildet auf $7$ ab, $7$ auf $4$, $4$ auf $5$, $5$ auf $6$, und weil $6$ wieder auf $1$ abbildet ist der Zyklus vollendet. $2$ und $3$ bilden auf sich selbst ab und werden daher nicht aufgeschrieben.

$$
\begin{matrix}
1 & 2 & 3 & 4 & 5 & 6 & 7 \\
7 & 2 & 3 & 5 & 6 & 1 & 4
\end{matrix}
= (17456)
$$

**Wichtig**: $(\ (146)(23)\ )\ ◦\ (\ (17)(23)(45)\ )$ und $(\ (17)(23)(45)\ )\ ◦\ (\ (146)(23)\ )$ sind nicht gleich!

#### Beispiel 2
Bestimmen die Umkehrpermutation von $(146)(23)$.

Dazu muss man eigentlich nur die "Pfeile umdrehen". Die kleinste Zahl wird immer noch am Anfang geschrieben. Zweier Paare verändern sich daher nicht.

$$
(146)(23) = (1↦4↦6↦...)(2↦3↦...) \\
$$
$$
(\ (146)(23)\ )^{-1} = (...↤1↤4↤6)(...↤2↤3) = (1↦6↦4↦...)(2↦3↦...) = (164)(23)
$$

# Algorithmentheorie
## Definitionen
**Formale Sprachen**: Mengen von Zeichenfolgen, die basierend auf bestimmten Regeln gebildet werden
**Alphabet $Σ$**: Ein endliche Menge von Zeichen oder Symbolen, aus dem die Zeichenfolgen gebildet werden: $Σ = \{α_1,α_2,...,α_n\}$
**Wort $ω$**: Ein endliches oder leeres Tupel $(w_1,w_2,...,w_n) ∈ Σ^n$ von Zeichen $w_k ∈ Σ$ eines Alphabets mit Länge $|ω|=n$ der Anzahl der Zeichen. Meist werden keine Klammern oder Kommata geschrieben: $w_1w_2$
**Wortmengen**: Gibt die Menge der Worte an (Siehe Symbole)
**Grammatik**: Regelsystem oder Vorschrift, das die Struktur einer formalen Sprache definiert
**Abschluss**: Auf einer Menge mit einer Verknüpfung, jede Anwendung der Operation mit Elementen aus einer Kleene-Abschluss-Menge wieder ein Element aus der Menge ergibt[Überarbeiten]
**Rechnermodell**: Eine theoretische Darstellung eines Computers, die dazu dient, die Prinzipien der Informationsverarbeitung zu verstehen und zu analysieren. Dazu gehören die Turing-Maschine, das Lambda-Kalkül oder endliche Automaten[Unverständlich?]
**Deterministisch**: Ein System oder Prozess, bei dem der Ausgangszustand eindeutig durch den Eingabe- oder Anfangszustand bestimmt wird. Bei gleicher Eingabe wird immer exakt dieselbe Abfolge von Schritten und Ergebnissen erzeugt
**Nicht-deterministisch**: Ein System oder Prozess, bei dem mehrere mögliche Ergebnisse von einem bestimmten Eingabe- oder Anfangszustand ausgehen können. Prozesse können viele mögliche Pfade zum Ergebnis haben
**Terminieren**: Der Abschluss eines Berechnungsprozesses oder Algorithmus. Ein Programm terminiert, wenn es nach einer endlichen Anzahl von Schritten stoppt und ein Ergebnis liefert
**Automaten**: Theoretische Maschinen, die zur Erkennung formaler Sprachen verwendet werden (z.B. endliche Automaten, Kellerautomaten)[Mehr]
**Turing-Maschine**: Ein theoretisches, standardmäßig deterministisches Rechenmodell, das aus einem unendlichen Band und einem Lesekopf besteht. Es führt Berechnungen durch, indem es Symbole auf dem Band gemäß festgelegten Regeln liest, schreibt und den Kopf bewegt. Dies dient zur Untersuchung der Grenzen dessen, was mit algorithmischen Prozessen berechenbar ist
**Orakelmaschinen**: Eine nichtdeterministische Turing-Maschine mit Zugriff auf ein Orakel, das an jeder Verzweigungsmöglichkeit den zuerst erfolgreich terminierenden Pfad vorhersagen kann. Das Orakel ist rein hypothetisch und dient lediglich als theoretisches Hilfsmittel, um die Grenzen von Berechenbarkeit und Komplexität zu untersuchen
**Parallele Turing-Maschine [Hat sie einen Namen?]**: Eine nichtdeterministische Turing-Maschine, welche jede Verzweigungsmöglichkeit bzw. Alternative gleichzeitig parallel ausführen kann und terminiert, sobald eine parallele Ausführung erfolgreich endet
**Brute-force**: Methode zur Problemlösung, bei der alle möglichen Lösungen oder Kombinationen iterativ ausprobiert werden, bis die richtige oder optimale Lösung gefunden wird
**Algorithmus**: Eine eindeutige Vorschrift aus durchführbaren Anweisungen oder Schritten zur Lösung eines Problems oder zur Durchführung einer Aufgabe. In der Regel werden gegebene Eingabedaten oder Parameter verarbeiten und erzeugen eine Ausgabe, die das Problem löst
**Vorschrift**: Eine Beschreibung in Form einer Programmiersprache, sprachlichen Beschreibungen oder als Ablaufdiagramme usw., welche die Problemlösung eindeutig, durchführbar und verständlich beschreibt
**Programmablaufpläne / Flussdiagramme**: Grafische Darstellung eines Algorithmus oder Prozesses, die verschiedene Schritte in einer bestimmten Reihenfolge mit Knoten, Kanten usw. veranschaulicht
**Knotentyp**: Eine Art Knoten in einem Diagramm oder Netzwerk, der unterschiedliche Funktionen erfüllt
**Terminator**: Markiert den Start oder das Ende eines Prozesses
**Operation**: Stellt eine Berechnung oder Aktion dar
**Ein-/Ausgabe**: Zeigt, wo Daten eingegeben oder ausgegeben werden
**Entscheidung**: Repräsentiert einen Punkt, an dem sich der Prozess verzweigt
**Einstiegspunkt**: Zeigt den Beginn eines Prozesses an
**Pseudocode**: Eine vereinfachte, leicht verständliche Darstellung eines Algorithmus, die natürliche Sprache mit Programmierelementen kombiniert, um die Logik eines Programms unabhängig von einer Programmiersprache zu beschreiben

[Literale oben oder hier?]
[Es fehlen Definitionen aus 3.1 und 3.2]

## Symbole
**Leeres Wort**: $ε$ oder ()
**Wortemenge ohne Zeichen**: $Σ^0:=\{ε\}$
**Wortemenge mit beliebig vielen Zeichen**: $Σ^*:=\bigcup_{n\geq0}Σ^n$
**Wortemenge mit mindestens einem Zeichen**: $Σ^+:=\bigcup_{n>0}Σ^n$
[Kleene Abschluss Menge]
≡
mod?

## Formale Sprachen 3.1
### Alphabete und Wortmengen
**Alphabete, die es gibt**:
Alphabet (Form): $Σ = \{α_1,α_2,...,α_n\}$
Lateinische Alphabet: $Σ_{lat} = \{a,b,c,...,z\}$
Dezimal Zahlen: $Σ_{10} = \{0,1,2,3,4,5,6,7,8,9\}$
Unicode: $Σ_{Unicode} = \{x|x\text{ ist ein Zeichen im Unicode}\}$

**Beispiel mit Wortmengen**:
$M_0 = \{ε\}$
$M_1 = \{01,2\}$
$M_2 = \{0101,012,201,22\}$

$M^+ = M^1 ∪ M^2 = \{01,2,0101,012,201,22\}$
$M^∗ = M^0 ∪ M^+ = \{ε,01,2,0101,012,201,22\}$

**Kartesisches Produkt**: $A×B$ oder $A^n$ für $n∈N$ von Mengen oder Alphabeten bezeichnet die Menge der Tupel $(a,b)$ oder $(a_1,...,a_n)$ von Elementen der Mengen:

$$
A×B := \{(a,b) |a∈A, b∈B\} \\
A^n := A×...×A = \{(a_1,...,a_n) |a_1,...,a_n ∈A\}
$$

- Für zwei Wörter $u = (u_1,...,u_n)$ und $w = (w_1,...,w_m)$ ist das Produkt oder Konkatenation $u·w = uw = (u_1,...u_n,w_1,...,w_m) = u_1 ...u_nw_1 ...w_m$
- Die $n$-te Potenz eines Wortes $w$ ist $w^n=w·...·w$ für n>0, oder das leere Wort $w_0 = ε$ für $n = 0$.

**Jede Teilmenge $L⊆Σ^∗$ ist eine formale Sprache über dem Alphabet $Σ$**:
$L_{Prim} = \{n∈Σ_{Zahl}^∗|n\text{ ist eine Primzahl}\}$
$L_{Java} = \{p∈Σ_{Unicode}^∗ |p\text{ ist ein syntaktisch korrektes Java-Programm}\}$
$L_{JQuine} = \{p∈L_{Java} | \text{Die Ausgabe bei Ausführung von }p\text{ ist }p\}$

[Collatz-Funktion hinzufügen]

## Komplexitätsklassen 3.2
- Frage der Berechenbarkeit handelt davon, ob algorithmisch bestimmt werden kann, ob ein Wort Teil einer Sprache ist oder nicht
- Frage nach der Komplexität handelt davon, welcher Aufwand zur Beantwortung der Frage erforderlich ist
- Komplexitätsklassen werden verwendet, um Probleme basierend auf den Ressourcen zu kategorisieren, die zu ihrer Lösung benötigt werden, insbesondere Zeit und Speicherplatz
- Die Länge einer Zeichenkette wird als $n = |w|$ notiert
- Die Klassenhierarchie für Komplexitätsklassen: $P ⊆ NP ⊆ PSPACE = NPSPACE$

Sei $L$ eine formale Sprache, mit $M$ ein deterministisches Rechnermodell, mit $N$ ein nichtdeterministisches Rechnermodell, die $L$ erkennen. Dann ist…
$L∈time(f)$, wenn es $M$ gibt, die für $w∈L$ nach max. $f(|w|)$ Schritten terminieren,
$L∈ntime(f)$, wenn es $N$ gibt, die für $w∈L$ nach max. $f(|w|)$ Schritten terminieren kann,
$L∈space(f)$, wenn es $M$ gibt, die für $w∈L$ maximal $f(|w|)$ Speicherpositionen nutzt,
$L∈nspace(f)$, wenn es $N$ gibt, die für $w∈L$ optimal maximal $f(|w|)$ Speicherpositionen nutzt.

*Diese Einteilungen sind sehr grob, weil weder einem Schritt eine Zeiteinheit zugeordnet werden kann, noch eine Speicherposition eine bezifferbare Speichermenge beschreibt. Außerdem wird keine Zeit oder kein Raum für die Initialisierung oder Finalisierung berücksichtigt.*

### $P$ (Polynomialzeit)
- Umfasst alle Entscheidungsprobleme, die von einer deterministischen Turing-Maschine in polynomieller Zeit gelöst werden können
- D.h., dass es einen Algorithmus gibt, der das Problem in einer Anzahl von Schritten löst, die durch ein Polynom in der Länge der Eingabe $n$ beschränkt ist
- Probleme in $P$ gelten als effizient lösbar

$$
P:=\bigcup_{k \in N} time(n^k)
$$

**Beispiel**:
- Algorithmen wie Merge-Sort oder Quick-Sort können eine Liste mit $n$ Zahlen in $O(n \log(n))$ Zeit sortieren, was polynomiell ist
- Da diese Algorithmen deterministisch sind und innerhalb einer Zeit, die durch ein Polynom in Bezug auf die Eingabelänge begrenzt ist, arbeiten, gehört das Problem zur Klasse $P$

### $NP$ (Nichtdeterministische Polynomialzeit)
- Umfasst alle Entscheidungsprobleme, für die eine Lösung, wenn sie einmal gefunden ist, in polynomieller Zeit von einer deterministischen Turing-Maschine verifiziert werden kann
- Alternativ kann man sich $NP$ auch als die Klasse von Problemen vorstellen, die von einer nichtdeterministischen Turing-Maschine in polynomieller Zeit gelöst werden können
- Ein bekanntes offenes Problem in der Informatik ist die Frage, ob $\text{P} = \text{NP}$ oder $NP = PSPACE$

$$
NP:=\bigcup_{k \in N} ntime(n^k)
$$

**Beispiel**:
- SAT ist das Problem, die Erfüllbarkeit einer booleschen Formel zu bestimmen, d.h., ob es eine Zuweisung von Wahr/Falsch-Werten gibt, die die Formel wahr macht[?]
- Eine mögliche Lösung kann in polynomieller Zeit verifiziert werden, indem man die Zuweisung in die Formel einsetzt; jedoch ist es im Allgemeinen nicht bekannt, ob die Lösung deterministisch in polynomieller Zeit gefunden werden kann, weshalb das Problem in $NP$ ist

### $PSPACE$ (Polynomialer Speicherplatz)
- Die Klasse aller Entscheidungsprobleme, die von einer deterministischen Turing-Maschine mit einer Speicherplatzbeschränkung gelöst werden können, die durch ein Polynom in der Länge der Eingabe $n$ begrenzt ist
- $PSPACE$-Probleme könnten theoretisch mehr als polynomielle Zeit benötigen, sind aber durch den Speicherplatz beschränkt

$$
PSPACE:=\bigcup_{k \in N} space(n^k)
$$

**Beispiel**:
- Das Generalisierte Schieben von Spielen beschäftigt sich damit, ob ein Spieler eine Gewinnstrategie hat, basierend auf einer gegebenen Startkonfiguration[?]
- Der benötigte Speicher, um alle möglichen Züge und Spielkonfigurationen zu berücksichtigen, kann durch ein Polynom in der Größe des Spielfeldes begrenzt werden
- Das Problem gehört daher zu $PSPACE$ aufgrund des speicherbedingten Erfordernisses, alle möglichen Zustände zu verfolgen.

### $NPSPACE$ (Nichtdeterministischer polynomieller Speicherplatz)
- $NPSPACE$ ist die Klasse aller Entscheidungsprobleme, die von einer nichtdeterministischen Turing-Maschine mit einer Speicherplatzbeschränkung gelöst werden können, die durch ein Polynom in der Länge der Eingabe $n$ begrenzt ist
- Nach dem Savitch-Theorem ist bekannt, dass $\text{NPSPACE} = \text{PSPACE}$, was bedeutet, dass nichtdeterministische polynomiale Speicherplatzkomplexität mit deterministischer polynomieller Speicherplatzkomplexität übereinstimmt

$$
NPSPACE:=\bigcup_{k \in N} nspace(n^k)
$$

**Beispiel**:
- Gegeben ist ein gerichteter Graph, bei dem man prüfen soll, ob es Pfade zwischen bestimmten Knoten gibt
- In einem nichtdeterministischen Berechnungsmodell lässt sich der Pfad mit polynomiellem Speicherplatz verfolgen
- Da die Beziehung zwischen $NPSPACE$ und $PSPACE$ durch Savitch’s Theorem demonstriert, dass sie äquivalent sind, gehört es auch zur $PSPACE$. 

### Polynomielle Reduzierbarkeit
- Ein Problem, in diesem Fall eine Sprache $L ⊆Σ^∗$ ist polynomiell reduzierbar auf eine Sprache $N ⊆ Γ^∗$ ($N ≤_{poly} L$), falls es eine Funktion $f : Γ^∗→Σ^∗$ gibt, die Instanzen von $L$ in Instanzen von $N$ umwandelt, wobei $f$ in polynomialer Zeit berechenbar ist: $∀w∈Γ^∗: w∈N ⇔f(w) ∈L$
- Polynomiell bedeutet, dass etwas in polynomieller Zeit lösbar ist
- D.h., wenn man einen polynomiellen Algorithmus hat, der $N$ entscheidet, und man $L$ auf $N$ reduzieren kann, dann hat man auch einen polynomialen Algorithmus, um $L$ zu entscheiden, indem man die Reduktion benutzt und den Algorithmus für $N$ ausführt

**Beispiel**: $N$ sei ein Entscheidungsproblem (entweder "ja" oder "nein"), das durch einen polynomiellen Algorithmus lösbar ist. $L$ sei ein Entscheidungsproblem, das auf $N$ polynomial reduzierbar ist. Das bedeutet, es gibt eine polynomielle Reduktionsfunktion $f$, die Instanzen von $L$ in Instanzen von $N$ umwandelt, sodass das Ergebnis für $L$ auch nur dann "ja" ist, wenn das Ergebnis für die durch $f$ transformierte Instanz für $N$ auch "ja" ist.

- Da jedes Problem auf $L$ in ein Problem in $N$ äquivalent umgeformt werden kann, so muss $N$ mindestens so schwer sein wie $L$
- Eine Sprache $L$ ist
	- $NP$-schwer, wenn für alle $N∈NP$ gilt, dass $N ≤_{poly} L$
	- $NP$-vollständig oder $L∈NPC$ (NP-complete), wenn $L$ $NP$-schwer und $L∈NP$ ist
- $NP$-schwer ist schwer nachweisbar, wenn überhaupt nicht alle NP-Probleme bekannt sind
- Ein Anwendungsbeispiel von Polynomielle Reduzierbarkeit ist, dass 3SAT auf SAT polynomial reduzierbar ist, was bedeutet, dass wir jede Instanz von 3SAT in eine Instanz von SAT umwandeln können, sodass die Lösung beider Probleme übereinstimmt

### SAT-Problem
- SAT steht für satisfiability und wird oft auch Erfüllbarkeitsproblem der Aussagenlogik genannt
- Es bezeichnet die Frage, ob es für einen gegebenen geklammerten logischen Ausdruck aus booleschen Variablen mit den logischen Operationen von Konjunktion, Disjunktion und Negation in konjunktiver Normalform wie $X_1 ∧ (X_1 ∨ X_2)$ eine Belegung der Variablen gibt, so dass der gesamte Term wahr wird
- **Einfacher gesagt**: Welche Variablen müssen wahr oder falsch sein, damit der Term wahr wird
- $SAT = \{F|F\text{ ist boolescher Ausdruck und erfüllbar}\}$
- Jedes Problem, für das ein polynomialer Algorithmus für eine nichtdeterministische Turing-Maschine angegeben werden kann, ist unmittelbar darstellbar als ein SAT-Problem, weshalb das SAT-Problem **$NP$-schwer** ist
- Weil es in polynomialer Zeit auf einer nichtdeterministischen Turing-Maschine gelöst werden kann, einfach durch Ausprobieren einer korrekten Lösung, ist es **$NP$-vollständig**

#### Beispiel
$f(x_1,x_2,x_3,x_4) = \overline{x_3} ∧ (x_1 ∨x_2) ∧ (\overline{x_2} ∨ x_3 ∨\overline{x_2} ∨ x_3) ∧ (x_4 ∨ \overline{x_1})$

**Betrachte die Klauseln einzeln**:
- **Klausel 1:** $\overline{x_3}$ bedeutet, dass $x_3$ falsch sein muss
- **Klausel 2:** $(x_1 \lor x_2)$ mindestens eine der Variablen $x_1$ oder $x_2$ muss wahr sein
- **Klausel 3:** $(\overline{x_2} \lor x_3 \lor \overline{x_2} \lor x_3)$ vereinfacht sich zu $(\overline{x_2} \lor x_3)$. Diese Klausel ist wahr, wenn $x_2$ falsch ist oder $x_3$ wahr ist. Da wir bereits $x_3$ auf falsch setzen müssen, muss hier $\overline{x_2}$ wahr sein, also $x_2$ falsch
- **Klausel 4:** $(x_4 \lor \overline{x_1})$ mindestens eine der Variablen $x_4$ oder $\overline{x_1}$ muss wahr sein, d.h. $x_4$ muss wahr sein oder $x_1$ muss falsch sein

**Erfüllung der Bedingungen**:
- Aus Klausel 1 wissen wir, dass $x_3 = 0$
- Aus Klausel 3 folgt, dass $x_2 = 0$
- Aus Klausel 2 folgt, dass $x_1$ wahr sein muss, da $x_2$ falsch ist
- Aus Klausel 4 folgt, dass $x_4$ wahr sein muss, weil $x_1$ nicht falsch sein kann (schon wahr gesetzt wird in Klausel 2)

![SAT Beispiel.png](./Anhang/SAT Beispiel.png)

Der Term ist wahr, wenn $x= (1,0,0,1)$.

### 3SAT-Problem
- Das 3SAT-Problem bezeichnet die Frage, ob logische Terme in konjunktiver Normalform mit maximal (oder genau) drei Literalen erfüllbar sind
- Das Problem ist $NP$-schwer, da das SAT-Problem polynomiell auf das 3SAT-Problem zurückgeführt werden kann: $SAT ≤_{poly} 3SAT$
- Um das zu Beweisen muss man SAT-Problem in ein äquivalentes 3SAT-Problem überführen:
	- Besteht ein Term aus genau drei Termen, so kann er übernommen werden
	- Besteht ein Term aus weniger als drei Termen, so können Literale neutral vervielfältigt werden (z.B. $x_4$ zu $x_4 ∨ x4$)
	- Besteht ein Term aus mehr als drei Termen, können diese mit Hilfsvariablen aufgespalten werden (z.B. $(x_1 ∨ x_2 ∨ x_3 ∨ x_4)$ zu $(x_1 ∨ x_2 ∨ y)\land(\overline{y} ∨ x_3 ∨ x_4)$)[Das Skript erklärt das etwas komplizierter, scheint aber auf das gleiche hinauszulaufen]
- Damit ist das 3SAT-Problem mit dem SAT-Problem auch $NP$-schwer und somit $NP$-vollständig

#### Beispiel
$f(x_1,x_2,x_3,x_4) = \overline{x_3} ∧ (x_1 ∨x_2) ∧ (\overline{x_2} ∨ x_3 ∨\overline{x_2} ∨ x_3) ∧ (x_4 ∨ \overline{x_1})$

**Anwendung der oben genannten Regeln**:
- $\overline{x_3}$ muss auf $(\overline{x_3} ∨\overline{x_3} ∨\overline{x_3})$ verlängert werden
- $(x_1 ∨x_2)$ wird mit $(x_1 ∨x_2 ∨x_2)$ verlängert
- $(\overline{x_2} ∨ x_3 ∨\overline{x_2} ∨ x_3)$ wird in $(\overline{x_2} ∨x_3 ∨y_1)$ und $(\overline{y_1} ∨\overline{x_2} ∨x_3)$ aufgeteilt
- $(x_4 ∨ \overline{x_1})$ wird mit $(x_4 ∨\overline{x_1} ∨\overline{x_1})$ verlängert

$f(x_1,x_2,x_3,x_4,y_1) = (\overline{x_3} ∨\overline{x_3} ∨\overline{x_3}) ∧(x_1 ∨x_2 ∨x_2) ∧(\overline{x_2} ∨x_3 ∨y_1) ∧(\overline{y_1} ∨\overline{x_2} ∨x_3) ∧(x_4 ∨\overline{x_1} ∨\overline{x_1})$

### Teilsummenproblem
- Das Teilsummenproblem oder SSP-Problem (subset sum problem) bezeichnet die Frage, ob es eine nicht-leere Teilmenge $N ⊆ M$ von Zahlen gibt, aus einer Menge von natürlichen Zahlen $M= \{m_1,...,m_n\}$, deren Summe genau einem vorgegebenen Wert $S$ entspricht
- **Einfacher gesagt**: Man hat eine Menge $M$ aus der man sich Zahlen aussucht, die zusammenaddiert bestimmte Zahlen aus einer anderen Menge (Teilsummen $T$) ergeben. Die zusammenaddierten Zahlen sine eine Teilmenge $N$ von $M$
- Das Problem liegt in $NP$, da eine Summe direkt geprüft werden kann

#### Beispiel
Mit einer gegebenen Menge $M = \{2,4,5,11,20\}$ können welche Teilsummen $T∈\{25,34,37\}$ erreicht werden?

- Offensichtlich ist: $20 + 5 = 25$
- Da $34$ gerade ist dürfen entweder nur gerade Zahlen vorkommen, oder beide ungerade Zahlen müssen verwendet werden:
	- Die größte Summe mit nur geraden Zahlen ist $2 + 4 + 20 = 26$
	- Mit ungeraden Zahlen erreicht man entweder $20 + 11 + 5 = 36$, was zu hoch ist, oder $2 + 4 + 11 + 5 = 22$, was zu niedrig ist
	⇒ $34$ ist somit nicht erreichbar
- $37$ ist ungerade und muss somit entweder $5$ oder $11$ enthalten:
	- Mit $5$ erreicht man nur: $20 + 5 + 4 + 2 = 31$
	- Aber mit $11$ erreicht man $20 + 11 + 4 + 2 = 37$
	⇒ $37$ ist also erreichbar

### 3SAT-Problem zu Teilsummenproblem
- Da es sich bei dem Teilsummenproblem um ein $NP$-vollständiges Problem handelt, gibt es keine bekannte Lösung, die in polynomieller Zeit für alle Fälle funktioniert
- Der Grund ist, dass das 3SAT-Problem polynomiell auf das SSP-Problem zurückgeführt werden kann, also $3SAT ≤_{poly} SSP$
- Ein Term eines 3SAT-Problems kann in ein äquivalentes SSP-Problem überführt werden

**Anleitung**:
- Die Anzahl an $x$ gibt die Variablen $n$ an
- Die Anzahl an Klammern die Terme $m$
- Ist ein $x$ in einem 3SAT-Term vorhanden, wird es zu einer $1$, ist es negiert oder nicht vorhanden, wird es zu einer $0$
- Danach werden alle Terme $m$ negiert, wobei die nicht vorhandenen $x$ bei $0$ bleiben
- Man versucht eine Kombination von allen $x$ und $\overline{x}$ zu finden, bei denen die Summen der einzelnen Ziffern zwischen $1$ und $4$ sind (**$0$ geht nicht auf**)
- Am Ende sollte Zielsumme $T = 111\ 44444$ entstehen
- Weil es trotzdem meist nicht genug $1$er für jede $4$ gibt kann man Füllzahlen bzw. -terme verwenden
- Eine Füllzahl kann jede Ziffer um $1$ oder $2$ erhöhen, darf aber pro Ziffer nur einmal verwendet werden (deswegen keine $0$)
- Die Kombination an $x$ und $\overline{x}$ die funktioniert ist die Lösung, wobei $x=1$ und $\overline{x} = 0$
[Das Skript formuliert diese Regeln formeller]

#### Beispiel
$(x_3 ∨ \overline{x_2} ∨ \overline{x_1}) ∧ (x_3 ∨ x_2 ∨ x_3) ∧ (x_1 ∨ \overline{x_3} ∨ \overline{x_2}) ∧ (x_1 ∨ \overline{x_2} ∨ x_3) ∧ (\overline{x_1} ∨ \overline{x_3} ∨ \overline{x_1})$

Für das 3SAT-Problem ergeben sich diese Zahlen (Summanden für die $n=3$) für jede Variable:
![3SAT1.png](./Anhang/3SAT1.png)

Außerdem gibt es die **optionalen** Füllzahlen (Summanden zum Auffüllen für die $m = 5$) für jeden Terme:
![3SAT2.png](./Anhang/3SAT2.png)

Die hier eindeutige Lösung des Teilsummenproblems lautet:
![3SAT3.png](./Anhang/3SAT3.png)

Damit lautet die eindeutige Lösung $x_1 = x_2 = 0$ und $x_3 = 1$.

### Faktorisierung
- Das Problem der Faktorisierung (FACTORIZE) einer ganzen Zahl $n = pq \in \mathbb{Z}$ in zwei ganzzahlige Primfaktoren $p, q \in \mathbb{Z}$ liegt in $NP$
- **Einfach gesagt**: Es bezieht sich auf die Zerlegung einer ganzen Zahl in ein Produkt von kleineren Primzahlen, die als Faktoren bezeichnet werden
- Die Multiplikation von zwei Primfaktoren ist in polynomialer Zeit, bezogen auf die Länge des Produkts durchführbar
- In einem nichtdeterministisches Rechnermodell können alle in Frage kommenden Faktoren parallel in polynomialer Zeit bestimmt werden
- Es ist bisher nicht gelungen für die Faktorisierung $NP$-schwer oder $NP$-vollständig nachzuweisen

### Vereinfachtes Teilsummenproblem
- Ein vereinfachte Teilsummenproblem schränkt das Teilsummenproblem ein, wodurch es aus bestimmten Gründen leichter handhabbar ist
- Einige Eigenschaften sind z.B.:
	- Wenn alle Elemente der Menge positiv sind, kann man sofort schließen, dass keine Teilmenge eine negative oder null Summe haben kann
	- Bei einer geringeren Anzahl von Elementen, lässt sich das Problem oft durch "brute force" lösen
	- Wenn die Summanden $M = \{m_1, . . . , m_n\}$ streng stark anwachsend sind, also größer als die Summe der vorangehenden Summanden sind ("super-increasing knapsack"): $m_k > \sum_{i=1}^{k-1} m_i$

#### Beispiel
Beispiele für ein vereinfachtes Teilsummenprobleme sind die Fragen bei der gegebenen Menge $M = \{1, 2, 6, 10, 20\}$, welche Teilsummen $T \in \{22, 24, 27\}$ aus dieser Menge erreicht werden können. Es kann nun jeweils der Größe nach probiert werden, ob die Zahlen abgezogen werden können.

**So funktionierts**:
1. $22$ durch $20$ teilbar: ja
2. Rest davon durch $10$ oder $6$ teilbar: nein
3. Kommt $0$ raus ist man erfolgreich

![Vereinfachtes Teilsummenproblem Beispiel.png](./Anhang/Vereinfachtes Teilsummenproblem Beispiel.png)

- Damit sind $22 = 20 + 2$ und $27 = 20 + 6 + 1$ und $24$ ist nicht darstellbar
- Es ist auch unmittelbar ersichtlich, wie die Binärzahl $01001_2$ in der Zahl $22$ und die Binärzahl $10101_2$ in der Zahl $27$ eindeutig kodiert wird.

### Merkle-Hellman-Kryptosystem
- In 1978 von Ralph Merkle und Martin Hellman entwickeltes asymmetrisches Verschlüsselungsverfahren, das auf dem super-increasing knapsack basiert
- Adi Shamir veröffentlichte eine Arbeit, die nachwies, dass aus dem öffentlichen Schlüssel effzient passende Zahlen gefunden werden können, die das nur scheinbar sichere Teilsummenproblem wieder in ein vereinfachtes Teilsummenproblem wandeln
- Daher wird das Merkle-Hellman-Kryptosystem nicht mehr verwendet

#### **Schlüsselerzeugung**
- Eine Menge $M=\{m_1​,...,m_n​\}$, die eine superincreasing Sequenz bildet (jede Zahl​ ist größer als die Summe aller vorherigen)
- Zwei zufällige natürliche Zahlen $C,e∈\mathbb{N}$, wobei:
- $C>m_k$​ für alle $m_k$​ in $M$, also $C$ größer als jedes Element der Sequenz ist
- $ggT(C,e)=1$, $e$ ist teilerfremd zu $C$, sodass ein multiplikatives Inverses existiert
- Das multiplikative Inverse von $e$ modulo $C$ ist eine Zahl $d$, sodass gilt: $e×d≡1\ mod\ C$
- Das bedeutet, wenn $e$ und $d$ miteinander multipliziert und dann durch $C$ geteilt werden, der Rest $1$ ist
- Mit $d$ kann man $e$ "rückgängig" machen, wenn man modulo $C$ rechnet
- $d$ wird mit dem erweiterten euklidischen Algorithmus bestimmt

2. **Erstellung der Schlüsselsequenzen**
	- Jedes Element von $M$ wird mit $e$ multipliziert und modulo $C$ reduziert: $w_k​≡ e×m_k\ ​mod\ C$
	- Die resultierende Sequenz $K_{pub}​=(w_1​,...,w_n​)$ ist der öffentliche Schlüssel
	- Der private Schlüssel besteht aus $K_{priv}​=(m_1​,...,m_n​,d,C)$, also der ursprünglichen superincreasing Sequenz und den geheimen Zahlen $d$ und $C$

#### **Verschlüsselung**
- Die zu verschlüsselnde Nachricht wird in eine binäre Zeichenkette der Länge $n$ umgewandelt: $b=(b_1​,b_2​,...,b_n​),b_k​∈\{0,1\}$
- Die Chiffre $u$ ist die gewichtete Summe der Bits mit den öffentlichen Schlüsseln: $u = E(b) = \sum_{k=1}^n b_k w_k$
- Jedes Bit $b_k$​ der Nachricht bestimmt, ob $w_k$​ in die Summe aufgenommen wird

#### **Entschlüsselung**
1. **Rücktransformation in die superincreasing Sequenz**
	- Multipliziere die Chiffre $u$ mit $d$ modulo $C$: $v≡d×u\ mod\ C$
	- Dies stellt sicher, dass die ursprüngliche Summenstruktur aus $M$ zurückgewonnen wird, weil: $v≡d×∑b_k ​w_k\ ​mod\ C$ und $v≡∑b_k​(d×w_k​)\ mod\ C$
	- Da $d×w_k​≡m_k\ ​mod\ C$ gilt, reduziert sich die Summe auf die ursprüngliche superincreasing Sequenz: $v=∑b_k ​m_k​$

2. **Lösen des Teilsummenproblems**
	- Da $M$ superincreasing ist, kann $v$ eindeutig durch die Summe von Teilmengen aus $M$ dargestellt werden
	- Verwende das "Greedy Algorithmus"-Verfahren, um die binären Werte $m_k$​ zurückzuholen:
		- Beginne mit dem größten Wert in der superincreasing Sequenz und subtrahiere ihn von $v$, falls möglich
		- Setze das zugehörige $m_k$​ auf $1$, andernfalls auf $0$

#### Beispiel
- Die Menge $M = \{1, 2, 6, 10, 20\}$ ist die Menge eines vereinfachten Teilsummenproblems mit der Gesamtsumme $39$
- Sei $C = 41$ und $e = 17$, dann ist $ggT(41, 17) = 1$ und $17 \times d ≡ 1\ mod\ 41$

1. $41=2×17+7$
2. $7=2×3+1\ \checkmark$

3. $17=2×7+3$
4. $3=3×1+0$

Den letzten nicht-null Rest (2) rückwärts aufschreiben:
$1=7−2×3$

Setze $3=17−2×7$ (3) ein:
$1=7−2×(17−2×7)$
$1=5×7−2×17$

Setze $7=41−2×17$ (1) ein:
$1=5×(41−2×17)−2×17$
$1=5×41−12×17$

Gleichung umschreiben:
$17×−12≡1\ mod\ 41$

Da $d$ nicht negativ sein darf wird $41$ addiert:
$d=−12+41=29$

Öffentlicher Schlüssel: $K_{pub} = (17, 34, 20, 6, 12)$
Private Schlüssel ist: $K_{priv} = (1, 2, 6, 10, 20, 29, 41)$

Soll nun die Nachricht $21 = 10101_2$ verschlüsselt werden, so ergibt sich
$u = E(21) = 1 \times 17 + 0 \times 34 + 1 \times 20 + 0 \times 6 + 1 \times 12 = 49$

Die Nachricht kann dann mit Hilfe des privaten Schlüssels mit $v = 49 \times 29 ≡ 27\ mod\ 41$ und dann wie im Beispiel zuvor
$27 - 1 \times 20 = 7$
$7 - 0 \times 10 = 7$
$7 - 1 \times 6 = 1$
$1 - 0 \times 2 = 1$
$1 - 1 \times 1 = 0$
zu $10101_2 = 21$ dechiffriert werden.

## Beschreibung von Algorithmen 3.3
- Bei der Frage, ob ein allgemeiner Boole'scher Ausdruck lösbar ist, liegt der Fokus auf der Problemstellung
- Bei der Frage, wie das Problem gelöst werden kann, liegt der Fokus auf der Lösungsmethode
- Ist eine Lösungsmethode allgemein anwendbar und eindeutig beschreibbar, so geht es um Algorithmen

### Programmablaufplan (PAP)
- Stellt den Ablauf eines Programms mit Hilfe eines gerichteten Graphen mit unterschiedlichen Knotentypen dar
![Knotentypen.png](./Anhang/Knotentypen.png)

#### Beispiel
Algorithmus für den größten gemeinsamen Teiler $ggT(a, b)$ (größte natürliche Zahl, die $a$ und $b$ teilt)

![Programmablaufplan.png](./Anhang/Programmablaufplan.png)

Eingabe: Natürliche Zahlen $p$, $q$
Ausgabe: Ganzzahl $ggT\ g$
1. Ermittele Minimum $m$ von $p$, $q$
2. Zähle $z$ absteigend von $m$ bis $1$
3. Prüfe, ob $p$ und $q$ sich ohne Rest durch $z$ teilen lassen
4. Wenn ja, so ist $g=z$ und Ende, sonst mit nächstem $z$ mit Schritt 3
```Python [Kein Python Code]
Algorithmus ggT-Naiv(p, q)
	z = min(p, q)
	while p mod z ≠ 0 or q mod z ≠ 0 do
		z = z - 1
	return z
```
[Es gibt auch den Euklidischen Algorithmus, den ich aus Zeitgründen überspringe]

### Eigenschaften von Algorithmen
**Allgemeinheit**: Algorithmen sollten eine Problemklasse und nicht nur ein spezifisches Problem lösen. Das bedeutet, er sollte in der Lage sein, mit verschiedenen Eingabedaten umzugehen und trotzdem das korrekte Ergebnis zu liefern.
**Ausführbarkeit**: Jeder Schritt eines Algorithmus muss (in endlicher Zeit) ausführbar sein. Z.B. durch ein theoretisches Rechnermodell wie die Turingmaschine.
**Determinismus**: Die Ausführung jedes Schrittes ist eindeutig und festgelegt, also nicht zufällig oder von Ein-/Ausgabe abhängig. Jede Eingabe liefert immer die gleiche Ausgabe.
**Determiniertheit**: Gleiche Eingangswerte durchlaufen die gleichen Schritten, was bei erneuter Ausführung den gleichen Ausgangswert liefert. Trifft nicht zu oder führt zu Problemen bei: Absichtlichem Zufall, probabilistische Verfahren, paraller Ausführung (Synchronisation), Quantencomputer oder kosmischer Strahlung
**Finitheit**: Die Beschreibung bzw. Anzahl von Anweisungen ist endlich. Selbstverständlich bei endlich dargestellten Algorithmen, jedoch nicht für algorithmisch beschriebene Algorithmen oder selbst modifizierendem Algorithmen.
**Terminierung**: Die Ausführung stoppt bei endlicher Eingabe nach einer endlichen Anzahl von Schritten (keine Endlosschleife). Wenn die Wahrscheinlichkeit, dass ein Algorithmus nicht terminiert gegen null läuft, ist er terminiert.
**Dynamische Finitheit**: Die Ausführung hat beschränkten bzw. endlichen Ressourcenbedarf (Speicher oder Rechenzeit) bei endlicher Eingabe. Besteht die Chance, dass unendlich viele Ressourcen verbraucht werden, ist ein Algorithmus dynamisch finit.
**Komplexität**: Die Laufzeit oder der Ressourcenbedarf ist in Abhängigkeit von der Eingabe funktional abschätzbar. Wird häufig in Bezug auf Zeitkomplexität (wie lange dauert die Ausführung?) und Raumkomplexität (wieviel Speicherplatz wird benötigt?) betrachtet.

#### Zusammengefasst
1. **Allgemeinheit**: Anwendbar auf verschiedene Problemfälle
2. **Ausführbarkeit**: Jeder Schritt ist in endlicher Zeit machbar
3. **Determinismus**: Jeder Schritt ist eindeutig und festgelegt
4. **Determiniertheit**: Gleiche Eingangswerte liefern gleiche Ausgangswert
5. **Finitheit**: Die Beschreibung ist endlich
6. **Terminierung**: Stoppt nach einer endlichen Anzahl von Schritten
7. **Dynamische Finitheit**: Ausführung braucht endlich Ressourcen
8. **Komplexität**: Ressourcenbedarf ist abschätzbar

#### Beispiel
1. Auf einem quadratischen Gitter der Größe $n×n$ Knoten soll startend von ganz links unten die Weglänge in Kanten nach ganz rechts oben gemessen werden. In jedem Schritt wird zufällig nach rechts oder oben gegangen, wenn dort eine Kante existiert, und der Schritt gezählt. Die Ausgabe ist die Anzahl erforderlicher Schritte, wenn der obere rechte Knoten des zu messenden Gitters erreicht wird.

- Algorithmus kann ausgehend von $x = (1,1)$ zufällig Schritte auswählen und erste oder zweite Komponente erhöhen, falls die Kante vorhanden ist, bis $(n, n)$ erreicht ist
- Algorithmus ist **ausführbar**, wegen der Zufallskomponente **nicht deterministisch**
- Ergebnis ist **determiniert** auf $2n$
- Beschreibung ist **finit**, wird **terminieren** und ist auch **dynamisch finit**

2. Das zu messende Gitter ist Teil eines unendlichen in alle Richtungen ausgedehnten Gitters, Schritte nach oben und rechts sind also immer möglich. Das Vorgehen zum Messen startend von links unten nach rechts oben ist wie zuvor.

- Algorithmus kann wie zuvor gestaltet werden, doch die Abfrage, ob eine Kante vorhanden ist, fällt weg
- Algorithmus ist weiterhin **ausführbar** und **nicht deterministisch** und Beschreibung ist **finit**
- Algorithmus **terminiert** nur dann, wenn der Zielknoten erreicht wird
- Nur dann **determiniert** auf $2n$, wenn es terminiert
- Nicht **dynamische finit**, weil der Zähler für die Kanten über alle Grenzen wachsen kann

3. Das zu messende Gitter ist Teil eines $2n× 2n$ Knoten großen Gitters, dessen Enden rechts mit den linken Knoten und oben mit den unteren Knoten verbunden sind, das auf diese Weise einen Torus bildet. Das Vorgehen zum Messen startend von links unten nach rechts oben ist wie zuvor.

- Wie zuvor kann der Algorithmus gestaltet werden, jedoch nach $2n$ in einer Komponente wird im nächsten Schritt bei Erhöhung die Komponente auf $0$ gesetzt
- Algorithmus ist weiterhin **ausführbar** und **nicht deterministisch** und Beschreibung ist **finit**
- Ergebnis ist **nicht determiniert**, da Vielfache $2n$ erreicht werden können
- Die Wahrscheinlichkeit, dass der Algorithmus nicht **terminiert** läuft gegen $0$, aber es gibt keine obere Schranke auf die Laufzeit
- **Dynamisch finit** ist das Verfahren nicht, da die Laufzeit beliebig lang sein kann

## Rekursion und Iteration 3.4
- Zur Lösung vieler Problemstellungen werden Wiederholungen benötigt
- Es gibt verschiedene Umsetzungsmöglichkeiten, wie Rekursion, Turing-Vollständigkeit oder iterativen und imperativen for, while, do-while oder repeat-until-Schleifen
- Eine Schleife ist eine Kontrollstruktur in Algorithmen, die eine bedingte wiederholte Ausführung von einzelnen Ausführungsschritten darstellt
- Eine einzelne Durchführung wird als Iteration bezeichnet
- Kopfgesteuerte Schleife oder while-Schleife: Bedingung wird zu Beginn und vor erster Iteration geprüft
- Fußgesteuerten Schleife oder do-while-Schleife (auch repeat-until-Schleife): Bedingung nach einer Iteration geprüft, ob eine weitere Durchführung erfolgen kann
- Die verschiedenen Schleifenarten können in die andere umgewandelt werden, indem z.B. die erste Iteration vor der Schleife passiert (Fuß. → Kopf.)
- Ein Algorithmus ist rekursiv, wenn in der Beschreibung des Algorithmus der Algorithmus selbst als ein Ausführungsschritt aufgerufen wird

**Iterative Schleife**:
```Python [Kein Python Code]
Algorithmus IterativeWhile(state)
	while condition(state) do
		state = iterate(state)
	return state
```
**Rekursive Schleife**:
```Python [Kein Python Code]
Algorithmus RecursiveWhile(state)
	if condition(state) then
		return RecursiveWhile(iterate(state))
	return state
```
### Beispiel
Die Fibonacci-Zahlen $1, 1, 2, 3, 5, 13,...$ sind definiert durch

$$
a\_k = \begin{cases} 1, & \text{für } k \leq 2 \\ a\_{k-1} + a\_{k-2}, & \text{sonst} \end{cases}
$$

**Rekursiver Algorithmus zur Berechnung der Fibonacci-Zahlen**:
```Python [Kein Python Code]
Algorithmus fib(k)
	if k < 3 then
		return 1
	else
		return fib(k - 1) + fib(k - 2)
```
$fib(3) = fib(2) + fib(1) = 1 + 1 = 2$
$fib(4) = fib(3) + fib(2) = fib(2) + fib(1) + fib(2) = 1 + 1 + 1 = 3$
$fib(5) = fib(4) + fib(3) = fib(3) + fib(2) + fib(2) + fib(1) = ...$

*In diesem imperativem Ausführungsmodell steigt die Anzahl der durchgeführten Auswertungen exponentiell, da frühere Berechnungen wieder neu ausgeführt werden.*

**Linear rekursiver Algorithmus zur Berechnung der Fibonacci-Zahlen**:
```Python [Kein Python Code]
Algorithmus fib2(k, i = 2, ai = 1, ai1 = 1)
	if k > i then
		return fib2(k, i + 1, ai + ai1, ai)
	else if k= i then
		return ai
	else
		return ai1
```
$fib2(5) = fib2(5, 2, 1, 1)$
$= fib2(5, 3, 2, 1)$
$= fib2(5, 4, 3, 2)$
$= fib2(5, 5, 5, 3) = 5$

*Indem der doppelte Aufruf durch einen einzelnen Aufruf ersetzt wird, müssen Berechnungen kein zweites mal ausgeführt werden, was Ressourcen schont.*

## Algorithmische Korrektheit 3.5
- Der Beweis der Korrektheit ist Eine Methode um zu prüfen, ob Algorithmen die Lösung auch bestimmen können
- Grundsätzlich gibt es mehrere Möglichkeiten die Korrektheit eines Algorithmus zu beweisen
- Das Hoare-Kalkül ist dabei eine systematische Vorgehensweise, um auf Ebene der einzelnen Algorithmenschritte die Korrektheit nachzuweisen

**Hoare-Tripel bestehen aus**:
- Präposition oder Vorbedingung $P$
- Zustände, einer Anweisung $S$
- Konklusion oder Nachbedingung $K$

$$
P\ \{\ S\ \}\ K
$$

*$K$ wird nach Ausführung aus $S$ mit der $P$ gefolgert*[?]

**Partielle Korrektheit**: Falls Programm terminiert (nicht garantiert) und $K$ korrekt ist
**Totale Korrektheit**: Ein Programm wird terminieren (garantiert) und $K$ ist korrekt

*Totale Korrektheit setzt immer partielle Korrektheit voraus.*

### Komposition
- Kombination mehrerer aufeinanderfolgender Anweisungen
- Komposition zweier Hoare-Tripel $P_1\ \{\ S_1 \}\ K_1$ und $P_2\ \{\ S_2 \}\ K_2$ ergibt ein Hoare-Tripel $P_1\ \{\ S_1;S_2 \}\ K_2$
- Wenn $P_2$ aus $K_1$ folgt oder gleich sind und $S_2$ nach $S_1$ ausgeführt wird, sind $K_1$ und $P_2$ Zwischenbedingungen

![Komposition.png](./Anhang/Komposition.png)

### Iteration
- Das Hoare-Tripel einer Iteration wird mit einer Schleifenbedingung $B$ und einer Invariante $I$ bewiesen
- $B$ ist eine logische Aussage, die bei jedem Durchlauf einer Schleife überprüft wird und $S$ so lange ausführt, bis $B$ nicht mehr erfüllt ist (kann auch endlos laufen → Partielle Korrektheit)
- $I$ ist eine Aussage, die dauerhaft wahr ist, um Korrektheit der Schleife zu beweisen
- Bei $I\ \land\ B\ \{\ S\ \}\ I$ folgt das Hoare-Tripel der Schleife über $S$ solange $B$ gilt
- Um eine geeigneten Invariante zu bestimmen, hilft es, eine Schleifen auszuführen und die Eigenschaften zu beschreiben, die immer vor und damit auch nach einer Iteration vorliegen

![Iteration.png](./Anhang/Iteration.png)

### Fallunterscheidung
- Je nachdem ob $B$ wahr ist, wird $S_1$ oder $S_2$ ausgeführt
- $K$ der Fallunterscheidung ist eine Hoare-Tripel, weil es in beiden Fällen $P \land B$ oder $P \land ¬B$ durch Ausführen von $S_1$ oder $S_2$ K erfüllt wird

![Fallunterscheidung.png](./Anhang/Fallunterscheidung.png)

### Beispiel
Bestimmen zu diesem Algorithmus für $n \in \mathbb{N}$ zur Berechnung der Summe der Zahlen von $1$ bis $n$ die Schleifeninvariante und beweisen Sie die Korrektheit des Algorithmus nach Hoare-Kalkül.
```Python [Kein Python Code]
1. Algorithmus summe(n)
2.	s = 0
3.	i = n
4.	while i > 0 do
5.		s = s + i
6.		i = i−1
7.	return s
```
Eine mögliche Schleifeninvariante lautet:
$n \in \mathbb{N} \land s = \frac{n^2}{2}+\frac{n}{2}-\frac{i^2}{2}-\frac{i}{2} = \sum_{k=1}^n k - \sum_{k=1}^i k$

`1. Algorithmus summe(n)`
Vorbedingung: $n∈\mathbb{N}$
`2.	s = 0`
Zwischenbedingung: $n∈\mathbb{N} ∧ s = 0$
`3.	i = n`
Zwischenbedingung: $n∈\mathbb{N} ∧ s = 0 ∧ i = n$
Invariante: $n∈\mathbb{N} ∧ s = \frac{n^2}{2}+\frac{n}{2}-\frac{i^2}{2}-\frac{i}{2}$
`4.	while i > 0 do`
Vorbedingung: $n∈\mathbb{N} ∧ s = \frac{n^2}{2}+\frac{n}{2}-\frac{i^2}{2}-\frac{i}{2} ∧ i > 0$
`5.		s = s + i`
Zwischenbedingung: $n∈\mathbb{N} ∧ s = \frac{n^2}{2}+\frac{n}{2}-\frac{(i-1)^2}{2}-\frac{i-1}{2} ∧ i > 0$
`6.		i = i−1`
Nachbedingung: $n∈\mathbb{N} ∧ s = \frac{n^2}{2}+\frac{n}{2}-\frac{i^2}{2}-\frac{i}{2} ∧ i \geq 0$ (`while` Ende)
Nachbedingung: $n∈\mathbb{N} ∧ s = \frac{n^2}{2}+\frac{n}{2} ∧ i = 0$
`7.	reurn s`

[Ich check nicht wie man auf die Invariante gekommen ist]

Hoare-Tripel bewiesen und (partiell) korrekt. Ist nach einer Iteration B wahr, so ist das Hoare-Tripel bewiesen und (total) korrekt.

# Deklarative Programmierung
## Definitionen
Paradigmen

## Paradigmen 4.1
- **Deklarative Programmiermodell**: Stellt die Beschreibung von Zusammenhängen, Fragestellungen oder erwartete Lösung in den Vordergrund
- Die eigentliche Bestimmen der Lösung ergibt sich aus den Beschreibungen, wobei die tatsächliche Auswahl und Reihenfolge der Lösungsschritte dem Ausführungsmodell überlassen werden
- **Imperative Programmiermodell**: Stellt die genaue Beschreibung der Lösungsschritte in den Vordergrund
- Im deklarativen Programmiermodell werden besonders logische und funktionale Modelle unterschieden

Die
Abbildung 4.1.1 versucht eine zeitliche Entwicklung und Einflüsse der Paradigmen und Programmierspra-
chen in einem unvollständigen Überblick darzustellen. 

Da Sprachen über viele Jahre weiterentwickelt
werden, werden die Sprachen inzwischen auch Paradigmen zugeordnet, die zum dargestellten ersten
Einführung noch kein Thema waren, wie beispielsweise die Objekt-Orientierung in Ada.

Im deklarativen Programmiermodell werden besonders die logischen und das funktionalen Modelle un-
terschieden. Das Logische Programmiermodell basiert auf einer regelbasierten Datenbasis, aus der
Ziele als logische Folgerungen aus der Datenbasis abgeleitet werden. 

Die Sprache Prolog ist ein wichtiges Beispiel für dieses Modell. Das Funktionale Programmiermodell identifiziert alle Fragestellungen
als funktionale und ideal nebenwirkungsfreie Auswertungen, wodurch Zusammenhänge durch ihre funk-
tionalen Abhängigkeiten beschrieben werden, deren Auswertungsreihenfolge und Auswertungszeitpunkt
aber nicht festgelegt wird. Liegt eine Nebenwirkungsfreiheit vor, so sind einmal getätigte Funktionsaus-
wertungen allgemein gültig und können jederzeit wieder eingesetzt werden. Sehr früh wurden funktionale
Konzepte in der Programmiersprache LISP konzipiert, inzwischen ist die Sprache Haskell ein wichtiger
Vertreter dieses Programmiermodell. Weiterhin werden viele domänenspezifische Sprachen eher dem
deklarativen Modell zugeordnet, wie SQL oder Make.

Im imperativen Programmiermodell gibt es eine Vielzahl von sich teilweise überschneidenden Konzepten.
Die Programmiersprachen ALGOL und Pascal werden zentral dem imperativen Konzept zugeordnet, da
die schrittweise Beschreibung von Algorithmen ein zentraler Aspekt ist. Das Prozeduale Programmier-
modell legt einen zusätzlichen Fokus auf die Strukturierung von Algorithmenanteilen in Prozeduren mit
lokalen Variablen. Das Modell wird besonders durch BCPL und C eingesetzt. Das Objekt-Orientierte
Programmiermodell fokussiert sich auf den unmittelbaren Zusammenhang zwischen Datenstrukturen,
deren verarbeitenden Methoden und Abhängigkeiten von Datenmodellen. Dieses Konzept wird besonders
auf die Sprachen Simula und Smalltalk zurückgeführt und hat viele moderne Programmiersprachen
entscheidend beeinflusst.
Im Folgenden werden in Ergänzung zu den klassischen Programmiervorlesungen zu imperativen Pro-
grammiersprachen zwei wichtige Konzepte der deklarativen Programmierung vorgestellt.

![Entwicklung von Programmiersprachen und Paradigmen.png](./Anhang/Entwicklung von Programmiersprachen und Paradigmen.png)











