Exercici GIT 3: Desfer canvis

Verónica Lull Torres
Entorns de desenvolupament
IES Enric Valor (Pego)
Índex:

Exercici GIT 3: Desfer canvis	1
Índex:	2

Activitat 1:	3
Pas 1: Elimina l'última línia del fitxer index.txt i guarda-ho.	3

Pas 2: Comprova l'estat del repositori.	3

Pas 3: Desfés els canvis realitzats al fitxer index.txt per tornar a la versió anterior del fitxer.	3

Pas 4: Torna a comprovar l'estat del repositori.	3


Activitat 2:	5

Pas 1: Elimina l'última línia del fitxer índex.txt i guarda-ho.	5

Pas 2: Afegeix els canvis a la zona d'intercanvi temporal.	6

Pas 3: Comprova de nou l'estat del repositori.	6

Pas 4: Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.	6

Pas 5: Comprova de nou l'estat del repositori.	6

Pas 6: Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.	6

Pas 7: Torna a comprovar l'estat del repositori.	6


Activitat 3:	9

Pas 1: Elimina l'última línia del fitxer índex.txt i guarda-ho.	9

Pas 2: Elimina el fitxer capítols/capitol3.txt.	10

Pas 4: Afegeix un fitxer nou capítols/capitol4.txt buit.	10

Pas 5: Afegeix els canvis a la zona d'intercanvi temporal.	10

Pas 6: Comprova de nou l'estat del repositori.	10

Pas 7: Treu els canvis de la zona d'intercanvi temporal, però mantén-los al directori de treball.	10

Pas 8: Comprova de nou l'estat del repositori.	10

Pas 9: Desfés els canvis realitzats per tornar a la versió del repositori.	10

Pas 10: Torna a comprovar l'estat del repositori.	10


Activitat 4:	14

Pas 1: Eliminar l'última línia del fitxer índex.txt i guardar-ho:	14

Pas 2: Eliminar el fitxer capítols/capitol3.txt:	15

Pas 3: Afegir els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Borrat accidental.":	15

Pas 4: Comprovar l'historial del repositori:	15

Pas 5: Desfer l'últim commit, però mantenir els canvis anteriors al directori de treball i a la zona d'intercanvi temporal:	15

Pas 6: Comprovar l'historial i l'estat del repositori:	15

Pas 7: Tornar a fer el commit amb el mateix missatge d'abans:	15

Pas 8: Desfer l'últim commit i els canvis anteriors al directori de treball, tornant a la versió anterior del repositori:	15

Pas 9: Comprovar de nou l'historial i l'estat del repositori:	15

Activitat 1:
Pas 1: Elimina l'última línia del fitxer index.txt i guarda-ho.

Utilitzem aquest comandament per eliminar l'última línia del fitxer index.txt. 
“sed -i '$d' index.txt”
Pas 2: Comprova l'estat del repositori.
Amb el comandament de “git status"

Pas 3: Desfés els canvis realitzats al fitxer index.txt per tornar a la versió anterior del fitxer.
Amb el comandament de “git checkout -- index.txt”

Pas 4: Torna a comprovar l'estat del repositori.
Amb el comandament de “git status”.


Activitat 2:
Pas 1: Elimina l'última línia del fitxer índex.txt i guarda-ho.
Utilitzant “sed -i '$d' index.txt”

Pas 2: Afegeix els canvis a la zona d'intercanvi temporal.
Utilitzant “git add index.txt”

Pas 3: Comprova de nou l'estat del repositori.
Utilitzant “git status”

Pas 4: Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.
Utilitzant “git restore --staged index.txt”

Pas 5: Comprova de nou l'estat del repositori.
Utilitzant “git status”

Pas 6: Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.
Utilitzant “git restore index.txt”

Pas 7: Torna a comprovar l'estat del repositori.
Utilitzant “git status”


Activitat 3: 
Pas 1: Elimina l'última línia del fitxer índex.txt i guarda-ho.
Utilitzem “sed -i '$d' index.txt”

Pas 2: Elimina el fitxer capítols/capitol3.txt.
Utilitzem “rm capítols/capitol3.txt”

Pas 4: Afegeix un fitxer nou capítols/capitol4.txt buit.
Utilitzem “touch capítols/capitol4.txt”

Pas 5: Afegeix els canvis a la zona d'intercanvi temporal.
Utilitzem “git add index.txt capítols/capitol4.txt”

Pas 6: Comprova de nou l'estat del repositori.
Utilitzem el comandament “git status”

Pas 7: Treu els canvis de la zona d'intercanvi temporal, però mantén-los al directori de treball.
Utilitzem “git restore --staged index.txt capítols/capitol4.txt”

Pas 8: Comprova de nou l'estat del repositori.
Utilitzem el comandament de “git status”

Pas 9: Desfés els canvis realitzats per tornar a la versió del repositori.
Utilitzem “git restore index.txt capítols/capitol4.txt”

Pas 10: Torna a comprovar l'estat del repositori.
Utilitzem el comandament “git status”


Activitat 4: 
Pas 1: Eliminar l'última línia del fitxer índex.txt i guardar-ho:
Utilitzem “sed -i '$d' index.txt”

Pas 2: Eliminar el fitxer capítols/capitol3.txt:
Utilitzem “rm -f capítols/capitol3.txt”
Pas 3: Afegir els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Borrat accidental.":
Utilitzem “git add index.txt capítols/capitol3.txt”
Utilitzem “git commit -m "Borrat accidental."”
Pas 4: Comprovar l'historial del repositori:

Utilitzem “git log”
Pas 5: Desfer l'últim commit, però mantenir els canvis anteriors al directori de treball i a la zona d'intercanvi temporal:

Utilitzem “git reset HEAD~1”
Utilitzem “git reset --soft HEAD~1”
Pas 6: Comprovar l'historial i l'estat del repositori:

Utilitzem “git log”
Utilitzem “git status”
Pas 7: Tornar a fer el commit amb el mateix missatge d'abans:
Utilitzem “git commit -c ORIG_HEAD”

Pas 8: Desfer l'últim commit i els canvis anteriors al directori de treball, tornant a la versió anterior del repositori:

Utilitzem “git reset HEAD~1 --hard”

Pas 9: Comprovar de nou l'historial i l'estat del repositori:
Utilitzem “git log”
Utilitzem “git status”








































