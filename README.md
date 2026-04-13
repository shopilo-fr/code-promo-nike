# Code promo Nike, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Nike** depuis [shopilo.fr](https://shopilo.fr/reductions/nike.com). Renvoie les **coupons Nike** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-nike](https://shopilo-fr.github.io/code-promo-nike/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-nike
cd code-promo-nike
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Nike",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% de reduction sur les vetements de sport",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/nike.com"
  }
]
```

## Coupons Nike disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 20% | 20% de reduction sur les vetements de sport | [shopilo.fr](https://shopilo.fr/reductions/nike.com) |

Codes actifs : **[shopilo.fr/reductions/nike.com](https://shopilo.fr/reductions/nike.com)**

## Questions frequentes

### Comment utiliser un code promo Nike ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/nike.com), ajoutez les produits a votre panier sur Nike et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Nike ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Nike les plus recents ?
La page [shopilo.fr/reductions/nike.com](https://shopilo.fr/reductions/nike.com) est mise a jour quotidiennement avec les codes promo Nike, bons de reduction Nike et coupons promotionnels Nike les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Nike

Nike est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/nike.com), retrouvez les meilleurs codes promo Nike, coupons Nike verifies et bons de reduction Nike actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-nike
```

```javascript
const { fetchCoupons } = require('code-promo-nike');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
