`git status` - wyświetla status zmian (i które są dodane do commita)
`git fetch` - pobiera informację o zmianach i nowych branchach - warto wykonać komendę przed git checkout
`git add -A` - dodaje wszystkie zmiany do commita
`git add sciezka/do/pliku` - dodaje folder/plik do commita
`git commit -m "Tytul commita/komentarz"` - tworzy commita
`git push` - wypycha zmiany do remote'a (o ile remote na remote branch został ju stworzony)
`git push -u origin/nazwa-brancha` - wypycha zmiany do remote'a i tworzy branch w remote repo
`git checkout nazwa-brancha` - przełącza na branch
`git checkout -b nazwa-brancha` - tworzy nowy branch (lokalnie)
`git pull` - pobiera zmiany z repo (dla obecnie wybranego brancha)
`git reset --hard origin/nazwa-brancha` - resetuje lokalnego brancha do stanu z danego brancha na remote (nieodwracalne)



Przykładowy flow gdy tworzymy branch lokalnie:

git checkout master
git pull
git checkout -b nazwa-brancha
// zmiany w plikach
git add -A
git commit -m "Nazwa commita"
git push -u origin nazwwa/brancha
// wchodzimy na GitHuba i tworzymy Pull Requests



Przykładowy flow gdy tworzymy branch na GitHubie

git fetch
git checkout nazwa-brancha
git pull
// zmiany w plikach
git add -A
git commit -m "Nazwa commita"
git push