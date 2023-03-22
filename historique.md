# Historique des commandes du TP1

### Création d'un dépôt

- Initialise un dépôt vide, cette commande est exécuté une seule fois.
- Si on l'execute une deuxième fois on detruit le dépôt. 
- `git init`

---

### Vérifier le status

- `git status`

---

### Afficher l'historique des commits
- `git log`
- `git log --oneline`

---

### Naviguer dans les branches
- Pour changer le nom d'une branche
  - `git branch -m nom-branche`
  - `git branch -m main` // change lo nom de la branche courante pour main

- Pour creer une nouvelle branche
  - `git branch nouvelle-branche`

- Pour changer de branche
  - `git checkout nom-de-la-branche`
  - On ne peut pas changer de branche si la branche courante n'a pas été «commit» valider 
  - `git checkout id-du-commit`   
  - `git checkout etiquette du commit`

- Pour creer une etiquette (tag)
  - `git tag v1.0.0` // creation de l'etiquette v1.0.0
  - `git tag` // permet d'afficher l'ensemble des tag
  - `git checkout v1.0.0` // pour se déplacer dans le commit v1.0.0 (deplace le pointeur HEAD)

---

### Serveur distant
  - Pour definir un alias identifiant le serveur distant
  - `git remote add 41e https://github.com/pgng08/41e/`
  - `git remote -v` // permet de voir la liste des alias du serveur distant
  - `git push 41e main` // pousser mon dernier commit vers la branche main du depot distant 41e
  - `git pull 41e main` // recuperer la dernière version du depot distant 41e
