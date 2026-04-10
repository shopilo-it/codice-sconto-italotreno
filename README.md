# Codice sconto Italo Treno, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Italo Treno** da [shopilo.it](https://shopilo.it/negozi/italotreno.it). Restituisce **coupon Italo Treno** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-italotreno](https://shopilo-it.github.io/codice-sconto-italotreno/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-italotreno
cd codice-sconto-italotreno
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Italo Treno",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su biglietti alta velocita",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/italotreno.it"
  }
]
```

## Coupon Italo Treno disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su biglietti alta velocita | [shopilo.it](https://shopilo.it/negozi/italotreno.it) |

Codici attivi: **[shopilo.it/negozi/italotreno.it](https://shopilo.it/negozi/italotreno.it)**

## Domande frequenti

### Come utilizzo un codice sconto Italo Treno?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/italotreno.it), aggiungi i prodotti al carrello su Italo Treno e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Italo Treno?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Italo Treno piu recenti?
La pagina [shopilo.it/negozi/italotreno.it](https://shopilo.it/negozi/italotreno.it) viene aggiornata quotidianamente con i codici sconto Italo Treno, voucher Italo Treno e coupon promozionali Italo Treno piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Italo Treno

Italo Treno e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/italotreno.it) trovi i migliori codici sconto Italo Treno, coupon Italo Treno verificati e voucher Italo Treno attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-italotreno
```

```javascript
const { fetchCoupons } = require('codice-sconto-italotreno');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
