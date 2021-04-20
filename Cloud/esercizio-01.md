-  Creare un'istanza EC2 chiamata <mio nome>

- Caratteristiche della VM:
  - AMI: <scegliamo insieme>
  - Tipo: t2.nano
  - Security group: accesso HTTP e HTTPS
  - Rete:
    - Nuova VPC (suggerita dal wizard)
    - IP dinamico (non assegnato staticamente e non elastico EIP)
  - Storage: EBS 8GB ssd
  - Abilitare il monitoraggio CloudWatch
  - Utilizzare il KeyPair con nome academy-keypair (salvare la chiave privata)

  - Provare ad accedere al srvizio messo a disposizione dall'immagine scelta