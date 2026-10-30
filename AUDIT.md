# AUDIT.md : à compléter

## 1. Audits outillés

Lance les 3 audits sur la page (`npm run dev`, puis ouvre-la dans Chrome) et
colle ici un résumé de ce que chacun remonte :

- **Lighthouse** (DevTools → onglet Lighthouse → catégorie Accessibility) :
- **axe DevTools** (extension Chrome) :
- **WAVE** (https://wave.webaim.org/, ou l'extension) :

## 2. Les éléments à corriger

| Élément | Couleur texte | Couleur fond | Ratio mesuré | Ratio AA requis | Conforme ? |
|---------|---------------|--------------|--------------|------------------|------------|
| `.subtitle` | #aaaaaa |  #ffffff | 2.32:1 | 4.5:1 | Non Conforme |
| `.label` | #999999 | #ffffff | 2.84:1 | 4.5:1 | Non Conforme |
| `.hint` | #bbbbbb | #ffffff | 1.91:1 | 4.5:1 | Non Conforme |
| `.btn-primary` | #ffffff | #6fa8dc | 2.52:1 | 4.5:1 (texte) | Non Conforme |

> Utilise un vérificateur de contraste (ex. le picker de couleur de Chrome
> DevTools affiche déjà le ratio AA/AAA quand tu modifies une couleur).

## 3. Priorisation

Classe les 4 corrections par ordre d'impact (1 = le plus urgent) et explique pourquoi.

1. .btn-primary : c'est le seul élément interactif de la page et l'action principale (« Gérer mon abonnement »). 
2. .hint : le pire ratio de la page (1.91:1), quasiment illisible alors qu'il donne une information utile.
3. .label : texte le plus petit, il donne le contexte des valeurs (« Statut de l'abonnement », « Astuce »).
4. .subtitle : n'apporte pas d'information indispensable 

