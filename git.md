# Git

#### Name und Email setzten

```bash
git config --global user.email "<email>"
git config --global user.name "<name>"
```

#### Github access über das Terminal

 Zuerst muss man sich auf Github einen *personal access token* erstellen ([Hier](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)). Den habe ich mir dann abgespeichert.

Wenn man nun will, dass man auf dem ganzen System diesen *Access Token* verwenden kann um zu pullen, pushen oder committen, muss man Benutzername und Token mit folgendem Befehl global setzten.

```bash
git config --global url."https://${username}:${access_token}@github.com".insteadOf "https://github.com"
```

