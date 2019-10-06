[Sommaire](https://ursi-2020.github.io/Documentation/)

# Données

## Clients

```
{
    "Nom": <string> nom du client,
    "Prenom": <string> prénom du client,
    "Credit": <float> crédit fidélité, // Transformé en centimes d'euros par CRM
    "Paiement": <integer> nombre de paiements valides,
    "Compte": <string> identifiant du compte,
    "carteFid": <integer> numéro de la carte de fidélité
}
```

Exemple:
```
{"clients" : [
    {
        "Nom": "Eddison-18",
        "Prenom": "Jean",
        "Credit": 0.0,
        "Paiement": 0,
        "Compte": "BKN1CST18"
    },
    {
        "Nom": "Sarkozy-51",
        "Prenom": "Marc",
        "Credit": 0.0,
        "Paiement": 0
    },
    {
        "Nom": "Eddison-53",
        "Prenom": "Anne",
        "Credit": 154.62542724609375,
        "Paiement": 3,
        "Compte": "BKN1CST53"
    }
]
}
```

## Produit

```
{
    "codeProduit": <string> identifiant fournisseur du produit,
    "familleProduit": <string> type de produit,
    "descriptionProduit": <string> description du produit,
    "quantiteMin": <integer> quantité minimale d'achat du produit,
    "packaging": <integer> quantité unitaire lors de l'achat du produit,
    "prix": <integer> prix du packaging
}
```

Exemple:
```
{
    "produits": [
        {
            "codeProduit": "X1-0",
            "familleProduit": "Frigos",
            "descriptionProduit": "Frigos:P1-0",
            "quantiteMin": 15,
            "packaging": 2,
            "prix": 4.24
        },
        {
            "codeProduit": "X1-1",
            "familleProduit": "Console",
            "descriptionProduit": "Console:P3-1",
            "quantiteMin": 5,
            "packaging": 1,
            "prix": 1.54
        },
        {
            "codeProduit": "X1-2",
            "familleProduit": "Frigos",
            "descriptionProduit": "Frigos:P3-2",
            "quantiteMin": 10,
            "packaging": 1,
            "prix": 79.48
        },
        {
            "codeProduit": "X1-3",
            "familleProduit": "TV",
            "descriptionProduit": "TV:P1-3",
            "quantiteMin": 15,
            "packaging": 5,
            "prix": 76.76
        },
        {
            "codeProduit": "X1-4",
            "familleProduit": "TV",
            "descriptionProduit": "TV:P3-4",
            "quantiteMin": 15,
            "packaging": 4,
            "prix": 74.00
        },
        {
            "codeProduit": "X1-8",
            "familleProduit": "Console",
            "descriptionProduit": "Console:P1-8",
            "quantiteMin": 5,
            "packaging": 4,
            "prix": 58.87
        },
        {
            "codeProduit": "X1-9",
            "familleProduit": "Frigos",
            "descriptionProduit": "Frigos:P2-9",
            "quantiteMin": 10,
            "packaging": 5,
            "prix": 71.95
        },
        {
            "codeProduit": "X1-10",
            "familleProduit": "TV",
            "descriptionProduit": "TV:P3-10",
            "quantiteMin": 15,
            "packaging": 2,
            "prix": 26.24
        }
    ]
}
```

## Vente

Exemple:
```
{
  "success": "true",
  "result": "ok, 17 tickets generated",
  "tickets": [
    {
      "caisse": "3",
      "panier": [
        {
          "codeProduit": "Y2-43",
          "description": "Livre:P2-43",
          "quantity": 1
        }
      ],
      "modePaiement": "CASH"
    },
    {
      "caisse": "1",
      "panier": [
        {
          "codeProduit": "X1-48",
          "description": "TV:P2-48",
          "quantity": 1
        },
        {
          "codeProduit": "X1-13",
          "description": "TV:P1-13",
          "quantity": 2
        },
        {
          "codeProduit": "Y2-39",
          "description": "Livre:P2-39",
          "quantity": 1
        }
      ],
      "modePaiement": "CASH"
    },
    {
      "caisse": "2",
      "panier": [
        {
          "codeProduit": "X1-18",
          "description": "Frigos:P1-18",
          "quantity": 1
        },
        {
          "codeProduit": "X1-46",
          "description": "Console:P2-46",
          "quantity": 2
        },
        {
          "codeProduit": "X1-14",
          "description": "Console:P2-14",
          "quantity": 2
        }
      ],
      "carteFid": "33",
      "modePaiement": "DIFFERED"
    },
    {
      "caisse": "4",
      "panier": [
        {
          "codeProduit": "X1-24",
          "description": "Console:P3-24",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-34",
          "description": "DVD:P2-34",
          "quantity": 1
        },
        {
          "codeProduit": "X1-27",
          "description": "Console:P2-27",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-12",
          "description": "DVD:P2-12",
          "quantity": 1
        }
      ],
      "modePaiement": "CASH"
    },
    {
      "caisse": "3",
      "panier": [
        {
          "codeProduit": "X1-26",
          "description": "Console:P3-26",
          "quantity": 1
        }
      ],
      "modePaiement": "CARD",
      "card": "BKN1CST17"
    },
    {
      "caisse": "4",
      "panier": [
        {
          "codeProduit": "Y2-0",
          "description": "BlueRay:P4-0",
          "quantity": 1
        }
      ],
      "modePaiement": "CASH"
    },
    {
      "caisse": "4",
      "panier": [
        {
          "codeProduit": "X1-31",
          "description": "Console:P1-31",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-40",
          "description": "BlueRay:P2-40",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-15",
          "description": "DVD:P4-15",
          "quantity": 1
        }
      ],
      "carteFid": "33",
      "modePaiement": "CASH"
    },
    {
      "caisse": "3",
      "panier": [
        {
          "codeProduit": "X1-50",
          "description": "TV:P2-50",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-43",
          "description": "Livre:P2-43",
          "quantity": 2
        }
      ],
      "carteFid": "33",
      "modePaiement": "CASH"
    },
    {
      "caisse": "3",
      "panier": [
        {
          "codeProduit": "Y2-17",
          "description": "DVD:P2-17",
          "quantity": 1
        },
        {
          "codeProduit": "X1-20",
          "description": "Frigos:P2-20",
          "quantity": 1
        },
        {
          "codeProduit": "X1-34",
          "description": "Console:P3-34",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-17",
          "description": "DVD:P2-17",
          "quantity": 1
        }
      ],
      "modePaiement": "CARD",
      "card": "BKN1CST36"
    },
    {
      "caisse": "3",
      "panier": [
        {
          "codeProduit": "X1-15",
          "description": "Console:P3-15",
          "quantity": 2
        },
        {
          "codeProduit": "X1-44",
          "description": "Frigos:P1-44",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-47",
          "description": "Livre:P4-47",
          "quantity": 1
        }
      ],
      "carteFid": "33",
      "modePaiement": "CASH"
    },
    {
      "caisse": "3",
      "panier": [
        {
          "codeProduit": "X1-11",
          "description": "Frigos:P1-11",
          "quantity": 1
        },
        {
          "codeProduit": "X1-51",
          "description": "TV:P1-51",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-30",
          "description": "DVD:P2-30",
          "quantity": 1
        },
        {
          "codeProduit": "X1-4",
          "description": "Frigos:P3-4",
          "quantity": 1
        }
      ],
      "carteFid": "33",
      "modePaiement": "CASH"
    },
    {
      "caisse": "2",
      "panier": [
        {
          "codeProduit": "Y2-27",
          "description": "DVD:P4-27",
          "quantity": 2
        },
        {
          "codeProduit": "Y2-18",
          "description": "DVD:P2-18",
          "quantity": 2
        }
      ],
      "modePaiement": "CARD",
      "card": "BKN1CST5"
    },
    {
      "caisse": "1",
      "panier": [
        {
          "codeProduit": "Y2-8",
          "description": "BlueRay:P2-8",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-5",
          "description": "Livre:P4-5",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-1",
          "description": "Livre:P2-1",
          "quantity": 1
        }
      ],
      "modePaiement": "CASH"
    },
    {
      "caisse": "2",
      "panier": [
        {
          "codeProduit": "Y2-4",
          "description": "Livre:P4-4",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-34",
          "description": "DVD:P2-34",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-2",
          "description": "BlueRay:P4-2",
          "quantity": 2
        }
      ],
      "modePaiement": "CARD",
      "card": "BKN1CST12"
    },
    {
      "caisse": "1",
      "panier": [
        {
          "codeProduit": "Y2-43",
          "description": "Livre:P2-43",
          "quantity": 2
        },
        {
          "codeProduit": "Y2-41",
          "description": "Livre:P4-41",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-10",
          "description": "Livre:P2-10",
          "quantity": 2
        },
        {
          "codeProduit": "X1-50",
          "description": "TV:P2-50",
          "quantity": 1
        }
      ],
      "modePaiement": "CASH"
    },
    {
      "caisse": "2",
      "panier": [
        {
          "codeProduit": "Y2-28",
          "description": "DVD:P4-28",
          "quantity": 1
        },
        {
          "codeProduit": "X1-19",
          "description": "Frigos:P3-19",
          "quantity": 1
        },
        {
          "codeProduit": "Y2-48",
          "description": "Livre:P2-48",
          "quantity": 1
        }
      ],
      "modePaiement": "CARD",
      "card": "BKN1CST45"
    },
    {
      "caisse": "3",
      "panier": [
        {
          "codeProduit": "Y2-17",
          "description": "DVD:P2-17",
          "quantity": 2
        },
        {
          "codeProduit": "Y2-37",
          "description": "Livre:P2-37",
          "quantity": 1
        }
      ],
      "modePaiement": "CARD",
      "card": "BKN1CST2"
    }
  ]
}
```