# 🎵 Musique - Recherche Chanson / Vidéo YouTube

Une application web permettant de **rechercher des chansons ou artistes**, et d’afficher soit un **fichier MP3 local**, soit une **vidéo YouTube** correspondante.  

---

## 🖼️ Aperçu

![Page d'accueil](screenshots/home.png)  
*Page principale avec champ de recherche et boutons de catégorie.*

![Résultats MP3](screenshots/mp3_result.png)  
*Si le MP3 local est trouvé, le lecteur audio apparaît.*

![Résultats YouTube](screenshots/youtube_result.png)  
*Si le MP3 local n’existe pas, les vidéos YouTube correspondantes sont affichées.*

---

## 🛠 Fonctionnalités

- Recherche par **titre ou artiste**.
- Lecture des fichiers **MP3 locaux** si présents dans le dossier `musique/`.
- Recherche automatique sur **YouTube** si le MP3 local n’est pas disponible.
- Interface responsive et moderne.
- Affichage des résultats sous forme de cartes avec lecteur audio ou vidéo intégrée.

---

## 📂 Structure du projet

/projet-musique/
│
├─ index.html # Page principale avec HTML, CSS et JS
├─ README.md # Documentation du projet
├─ screenshots/ # Captures d'écran pour le README
│ ├─ home.png
│ ├─ mp3_result.png
│ └─ youtube_result.png
└─ musique/ # Dossier contenant les MP3 locaux
├─ BlackClover.mp3
├─ MySong.mp3
└─ ...

---

## ⚙️ Installation et utilisation

1. **Cloner le projet** ou télécharger les fichiers.  
2. **Créer un dossier `musique/`** à côté de `index.html`.  
3. Ajouter des fichiers MP3 dans ce dossier, par exemple :  
4. **Ouvrir `index.html`** via un serveur local recommandé :  
- **VS Code + Live Server**  
- Ou **Python `http.server`** :  
  ```bash
  python -m http.server 5500
  ```
5. **Rechercher un titre ou artiste** dans le champ de recherche.  
6. Le lecteur audio local s’affichera si le MP3 existe, sinon les vidéos YouTube correspondantes seront affichées.

---

## 🔑 Configuration de la clé API YouTube

1. Crée un projet sur [Google Cloud Console](https://console.developers.google.com/).  
2. Active **YouTube Data API v3**.  
3. Crée une **clé API** et remplace la variable `apiKey` dans `index.html` :  

```javascript
const apiKey = 'VOTRE_CLE_API';
📝 Technologies utilisées

HTML5 / CSS3

JavaScript (fetch API, manipulation DOM)

YouTube Data API v3

⚠️ Remarques

Pour que la vérification des fichiers MP3 fonctionne correctement, il est recommandé de lancer le projet via un serveur local.

Les vidéos YouTube fonctionnent même si le HTML est ouvert directement sans serveur.

👤 Auteur

Josue KIALENGELA-TAZI

Étudiant en BTS SIO – Option SLAM