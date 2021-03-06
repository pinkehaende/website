# Pinke Hände Portfolio

Dieses Repository dient als vollständige Quelle für den Webauftritt der Pinken Hände.

## Schneller Einstieg

0. [git](https://git-scm.com/downloads) und [hugo](https://gohugo.io/getting-started/installing/) installieren
1. Dieses Repository klonen
```sh
git clone --recurse-submodules https://github.com/pinkehaende/website.git
cd website

# Einen eigenen Branch erstellen (optional)
git checkout -b DEIN_BRANCH origin/master
git branch -u DEIN_BRANCH
```
2. hugo Live Server starten (optional, aber empfohlen)
```sh
hugo server -D -E -F
# Erreichbar unter http://localhost:1313/
```
3. Dinge hinzufügen, ändern, entfernen
4. Änderungen versionieren
```sh
git add . # Oder eine Liste mit geänderten Dateien
git commit -m "Meine tolle neue Idee: Zigarettenfilter mit Asbest"
git push 
```
5. Änderungen veröffentlichen
```sh
hugo --minify
# Dateien in `public/` auf den Webhoster laden
rsync -avz --delete public/ username@meinhoster.de:~/www/
```
