# Hinweise für den Versuch **Vakuum**

## Wärmeleitungs-Vakuummeter ($10^{-4}\lesssim p \lesssim 10^{3}\ \mathrm{mbar}$)

Das Wärmeleitungs- oder [Pirani-Vakuummeter](https://de.wikipedia.org/wiki/Pirani-Vakuummeter) nutzt die Abhängigkeit der Wärmeleitung von Gasen vom Druck. Im Vakuum befindet sich ein (meist aus Wolfram oder Nickel bestehender) Messdraht, der Bestandteil einer [Wheatstoneschen Messbrücke](https://de.wikipedia.org/wiki/Wheatstonesche_Messbr%C3%BCcke) ist. Der Widerstand $R$ des Drahts hängt von dessen Temperatur $\vartheta$ ab. Die am Draht anliegende Spannung wird so geregelt, dass $R=const$ gilt. Die dabei aufzuwendende elektrische Leistung entspricht im thermischen Gleichgewicht der abgeführten Wärmeleistung des Drahts. Abhängig vom Druck lässt sich die abgeführte Wärmeleistung in drei Bereiche aufteilen: 

- $p\lesssim10^{-4}\ \mathrm{mbar}$: Hier erfolgt der Wärmegang **unabhängig von $p$ vor allem durch Wärmestrahlung** des Drahtes, sowie Wärmeableitung an den Drahtenden. 
- $10^{-4}\lesssim p \lesssim 1\ \mathrm{mbar}$: Hier erfolgt der Wärmegang vor allem durch die **Wärmeleitung im Gas. Diese ist i.a. linear von p abhängig**. 
- $1\lesssim p\lesssim 10^{3}\ \mathrm{mbar}$: Hier erfolgt der Wärmegang durch **Konvektion**. Obwohl auch dieser i.a. unabhängig von $p$ ist gelingt es durch die Dimensionierung der Messsonde auch hier eine Abhängigkeit von $p$ zu realisieren, die jedoch i.a. nicht mehr linear ist und somit linearisiert werden muss. 

Wärmeleitungs-Vakuummeter sind daher über einen weiten Bereich von $10^{-4}\lesssim p \lesssim 10^{3}\ \mathrm{mbar}$ einsetzbar, in dem sie im %-Bereich reproduzierbare Drucke wiedergeben. 

Für die eingesetzen Geräte ([THERMOVAC Transmitter TTR91](https://gitlab.kit.edu/kit/etp-lehre/p2-praktikum/students/-/blob/main/Vakuum/doc/LeyboldTN91_Tansducer.pdf)) macht der Hersteller die folgenden Angaben zur Messgenauigkeit: 

- $5\times10^{-4}\lesssim p \lesssim 10^{-3}\ \mathrm{mbar}$: $\pm10\%$ (of reading);
- $10^{-3}\lesssim p \lesssim 10^{2}\ \mathrm{mbar}$: $\pm5\%$ (of reading);

- $10^{2}\lesssim p \lesssim 10^{3}\ \mathrm{mbar}$: $\pm25\%$ (of reading);
- $10^{-3}\lesssim p \lesssim 10^{2}\ \mathrm{mbar}$: $\pm2\%$ (or reading) Reproduzierbarkeit;

## Ionisations-Vakuummeter ($10^{-8}\lesssim p\lesssim 10^{-3}\ \mathrm{mbar}$)

[Ionisations-Vakuummeter](https://de.wikipedia.org/wiki/Ionisations-Vakuummeter) basieren auf der Abhängigkeit des elektrischen **Entladungsstroms** einer evakuierten Diode von der Restteilchenzahldichte $n$. 

Aus einer Kathode werden unter Hochspannung Elektronen emittiert und im Feld der Hochspannung beschleunigt. Die Elektronen ionisieren die Restgasteilchen durch Stöße. Diese wandern als positiv geladene Ionen zur Kathode. Dort können Sie haften bleiben oder beim Auftreffen Material aus der Kathode ausschlagen (Kathodenzerstäubung). Das ausgeschlagene Material schlägt sich dann an den Wänden des Messgeräts nieder. Durch diesen Prozess wird die Kathode langsam verbraucht. Sie ist daher i.a. austauschbar.

Um auch bei sehr niedrigen Drucken und sehr kleinen $n$ einen messbaren Ionisationsstrom zu garantieren können die Elektronen durch ein zusätzlich angelegtes Magnetfeld auf eine Spiralbahn gezwungen werden, um ihren Weg durch die Ionisationskammer und damit die Wahrscheinlichkeit für Stöße mit Restgasteilchen zu erhöhen. Man bezeichnet dieses Vorgehen als invertiertes Magnetron-Prinzip und ein Messgerät, das nach diesem Prinzip funktioniert als Penning-Vakuummeter. Bei dem eingesetzten Gerät (PENNINGVAC PTR 225) handelt es sich um ein Penning-Kaltkathoden-Vakuummeter. 

Die Messgenauigkeit gibt der Hersteller mit $\pm30\%$ im Bereich $10^{-8}\lesssim p\lesssim 10^{-3}\ \mathrm{mbar}$ an.  

## Kalibration von Vakuummetern

Alle Vakuummeter müssen vor Betrieb kalibiert werden. Hierzu dienen *statische Verfahren* mit bekannten Messgeräten (z.B. U-Rohrmanometern, wie Sie sie im P2-Versuch [Ideales und reales Gas](https://gitlab.kit.edu/kit/etp-lehre/p2-praktikum/students/-/tree/main/Ideales_und_reales_Gas) sehen können) oder *dynamische Verfahren* mit Hilfe von Pumpen mit bekanntem Saugvermögen. 

### Dynamisches Kalibrationsverfahren

Ein einfaches **dynamisches Kalibrationsverfahren** würde z.B. wie folgt ablaufen:

- Sie statten einen Rezipienten R1 mit regelbarem Belüftungsventil und einem Referenzdruckmessgerät G1 aus. 

- Sie verbinden R1 über ein Rohr mit bekanntem Leitwert $L$ mit einem zweiten Rezipienten R2, an dem sich das zu kalibierende Messgerät und eine Pumpe P2 mit bekannter, hoher effektiver Saugleistung $S_{\mathrm{eff}}$ befindet. 

- Im Betrieb ist der Druck $p_{2}$ in R2 durch 

  ```math
  \begin{equation*}
  p_{2}=\frac{L}{S_{\mathrm{eff}}}\,p_{1}
  \end{equation*}
  ```

  gegeben, wobei $p_{1}$ dem mit G1 gemessenen Druck in R1 entspricht. 

### Statisches Kalibrationsverfahren

Ein einfaches **statisches Kalibrationsverfahren** würde z.B. wie folgt ablaufen: 

- Sie definieren mehrere bekannte Volumina $V_{i}$, die Sie durch Ventile voneinander trennen können. 

- Sie evakuieren alle Volumina bei zunächst geöffneten inneren Ventilen. Daraufhin schließen Sie alle Ventile und isolieren die $V_{i}$ auf diese Weise voneinander.

- Im folgenden belüften Sie das Volumen $V_{0}$ und bestimmen den sich darin einstellenden Druck $p_{0}$, z.B. mit Hilfe eines bekannten Messgeräts G1; das zu kalibierende Messgerät kann in diesem Fall direkt gegen G1 abgeglichen werden. Isolieren Sie hierzu $V_{0}$ wieder von der Umgebung. 

-  Im folgenden öffnen Sie sukzessive ein Volumen nach dem anderen. Nach dem [Gesetz von Boyle-Mariotte](https://de.wikipedia.org/wiki/Thermische_Zustandsgleichung_idealer_Gase#Gesetz_von_Boyle-Mariotte) gilt 
  ```math
  \begin{equation*}
  p_{i+1}=\frac{\sum\limits_{k=0}^{i}V_{k}}{\sum\limits_{k=0}^{i+1}V_{k}}\cdot p_{i}.
  \end{equation*}
  ```

Auf diese Weise lässt sich das Gerät auch außerhalb des Messbereichs von G1 kalibrieren. 

### Statisches Kalibrationsverfahren aus Aufgabe 3.1

Für **Aufgabe 3.1** führen Sie ein einstufiges, statisches Kalibrierungsverfahren, unter Anwendung des Gesetzes von [Boyle-Mariotte](https://en.wikipedia.org/wiki/Boyle%27s_law) für T3 durch. 

Hierzu gehen Sie iterativ so vor, wie in den [Kommentaren zu dieser Aufgabe](https://gitlab.kit.edu/kit/etp-lehre/p2-praktikum/students/-/blob/main/Vakuum/Vakuum_Hinweise.ipynb) beschrieben. Für den Druck nach einer Iteration gilt: 
$$
\begin{equation*}
\begin{split}
&\bigl(p_{\mathrm{RZ}}+\Delta p\bigr)\,\bigl(V_{\mathrm{RZ}}+V_{\mathrm{RV}}\bigr) = \bigl(n_{\mathrm{RZ}}+n_{\mathrm{RV}}\bigr)\,R\,T; \\
&\\
&\text{mit:}\\
&\\
&n_{\mathrm{RZ}} = \frac{p_{\mathrm{RZ}}\,V_{\mathrm{RZ}}}{R\,T};\qquad
n_{\mathrm{RV}} = \frac{p_{0}\,V_{\mathrm{RV}}}{R\,T} \\
&\\
&\bigl(p_{\mathrm{RZ}}+\Delta p\bigr)\,\bigl(V_{\mathrm{RZ}}+V_{\mathrm{RV}}\bigr) = p_{\mathrm{RZ}}\,V_{\mathrm{RZ}}+p_{0}\,V_{\mathrm{RV}};\\
\end{split}
\end{equation*}
$$
wobei $p_{\mathrm{RZ}}$ und $V_{\mathrm{RZ}}$ dem Druck und Volumen im RZ und $V_{\mathrm{RV}}$ dem RV entsprechen. Daraus folgt der Zusammenhang: 
$$
\begin{equation}
\Delta p = \frac{V_{\mathrm{RV}}}{V_{\mathrm{RV}}+V_{\mathrm{RZ}}}\left(p_{0} - p_{\mathrm{RZ}}\right).
\end{equation}
$$
Mit zunehmendem Druck im RZ nimmt $\Delta p$ also linear ab! 

# Navigation

[Main](https://gitlab.kit.edu/kit/etp-lehre/p2-praktikum/students/-/tree/main/Vakuum)



