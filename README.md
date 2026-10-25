<h1 align="center">🪢 Hangman</h1>

<p align="center"><em>Trouve le mot avant que le bonhomme ne finisse au bout de sa corde. Puis fais deviner les tiens à tes amis.</em></p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python 3" />
  <img src="https://img.shields.io/badge/d%C3%A9pendances-aucune-success?style=for-the-badge" alt="Aucune dépendance" />
  <img src="https://img.shields.io/badge/projet%20d%27apprentissage-ff69b4?style=for-the-badge" alt="Projet d'apprentissage" />
</p>

---

## ✨ Pourquoi tu vas l'adorer

- **Deux versions** : une version de base avec des mots tirés au sort, et une version complète en mode « maître du jeu » à deux joueurs.
- **Pendu en ASCII** : le dessin se construit à chaque erreur, jusqu'à la victoire.
- **Saisies verrouillées** : une seule lettre à la fois, sans doublon.

## 🎮 Les deux versions

| Version | Fichier | Mots | Essais |
|---|---|---|:---:|
| V0 | `Code_Python_Hangman_V0` | Tirés au sort : `python`, `java`, `kotlin`, `javascript` | 8 |
| V1 | `code_Python_Hangman_V1` | Saisis par un joueur, avec un indice | 10 |

## 🚀 Lancer

```bash
python3 Code_Python_Hangman_V0
python3 code_Python_Hangman_V1
```

Tape `play` pour jouer, `exit` pour quitter.

## 🕹️ Exemple (V1, mode maître du jeu)

```text
Type "play" to play the game, "exit" to quit: play
Type "back" to go to the menu or the word to guess followed by a hint word :
example : "dog animal" : dog animal
is "dog" the word to guess and "animal" the hint word ? "yes" or "no" ?yes
Player : you have to find a 3 letters word. hint : animal
you have 10 tries. good luck !
```

Ensuite, le dessin du pendu apparaît et le jeu demande `Input a letter:`.

## 🧠 Sous le capot

- Le mot est caché sous forme de tirets `-`, révélés lettre après lettre (`hide_my_word`, `show_my_word`).
- Les lettres déjà proposées sont rangées dans un `set` : impossible de jouer deux fois la même.
- Les dessins du pendu sont stockés dans un tuple, indexé par le nombre d'erreurs.
- Pour « nettoyer » l'écran, le programme affiche 10 000 sauts de ligne : la méthode la plus rustique qui soit.

## 🔭 Pistes d'évolution

- Réactiver la fonction `clear()` déjà présente (commentée) pour un vrai nettoyage de l'écran.
- Ajouter un score et plusieurs manches.

---

<p align="center"><sub>Fait avec ❤️ et Python par DSKarim</sub></p>
