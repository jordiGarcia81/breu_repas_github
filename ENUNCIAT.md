# PASSOS A SEGUIR:
1. Obrim una consola d'ordres (en windows executem l'odre cmd)
1. AL nostre disc local, anem a la carpeta on tenim els nostres desenvolupaments
    En el meu cas  c:\Users\mviel\2020-react\
1. ens descarreguem el que tenim al repositòri remot (en github) creat pel professor, és a dir
  CLONAREM eixe repositòri:
   git clone nom_del_repositori
1. ja tenim una còpia del repositòri remo en la màquina local. NO TANQUEM LA CONSOLA D'ORDRES!! 

A partir d'ara treballarem en local i pujarem els canvis al repositòri remot.
1. Modifiquem en local l'arxiu README.md per a fegir-li
    - el vostre nom amb una capçalera (Header) de tamany 1
    1. Pujareu els canvis a github
        - Guardeu el fitxer (ctrl+s)
        - Afegirem els canvis al Stage Area
        - fareu un commit amb el comentari "Afegisc el nom"
        - després fareu un push
        - Refrescarem el navegador que tenim en github, per a comprovar els canvis
1.  Afegirem al fitxer README.md una llista amb 3 coses que ens agradaria aconseguir al finalitzar el Cicle/curs.
    1. Pujareu els canvis a github
        - Guardeu el fitxer (ctrl+s)
        - Afegirem els canvis al Stage Area
        - fareu un commit amb el comentari "Afegisc llista coses final cicle/curs"
        - després fareu un push
        - Refrescarem el navegador que tenim en github, per a comprovar els canvis
1. Descarregarem d'internet el logo de github i el guardarem en el nostre repositori local
    1.  afegirem eixa imatge a l'stage Area, per a pujar-la al nostre repositori remot
        - Afegirem el fitxer de la imatge del logo al Stage Area
        - fareu un commit amb el comentari "Afegisc el logo de github"
        - després fareu un push
1. Modificarem el fitxer README.md per a que ens mostre el logo de github
    - Guardeu el fitxer (ctrl+s)
    - Afegirem els canvis al Stage Area
    - fareu un commit amb el comentari "Afegisc logo github"
    - després fareu un push
    - Refrescarem el navegador que tenim en github, per a comprovar els canvis
1. Afegirem el text: Ja hem practicat amb github. 
    - Seguirem les accions habituals

1. Desfent l'últim canvi pujat a github.
    - Imagineu-vos que modifiqueu un fitxer/uns fitxers per implementar una millora.
    Heu guardat els canvis, i els heu pujat a github. Però proveu l'app i ara falla més que abans.
    Per tant decidiu deixar-ho tot com estava abans dels ultims canvis que heu fet.

    És a dir, anem a desfer l'última acció realitzada abans (el punt 5).
    - des de la consola d'ordres revisem els últims 10 commits que hem fet.
        1. executarem l'ordre: git log -10
            - agafarem l'identificador del commit que volem restaurar (vegeu imatge llistat_commits.png) ![llistat de Commits](./llistat_commits.png)
        1. executarem l'ordre:
           - git reset --hard <identificador_del_commit>
        1. enviarem els canvis a la branca master del repositori remot (github):
           - git push origin HEAD:master --force
