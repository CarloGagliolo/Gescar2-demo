# Gescar – Demo Centro Revisioni

Demo interattiva statica del gestionale **Gescar** per centri revisioni auto.

> **Tutti i dati mostrati sono completamente fittizi.**

---

## Cosa mostra questa demo

- **Dashboard** — KPI scadenze con badge semaforo (rosso = scaduta, giallo = ≤30 giorni, verde = ok)
- **Scadenze** — lista completa assicurazioni, bolli e patenti ordinata per data
- **Clienti** — anagrafica con ricerca rapida per nome, email o codice fiscale
- **Scheda cliente** — veicoli intestati con stato scadenze, patenti e storico notifiche
- **Veicoli** — lista con stato assicurazione e bollo in evidenza
- **Scheda veicolo** — dettaglio con intestatario e scadenze
- **Notifiche** — popup di composizione messaggio email/SMS + log storico invii

---

## Avvio locale

Nessuna installazione, nessun server, nessuna dipendenza:

```bash
git clone https://github.com/tuouser/gescar-demo.git
cd gescar-demo
open index.html   # oppure trascina il file nel browser
```

---

## Deploy su GitHub Pages

1. Crea un repository pubblico su GitHub (es. `gescar-demo`)
2. Carica il file `index.html` nella root del repository
3. Vai su **Settings → Pages**
4. In **Source**, seleziona `Deploy from a branch`
5. Branch: `main` — Folder: `/ (root)` → clicca **Save**
6. Dopo qualche minuto la demo sarà disponibile su:
   `https://tuouser.github.io/gescar-demo/`

> Non è necessario nessun file `_config.yml` o workflow CI/CD — GitHub Pages pubblica direttamente i file statici.

---

## Stack demo

HTML · Bootstrap 5.3 · Bootstrap Icons 1.11 · Vanilla JS (no framework, no dipendenze npm)

## Stack applicazione reale

PHP 8.2 · Symfony 7.3 · Doctrine ORM 3 · MySQL 8.0 · Bootstrap 5.3

---

Il codice sorgente dell'applicazione reale è in un repository privato separato.
