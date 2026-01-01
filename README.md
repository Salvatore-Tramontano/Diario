# 📓 Diario

**Diario** è un'applicazione web "personal tracker" completa e reattiva, progettata per registrare e analizzare le attività quotidiane. Costruita come un singolo file HTML, offre un'interfaccia moderna in stile *glassmorphism* e funzionalità avanzate per visualizzare i trend della tua vita.

## ✨ Funzionalità Principali

### 1. Tracciamento Multi-Categoria
L'applicazione supporta diverse categorie predefinite, ognuna con campi di inserimento specifici:
* **Intrattenimento:** Film, Serie TV (gestione stagioni/episodi), Libri (pagine), Teatro, Concerti, Podcast.
* **Produttività:** Lavoro (con slider per produttività vs "livello rottura").
* **Benessere:** Sport, Sociale.
* **Diario Personale:** Giornata (mood tracking).

### 2. Dashboard BI & Reportistica
Una vista dedicata (**Report**) trasforma i dati inseriti in grafici e KPI:
* **KPI Cards:** Totali, medie voto e statistiche specifiche (es. "% Giornate Lavoro OK").
* **Grafici (Chart.js):**
    * Distribuzione voti (Bar chart).
    * Trend temporali (Bar chart).
    * Analisi specifiche (es. Cinema vs Casa, Rewatch vs Nuovi, Produttività vs Stress).
* **Aggregazione Temporale:** Possibilità di raggruppare i dati per Giorno, Settimana, Mese o Anno.

### 3. Filtri Avanzati
Un potente sistema di filtraggio per esplorare il diario:
* **Temporale:** Oggi, 7 Giorni, Questo Mese, Quest'Anno, Tutto.
* **Rating:** Filtro per numero di stelle (1-5).
* **Flag Specifici:** Filtri dinamici in base alla categoria (es. "Visti al Cinema", "Libri Finiti", "Rewatch").

### 4. Gestione Dati & Privacy
* **Local Storage:** Tutti i dati vengono salvati istantaneamente nella memoria del browser (`localStorage`). Nessun dato viene inviato a server esterni.
* **Import/Export:** Funzionalità completa di backup.
    * Esportazione in **Excel (.xlsx)**, **CSV** e **JSON**.
    * Importazione da file per ripristinare i backup.

## 🛠️ Stack Tecnologico

Il progetto è contenuto in un unico file `index.html` e utilizza le seguenti tecnologie via CDN (non è richiesta installazione di Node.js):

* **Core:** HTML5, Vanilla JavaScript.
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (UI moderna e responsive).
* **Icone:** [FontAwesome 6](https://fontawesome.com/).
* **Grafici:** [Chart.js](https://www.chartjs.org/).
* **Dati:** [SheetJS (XLSX)](https://sheetjs.com/) per l'export Excel.
* **UI:** Design responsive ottimizzato per mobile (Bottom Navigation) e desktop.

## 🚀 Installazione e Uso

1.  **Avvio:** Scarica il file, rinominalo in `index.html` e aprilo con un qualsiasi browser moderno (Chrome, Edge, Firefox, Safari).
2.  **Inserimento:** Clicca il pulsante **+** flottante in basso a destra per aggiungere una nuova voce.
3.  **Visualizzazione:** Usa la barra di navigazione in basso per passare dalla vista "Diario" (lista) alla vista "Report" (grafici).
4.  **Backup:** Clicca l'icona di download in alto a destra per scaricare periodicamente una copia dei tuoi dati.

## ⚠️ Nota sulla Persistenza Dati

L'applicazione utilizza il `localStorage` del browser.
* **Importante:** Se cancelli la cache del browser, perderai i dati.
* **Consiglio:** Esegui regolarmente un backup cliccando sul pulsante di esportazione (JSON o Excel) per tenere i tuoi ricordi al sicuro.

## 🎨 Personalizzazione

Il codice include un sistema di temi basato su classi Tailwind. [cite_start]Le categorie sono definite nell'array `categories` all'inizio dello script, rendendo facile aggiungere o modificare tipi di attività modificando il codice sorgente.
