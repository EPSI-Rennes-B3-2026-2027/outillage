# Commandes de base
## Navigation

### Chemin absolu

Indique l'emplacement **complet** d'un fichier en partant de la **racine du système**.

| Système | Racine |
| --- | --- |
| Linux / macOS | `/` |
| Windows | `C:\` |

**Exemple :** 
```bash
cd /home/docus/dossier
```

### Chemin relatif

Indique l'emplacement d'un fichier **depuis l'endroit où on se trouve**. C'est le type de chemin le plus utilisé en programmation.

| Symbole | Signification | Exemple |
| --- | --- | --- |
| `.` | Répertoire **courant** | `./mon-script.sh` |
| `..` | Répertoire **parent** (un niveau au-dessus) | `cd ../` |
| `~` | Répertoire **utilisateur** (`/home/user`) | `cd ~` |

## La commande `cd`

Permet de **changer de répertoire courant**. En supposant qu'on est dans `/home/docus` :

```bash
cd ./dossier/   # → /home/docus/dossier/  (navigue dans le dossier)
cd ../          # → /home/               (remonte au dossier parent)
cd ~            # → /home/{user}    (va au répertoire utilisateur)
```

## Commandes de base git

- `git init` (initialisation d’un repository git)
- `git add {fichier(s)}` (ex: git add README.md) (permet d’ajouter des fichiers qui seront mis à jour sur le dépot) (plusieurs add sont disponible avant de commit)
- `git commit -m {message}` (ex: git commit -m “Maj README”) (comme un bouton de sauvegarde, il sauvegarde en local tout les fichiers modifiés) (plusieurs commits sont possible avant push)
- `git push {branche}` (permet de “pousser” les commits faits, sur le repository git)

# Processus

### Commandes pour voir les processus (linux)

- `free` (et option -h)
<img width="981" height="195" alt="image" src="https://github.com/user-attachments/assets/7e312751-297a-4b09-85e0-d15085a694f0" />

---

- `top`
<img width="981" height="195" alt="image" src="https://github.com/user-attachments/assets/8bcadf23-624b-43dd-9de0-70817108ae6c" />

---

- `htop` (top en version colorée, à installer)
<img width="1437" height="415" alt="image" src="https://github.com/user-attachments/assets/112cad29-fef2-40b4-9cc8-7552f9ea56a5" />

---

- `ps aux`
<img width="865" height="196" alt="image" src="https://github.com/user-attachments/assets/696f8a05-4c8c-4b24-8b6a-bb6de894d360" />

---

## Disques

- `df` (avec option -h)
<img width="1060" height="392" alt="image" src="https://github.com/user-attachments/assets/57bd5689-9d98-4ec7-a186-e7d363d1a9c0" />

---

- `lsblk`
<img width="580" height="158" alt="image" src="https://github.com/user-attachments/assets/354d872b-3e38-458c-b19d-fb0ab70dd661" />

## Vérifier la version d'un outil

Pour savoir quelle version d'un programme est installée :

```bash
node --version    # ex: v22.1.0
python --version  # ex: Python 3.12.3
git --version     # ex: git version 2.44.0
```
