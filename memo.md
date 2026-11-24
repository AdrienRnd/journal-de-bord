# 🚀 Mémo Git Essentiel

## 1. Configuration initiale

| Commande | Description |
| :--- | :--- |
| `git config --global user.name "Nom"` | Définit ton nom d'utilisateur global. |
| `git config --global user.email "email@exemple.com"` | Définit ton adresse e-mail globale. |
| `git config --list` | Affiche toute la configuration actuelle. |

---

## 2. Démarrer un projet

| Commande | Description |
| :--- | :--- |
| `git init` | Initialise un nouveau dépôt Git local. |
| `git clone <url>` | Télécharge un dépôt distant sur ta machine. |

---

## 3. Cycle de base (Travail quotidien)

| Commande | Description |
| :--- | :--- |
| `git status` | Vérifie l'état des fichiers (modifiés, suivis, ignorés). |
| `git add <fichier>` | Ajoute un fichier spécifique à la zone de transit (*staging*). |
| `git add .` | Ajoute tous les fichiers modifiés et nouveaux au *staging*. |
| `git commit -m "Message"` | Enregistre les modifications dans l'historique avec un message. |
| `git commit -am "Message"` | Ajoute et commit en une seule fois (fichiers déjà suivis uniquement). |

---

## 4. Gestion des branches

| Commande | Description |
| :--- | :--- |
| `git branch` | Liste toutes les branches locales. |
| `git branch <nom>` | Crée une nouvelle branche. |
| `git switch <nom>` | Bascule sur une branche existante (remplace `checkout`). |
| `git switch -c <nom>` | Crée une nouvelle branche et bascule dessus immédiatement. |
| `git merge <branche>` | Fusionne la branche spécifiée dans la branche actuelle. |
| `git branch -d <nom>` | Supprime une branche locale (si déjà fusionnée). |

---

## 5. Dépôts distants (GitHub, GitLab...)

| Commande | Description |
| :--- | :--- |
| `git remote -v` | Affiche les dépôts distants liés. |
| `git remote add origin <url>` | Lie le dépôt local à un dépôt distant nommé `origin`. |
| `git pull` | Récupère et fusionne les modifications du dépôt distant. |
| `git push` | Envoie tes commits locaux vers le dépôt distant. |
| `git push -u origin <branche>` | Envoie une nouvelle branche sur le dépôt distant et la lie. |

---

## 6. Historique & Inspection

| Commande | Description |
| :--- | :--- |
| `git log` | Affiche l'historique complet des commits. |
| `git log --oneline --graph` | Affiche un historique condensé avec l'arbre des branches. |
| `git diff` | Montre les modifications non encore ajoutées au *staging*. |
| `git diff --staged` | Montre les modifications prêtes à être commitées. |

---

## 7. Annuler & Réparer (Urgences)

| Commande | Description |
| :--- | :--- |
| `git restore <fichier>` | Annule les modifications locales d'un fichier non stagé. |
| `git restore --staged <fichier>` | Retire un fichier de la zone de *staging* (garde les modifs). |
| `git commit --amend -m "Nouveau"` | Modifie le message (ou le contenu) du dernier commit. |
| `git revert <id-commit>` | Crée un nouveau commit qui annule proprement un commit passé. |
| `git reset --hard <id-commit>` | ⚠️ **Destructif** : revient à un commit précis et efface tout après. |

---

## 8. Mise de côté temporaire (Stash)

| Commande | Description |
| :--- | :--- |
| `git stash` | Sauvegarde temporairement les modifications non commitées. |
| `git stash pop` | Réapplique les dernières modifications mises de côté et les supprime du stash. |
| `git stash list` | Liste toutes les sauvegardes temporaires. |
Utilisez le code avec précaution.
