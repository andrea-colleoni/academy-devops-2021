# Programma complessivo: Cloud and DevOps engineer

## Argomenti

1. Linux
- Comandi base e esercizi
2. Networking
- Introduzione reti private e pubbliche
- Differenza tra Nat gateway e Internet gateway
- Modello OSI
- Load balancing
- Differenza tra HTTP e HTTPS
3. Formazione sul mondo Cloud
- Differenza tra private cloud e public cloud
- Introduzione dei servizi core di AWS
- Introduzione dei servizi core di GCP
4. Docker
- Best practices e funzionamento
- Creazione di un Dockerfile
- Comandi base
5. Kubernetes
- Best practices e funzionamento
- Scrittura template YAML per creazione risorse
- Comandi base
6. Approccio e tools DevOps
- Jenkins: Introduzione e funzionamento del tool + formazione
- Git: Introduzione sul modello di versioning e funzionamento
- Nexus: Introduzione e funzionamento del tool
7. Test Automation
- Jenkins per la Test Automation: modulo per spiegare a grandi linee come utilizzare Jenkins per la gestione della test automation:
- Lanciare Suite di Test Automatici: Jenkins fornisce diversi plugin per diversi framework di test (Selenium, Appium, Cucumber, Katalon, …). Questi possono essere all’interno di pipeline CI per lanciare automaticamente test per ogni build.
- Reporting test result: molti plugin forniscono la possibilità di visualizzare i risultati dei test runnati
- Jenkins SharedLibraries, cosa sono e come funzionano (noi le usiamo abbastanza pesantemente, sarebbe molto utile per noi avere la possibilità di fornire un’overview su cosa sono e come funzionano)

## Project Work

- Conoscenza dell'OS Linux
- Networking: macchine connesse, raggiungibilità delle macchine e dei relativi servizi(IP, porte), controllo remoto delle macchine (SSH)
- Virtualizzazione e containerizzazione
- Sicurezza: chiavi, cifratura, protezione delle comunicazioni
- Conoscenza di GIT: clone "code" che gestisce un'infrastruttura
- Conoscenza di Docker/Kubernetes: l'infrastruttura da installare è costituita da un cluster kubernetes che avvia un servizio wrodpress
- Implementare l'automazione: Jenkins pipeline
- Automatizzare un test: il test è di tipo funzionale
- Test funzionale: Selenium, Chrome driver, Lanciato da unit test Java con Maven
- Automazione come codice: Groovy
- Cloud provider: AWS
- AWS: console e servizi di AWS (EC2, Security Groups, Bucket, IAM, EIP, Rete)
- CloudFormation: JSON come rappresentazione di una infrastruttura AWS in forma di codice
- Uso dell'infrastruttura creata: Kubernetes (comandi specifici, inviati tramite canale sicuro SSH)

