# Cod reducere vidaXL — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere vidaXL** de pe [shopilo.ro](https://shopilo.ro/magazin/vidaxl.ro). Returneaza **cupoane vidaXL** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-vidaxl](https://shopilo-ro.github.io/cod-reducere-vidaxl/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-vidaxl
cd cod-reducere-vidaxl
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "vidaXL",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la mobilier si gradinarit",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/vidaxl.ro"
  }
]
```

## Cupoane vidaXL disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la mobilier si gradinarit | [shopilo.ro](https://shopilo.ro/magazin/vidaxl.ro) |

Codurile active: **[shopilo.ro/magazin/vidaxl.ro](https://shopilo.ro/magazin/vidaxl.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere vidaXL?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/vidaxl.ro), adauga produsele in cos pe vidaXL, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele vidaXL?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri vidaXL?
Pagina [shopilo.ro/magazin/vidaxl.ro](https://shopilo.ro/magazin/vidaxl.ro) este actualizata zilnic cu cele mai noi cod reducere vidaXL, voucher vidaXL si cupon promotional vidaXL.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre vidaXL

vidaXL este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/vidaxl.ro) cele mai bune cod reducere vidaXL, cupoane vidaXL verificate si voucher vidaXL active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-vidaxl
```

```javascript
const { fetchCoupons } = require('cod-reducere-vidaxl');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
