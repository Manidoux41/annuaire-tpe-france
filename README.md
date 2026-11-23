# Annuaire national des tribunaux pour enfants

Application web statique en HTML, CSS et JavaScript.

## Données réunies

- 156 tribunaux pour enfants récupérés en direct depuis l'API officielle de l'Annuaire de l'administration (DILA / Service Public).
- Les adresses électroniques actuellement publiées sur les fiches officielles restent dans la colonne « Courriel publié actuellement ».
- Les anciennes adresses de la liste Justice.fr du 23 avril 2020 sont rapprochées par ville et présentées séparément comme « Historique 2020 · à confirmer ».
- Les anciens contacts sont généralement des boîtes générales de tribunaux judiciaires de rattachement, pas des adresses dédiées aux TPE.
- Les adresses historiques ne sont jamais présentées comme vérifiées ou actives.
- Les sources et statuts sont conservés dans les fichiers JSON de `data/`.

## Fonctionnalités

- Recherche par ville, tribunal, adresse, téléphone ou courriel.
- Filtres par département, région et disponibilité des courriels (actuels / historiques / aucun).
- Tri par ville ou département.
- Export CSV et Excel.
- Liens vers les fiches officielles Service Public.

## Sources

- API officielle : https://api-lannuaire.service-public.gouv.fr/api/explore/dataset/api-lannuaire-administration/
- Documentation API : https://www.data.gouv.fr/dataservices/api-annuaire-de-ladministration-et-des-services-publics
- Liste historique Justice.fr : publiée le 23/04/2020, à confirmer.
- Sièges et ressorts légaux : https://www.legifrance.gouv.fr/codes/article_lc/LEGIARTI000039060197/2026-07-15

## Lancer en local

Ouvrir `index.html` via un serveur statique, par exemple :

```bash
npx serve .
```

L'API DILA et les fichiers JSON historiques doivent être accessibles depuis le même hébergement.
