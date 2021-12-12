# Git

Christian Grubmüller, 19.11.2021

#### Name und Email setzten

```bash
git config --global user.email "<email>"
git config --global user.name "<name>"
```

#### Github access über das Terminal (SSH)

In Linux kann man mit folgendem Command einen SSH-Key erstellen.

```bash
ssh-keygen -t rsa -b 4096
```

Dann muss man die zwei Files, die in dem aktuellen Ordner erstellt werden, in `~/.ssh` hineinverschiebt.

Dann muss man auf Github unter `Settings>SSH and GPG key` auf  *New Key* drücken und den öffentlichen Schlüssel hineinkopieren. (Inhatl von `.pub` File)

Um Repositories dann zu klonen muss man ssh auswählen.



## Files zu .gitignore hinzufügen

1. File/Ordner zu `.gitignore` hinzufügen.

2. Cache löschen

   ```bash
   # Cache für alle Files/Ordner
   git rm -r --cached .
   # Cache für spezifische Files/Ordner
   git rm -r --cached <file_name.ext>
   ```

3. Andere Files/Ordner hinzufügen

   ```bash
   # Alle Files/Ordner
   git add .
   # spezifische Files/Ordner
   git add <file_name.ext>
   ```

4. Commiten

   ```bash
   git commit -m "commit message"
   ```

   

