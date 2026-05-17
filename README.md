# Tableau Multi-Devises Achat / Vente

Application web **single-file** (`index.html`) pour afficher un tableau de change multi-devises Achat/Vente pour **50 pays** (Afrique + grandes puissances).

## Aperçu

Interface sombre responsive avec :
- sélection du pays source,
- récupération automatique des taux via API,
- tableau interactif Achat/Vente/Écart/Variation,
- filtres (recherche + région),
- export CSV/JSON,
- persistance localStorage des taux modifiés.

## Screenshot (description)

Un header sombre avec le pays source, l'heure de mise à jour et les boutons d'action, suivi de cartes résumées puis d'un tableau scrollable montrant les 49 autres pays avec drapeaux, achat/vente éditables et variations.

## Utilisation

1. Ouvrir `index.html` dans un navigateur moderne.
2. Choisir un pays source (par défaut **Guinée - GNF**).
3. Cliquer sur **🔄 Actualiser** pour charger les taux API.
4. Filtrer via la barre de recherche ou les boutons de région.
5. Double-cliquer sur **Achat** ou **Vente** pour modifier un taux manuellement.
6. Exporter l'affichage courant via **Export CSV** ou **Export JSON**.

## API utilisée

Priorité:
1. `https://open.er-api.com/v6/latest/{base}`
2. `https://api.exchangerate-open.com/v6/latest/{base}`

En cas d'échec réseau/API, l'application utilise automatiquement un jeu de taux fallback statiques réalistes.

## Liste des 50 pays (ordre imposé)

### Afrique de l'Ouest (16)
1. Guinée (GNF)
2. Sénégal (XOF)
3. Mali (XOF)
4. Côte d'Ivoire (XOF)
5. Sierra Leone (SLL)
6. Liberia (LRD)
7. Guinée-Bissau (XOF)
8. Gambie (GMD)
9. Mauritanie (MRU)
10. Ghana (GHS)
11. Nigeria (NGN)
12. Bénin (XOF)
13. Togo (XOF)
14. Burkina Faso (XOF)
15. Niger (XOF)
16. Cap-Vert (CVE)

### Afrique Centrale (5)
17. Cameroun (XAF)
18. Congo-Brazzaville (XAF)
19. RD Congo (CDF)
20. Gabon (XAF)
21. Tchad (XAF)

### Afrique du Nord (4)
22. Maroc (MAD)
23. Algérie (DZD)
24. Tunisie (TND)
25. Égypte (EGP)

### Afrique de l'Est (3)
26. Kenya (KES)
27. Éthiopie (ETB)
28. Tanzanie (TZS)

### Grandes Puissances & Reste du Monde (22)
29. États-Unis (USD)
30. France / Zone Euro (EUR)
31. Canada (CAD)
32. Chine (CNY)
33. Royaume-Uni (GBP)
34. Japon (JPY)
35. Inde (INR)
36. Russie (RUB)
37. Brésil (BRL)
38. Australie (AUD)
39. Suisse (CHF)
40. Arabie Saoudite (SAR)
41. Émirats Arabes Unis (AED)
42. Turquie (TRY)
43. Mexique (MXN)
44. Corée du Sud (KRW)
45. Indonésie (IDR)
46. Afrique du Sud (ZAR)
47. Argentine (ARS)
48. Norvège (NOK)
49. Suède (SEK)
50. Singapour (SGD)

## GitHub Pages

Après push sur la branche principale, activer **Settings → Pages** et sélectionner la branche publiée.
Le lien sera de la forme: `https://adbrim.github.io/multi-devises-tableau/`.
