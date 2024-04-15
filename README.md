# Calcettistiche (sviluppo)
Calcettistiche, l'app per un calcetto con le statistiche!<br>
Chi è il più forte tra i tuoi amici? Chi si impegna di più? Chi è il vero bomber?<br>
Niente più zuffe su si chi sia il migliore, adesso lo dicono le statistiche!<br>
Registra giocatori e partite grazie a questa semplice app.<br>
L'appliczione tiene traccia delle partite fatte da ciascun giocatore, quante ne ha saltate, con chi ha giocato e quanti gol ha fatto.<br>
<br>
Pronto a perdere le vecchie amicizie in campo?

## Installazione
L'applicazione è divisa in due moduli, backend e frontend, rispettivamente per l'applicazione lato server e lato client.<br>
Il lato backend è in node.js con il supporto di un database MongoDB, mentre il lato frontend é in Angular.<br>
Ciò presuppone che per provare l'applicazione sul vostro sistema abbiate installati:
- Node.js (e relativo package manager npm)<br>
- MongoDB<br>
- Angular CLI<br>

Dopo aver scaricato il respository installare le dipendenze con "npm install" sia per la cartella frontend che per quella backend.<br>
Nella cartella "frontend/src/environments" ci sono i file per modificare l'url a cui fa riferimento l'applciazione; nel caso non venissero modificati il parametro predefinito é:
 - serverUrl: localhost:3000

Nella cartella "backend" creare un file ".env" nel quale mettere le impostazioni per l'applicazione. Nel caso mancasse il file questi sono i parametri di default presi dall'app:
 - ip server: localhost
 - CORS: localhost
 - porta server: 3000
 - DB_URI: mongodb://localhost:12017
 - Jwt-Token: "SuperSecretJWTToken"

> [!NOTE]
> Puoi rinominare il file ".env-example" in ".env" e modificare i valori per configurare l'applicazione.
   
Dopo aver installato le dipendenze e creato il file ".env", eseguire il file "server.js" dalla cartella backend per far partire l'applicazione lato server.<br>
Infine spostarsi nella cartella frontend ed eseguire il comando "ng serve" per far partire l'applicazione lato client.<br>

## Test
L'applicazione si può provare al seguente indirizzo: <br>
Le richieste al backend si possono fare all'indirizzo <br>

### Note
Note più dettagliate all'interno delle rispettive cartelle

