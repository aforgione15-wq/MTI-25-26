# Esercizio: Sette e Mezzo - Espansione a Partite Multiple

## 🎯 Obiettivo del Task
L'obiettivo di questo esercizio è prendere uno script Python funzionante che simula una **singola partita** del gioco di carte "Sette e Mezzo" e trasformarlo in un programma completo che permetta all'utente di giocare **più partite consecutive**, tenendo traccia del punteggio storico (numero di vittorie).


## 🛠️ Requisiti di Sviluppo

Partendo dal **Codice di partenza** fornito, devi implementare le seguenti funzionalità:

### 1. Implementazione del Ciclo Principale (Game Loop)
* Tutto il codice che gestisce la singola partita deve essere "racchiuso" (indentato) all'interno di un nuovo ciclo (while?).
* Il ciclo deve continuare a girare finché l'utente desidera giocare (sentinella?).

### 2. Tracciamento delle Vittorie (Contatori)
* Dichiara **due nuove variabili** all'inizio del programma (prima del ciclo principale) per tenere traccia delle vittorie:
  * Una per le vittorie del giocatore.
  * Una per le vittorie del banco.
* Inizializza entrambe le variabili a `0`.
* Aggiorna queste variabili incrementandole di `1` nei rispettivi blocchi `if/else` che decretano il vincitore della singola partita.

### 3. Re-inizializzazione dei Punteggi di Round
* Fai molta attenzione al posizionamento delle variabili `punteggio_giocatore` e `punteggio_banco`.
* Affinché il gioco funzioni correttamente in turni multipli, questi punteggi devono essere riportati a `0.0` **all'inizio di ogni nuova partita**.

### 4. Gestione della Scelta di Continuazione
* Al termine di ogni partita (dopo aver stampato chi ha vinto), chiedi all'utente se vuole giocare ancora con un `input()` (es: *"Vuoi continuare? (S/N)"*).
* Assicurati che l'input non sia sensibile alle maiuscole/minuscole (usa metodi delle stringhe come `.upper()` o `.lower()` per standardizzare la risposta).

### 5. Stampa del Resoconto Finale
* Quando l'utente decide di smettere (il ciclo principale termina), il programma deve stampare un riepilogo finale che mostri:
  * Il numero totale di vittorie del giocatore.
  * Il numero totale di vittorie del banco.

---

## 💻 Suggerimenti per l'implementazione

* **Hand-Tracing:** Prima di scrivere il codice, pensa a quali variabili devono "sopravvivere" tra una partita e l'altra (i contatori delle vittorie) e quali invece devono essere "resettate" (le carte in mano, la scelta "c" o "n" per la singola partita).
* **Indentazione:** Ricorda che in Python l'indentazione definisce i blocchi di codice. Quando aggiungi il ciclo più esterno, seleziona tutto il codice originale e spostalo a destra di un livello (di solito premendo il tasto `Tab`).

---

## 📋 Esempio di Output Atteso alla fine del programma
```text
...
Hai vinto!
Punteggio del banco: 5.5
Punteggio del giocatore: 7.0
Vuoi continuare? (S/N): n

Vittorie Giocatore: 2
Vittorie Banco: 1