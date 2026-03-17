# Movie Industry Correlation Analysis project

In questo progetto, l'obiettivo è esplorare un vasto dataset dell'industria cinematografica per analizzare e scoprire quali variabili (come budget, numero di voti, genere, ecc.) hanno la maggiore correlazione con il successo finanziario di un film, misurato tramite gli incassi lordi (gross earnings) al botteghino.

### Project Structure

* `Movie correlation project.ipynb`: notebook contenente l'intero workflow di analisi dei dati, suddiviso in:
    * **Pulizia e pre-elaborazione dei dati**: ispezione dei valori mancanti, controllo dei tipi di dato e conversione delle variabili categoriche (object) in formati numerici (`cat.codes`) per consentire il calcolo matematico.
    * **Analisi esplorativa e visualizzazione (EDA)**: creazione di grafici a dispersione (scatter plot) e grafici di regressione per analizzare visivamente il rapporto tra budget e incassi utilizzando Matplotlib e Seaborn.
    * **Analisi delle correlazioni**: calcolo delle matrici di correlazione utilizzando i metodi Pearson, Kendall e Spearman. Sviluppo di una Heatmap delle correlazioni numeriche e identificazione automatica delle coppie di variabili con la correlazione più alta.
* `requirements.txt`: librerie python che devono essere installate (Pandas, NumPy, Seaborn, Matplotlib).


### Dataset

**Input variables (Movie features):**
* `name` (text/categorical): titolo del film
* `rating` (categorical): classificazione del film (es. R, PG-13)
* `genre` (categorical): genere cinematografico
* `year` (numeric): anno di uscita
* `released` (text/categorical): data e luogo di rilascio
* `score` (numeric): valutazione media (es. punteggio IMDb)
* `votes` (numeric): numero totale di voti degli utenti
* `director` (text/categorical): regista
* `writer` (text/categorical): sceneggiatore principale
* `star` (text/categorical): attore protagonista
* `country` (text/categorical): paese di produzione
* `budget` (numeric): costo di produzione del film
* `company` (text/categorical): casa di produzione
* `runtime` (numeric): durata del film in minuti

**Target variable (valore di interesse principale):**
* `gross` (numeric) - incasso lordo totale del film al botteghino

### Results
L'analisi delle matrici di correlazione ha permesso di estrarre le seguenti conclusioni chiave:
* Il **numero di voti (`votes`)** e il **budget (`budget`)** hanno in assoluto la correlazione più alta e significativa con gli incassi lordi (`gross`). 
* Al contrario di quanto si potrebbe pensare, il punteggio della critica o degli utenti (`score`) ha un impatto molto basso sugli incassi reali del film.
