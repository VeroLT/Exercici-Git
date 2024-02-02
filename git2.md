Exercici GIT 2: Ús de l'historial de canvis


Verónica Lull Torres
Entorns de desenvolupament
IES Enric Valor (Pego)
Índex:


Exercici GIT 2: Ús de l'historial de canvis	1
Índex:	2

Activitat 1:	3

Pas 1: Crear un repositori i mostra el contingut	3
Pas 2: Configura Git definint el nom de l'usuari, el correu electrònic i activar l'exida en color. Mostrar la configuració final.	3
Activitat 2:	4

Pas 1: Comprova l'estat del repositori	4
Pas 2: Crea un fitxer amb contingut	4
Pas 3: Comprova l’estat del repositori	4
Pas 4: Afegeix el fitxer a la zona d’intercanvi temporal	4
Pas 5: Comprova l’estat del repositori	5

Activitat 3: Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i veure l'estat del repositori.	5
Pas 1: Realitzar el commit amb el missatge "Afegit índex del llibre"	5
Pas 2: Comprova l’estat del repositori	5

Activitat 4:	6
Pas 1: Canvia el fitxer índex.txt:	6
Pas 2: Mostrar els canvis respecte a l'última versió guardada al repositori:	6
Pas 3: Fer un commit dels canvis amb el missatge:
	6
Activitat 5:	7
Pas 1: Mostrar els canvis de l'última versió del repositori respecte a l'anterior:	7
Pas 2: Canviar el missatge de l'últim commit:	7
Pas 3: Tornar a mostrar els últims canvis del repositori:
	7
Activitat 6: Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els que tenen l'extensió out i les imatges (jpg, png, bmp i gif).	8
Pas 1: Creem un fitxer gitignore i posem les extensions següents:	8


Activitat 1:
Pas 1: Crear un repositori i mostra el contingut

Fem un “mkdir llibre” per crear un nou directori. 
El cd llibre per accedir al directori.
Un git init, per iniciar el nou repositori.
I finalment un “ls -la”, per mostrar el contingut del repositori.



Pas 2: Configura Git definint el nom de l'usuari, el correu electrònic i activar l'exida en color. Mostrar la configuració final.

Per configurar el nom de l'usuari gastem “git config --global user.name” i el nom de l’usuari.

Per configurar el correu electrònic posem “git config --global user.email” i el email.

Per activar l'exida en color fem el comando de “git config --global color.ui true”

Per mostrar la configuració final que tenim “git config --global --list”.



Activitat 2:
Pas 1: Comprova l'estat del repositori 
Utilitzant “git status”.

Pas 2: Crea un fitxer amb contingut
Creem un fitxer índex.txt amb contingut: 
Capitol 1: Introducció a Git
Capitol 2: Fluxe de treball bàsic
Capitol 3: Repositoris remots
Utilitzem el comando echo i afegim el contingut o gastem una fulla en blanc i després ho afegim a git.

Pas 3: Comprova l’estat del repositori 
Comprova de nou l'estat del repositori amb “git status”.

Pas 4: Afegeix el fitxer a la zona d’intercanvi temporal
Afegeix el fitxer a la zona d'intercanvi temporal amb “ git add index.txt”.

Pas 5: Comprova l’estat del repositori 
Tornar a comprovar una vegada més l'estat del repositori amb “git status”.


Activitat 3: Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i veure l'estat del repositori.

Pas 1: Realitzar el commit amb el missatge "Afegit índex del llibre"

Utilitzem git commit -m "Afegit índex del llibre" per realitzar el commit.

Pas 2: Comprova l’estat del repositori 
Tornar a comprovar una vegada més l'estat del repositori amb “git status”.


Activitat 4: 
Pas 1: Canvia el fitxer índex.txt:
Pots utilitzar un editor de text o el següent comandament per canviar el contingut del fitxer:
“echo "Afegir l’informació dins del fitxer" > índex.txt”

Pas 2: Mostrar els canvis respecte a l'última versió guardada al repositori:
Amb el comandament “git diff”. Aquest comandament mostra les diferències entre l'última versió guardada al repositori i els canvis actuals al teu directori de treball.

Pas 3: Fer un commit dels canvis amb el missatge:
Fem els següents passos:
“git add índex.txt  # Afegir el fitxer a la zona d'intercanvi temporal “
“git commit -m "Afegit capítol 3 sobre gestió de branques"”


Activitat 5:
Pas 1: Mostrar els canvis de l'última versió del repositori respecte a l'anterior:

“git diff HEAD^ HEAD”

Aquest comandament et mostrarà les diferències entre l'últim commit (HEAD) i el commit anterior (HEAD^).

Pas 2: Canviar el missatge de l'últim commit:

“git commit --amend -m "Missatge"”

Amb aquest comandament em modificat el commit anterior.

Pas 3: Tornar a mostrar els últims canvis del repositori:

“git diff HEAD^ HEAD”

Aquest comandament mostra les diferències entre l'últim commit i el commit anterior amb el nou missatge.


Activitat 6: Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els que tenen l'extensió out i les imatges (jpg, png, bmp i gif).
Pas 1: Creem un fitxer gitignore i posem les extensions següents:
Amb el comando “nano .gitignore”
Per ignorar el fitxer  daw es daw*, per ignorar l’extensió out es *.out i per ignorar les imatges es *.jpg, *.png, *.bmp, *.git
Afegir i fer commit de gitignore ”git add .gitignore”.
Ara git ignora els fitxers i directoris especificats en .gitignore



