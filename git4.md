Exercici GIT 4: Gestió de branques


Verónica Lull Torres
Entorns de desenvolupament
IES Enric Valor (Pego)

Índex:
Exercici GIT 4: Gestió de branques	1
Índex:	2

Activitat 1:	3

Pas 1: Crear la nova branca "bibliografia":	3

Pas 2: Canviar a la nova branca "bibliografia":	3

Pas 3: Comprovar que estem a la branca "bibliografia":	3

Pas 4: Mostrar totes les branques del repositori:	3


Activitat 2:	3

Pas 1: Crea el fitxer capítols/capitol4.txt amb el text desitjat. Podem utilitzar l'editor de text o la comanda echo:	3

Pas 2: Afegim els canvis a la zona d'intercanvi temporal:	4

Paso 3: Realitzem un commit amb el missatge "Afegit capítol 4":	4

Pas 4: Mostra la història del repositori, incloent totes les branques:	4


Activitat 3: Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i veure l'estat del repositori.	5

Pas 1: Canvia a la branca bibliografia	5

Pas 2: Crea el fitxer bibliografia.txt amb el contingut proporcionat	5

Pas 3: Afegim els canvis a la zona d'intercanvi temporal	5

Pas 4: Fem un commit amb el missatge "Afegida primera referència bibliogràfica."	5

Pas 5: Mostra la història del repositori incloent totes les branques	5


Activitat 4:	6

Pas 1:  Assegura't que estàs a la branca master	6

Pas 2: Fusió de la branca bibliografia amb la branca master	6

Pas 3:Mostra la història del repositori amb totes les branques	6

Pas 4: Eliminem la branca bibliografia	7

Pas 5: Mostra de nou la història del repositori amb totes les branques	7


Activitat 5:	8

Pas 1: Crea la branca "bibliografia".	8

Pas 2: Canvia a la branca "bibliografia".	8

Pas 3: Canvia el fitxer "bibliografia.txt" perquè continga les següents referències:	8

Pas 4: Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica".	8

Pas 5: Canvia a la branca "master".	8

Pas 6: Canvia el fitxer "bibliografia.txt" perquè continga les següents referències:	8

Pas 7: Afegeix els canvis a la zona d'intercanvi temporal i fem un commit amb el missatge "Afegida nova referència bibliogràfica".	9


Pas 8: Fusiona la branca "bibliografia" amb la branca "master".	9

Pas 9: Resol el conflicte deixant el fitxer "bibliografia.txt" amb les referències:	9

Pas 10: Afegeix els canvis a la zona d'intercanvi temporal i fem un commit amb el missatge "Resolt conflicte de bibliografia".	9

Pas 11: Mostra la història del repositori incloent totes les branques.	9


Activitat 1:
Pas 1: Crear la nova branca "bibliografia":

Fem el comandament “git branch bibliografia”.
Pas 2: Canviar a la nova branca "bibliografia":

Amb el comandament “git checkout bibliografia”
Pas 3: Comprovar que estem a la branca "bibliografia":

Fem un “git branch”
Pas 4: Mostrar totes les branques del repositori:
Fem un “git branch -a”

Activitat 2:
Pas 1: Crea el fitxer capítols/capitol4.txt amb el text desitjat. Podem utilitzar l'editor de text o la comanda echo:
Fem un “echo "En aquest capítol veurem com utilitzar GitHub per allotjar repositoris en remot." > capítols/capitol4.txt”

Pas 2: Afegim els canvis a la zona d'intercanvi temporal:
Fem un “git add capítols/capitol4.txt”

Paso 3: Realitzem un commit amb el missatge "Afegit capítol 4":
Fem un “git commit -m "Afegit capítol 4."”

Pas 4: Mostra la història del repositori, incloent totes les branques:
Fem un “git log --all --graph --oneline --decorate”


Activitat 3: Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i veure l'estat del repositori.

Pas 1: Canvia a la branca bibliografia
Fem un “git checkout bibliografia”

Pas 2: Crea el fitxer bibliografia.txt amb el contingut proporcionat
Fem un  “echo "Afegeix els canvis a la zona d'intercanvi temporal." > bibliografia.txt”

Pas 3: Afegim els canvis a la zona d'intercanvi temporal
Fem un “git add bibliografia.txt”

Pas 4: Fem un commit amb el missatge "Afegida primera referència bibliogràfica."
Fem un “git commit -m "Afegida primera referència bibliogràfica."”

Pas 5: Mostra la història del repositori incloent totes les branques
Fem un “git log --all --graph --oneline --decorate”

Activitat 4: 
Pas 1:  Assegura't que estàs a la branca master
Fem un “git checkout master”

Pas 2: Fusió de la branca bibliografia amb la branca master
Fem un “git merge bibliografia”

Pas 3:Mostra la història del repositori amb totes les branques
Fem un “git log --all --graph --oneline --decorate”

Pas 4: Eliminem la branca bibliografia
Fem un “git branch -d bibliografia”

Pas 5: Mostra de nou la història del repositori amb totes les branques
Fem un  “git log --all --graph --oneline --decorate”


Activitat 5:
Pas 1: Crea la branca "bibliografia".
Fem un “git branch bibliografia”

Pas 2: Canvia a la branca "bibliografia".
Fem un “git checkout bibliografia”

Pas 3: Canvia el fitxer "bibliografia.txt" perquè continga les següents referències:
“Scott Chacon, Ben Straub. Pro Git. Apress.”
“Ryan Hodson. Ry's Git Tutorial. Smashwords (2014).”

Pas 4: Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica".
Fem un “git add bibliografia.txt”
i un “git commit -m "Afegida nova referència bibliogràfica"”

Pas 5: Canvia a la branca "master".
Fem un “git checkout master”

Pas 6: Canvia el fitxer "bibliografia.txt" perquè continga les següents referències:
“A. Scott Chacon, B. Ben Straub. Pro Git. C. Apress.”
“D. Ryan Hodson. Ry's Git Tutorial. E. Smashwords (2014).”

Pas 7: Afegeix els canvis a la zona d'intercanvi temporal i fem un commit amb el missatge "Afegida nova referència bibliogràfica".
Fem un  “git add bibliografia.txt”
i un  “git commit -m "Afegida nova referència bibliogràfica"”

Pas 8: Fusiona la branca "bibliografia" amb la branca "master".
Fem un “git merge bibliografia”

Pas 9: Resol el conflicte deixant el fitxer "bibliografia.txt" amb les referències:
“A. Scott Chacon, B. Ben Straub. Pro Git. C. Apress.”
“D. Ryan Hodson. Ry's Git Tutorial. E. Smashwords (2014).”

Pas 10: Afegeix els canvis a la zona d'intercanvi temporal i fem un commit amb el missatge "Resolt conflicte de bibliografia".
Fem un “git add bibliografia.txt”
i un  “git commit -m "Resolt conflicte de bibliografia"”

Pas 11: Mostra la història del repositori incloent totes les branques.
Fem un “git log --all --graph --decorate --oneline”
