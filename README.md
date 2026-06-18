# Progetto di Introduzione al Pensiero Computazionale e alla Data Science — A.A. 2025/2026
**Alma Mater Studiorum - Università di Bologna**

## 👥 Membri del Team
* **Ederone Aurora** — Matricola: `1217218`
* **Querqui Chiara** — Matricola: `1216931`
* **Giovannini Stefano** — Matricola: `1216560`

**Numero Team:** 13

## Obiettivo del Progetto
L'obiettivo di questo progetto è sviluppare un'analisi di Data Science completa, riproducibile e documentata per prevedere il fenomeno del **Customer Churn** (l'abbandono del servizio da parte dei clienti) nel contesto di una compagnia di telecomunicazioni. 
Il progetto integra tecniche per la pulizia dei dati, analisi esplorativa visiva e l'addestramento di modelli di Machine Learning per identificare i fattori critici che influenzano la fedeltà del cliente.

## Descrizione del Dataset
Il dataset utilizzato è **Customer Churn** e analizza il comportamento dei clienti tracciando diverse tipologie di caratteristiche:
* **Dati demografici:** genere, età, presenza di partner o dipendenti.
* **Servizi attivi:** tipologia di linea internet (DSL, Fibra ottica), servizi di supporto e sicurezza (TechSupport, OnlineSecurity, OnlineBackup) e streaming TV/movies.
* **Informazioni commerciali:** tipo di contratto (mese-per-mese, annuale, biennale), metodo di pagamento, costi mensili e spesa totale.
* **Target:** `Churn` (indica se il cliente ha abbandonato o meno il servizio).

## Modelli di Machine Learning Confrontati
Per soddisfare i requisiti del corso, l'analisi mette a confronto le prestazioni di tre algoritmi differenti:
1. **Modello Lineare:** Regressione Logistica (*Logistic Regression*)
2. **Modelli Non Lineari:**
   * K-Nearest Neighbors (K-NN)
   * Random Forest (utilizzato anche per l'estrazione della *feature importance*)

Tutti i modelli vengono valutati tramite metriche di classificazione: Accuracy, Confusion Matrix, Precision, Recall e F1-Score.

## Struttura del Repository e Istruzioni per l'Esecuzione
Il repository è organizzato seguendo la struttura richiesta:
* `/data`: contiene il dataset originale `Customer_Churn.csv`.
* `/notebooks`: contiene i file Colab `.ipynb` con il codice di pulizia, EDA e modellazione.
* `/figures`: grafici ed esportazioni visive generate durante l'analisi.
* `/report`: file sorgenti in LaTeX e la relazione finale in formato PDF.
