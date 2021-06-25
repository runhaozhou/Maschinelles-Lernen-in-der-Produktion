## Regressionsarten

### Einfach lineare Regression



### Quadratische Regression



### Polynomiale Regression

<img src="https://latex.codecogs.com/svg.image?\bg_white&space;h_w(x)=w_0&plus;\sum_{j=1}^{n}w_j*x_j" title="\bg_white h_w(x)=w_0+\sum_{j=1}^{n}w_j*x_j" />

## Bewertung der Einflussgrößen

Regression erlaubt die Bewertung der Einflussgrößen hinsichtlich ihres Einflusses auf die Zielgröße (Sensitivitätsanalyse)

Bewertung erfolgt durch die Koeffizienten oder Gewichte

​	Betragsmäßig großes Gewicht --> großer Einfluss

​	Betragsmäßig kleines Gewicht --> kleiner Einfluss

**Am Besten bei linearer Regression**

### Feature scaling / Normalisierung

Die Normalisierung ist Teil der Datenvorbereitung/ Data Preparation und vereinheitlicht den Wertebereich der Parameter.

#### Rescaling / MinMaxScaler

Wertebereich [0, 1]  nach Skalierung
$$
x_{scaled}=\frac{x-min(x)}{max(x)-min(x)}\qquad
$$
<img src="https://github.com/runhaozhou/Maschinelles_Lernen_in_der_Produktion/blob/master/V1_Regression/Abbildung/MaxAbsScaler.JPG" style="zoom:80%;" />

#### Mean normalisation / MaxAbsScaler

Wie Rescaling aber Verschiebung um Mittelwert (Wertebereich [-1, 1])
$$
x_{scaled}=\frac{x-mean(x)}{max(x)-min(x)}\qquad
$$
<img src="C:\Users\runha\Desktop\Neuer Ordner\Job und Doktorand\2022申博\Project\Maschinelles_Lernen_in_der_Produktion\V1_Regression\Abbildung\MaxAbsScaler.JPG" style="zoom:80%;" />

#### Standardization / (Z-Score) Scaler

Standardmethode bei vielen ML-Anwendungen, danach Mittelwert = 0 und Standardabweichung = 1
$$
x_{scaled}=\frac{x-min(x)}{sd(x)}\qquad
$$
<img src="C:\Users\runha\Desktop\Neuer Ordner\Job und Doktorand\2022申博\Project\Maschinelles_Lernen_in_der_Produktion\V1_Regression\Abbildung\ZScoreScaler.JPG" style="zoom:80%;" />