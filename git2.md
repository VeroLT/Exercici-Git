Exercici GIT 2: Ús de l'historial de canvis
=

Exercici 1
-
    Mostra l'historial de canvis del repositori.
    Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb el següent text:
    Afegeix els canvis a la zona d'intercanvi temporal (staging area)
    Fes un commit dels canvis amb el missatge "Afegit capítol 1."
    Torna a mostrar l'historial de canvis del repositori.
    Comandos:
    	mkdir llibre
     	cd llibre
      	git init
       	ls -la
		git config --global user.name
	 	git config --global user.email
	  	git config --global color.ui true
	   	git config --global --list
  
Exercici 2
-
    Crea el fitxer capitol2.txt a la carpeta capítols amb el següent text:
    Afegeix els canvis a la zona d'intercanvi temporal.
    Fes un commit dels canvis amb el missatge "Afegit capítol 2."
    Mostra les diferències entre l'última versió i les dues versions anteriors.
    Comandos:
    	git status
     	Creem un fitxer índex.txt amb contingut:
		Capitol 1: Introducció a Git
		Capitol 2: Fluxe de treball bàsic
		Capitol 3: Repositoris remots
	  	git status
	   	git add index.txt
    	git status

Exercici 3
-
    Crea el fitxer capitol3.txt a la carpeta capítols amb el següent text:
    Afegeix els canvis a la zona d'intercanvi temporal.
    Fes un commit dels canvis amb el missatge "Afegit capítol 3."
    Mostra les diferències entre la primera i l'última versió del repositori.  
    Comandos:
    	git commit -m "Afegit índex del llibre"
     	git status

Exercici 4
-
    Afegir al final del fitxer índex.txt la següent línia:
    Afegir els canvis a la zona d'intercanvi temporal.
    Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex."
    Mostrar qui ha fet canvis sobre el fitxer índex.txt.   
    Comandos:
    	echo "Afegir l’informació dins del fitxer" > índex.txt
     	git diff
      	git add índex.txt # Afegir el fitxer a la zona d'intercanvi temporal
       	git commit -m "Afegit capítol 3 sobre gestió de branques"
       	
