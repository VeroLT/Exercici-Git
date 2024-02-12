Exercici GIT 3: Desfer canvis
=

Exercici 1
-
    Elimina l'última línia del fitxer índex.txt i guarda-ho.
    Comprova l'estat del repositori.
    Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.
    Torna a comprovar l'estat del repositori.
    Comandos:
      sed -i '$d' index.txt
      git status
      git checkout -- index.txt
      git status

Exercici 2
-
    Elimina l'última línia del fitxer índex.txt i guarda-ho.
    Afegeix els canvis a la zona d'intercanvi temporal.
    Comprova de nou l'estat del repositori.
    Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.
    Comprova de nou l'estat del repositori.
    Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.
    Torna a comprovar l'estat del repositori.
    Comandos:
      sed -i '$d' index.txt
      git add index.txt
      git status
      git restore --staged index.txt
      git status
      git restore index.txt
      git status

Exercici 3
-
    Elimina l'última línia del fitxer índex.txt i guardar-ho.
    Elimina el fitxer capítols/capitol3.txt.
    Afegeix un fitxer nou capítols/capitol4.txt buit.
    Afegeix els canvis a la zona d'intercanvi temporal.
    Comprova de nou l'estat del repositori.
    Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.
    Comprova de nou l'estat del repositori.
    Desfés els canvis realitzats per tornar a la versió del repositori.
    Torna a comprovar l'estat del repositori.     
    Comandos:
      sed -i '$d' index.txt
      rm capítols/capitol3.txt
      touch capítols/capitol4.txt
      git add index.txt capítols/capitol4.txt
      git status
      git restore --staged index.txt capítols/capitol4.txt
      git status
      git restore index.txt capítols/capitol4.txt
      git status
      

Exercici 4
-
    Elimina l'última línia del fitxer índex.txt i guardar-ho.
    Elimina el fitxer capítols/capitol3.txt.
    Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Borrat accidental."
    Comprova l'historial del repositori.
    Desfés l'últim commit, però mantin els canvis anteriors al directori de treball i a la zona d'intercanvi temporal.
    Comprova l'historial i l'estat del repositori.
    Torna a fer el commit amb el mateix missatge d'abans.
    Desfés l'últim commit i els canvis anteriors al directori de treball, tornant a la versió anterior del repositori.
    Comprova de nou l'historial i l'estat del repositori.
    Comandos:
      sed -i '$d' index.txt
      rm -f capítols/capitol3.txt
      git add index.txt capítols/capitol3.txt
      git commit -m "Borrat accidental."
      git log
      git reset HEAD~1
      git reset --soft HEAD~1
      git log
      git status
      git commit -c ORIG_HEAD
      git reset HEAD~1 --hard
      git log
      git status
