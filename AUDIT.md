# AUDIT.md : à compléter

Pour chaque ligne, retrouve le problème correspondant dans `src/App.tsx` / `src/App.css`
et remplis les 3 colonnes. Il y a **6 problèmes volontaires** dans ce starter.

| # | Problème trouvé (où, quoi) | Principe WCAG (P / O / U / R) | Pourquoi c'est bloquant, et pour qui |
|---|------------------------------|-------------------------------|----------------------------------------|
| 1 | img src="/hero.jpg" n'a pas d'alt  | Perceptible | Si l'image ne charge pas ou un utilisateur aveugle regarde la page il ne peut pas la voir  |
| 2 | div className="see-more" onClick utilisé une div au lieu d'un button | Opérable | le lecteur d'écran et l'utilisateur ne peuvent pas savoir que c'est un boutton|
| 3 | Statut "annulé"/"publié" avec la couleur du point rouge ou vert | Perceptible | Information très difficilement perceptible pour un daltonien (manque d'un texte de status)|
| 4 | Manque h2 après h1 qui passe directement a h3 | Robuste | Les titres permettent de naviguer efficacement sur la page|
| 5 | Trois liens avec le même texte "cliquez ici" | Compréhensible | On ne sait pas ce que chaque lien fait avec un lecteur d'écran|
| 6 | Le carousel s'affiche sans aucun moyen de le fermer | Opérable | WCAG 2.2.2 : tout contenu qui apparaît doit pouvoir être maîtrisé par l'utilisateur |

> Rappel : P = Perceptible, O = Opérable, U = Utilisable (Compréhensible), R = Robuste.
