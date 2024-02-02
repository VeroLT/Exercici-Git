Exercici GIT 1: Exercicis de creació i actualització de repositoris 

Verónica Lull Torres 
Entorns de desenvolupament 
IES Enric Valor (Pego)





Índex: 
Exercici GIT 1: Exercicis de creació i actualització de repositoris. 1 
Índex:.......................................................................................................2 Activitat 1:...............................................................................................................................3 Pas 1: Mostra l'historial de canvis del repositori.....................................................3 Pas 2:Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb un text..............3 Pas 3: Afegeix els canvis a la zona d'intercanvi temporal (staging area).......................... 3 Pas 4: Fes un commit dels canvis amb el missatge "Afegit capítol 1.".............................. 3 Pas 5: Torna a mostrar l'historial de canvis del repositori.................................................. 3 Activitat 2:...............................................................................................................................5 Pas 1: Crea el fitxer capitol2.txt a la carpeta capítols amb el text......................................5 Pas 2: Realizar un commit de los cambios con el mensaje "Afegit capítol 2."...................5 Paso 3: Mostrar las diferencias entre la última versión y las dos versiones anteriores..... 6 
Activitat 3: Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i veure l'estat del repositori...................................................................................... 9 Pas 1: Crea el fitxer capitol3.txt a la carpeta capítols amb un text:....................................9 Pas 2: Afegeix els canvis a la zona d'intercanvi temporal..................................................9 Activitat 4:.............................................................................................................................10 Pas 1: Afegir al final del fitxer índex.txt la següent línia:..................................................10 Pas 2: Afegir canvis a la zona d'intercanvi temporal (staging area).................................10 Pas 3: Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex."...............11 Pas 4: Mostrar qui ha fet canvis sobre el fitxer índex.txt.................................................. 11 

Activitat 1: 
Pas 1: Mostra l'historial de canvis del repositori. 
fent el comandament “git log”. 
Pas 2:Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb un text. 
Crea l’arxiu capitol2.txt amb el text proporcionat. 
echo "Git és un sistema de control de versions ideat per Linus Torvalds" > capítols/capitol2.txt” 
Pas 3: Afegeix els canvis a la zona d'intercanvi temporal (staging area) 
Afegim el comandament “git add capítols/capitol2.txt” 
Pas 4: Fes un commit dels canvis amb el missatge "Afegit capítol 1." 
Afegim el comandament “git commit -m "Añadido archivo capitol2.txt en capítols"”. 
Pas 5: Torna a mostrar l'historial de canvis del repositori. Afegim el comandament “git log” 

Activitat 2: 
Pas 1: Crea el fitxer capitol2.txt a la carpeta capítols amb el text 
Crear la carpeta 'capítols' si no està creada 
mkdir -p capítols 
Crear l’arxiu capitol2.txt amb el text proporcionat 
echo "Texto del capítulo 2" > capítols/capitol2.txt 
Afegir els canvios a la zona d’intercanvi temporal (staging area) 
git add capítols/capitol2.txt 
Comprobar l’estat del repositori. 
git status 
Pas 2: Realizar un commit de los cambios con el mensaje "Afegit capítol 2." 
Realitzar el commit amb el missatge especificat 
git commit -m "Afegit capítol 2." 
Mostrar l’historial de canvis del repositori git log 
Paso 3: Mostrar las diferencias entre la última versión y las dos versiones anteriores 
Mostrar les diferències respecte a l’última versió 
git diff HEAD^ HEAD 

Activitat 3: Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i veure l'estat del repositori. 
Pas 1: Crea el fitxer capitol3.txt a la carpeta capítols amb un text: 
Amb el comandament “echo -e"Git permet la creació de branques, la qual cosa permet tindre distintes versions del mateix projecte i treballar simultàniament en elles."” 
Pas 2: Afegeix els canvis a la zona d'intercanvi temporal. 
Afegir canvis a la zona d'intercanvi temporal (staging area) 
“git add capítols/capitol3.txt” 
Fer el commit amb el missatge especificat 
“git commit -m "Afegit capítol 3."” 
Mostrar les diferències entre la primera i l'última versió del repositori “git log” 


Activitat 4: 
Pas 1: Afegir al final del fitxer índex.txt la següent línia: 
Pots utilitzar un editor de text o el següent comandament per canviar el contingut del fitxer: “echo "Afegir l’informació dins del fitxer" > índex.txt” 
Pas 2: Afegir canvis a la zona d'intercanvi temporal (staging area) 
Amb el comandament de “git add index.txt” 
Pas 3: Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex." 
Afegim un “git commit -m "Afegit capítol 5 a l'índex."” 
Pas 4: Mostrar qui ha fet canvis sobre el fitxer índex.txt. I per últim, “git log índex.txt”. 

