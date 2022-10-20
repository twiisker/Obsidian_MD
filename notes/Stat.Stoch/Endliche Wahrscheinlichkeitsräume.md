## Definition
1. Grundraum $\Omega + \varnothing$ = Menge von Ergebnissen
2. System |A von Teilmengen von Omega; Mengenalgebra A
   $A \in \mathbb{A}$ Ereignis: $|A|$ = 1 : Elementarereignis
   $A \in \mathbb{A}$ Würfelzahl gerade: A = {2,4,6}
   $B \in \mathbb{A}$ Würfelzahl durch 3 teilbar B = {3,6}
   Mengen. $\mathbb{A} = \{\{\},\{1\},\{2\},\{3\},...,\{1,2\},\{1,3\},...\{1,2,3,4,5,6\}\}$ 
   $\{\} \leftarrow$ Leere Menge $\varnothing$ (unmögliches Ergebnis)
   $\{1,2,3,4,5,6\} \leftarrow \Omega$ (sicheres Ereignis)}
3. Wahrscheinlichkeitsverteilung
   $\mathbb{P} : \mathbb{A} \rightarrow \mathbb{R}$

## Arbeiten mit W-Räumen
Ereignisse = Mengen
- $A \cap B = \{6\}$
- $A \cup B = \{2,3,4,6\}$
- $B \setminus A = \{3\}$  (durch 3 Teilbar aber nicht gerade)
- $\overline{\rm A}:=\Omega \setminus A=\{1,3,5\}$

### Neue Schreibweise
- $A \cup B: A + B$
	- falls unvereinbar, disjunkt, $\Leftrightarrow A \cap B = \varnothing$
- Forderung an $\mathbb{A}$: abgeschlossen unter {schnitt, vereinigung, ohne, komplement}

## Lernzielkontrolle
Homework! Folie 7

## Axiome des endlichen W-Raums

- (A1): Nichtnegativität: $\mathbb{P}(A) \geq 0$
- (A2): Normiertheit: $\mathbb{P}(\Omega) = 1$
- (A3): Additivität im Fall unvereinbarer Ereignisse: $\mathbb{P}(A+B) = \mathbb{P}(A) + \mathbb{P}(B)$

### Folgerungen

- Unmögliches Ereignis hat Wahrscheinlichkeit 0:
  $$1 = \mathbb{P}(\Omega) = \mathbb{P}(\Omega + \{\}) = \mathbb{P}(\Omega) + \mathbb{P}(\{\}) = 0$$
						    (A2)                                              (A3)
- (Endliche) Additivität für unvereinbare Ereignisse a1,....,an:
  (A3) + vollst. Induktion
- Wahrscheinlichkeiten sind immer zwischen 0 und 1:
  (A1)   $$0 \in \mathbb{P}(A) \leq 1$$
  $$A \subseteq \Omega : \overline{A} \Rightarrow \Omega = A + \overline{A}$$
- Komplementäre Wahrscheinlichkeit (Gegenereignis)
  (A1)$$1 = \mathbb{P}(\Omega) = \mathbb{P}(\overline{A} + A) = \mathbb{P}(\overline{A}) + \mathbb{P}(A)$$
- Monotonie
  $$B = A + (B \setminus A)$$
  $$\mathbb{P}(B) = \mathbb{P}(A) + \mathbb{P}(B \setminus A)$$
- Additionsgesetz nicht notwendigerweise disjunkter Mengen
  $$A \cup B = (A\setminus B) + (A \cap B) + (B\setminus A)$$
  $$\mathbb{P}(A) = \mathbb{P}(A \cap B) + \mathbb{P}(A \setminus B)$$
  $$\mathbb{P}(B) = \mathbb{P}(A \cap B) + \mathbb{P}(B \setminus A)$$
- Subadditivität für nicht notwendigerweise disjunkte Mengen
  Über vorheriges + Induktion über $n = |\Omega|$
  
- Siebformel: Für alle A1,A2,A3 Teilmenge Omega gilt:
  A1 + A2 + A3 - doppelte Mengen + die zuviel abgezogene Menge

## Verteilung $\mathbb{P}$ spezifizieren
~~Über $\mathcal{P}(\mathbb{A})$ spezifizieren: ?? müssen wir nicht~~
es genügt:
Definition: $$p: \Omega \rightarrow [0, 1]$$mit Elementarereignisse.

für alle Ereignisse $A \subseteq \Omega: \mathbb{P}(A) = \sum_{w \in A} p(w)$
wird nahegelegt durch Axiom 3

### Beispiel Oktaeder (1W8)
$\Omega = \{1,2,3,4,5,6,7,8\}  \mathbb{A} = \mathcal{P}(\Omega)$
$\mathbb{P} \ über \ p: p(i) = \frac{1}{8}, i= 1,-,8$  (fair!)

Ereignis "prim" $A_{1} = \{2,3,5,7\}$
$\mathbb{P}(A_{1}) = \mathbb{P}\{2,3,5,7\} = \sum_{w \in A_{1}}, p(w) = p(2) + p(3)+p(5)+p(7) = 4 * \frac{1}{8} = \frac{1}{2}$

## Lernzielkontrolle
Homework! Folie 17

# Zufallsvariable, Verteilung
ZV: $X : \Omega \rightarrow \mathbb{R}$  ,W-Raum($\Omega, \mathbb{P}$)
Verteilung $\mathbb{P}^X: \mathcal{P}(X(\Omega)) \rightarrow \mathbb{R}$
$\mathbb{P}^X(B) := \mathbb{P}(X^{-1}(B))$ , $B \subseteq X(\Omega) \Rightarrow (X(\Omega)), \mathbb{P}^X$ endlicher W-Raum
$X^{-1} (B) = {w \in \Omega * X(w) \in B} \subseteq \Omega$
 
### Schreibweise
$\{X = x\} := X^{-1}(\{x\})$
$\mathbb{P}(X = x) := \mathbb{P}(\{X=x\}) = \mathbb{P}(X^{-1}({x}))$
$\mathbb{P}(a \leq X \leq b) := \mathbb{P}(a \leq X \leq b) = \mathbb{P}(X^{-1}([a,b]))$

### Beispiel Oktaeder
| $w \in \Omega$ | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 |
| ------------ | -- | -- | --| -- | -- | -- | -- |
| $X(\{w\})$ | 2 | 2 |6 |4 |10| 6 |14 |8

ZV: X := {2i, i ungerade}
             {i, i gerade}

$$X(\Omega) = \{2,4,6,8,10,14\}$$
$$\mathbb{P}^{X} ({2}) = \mathbb{P}(X^{-1}({2})) = \mathbb{P}({1,2}) = \frac{2}{8}$$

| $\tilde{w} \in \Omega$ | 2 | 4 | 6 | 8 | 10 | 14 |
| ------------ | -- | -- | --| -- | -- | -- |
| $X^{-1}(\{\tilde{w}\})$ | {1,2} | {4} | {3,6} | {8} | {5} | {7} |
|$P^{X}(\{\tilde{w}\})$ | 1/4 | 1/8 | 1/4 | 1/8 | 1/8 | 1/8 |

## Verteilungsfunktion

![[Verteilungsfunktion.jpg]]


## Lernzielkontrolle
Homework! Folie 20


## Erwähnung
Laplace - Experiment
Gleichverteilung