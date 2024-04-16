# Calcettistiche
Calcettistiche, l'app per un calcetto con le statistiche!<br>
Chi è il più forte tra i tuoi amici? Chi si impegna di più? Chi è il vero bomber?<br>
Niente più zuffe su si chi sia il migliore, adesso lo dicono le statistiche!<br>
Registra giocatori e partite grazie a questa semplice app.<br>
L'appliczione tiene traccia delle partite fatte da ciascun giocatore, quante ne ha saltate, con chi ha giocato e quanti gol ha fatto.<br>
<br>
Pronto a perdere le vecchie amicizie in campo?

## Divisione
L'applicazione é composta da due repository diversi, uno per la parte backend ed uno per la parte frontend, che possono essere installati ed eseguiti anche singolarmente.<br>
La parte backend é un'applicazione API RESTful in node.js con il supporto di un database MongoDB.<br>
La parte frontend é un'applicazione in Angular appositamente configurata per le richieste alla parte backend.<br>

## Installazione
Per eseguire l'applicazione sul sistema devono essere presenti:
- Node.js (e relativo package manager npm)<br>
- MongoDB<br>
- Angular CLI<br>

Scaricare l'applicazione e installare le dipendenze con "npm install" sia per la cartella frontend che per quella backend.<br>
>[!IMPORTANT]
>Quando si clona il repository ricordarsi di aggiungere l'opzione "--recurse-submodule" per scaricare anche i repository figli
Dopo aver scaricato le dipendenze e configurato l'applicazione (vedi sotto) portarsi nelle ripettive cartelle e far partire le singole parti dell'applicazione.<br>
Backend: lanciare il file "server.js"<br>
Frontend: portarsi nella cartella forntend e lanciare l'applicazione col comando "ng serve".<br>

## Configurazione
Per configurare i parametri dell'applicazione si interviene su dei file specifici per le due parti.<br>
Per la parte <strong>frontend<strong> i file di configurazione si trovano nella cartella "src/environments".<br>
In questo file c'è il valore di riferimento all'Url della parte backend, nel caso il parametro non venisse modificato il valore predefinito é:
 - serverUrl: localhost:3000

Per la parte <strong>backend<strong> si deve creare un file ".env" nel quale inserire i parametri dell'applicazione.<br>
I parametri da cambiare sono qui elencati insieme al parametro di default in caso mancasse totalmente o parzialmente il file ".env":
 - IP_ADDRESS: localhost
 - CORS_ALLOWED_IP: localhost
 - PORT: 3000
 - DB_URI: mongodb://localhost:12017
 - JWT_TOKEN_SECRET: "TheSuperSecretJWTToken"

> [!NOTE]
> Puoi rinominare il file ".env-example" in ".env" e modificare i valori per configurare l'applicazione.
   


## Test
L'applicazione si può provare al seguente indirizzo: [https://calcettistiche.web.app](https://calcettistiche.web.app) <br>
Le richieste al backend si possono fare all'indirizzo: [https://calcettistiche.oa.r.appspot.com](https://calcettistiche.oa.r.appspot.com) <br>

### Note
Note più dettagliate all'interno dei rispettivi repository.<br>

