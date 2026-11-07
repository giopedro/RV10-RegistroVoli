# Registro voli G3X

Web app per analizzare i voli dai registri dati di volo (FDR) del Garmin G3X e dai libretti di volo esportati in CSV: grafici del volo, motore, carburante, sintesi del singolo volo e di tutti i voli, libretto. Funziona nel browser, anche senza connessione, e si può installare sul telefono come un'app.

I file che carichi non escono dal dispositivo: vengono elaborati e salvati solo nel browser (o nell'app installata) che stai usando. Questo sito non contiene voli: il repository può restare pubblico.

## Pubblicazione su GitHub Pages

1. Su github.com crea un nuovo repository, per esempio `registro-voli-g3x`, impostato come **Public**.
2. Nella pagina del repository scegli **Add file → Upload files** e trascina tutto il contenuto di questa cartella: `index.html`, `manifest.webmanifest`, `sw.js`, `README.md` e la cartella `icons`. Conferma con **Commit changes**.
3. Vai in **Settings → Pages**. In *Build and deployment* scegli **Deploy from a branch**, branch **main**, cartella **/(root)**, poi **Save**.
4. Dopo uno o due minuti l'app è online su `https://TUO-NOME-UTENTE.github.io/registro-voli-g3x/` (l'indirizzo esatto compare in Settings → Pages).

## Installazione sul telefono

- **iPhone (Safari):** apri l'indirizzo, tocca Condividi e poi **Aggiungi alla schermata Home**.
- **Android (Chrome):** apri l'indirizzo, menu ⋮ e poi **Installa app** (o **Aggiungi a schermata Home**).

Apri l'app dall'icona e solo dopo carica i voli: l'app installata ha un archivio suo, separato da quello del browser.

## Portare i voli da un dispositivo all'altro

Ogni dispositivo ha il suo archivio. Per copiarlo: in **Impostazioni → Archivio dei voli** tocca **Salva una copia dell'archivio**; manda il file `.json` sull'altro dispositivo (email, cloud, messaggio) e aprilo lì con **Aggiungi file CSV**. I voli si uniscono senza doppioni.

La copia dell'archivio contiene i tuoi voli: non caricarla su GitHub.

## Aggiornare l'app

Carica il nuovo `index.html` nel repository con **Add file → Upload files**: sostituisce quello vecchio. Telefono e computer prendono la nuova versione alla prima apertura con connessione; l'archivio dei voli resta com'è.
