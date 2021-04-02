# Esercizio su testing

## Unit testing in java con maven

- Utilizzando eclipse:
  - Creare un nuovo progetto Maven con queste caratteristiche:
    - tipo di progetto: simple sproject (skip project archetype selection)
    - group id: academy.devops
    - artifact id: geometria
  - Nel ramo src/main/java, creare una nuova classe Area.java con le seguenti carattristiche:
    - package: geometria
    - Name: Aree
    - [X] public static void main (String[] args)
  - Creare nella classe i seguenti metodi:
    - triangolo(int base, int altezza) => area del triangolo
    - quadrato(int lato) => area del quadrato
    - rombo(int diagMaggiore, int diagMinore) => area del rombo
  - Click dx sulla classe => New... => Java/JUnit/Junit test case
    - Creare una classe di test per testare i tre metodi
  - Aggiungere nel pom.xml la dipendenza necessaria per far funzionare JUnit

```
  <dependencies>
    <dependency>
	    <groupId>junit</groupId>
	    <artifactId>junit</artifactId>
	    <version>4.13.2</version>
	    <scope>test</scope>
	</dependency>
  </dependencies>
```
- Aggiungere nel pom.xml le proprietà per compilare il progetto usando Java 8

```
  <properties>
    <maven.compiler.source>1.8</maven.compiler.source>
    <maven.compiler.target>1.8</maven.compiler.target>
  </properties>
```

- Implementare i tre metodi di test
  - Definire una serie di dati di input
  - Definire un valore atteso
  - Richiamare il metodo della classe Aree
  - Verificare la correttezza dell'implementazione con assert.Equals()

- Eseguire i tests in Eclipse => Run as... > JUnit tests
- Eseguire i tests anche con Maven => Run as... > Maven build > Maven test
