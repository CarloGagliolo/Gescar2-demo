# Demo Repo — Gescar

> Piano e istruzioni per il repository pubblico dimostrativo `gescar-demo`.
> Il repo demo è **separato** dal repo di produzione (`Gescar2`).

---

## Approccio scelto: pagina statica su GitHub Pages

**Nessun backend, nessuna API, nessun dato reale.**
La demo è un singolo file `index.html` con Bootstrap 5 CDN e dati fittizi hardcoded.
Si deploya su GitHub Pages in un click, senza server, senza Docker, senza costi.

---

## Struttura del repo demo

```
gescar-demo/
├── index.html    ← tutta la demo (HTML + CSS + JS inline, Bootstrap via CDN)
└── README.md     ← vetrina con link alla demo live e descrizione
```

Niente `docs/`, niente `src/`, niente `composer.json`. Solo questi due file.

---

## Cosa mostra la demo

| Sezione | Contenuto |
|---|---|
| Hero | Descrizione dell'app, numeri chiave (7k+ clienti, 4.5k veicoli) |
| Dashboard | KPI cards con badge semaforo + tabella revisioni urgenti |
| Scadenze | Lista con tab per tipo + filtro date |
| Clienti | Tabella con ricerca live funzionante |
| Scheda cliente | Veicoli con badge scadenze + storico notifiche |
| Notifiche | Registro avvisi con canale ed esito |
| Feature cards | 6 card che descrivono le funzionalità principali |
| Stack | Badge tecnologie usate |

---

## Deploy su GitHub Pages

1. Creare un nuovo repo pubblico: `CarloGagliolo/gescar-demo`
2. Caricare solo `index.html` e `README.md`
3. Andare su **Settings → Pages → Source: Deploy from branch → main / root**
4. Dopo ~1 minuto la demo è live su `https://carlogagliolo.github.io/gescar-demo`

**Comandi:**
```bash
# Partire dalla cartella gescar-demo/ già pronta nel repo di produzione
cd gescar-demo
git init
git add .
git commit -m "feat: demo statica Gescar per GitHub Pages"
git remote add origin https://github.com/CarloGagliolo/gescar-demo.git
git push -u origin main
```

---

## Aggiornare la demo in futuro

Quando l'app evolve (nuove funzionalità, nuovo UI), aggiornare `index.html` a mano:
- Aggiungere nuove sezioni o tab
- Aggiornare i dati fittizi se cambiano i campi
- Aggiornare i badge dello stack se cambiano le versioni

Non è necessario sincronizzare con il repo di produzione — è una vetrina indipendente.

---

## Checklist prima di pubblicare

- [ ] Nessun dato reale in nessun punto del file HTML
- [ ] Nessuna chiave, token, API key o URL di produzione
- [ ] Nessun riferimento al nome del centro reale (sostituire con "Centro Revisioni Demo")
- [ ] Link `https://carlogagliolo.github.io/gescar-demo` funzionante
- [ ] README aggiornato con il link corretto alla demo live
