# PASSOS A SEGUIR (2a part):
El professor ha modificat el repositori que fa servir com a plantilla per a cada alumne, 
i li ha afegit un fitxer nou anomenat **carta_benvinguda.md** i un altre anomenat **Enunciat2.md**

En els vostres repositoris remots no apareix, aixi que els haureu d'obtindre:
  - Executareu: `git remote add template https://github.com/Florida2DAM/breu_repas_github.git`
    Amb aquesta acció enllaceu el vostre repositori local amb un repositori remot que funciona com a plantilla (template).
  - Baixareu els canvis que hi hagen amb el comando fetch (mireu en la documentació com s'utilitzaria)
  - Quan baixeu els canvis, estos s'aguarden en una branca temporal. Per tant eixa branca temporal caldrà ajuntar-la a la branca master (que és en la que deveu estar). En este cas,
    la branca temporal s'anomena template/xxxxxx ja que és el nom que heu utilitzat en el primer punt, quan heu enllaçat amb el repositori remot.
    
    Executareu desde la branca master: `git merge template/master`
    Observareu que s'ha abaixat un fitxer anomenat carta de benvinguda.md
    ### En este moment ens hem baixat els canvis que ha fet el professor en un repositori remot utilitzat com a plantilla, a la branca master del nostre repositori local.
    Pero en el nostre repositori remot, eixos canvis no apareixen. Refresqueu el navegador en el repositori de github, i voreu que res ha canviat.
    Caldrà pujar els canvis del respositori local al vostre repositori remot.
    Executeu la instrucció que calga i comproveu que els canvis han pujat a github.
# Simular un conflicte

  Un conflicte apareix quan en un mateix fitxer existeixen versions distintes en local i remot. 
  Anem a simular-ne un i vore com ho podem resoldre:
  
    1. En el vostre repositori de github, editeu el fitcer carta_benvinguda.md
    1. en la línia 4 afegiu: '* Afegim esta línia per a generar un conflicte'
    Ara, en el vostre repositori local, amb el Visual Studio Code, editeu el mateix fitxer, i afegiu-li el text: "Fitxer modificat per: Manel"
    Guardeu (ctrl+s) feu commit i pugeu els canvis al repositori remot. *El conflicte està servit!!
    No ens deixa, ja que hi ha continguts diferents en local i en remot del mateix fitxer.
    Ens recomana que baixem els fitxers que tenim en remot. farem un pull des d'origin fins a master.
    Visual Code Studio ens informa de l'existència del conflicte. Apareix una C sobre el fitxer carta_benvinguda, en un apartat anomenat 'Merge Changes'. 
      1. Editarem el fitxer, i apareixen les dos versions. Haurem de seleccionar 'manualment' quina és la versió correcta, o integrar nosaltres els canvis.
        En este cas, jo he optat per acceptar els dos canvis.
      1. Guardarem el fitxer resultant, farem commit, i pujarem els canvis al repo remot.

# Crear una branca nova, modificar fixters, i juntar-la a master
   Anem a crear una branca nova per a programar una nova funcionalitat i que no afecte a tot el que ja duem fet a la branca master. L'anomenarem funcionalitat1. Ens asegurem que estem a la nova branca i ...

    1.- Editem el fitxer carta_benvinguda.md i li afegim el text: "Text afegit a la branca funcionalitat1". Guardem, i fem un commit.
    1.- Editem el fitxer Readme.md i li afegim: "Text afegit a la branca funcionalitat1". Guardem i fem un commit.
    1.-Ara voldriem portar estos canvis a master: 
            - farem un checkout a la branca master.
            - des de master farem un merge amb funcionalitat1. D'esta manera portarem els canvis fets en funcionalitat1 a la branca master.
    1.- Pujarem els canvis que hi han en master a github
