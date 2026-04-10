# Codice sconto Udemy, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Udemy** da [shopilo.it](https://shopilo.it/negozi/udemy.com). Restituisce **coupon Udemy** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-udemy](https://shopilo-it.github.io/codice-sconto-udemy/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-udemy
cd codice-sconto-udemy
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Udemy",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su corsi online",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/udemy.com"
  }
]
```

## Coupon Udemy disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su corsi online | [shopilo.it](https://shopilo.it/negozi/udemy.com) |

Codici attivi: **[shopilo.it/negozi/udemy.com](https://shopilo.it/negozi/udemy.com)**

## Domande frequenti

### Come utilizzo un codice sconto Udemy?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/udemy.com), aggiungi i prodotti al carrello su Udemy e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Udemy?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Udemy piu recenti?
La pagina [shopilo.it/negozi/udemy.com](https://shopilo.it/negozi/udemy.com) viene aggiornata quotidianamente con i codici sconto Udemy, voucher Udemy e coupon promozionali Udemy piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Udemy

Udemy e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/udemy.com) trovi i migliori codici sconto Udemy, coupon Udemy verificati e voucher Udemy attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-udemy
```

```javascript
const { fetchCoupons } = require('codice-sconto-udemy');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
