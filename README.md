# Einführung 

Dieses Projekt beschäftigt sich mit den 100 beliebstesten Filmen von 2003 bis 2022. Es werden unterschiedliche Aspekte untersucht, welche anbei aufgeführt sind. Das Ziel dieses Projekts ist zu erkennen was einen Film populär macht. Dieses Ziel wird anhand von explorativer Datenanalyse erreicht werden. 

Verwendet wurde folgender Datensatz: Top 100 popular movies from 2003 to 2022 
(iMDB)  https://www.kaggle.com/datasets/georgescutelnicu/top-100-popular-movies-from-2003-to-2022-imdb 

# Informationen zum Datensatz
Das Datenset enthält die meisten 100 beliebten Filme für jedes Jahr im Zeitraum 2003-2022.
Jede einzelne Information wurde durch Web-Scraping gesammelt und ist auf iMDB zu finden.

Das Datenset enthält:

•	Titel
•	Bewertung
•	Jahr 
•	Monat
•	Zertifikat
•	Laufzeit
•	Regisseur/e
•	Stars
•	Genre/s
•	Drehort
•	Budget 
•	Einnahmen
•	Herkunftsland


# Rohdaten

Die fehlenden Werte im Datensatz wurden entfernt

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/90e081b1-0c9a-4f1c-b11b-9d921c99630c)

•	Insgesamt gibt es 1965 Zeilen im Datensatz
•	Jede der 13 Spalten hat 1965 Nicht-Null-Werte.
•	Es gibt eine Spalte mit numerischen Daten (Dtype: float64), eine Spalte mit ganzzahligen Daten (Dtype: int64) und elf Spalten mit Objekten (Dtype: object).

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/94605448-30af-448c-a047-2b2567c9aa0b)

# Packages 
Das Projekt verwendet folgende Pakete: 
pandas: Zur Datenverarbeitung
black: Für die Code-Formatierung 

pandas 1.2.3 : zur Datenverarbeitung

numpy 1.24.3 : für Berechnungen

matplotlib 3.7.1 : für statistische Visualisierungen

seaborn 0.12.2: besonders gut geeignet für die Visualisierung von komplexen Datensätzen und unterstützt verschiedene Plottypen

black 22.3.0 : für die Code-Formatierung

sklearn 1.3.0 : für Regressionsanalyse 


# Welche Top-10 Genres sind am häufigsten in der Auswahl der Top-100-Filme pro Jahr vertreten?

Warum ist das wichtig? 
Die Identifikation beliebter Genres gibt Einblicke in Marktpräferenzen und hilft bei Entscheidungen über das Filmangebot.
Wirtschaftlicher Nutzen der Beantwortung dieser Frage: Investitionen in beliebte Genres können durchgeführt werden was dazu führt, dass sich die Einnahmen steigern. 

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/e3c73e2f-2ec8-4dee-9a37-248cbbe19f02)


![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/d515ff71-bd0e-44f5-8003-b70074092ac2)

# Welches Genre war am beliebtesten im Verlauf der Jahre? 

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/0d8343ca-b05b-4c26-b794-37c95877d692)


# Wie haben sich die durchschnittlichen Filmbewertungen im Laufe der Jahre entwickelt?

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/e94afa28-bcc8-408a-9471-4598e8949486)

# Besonderheiten 2020 

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/1556b9f8-923b-4c2c-9ec3-86a8939c7867)

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/df616134-1776-4f70-8667-7af56ba74d2a)


# Top 10 der Filme mit den schlechtesten Bewertungen im Jahr 2020 

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/1db9b0b9-9d02-4238-b18b-b586ce596b3f)


# Gibt es einen Zusammenhang zwischen einem höheren Filmbudget und besseren Ratings von Filmen? 
Warum ist das wichtig? Diese Untersuchung bietet Einblicke, wie Finanzierungsentscheidungen den kommerziellen Erfolg von Filmen beeinflussen und kann Produktionsstrategien informieren.

Wirtschaftlicher Nutzen der Beantwortung dieser Frage: Filmproduzenten können durch die Analyse der Budget-Erfolg-Korrelation bessere Entscheidungen bei der Budgetierung treffen. Optimale Budgetierungsstrategien können zu maximierten Einnahmen bei minimierten Kosten führen, wodurch die Rentabilität gesteigert wird. 

Um die Korrelation zu messen wurde der Pearson-Korrelationskoeffizient verwendet. 

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/1f350cd1-56c4-4649-adcb-fa512153585e)

Das Streudiagramm zeigt die Datenpunkte mit einer überlagerten Regressionslinie. Die Flachheit der Linie spiegelt die geringe Steigung wider, die aus der geringen Korrelation resultiert. Die Punkte liegen weit verstreut und zeigen keine deutliche Tendenz, der Linie zu folgen, was auf eine geringe Vorhersagekraft des Ratings für das Budget hindeutet.

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/5d9f032e-77ee-42da-8abc-f33056f8665a)

Die Heatmap zeigt eine Korrelationsmatrix, in der die Korrelation von 'Rating' zu sich selbst und von 'Budget' zu sich selbst jeweils 1 ist, was erwartet wird. Die Korrelation zwischen 'Rating' und 'Budget' wird als 0.053 angezeigt, was die sehr schwache Beziehung bestätigt.

Es besteht also keine starke lineare Beziehung zwischen dem Budget und dem Rating


# Gibt es einen Zusammenhang zwischen der Länge eines Films und den Ratings von Filmen? 

Warum ist das wichtig?
Die Analyse der Laufzeitbewertungskorrelation hilft, das optimale Gleichgewicht zwischen einer ansprechenden Laufzeit und Zuschauerzufriedenheit zu verstehen. 

![image](https://github.com/Alisa99j/Pr-sentation_Top100Movies/assets/155681145/0f6c5090-a364-4f1e-8702-40f6cb6c44ee)

Die Korrelation von ungefähr 0.38 weist darauf hin, dass es eine positive Assoziation zwischen der Laufzeit eines Films und seiner Bewertung gibt das heißt, Filme mit einer längeren Laufzeit tendieren dazu, höhere Bewertungen zu haben.

Korrelation zwischen Laufzeit und Bewertung: 0.3785280720080518

# Abschluss 
