# Page souvenirs — Souadou 🌸

Site statique (HTML + photos + vidéos), sans installation ni serveur.

## Contenu
- `index.html` : la page (enveloppe, petit mot, photos déplaçables, vidéos)
- `assets/photos/` : 12 photos (`photo-XX.jpg` en grand, `photo-XX-th.jpg` en miniature)
- `assets/videos/` : 5 vidéos (`video-1.mp4` à `video-5.mp4`, la 1 est affichée en premier)

## Tester en local
Ouvre `index.html` dans le navigateur.

## Mettre en ligne avec GitHub Pages
1. Crée un dépôt sur GitHub et envoie-y tout le contenu de ce dossier (`index.html` à la racine).
2. Dans le dépôt : **Settings → Pages**.
3. Source : **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
4. Après 1 à 2 minutes, le site est disponible à `https://TON-PSEUDO.github.io/NOM-DU-DEPOT/`.

## À savoir
- Un dépôt public rend les photos et vidéos accessibles à tous ceux qui trouvent l'adresse.
  Un dépôt privé ne marche avec GitHub Pages que sur certains plans payants.
- Pour changer le prénom, la date d'anniversaire ou activer le verrouillage, modifie les constantes
  `NAME`, `BDAY` et `LOCK` en haut du `<script>` dans `index.html`
  (`LOCK = true` : l'enveloppe ne s'ouvre qu'à partir du jour de l'anniversaire).
- Quand l’heure de `BDAY` arrive, l’écran d’ouverture affiche 3, 2, 1, 🎉 puis ouvre la page tout seul (aussi si la page est ouverte après la date).
  Pour tester, mets `BDAY` à quelques secondes dans le futur, par exemple `new Date(Date.now()+10000)`.
- Le verrouillage se base sur l'heure du téléphone : il n'est pas infaillible.
  Le plus sûr est de n'envoyer le lien que le jour J.
