# Progetto di Introduzione al Pensiero Computazionale e alla Data Science — A.A. 2025/2026
**Alma Mater Studiorum - Università di Bologna**

## Membri del Team
* **Ederone Aurora** — Matricola: `1217218`
* **Querqui Chiara** — Matricola: `1216931`
* **Giovannini Stefano** — Matricola: `1216560`

**Numero Team:** 13

## Obiettivo del Progetto
L'obiettivo di questo progetto è sviluppare un'analisi di Data Science completa, riproducibile e documentata per prevedere il fenomeno del **Customer Churn** (l'abbandono del servizio da parte dei clienti) nel contesto di una compagnia di telecomunicazioni. 
Il progetto integra tecniche per la pulizia dei dati, analisi esplorativa visiva e l'addestramento di modelli di Machine Learning per identificare i fattori critici che influenzano la fedeltà del cliente.

## Descrizione del Dataset
Il dataset utilizzato è **Customer Churn** e analizza il comportamento dei clienti tracciando diverse tipologie di caratteristiche:
* **Dati demografici:** genere, indicatore SeniorCitizen, presenza di partner o dipendenti.
* **Servizi attivi:** tipologia di linea internet (DSL, Fibra ottica), servizi di supporto e sicurezza (TechSupport, OnlineSecurity, OnlineBackup) e streaming TV/movies.
* **Informazioni commerciali:** tipo di contratto (mese-per-mese, annuale, biennale), metodo di pagamento, costi mensili e spesa totale.
* **Target:** `Churn` (indica se il cliente ha abbandonato o meno il servizio).

## Sintesi del Workflow
Il lavoro è stato organizzato in più fasi:
1. ⁠caricamento e comprensione iniziale del dataset;
2. controllo di duplicati, missing values e valori anomali;
3. ⁠analisi esplorativa delle variabili e delle relazioni con ⁠ Churn⁠;
4. ⁠conversione delle variabili categoriche in numeriche;
5. ⁠suddivisione train/test e standardizzazione delle feature;
6. ⁠addestramento e confronto di tre modelli di classificazione;
7. ⁠valutazione critica dei risultati tramite accuracy, precision, recall, F1-score e confusion matrix.

## Modelli di Machine Learning Confrontati
Per soddisfare i requisiti del corso, l'analisi mette a confronto le prestazioni di tre algoritmi differenti:
1. **Modello Lineare:** Regressione Logistica (*Logistic Regression*)
2. **Modelli Non Lineari:**
   * K-Nearest Neighbors (K-NN)
   * Random Forest (utilizzato anche per l'estrazione della *feature importance*)
Tutti i modelli vengono valutati tramite metriche di classificazione: Accuracy, Confusion Matrix, Precision, Recall e F1-Score.

## Struttura del Repository
Il repository è organizzato seguendo la struttura richiesta:
* `/data`: contiene il dataset originale `Customer_Churn.csv`.
* `/notebooks`: contiene i file Colab `.ipynb` con il codice di pulizia, EDA e modellazione.
* `/figures`: grafici ed esportazioni visive generate durante l'analisi.
* `/report`: file sorgenti in LaTeX e la relazione finale in formato PDF.

## Come eseguire il Progetto
Il notebook principale si trova nella cartella ⁠`/notebooks`⁠.
Per riprodurre l’analisi:
1. ⁠aprire il notebook in Google Colab;
2. ⁠caricare il file ⁠ Customer_Churn.csv ;
3. ⁠verificare che il percorso del file nel notebook sia corretto;
4.  ⁠eseguire le celle in ordine, dalla pulizia dei dati fino alla valutazione dei modelli.
Il dataset originale è conservato nella cartella ⁠ `/data`⁠, mentre il dataset pulito viene generato durante l’esecuzione del notebook.

## Librerie utilizzate
Il progetto è stato sviluppato in Python utilizzando le principali librerie viste durante il corso:
* pandas ⁠ e ⁠ numpy ⁠ per la gestione dei dati;
* matplotlib ⁠ e ⁠ seaborn ⁠ per la visualizzazione;
* scikit-learn ⁠ per la preparazione dei dati, l’addestramento dei modelli e la valutazione dei risultati.

## Risultati Principali 
L’analisi esplorativa ha evidenziato alcune relazioni rilevanti:
* ⁠i clienti con contratto mensile (⁠ Month-to-month ⁠) presentano un tasso di churn più elevato;
* i clienti con minore ⁠ tenure ⁠ risultano più propensi ad abbandonare;
* ⁠costi mensili più alti sembrano associati a una maggiore probabilità di churn;
* ⁠l’assenza di servizi come ⁠ TechSupport ⁠ e ⁠ OnlineSecurity ⁠ è collegata a tassi di churn più elevati.
Nella fase di modellazione sono stati confrontati tre algoritmi: Regressione Logistica, k-NN e Random Forest.

## Note sulla riproducibilità
Il repository è stato organizzato per rendere il progetto tracciabile e riproducibile.  
Il codice è contenuto nei notebook, i dati sono raccolti nella cartella ⁠ `/data`⁠, le figure principali nella cartella ⁠ `/figures` ⁠ e la relazione finale nella cartella ⁠ `/report`.
Le modifiche al progetto sono state tracciate tramite commit GitHub.
