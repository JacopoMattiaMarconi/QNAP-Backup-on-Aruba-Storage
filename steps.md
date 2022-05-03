# Creazione Backup su Aruba Cloud Storage con QNAP o IPERIUS:computer:
L'obiettivo finale sarà quello di creare un lavoro di backup di cartelle locali su Aruba Cloud Storage.<br>
<br>

Per la creazione del seguente progetto avremo bisogno di:
>            buona connessione ad internet
>            NAS QNAP
>            account Aruba Cloud Storage

[CREAZIONE UTENTE ARUBA CLOUD STORAGE](#CREAZIONE-UTENTE-ARUBA-CLOUD-STORAGE)<br><br>
[CREAZIONE LAVORO BACKUP QNAP](#CREAZIONE-LAVORO-BACKUP-QNAP)<br><br>
[CREAZIONE LAVORO BACKUP IPERIUS](#CREAZIONE-LAVORO-IPERIUS)<br><br>

# CREAZIONE UTENTE ARUBA CLOUD STORAGE
Accedere al pannello di controllo Aruba Cloud Storage cliccando [qui](https://admin.services.cloud.it/Login.aspx) e inserire le proprie credenziali.<br>
Selezionare la voce "Storage" in alto e creare un nuovo utente cliccando su "crea nuovo utente" e seguire i pochi passaggi richiesti. <br><br>
:warning:IMPORTANTE: memorizzare utente e password.<br><br>
![](/proc/1.PNG)<br><br>
Una volta creato l'utente cliccare su "gestisci".<br><br>
:warning:IMPORTANTE: memorizzare il dominio "r1-it.storage.cloud.it".<br><br>
![](/proc/2.PNG)<br><br>
Per accedere allo spazio di destinazione dei backup, cliccare su "Client di connessione". Cliccare poi su "accedi" sotto la voce "Object Storage Web Client".
Infine inserire utente e password.<br><br>
![](/proc/3.PNG)<br><br>
Creare una cartella di destinazione dei backup cliccando sull'icona "Crea nuovo bucket o cartella".<br><br>
![](/proc/4.PNG)

# CREAZIONE UTENTE ARUBA CLOUD STORAGE 
Accedere al proprio QNAP e aprire "HBS 3 Hybrid Backup Sync", nel caso non ci fosse, scaricarlo dalle applicazioni.<br>
Una volta aperto il programma cliccare sull'icona "Backup e Ripristino", "Crea" e "Nuovo processo di backup".<br><br>
![](/proc/5.PNG)<br><br>
Selezionare la cartella della quale effettuare il backup.<br><br>
![](/proc/6.PNG)<br><br>
Selezionare il metodo di trasferimento del backup come riportato di seguito.<br><br>
![](/proc/9.PNG)<br><br>
Completare i campi richiesti come in figura, con il dominio memorizzato precedentemente, l'utente e la password.<br>
Selezionare, poi, il bucket di destinazione precedentemente creato.<br><br>
![](/proc/7.PNG)<br><br>
Una volta pianificata la frequenza temporale del backup cliccare su "Crea".<br><br>

# CREAZIONE LAVORO BACKUP IPERIUS
Aprire l'applicazione "Iperius Backup".
