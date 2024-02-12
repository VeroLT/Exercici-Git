Exercici GIT 4: Gestió de branques
=

Exercici 1
-
  Crea una nova branca bibliografia i mostrar les branques del repositori.
  Comandos:
    git branch bibliografia
    git checkout bibliografia
    git branch
    git branch -a
    
Exercici 2
-
    Crear el fitxer capítols/capitol4.txt i afegir el següent text
    Afegir els canvis a la zona d'intercanvi temporal.
    Fer un commit amb el missatge "Afegit capítol 4."
    Mostrar la història del repositori incloent totes les branques.
    Comandos:
      echo "En aquest capítol veurem com utilitzar GitHub per allotjar repositoris
      en remot." > capítols/capitol4.txt
      git add capítols/capitol4.txt
      git commit -m "Afegit capítol 4."
      git log --all --graph --oneline --decorate

Exercici 3
-
    Canvia a la branca bibliografia.
    Crea el fitxer bibliografia.txt i afegir la següent referència:
    Afegeix els canvis a la zona d'intercanvi temporal.
    Fes un commit amb el missatge "Afegida primera referència bibliogràfica."
    Mostra la història del repositori incloent totes les branques.
    Comandos:
      git checkout bibliografia
      echo "Afegeix els canvis a la zona d'intercanvi temporal." > bibliografia.txt
      git add bibliografia.txt
      git commit -m "Afegida primera referència bibliogràfica."
      git log --all --graph --oneline --decorate

Exercici 4
-
    Fusiona la branca bibliografia amb la branca master.
    Mostra la història del repositori incloent totes les branques.
    Elimina la branca bibliografia.
    Mostra de nou la història del repositori incloent totes les branques.
    Comandos:
      git checkout master
      git merge bibliografia
      git log --all --graph --oneline --decorate
      git branch -d bibliografia
      git log --all --graph --oneline --decorate

Exercici 5
-
    Crea la branca bibliografia.
    Canvia a la branca bibliografia.
    Canvia el fitxer bibliografia.txt perquè continga les següents referències:
    Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."
    Canvia a la branca master.
    Canvia el fitxer bibliografia.txt perquè continga les següents referències:
    Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."
    Fusiona la branca bibliografia amb la branca master.
    Resol el conflicte deixant el fitxer bibliografia.txt amb les referències:
    Afegeix els canvis a la zona d'intercanvi temporal i fes un commit amb el missatge "Resolt conflicte de bibliografia."
    Mostra la història del repositori incloent totes les branques.
    Comandos:
      git branch bibliografia
      git checkout bibliografia
      Canvia el fitxer "bibliografia.txt" perquè continga les següents referències:
        “Scott Chacon, Ben Straub. Pro Git. Apress.”
        “Ryan Hodson. Ry's Git Tutorial. Smashwords (2014).”
      git add bibliografia.txt
      git commit -m "Afegida nova referència bibliogràfica"
      git checkout master
      Canvia el fitxer "bibliografia.txt" perquè continga les següents referències:
        “A. Scott Chacon, B. Ben Straub. Pro Git. C. Apress.”
        “D. Ryan Hodson. Ry's Git Tutorial. E. Smashwords (2014).”
      git add bibliografia.txt
      git commit -m "Afegida nova referència bibliogràfica"
      git merge bibliografia
      Resol el conflicte deixant el fitxer "bibliografia.txt" amb les referències:
        “A. Scott Chacon, B. Ben Straub. Pro Git. C. Apress.”
        “D. Ryan Hodson. Ry's Git Tutorial. E. Smashwords (2014).”
      git add bibliografia.txt
      git commit -m "Resolt conflicte de bibliografia"
      git log --all --graph --decorate --oneline
