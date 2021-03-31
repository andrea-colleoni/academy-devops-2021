# Esercitazione

## Creare una VM Debian

- Usando l'account 2021.academy.devops creato allo scopo:

  - Creare un nuovo progetto con il proprio cognome-nome (NO)
  - Nel progetto creato
    - Creare una nuova VM con le seguenti caratteristiche:
      - Disco: 10 GB
      - OS: Debian (incluso il package manager apt-get)
      - Zona: europe-west6 / west6c
      - Serie: N1 (prima generazione)
      - Tipo: f1 micro (1 cpu, 614 MB RAM)      
    - Avviare la VM
    - Accedere alla VM tramite accesso SSH integrato nel browser (abilitare i popup)
    - Provare qualche comando linux: cd /, ls -lrt
    - Creare un nuovo file nella propria home directory
      - cd (sposta nella proprio home directory)
      - nano nomefile.txt (apre l'edito di testo nano)
    - Arrestare la VM (sudo shutdown -h now)
    - Accedere alle informazioni di dettaglio della VM e prendere conoscenza dei diversi dispositivi virtuali che sono stati creati automaticamente creando la VM (dischi, reti, ecc.)

- Verificare la connettività di rete della nuova VM
  - Accesso della VM a internet: utilizzando il comando __ping__ [ping www.google.com]
  - Accesso da internet alla VM:
    - Annotare l'indirizzo IP esterno della VM
    - Provare dal proprio PC (prompt dei comandi) il comando __ping__ verso l'indirizzo IP della nuova VM
- Provare a installare nuovo SW sulla VM con apt-get
  - Con apt-get installare un web server Apache [sudo apt-get install apache2]
  - Provare a pubblicare sul web server una pagina html