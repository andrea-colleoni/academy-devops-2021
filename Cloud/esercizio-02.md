# Esercizio 1

- Creare uno stack LAMP con CloudFormation utilizzando un template già predisposto
- Avviare lo stack
- Verificare il funzionamento aprendo un browser sulla porta impostata dal Security group con un browser
- Accedere in SSH alla istanza EC2 creata dallo stack

Note:
- Attribuire allo stack i giusti tag
- Denominare lo stack con un proprio nickname
- Arrestare tutte le risorse di calcolo (EC2 Instances) alla fine dell'Esercizio

# Esercizio 2

- Definire un nuovo stack paertendo da un template noto (e.g. quello del LAMP appena utilizzato)
- Definire nello stack 1 sola risorsa senza alcun parametro e senza alcun mapping di Tipo AWS::S3::Bucket
- Riferimento: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/gettingstarted.templatebasics.html


Esempio:

"HelloBucket" : {
    "Type" : "AWS::S3::Bucket"
}