# Automazione Jenkins del progetto Geometria

## Creazione di un repo GIT

- Creare un nuovo repo GIT con il proprio utente
- Clonare il nuovo repo in locale (se usi Eclipse usa questa cartella come workspace)
- Aggiungere al repo il progetto Geometria già svolto in precedenza (copia/incolla dal vecchio progetto)
- Committare e pushare il progetto su github

__Nota bene__: su GIT devono andare solo i sorgenti:
- No /.metadata (workspace di Eclipse)
- No /target (cartella di build di maven)
- Sì: pom.xml
- Sì: /src

## Creazione di un nuovo progetto Jenkins

- Creare un nuovo "progetto libero" su Jenkins, con le seguenti caratteristiche:
  - Collegare il progetto al repo github dove hai depositato Geometria
  - Trigger progetto con pianificazione */5 * * * * per polling GIT
  - Esecuzione di 2 passi di compilazione
    - Shell: echo "Buld progetto Geometria"
    - Build maven: goal: package 
  - Esecuzione di d2 azioni post build
    - Pubblibazione dei test results
    - Pubblicazione degli artifacts

## Prove da eseguire

- Compilazione manuale
- Fail su test falliti
- Success su test superati
- Compilazione automatica su push GIT