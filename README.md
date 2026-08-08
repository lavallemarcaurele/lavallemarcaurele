# Marc-Aurèle Lavalle

J'automatise mon SEO avec Claude Code. Plutôt que de refaire chaque mois les mêmes analyses à
la main, j'écris des **skills** qui collectent, croisent et produisent les rapports à ma place.

Elles tournent sur 6 sites en production. Je les ouvre une par une.

## Skills publiées

**[gsc-seo](https://github.com/lavallemarcaurele/gsc-seo)** — Search Console → rapport SEO
actionnable. 7 collectes sur 3 fenêtres temporelles, requêtes à portée, cannibalisation,
opportunités de page, 5 priorités du mois. Inclut le CLI Python qui parle à l'API.

**[concurrence-seo](https://github.com/lavallemarcaurele/concurrence-seo)** — veille
concurrentielle sans API payante. 16 signaux on-page par page, content gaps, schémas JSON-LD
manquants, comparaison intention par intention. WebFetch uniquement, aucune dépendance.

Les deux se croisent : `concurrence-seo` lit le rapport de `gsc-seo` s'il le trouve, pour
isoler les requêtes où vous êtes au-delà de la position 10 et où un concurrent a une page
dédiée. Ce sont les cas où il y a quelque chose de précis à apprendre d'eux.

## Ce qui arrive

`maillage-interne`, `ai-search-seo`, `coverage-villes`, `lead-funnel`, `posthog-analytics` —
dix skills encore à nettoyer avant publication.

## Pourquoi c'est ouvert

Parce que ces outils ne valent pas grand-chose sans le terrain qui va avec, et que le terrain
ne se copie pas.

Ce qui m'a coûté du temps, ce ne sont pas les scripts : ce sont les pièges. Celui-ci est
documenté dans `gsc-seo` — l'API Search Console trie par clics décroissants et départage les
ex æquo **par ordre alphabétique**. Sur un site où la plupart des lignes sont à zéro clic, une
limite trop basse ne remonte donc que le début de l'alphabet. Le JSON reste valide, le rapport
a l'air normal, et rien ne signale que les données sont tronquées.

C'est ce genre de chose que je publie.

---

[LinkedIn](https://www.linkedin.com/in/lavallemarcaurele/) · [Email](mailto:lavallemarcaurele@gmail.com)
