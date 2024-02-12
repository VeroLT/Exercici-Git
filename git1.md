Exercici GIT 1: Creació i actualització de repositoris
=
Indica els comandaments amb els quals resoldries els escenaris plantejats en els diferents exercicis.

Exercici 1
-
    Crea un repositori nou amb el nom llibre i mostra el seu contingut.
    Configura Git definint el nom de l'usuari, el correu electrònic i activa l'exida en color. Mostra la configuració final.
    Comandos:
        git log
        echo "Git és un sistema de control de versions ideat per Linus Torvalds" >
        capítols/capitol2.txt”
        git add capítols/capitol2.txt
        git commit -m "Añadido archivo capitol2.txt en capítols"
        git log

        
Exercici 2
-
    Comprova l'estat del repositori.
    Crea un fitxer índex.txt amb el següent contingut:
    Comprova de nou l'estat del repositori.
    Afegeix el fitxer a la zona d'intercanvi temporal.
    Torna a comprovar una vegada més l'estat del repositori.
    Comandos:
        mkdir -p capítols
        echo "Texto del capítulo 2" > capítols/capitol2.txt
        git add capítols/capitol2.txt
        git status
        git commit -m "Afegit capítol 2.
        git log
        git diff HEAD^ HEAD

Exercici 3 Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i revisa l'estat del repositori.
-
    Comandos:
        echo -e
        git add capítols/capitol3.txt
        git commit -m "Afegit capítol 3."
        git log

Exercici 4
-
    Canvia el fitxer índex.txt perquè continga el següent:

    Mostra els canvis respecte a l'última versió guardada al repositori.
    Fes un commit dels canvis amb el missatge "Afegit capítol 3 sobre gestió de branques".
    Comandos:
        echo "Afegir l’informació dins del fitxer" > índex.txt
        git add index.txt
        git commit -m "Afegit capítol 5 a l'índex."+
        git log índex.txt
        

Exercici 5
-
    Mostra els canvis de l'última versió del repositori respecte a l'anterior.
    Canvia el missatge de l'últim commit a "Afegit capítol 3 sobre gestió de branques a l'índex."
    Torna a mostrar els últims canvis del repositori.
    Comandos:
        git diff HEAD^ HEAD
        git commit --amend -m "Missatge"
        git diff HEAD^ HEAD
        

Exercici 6
-
Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els que tenen l'extensió out i les imatges (jpg, png, bmp i gif).
Comandos: 
    nano .gitignore
    Per ignorar el fitxer daw es daw*, per ignorar l’extensió out es *.out i per ignorar les
    imatges es *.jpg, *.png, *.bmp, *.git
    git add .gitignore
    
    
