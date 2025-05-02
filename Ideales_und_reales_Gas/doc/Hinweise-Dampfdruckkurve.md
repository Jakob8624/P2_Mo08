# Hinweise für den Versuch: **Ideales und reales Gas** 

## Phasendiagramm und Dampfdruckkurve

Übergänge der einzelnen Phasen 

- fest, 
- flüssig und 
- gasförmig 

eines Stoffes werden durch [**Phasendiagramme**](https://de.wikipedia.org/wiki/Phasendiagramm) dargestellt. In einem abgeschlossenen Volumen $V$ gibt es, für eine gegebene Temperatur $T$, jeweils nur einen bestimmten Druck $p(T)$, bei dem zwischen zwei Phasen eines Stoffes ein thermodynamisches Gleichgewicht herrscht. Ein thermodynamisches Gleichgewicht zwischen allen drei Phasen eines Stoffs existiert nur an einem einzigen Punkt im Phasendiagramm, dem **Tripelpunkt**. 

Das Phasendiagramm für den **Übergang von flüssig zu gasförmig heißt Dampfdruckkurve**. Für einen reversiblen Kreisprozess (Carnot-Prozess) gilt allgemein:

$$
\begin{equation*}
\frac{\mathrm{d} W}{\mathrm{d}T} = -\frac{Q}{T}.
\end{equation*}
$$
Mit $\mathrm{d}W = \left(V_{\mathrm{fl}}-V_{\mathrm{gas}}\right)\mathrm{d}p$ und den Volumina $V_{\mathrm{fl}}$ und $V_{\mathrm{gas}}$, die ein gegebener Stoff in flüssigem und gasförmigem Zustand einnimmt, wird daraus die [Clausius-Clapeyron-Gleichung](https://de.wikipedia.org/wiki/Clausius-Clapeyron-Gleichung): 

$$
\begin{equation}
\frac{\mathrm{d}p}{\mathrm{d}T} = \frac{Q}{T\,\left(V_{\mathrm{gas}} - V_{\mathrm{fl}}\right)}.
\end{equation}
$$
Man benötigt also die Wärme $Q$, um bei der Temperatur $T$ eine Flüssigkeit mit dem Volumen $V_{\mathrm{fl}}$ in ein Gas mit dem Volumen $V_{\mathrm{gas}}$ zu überführen. 

Für die weiteren Betrachtungen machen wir die Annahme 

$$
\begin{equation*}
V_{\mathrm{fl}}\ll V_{\mathrm{gas}}
\end{equation*}
$$
 und betrachten den Dampf als ideales Gas mit 

$$
\begin{equation*}
V_{\mathrm{gas}} = \frac{n\,R\,T}{p},
\end{equation*}
$$
womit Gleichung **(1)**, nach **Separation der Variablen**, die folgende Form annimmt: 

$$
\begin{equation}
\begin{split}
&\frac{\mathrm{d}p}{p} = \frac{Q}{n\,R}\,\frac{\mathrm{d}T}{T^{2}} \\
&\\
&p(T) = p_{0}\exp\left(-\frac{Q}{n\,R\,T}\right). \\
\end{split}
\end{equation}
$$
Bei Gleichung **(2)** handelt es sich um die zu erwartende funktionale Form der Dampfdruckkurve für ein ideales Gas.

## Essentials

Was Sie ab jetzt wissen sollten:

- Sie sollten die **Clausius-Clapeyron-Gleichung erkennen und inhaltlich verstehen**. 
- Sie sollten unter den oben gemachten Annahmen aus Gleichung **(1)** die **erwartete Form der Dampfdruckkurve herleiten können**.

## Testfragen

1. Gibt es bei einem Idealen Gas den Übergang von gasförmig in flüssig?
2. Wie verändert sich Ihre Erwartung für $p(T)$, wenn Sie statt eines idealen Gases ein [reales Gas](https://de.wikipedia.org/wiki/Clausius-Gleichung) nach Clausius-Gleichung zugrundelegen?
3. Wie sieht das Diagramm einer Dampfdruckkurve aus, wenn man es auf alle drei Phasen, fest, flüssig und gasförmig erweitert?
4. Hat jedes Phasendiagramm einen Tripelpunkt?

# Navigation

[Main](https://gitlab.kit.edu/kit/etp-lehre/p2-praktikum/students/-/tree/main/Ideales_und_reales_Gas)

