# Rottamazione Quinquies - Simulatore Piano di Rateazione

Simulatore web per calcolare il piano di rateazione della **Definizione Agevolata 2026** (Rottamazione Quinquies), ai sensi della **Legge n. 199/2025, Art. 1, commi 82-93**.

![HTML5](https://img.shields.io/badge/HTML5-single--file-orange?logo=html5)
![License](https://img.shields.io/badge/License-GPL%20v3-blue)
![No Backend](https://img.shields.io/badge/Backend-none-green)

## Funzionalità

- **Calcolo piano di ammortamento** con fino a 54 rate bimestrali (ammortamento alla francese)
- **Interessi di dilazione** al 3% annuo a decorrere dal 1° agosto 2026
- **Caricamento PDF** del prospetto informativo di Agenzia delle Entrate-Riscossione con estrazione automatica dei dati (numero documento, ente creditore, importi)
- **Inserimento manuale** dell'importo totale o del dettaglio per singola cartella
- **Scelta flessibile** del numero di rate: preimpostati (1, 6, 12, 18, 24, 36, 54) o personalizzato da 2 a 54
- **Esportazione Excel** (.xlsx) con 3 fogli: Riepilogo, Piano Ammortamento, Dettaglio Cartelle
- **Esportazione PDF** con intestazione professionale, tabelle e piè di pagina
- **Calcolo risparmio** rispetto all'importo originario del debito

## Demo

Apri direttamente il file `rottamazione-quinquies.html` nel browser. Non richiede alcun server o installazione.

## Riferimenti normativi

- **Legge n. 199/2025** (Legge di Bilancio 2026), Art. 1, commi 82-93
- Tasso di interesse: **3% annuo** (art. 1, comma 83)
- Metodo di calcolo: **ammortamento alla francese** (rate di pari ammontare)
- Scadenze: da luglio 2026 a maggio 2035 (cadenza bimestrale)

## Scadenze rate

| Rate | Scadenze |
|------|----------|
| 1 | 31/07/2026 |
| 2 | 30/09/2026 |
| 3 | 30/11/2026 |
| 4-51 | Bimestrali dal 31/01/2027 al 30/11/2034 (gen, mar, mag, lug, set, nov) |
| 52 | 31/01/2035 |
| 53 | 31/03/2035 |
| 54 | 31/05/2035 |

## Tecnologie

Webapp single-file (zero dipendenze server), tutto gira nel browser:

- **PDF.js** 3.11.174 — parsing dei PDF di Agenzia delle Entrate-Riscossione
- **SheetJS** 0.18.5 — generazione file Excel (.xlsx)
- **jsPDF** 2.5.1 + **jspdf-autotable** 3.8.2 — generazione file PDF

## Utilizzo

1. Clona il repository:
   ```bash
   git clone https://github.com/TUO-USERNAME/rottamazionequinquies.git
   ```
2. Apri `rottamazione-quinquies.html` in un browser moderno (Chrome, Firefox, Edge, Safari)
3. Inserisci l'importo manualmente oppure carica il PDF del prospetto informativo
4. Seleziona il numero di rate desiderato
5. Clicca **Calcola Piano di Rateazione**

## Avvertenza

Questo simulatore è fornito **a scopo puramente informativo** e non costituisce consulenza fiscale o legale. I calcoli sono basati sulle disposizioni della Legge n. 199/2025 e potrebbero non riflettere eventuali variazioni normative successive. Per informazioni ufficiali, consultare il sito dell'[Agenzia delle Entrate-Riscossione](https://www.agenziaentrateriscossione.gov.it/).

## Licenza

Distribuito con licenza [GNU General Public License v3.0](LICENSE).

Made with ❤️ by Giacomo Greci
