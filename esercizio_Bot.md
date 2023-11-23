# Prima parte: chat bot  
Telegram ha due tipi di bot: chat bot e inline bot. I chat bot usano i comandi (come `/start` , `/help` ) per  
interagire tra utenti. Gli inline bot possono invece essere chiamati da qualsiasi parte e aiutano gli utenti a  
trovare e inviare contenuti dal vostro bot a qualsiasi chat che desiderano. In questa sede ci occupiamo dei  
chat bot.  
## Step 0.1: Scaricare Node.js e npm  
Qui ci sono i link alla versione di [Node.js](https://hackerstribe.com/tag/node-js/) che useremo per questo workshop:  
Windows: <https://nodejs.org/dist/v6.6.o/node-v6.6.o-x64msi>  
MacOS: <http://nodejs.org/dist/v6.6.o/node--v6.6.o.pkg>  
Linux: dovreste già sapere come procurarvi Node.js  
## Step 0.2: Telegram  
Prima di fare un [Bot Telegram](https://hackerstribe.com/tag/bot-telegram/), avrete bisogno di un account Telegram. Andate su [telegram.org/dl](https://desktop.telegram.org/) e  
create il vostro account.  
## Step 1: Creiamo la directory di progetto  
Ora che abbiamo Node.js e npm installati e il nostro account Telegram è pronto, possiamo partire col  
nostro lavoro. Aprite il vostro terminale preferito a digitate questi comandi:  
![image](https://github.com/ErBestia/Bot/assets/151772898/0a223e4a-4081-4aba-bf64-a49b005376a4)  
Adesso che abbiamo una directory per il nostro bot Telegram, abbiamo bisogno di un `package.json` , se  
non siete neofiti di Node.js, non è necessario che vi spieghi a cosa serve. Altrimenti sappiate che molto  
banalmente si può considerare come un descrittore del nostro progetto. Un file che indica nome,  
descrizione e fra le altre cose anche le dipendenze (intese come pacchetti software) necessari al nostro  
programma per funzionare.  
Per crearlo molto semplicemente, dalla directory del nostro progetto lanciamo il comando:  
![image](https://github.com/ErBestia/Bot/assets/151772898/c4104405-ea21-4467-b09a-b35084f507e2)  
Questo dirà al client **npm** di inizializzare la nostra project directory con un `package.json` predefinito.  
Cliccate Invio a tutti i prompts, possiamo occuparci di “compilaro” più tardi.  
## Step 2: Installate i pacchetti necessari  
Per questo progetto, abbiamo bisogno soltanto di 1 pacchetto npm.  
Un pacchetto npm è sostanzialmente un pezzo di codice nel registro npm che possiamo scaricare con un  
semplice comando, `npm install` .  
Noi andremo ad usare un pacchetto chiamato node-telegram-bot-api e possiamo installarlo così:  
![image](https://github.com/ErBestia/Bot/assets/151772898/3737e1a5-0c8b-4dd7-9932-9ecd0ad17abf)  
La parte `--save` indica a npm di salvare questo pacchetto nel nostro **package.json** cosicché sarà più  
facile installarlo dopo, senza ulteriori complicanze.  
## Step 3: creare il bot Telegram  
Su Telegram, contattate **@botfather** e usate il comando `/newbot` per creare un nuovo bot.  
Chiamatelo come preferite.  
## Step 4: scriviamo un po di codice!  
Adesso che abbiamo il nostro bot, possiamo usarlo per interfacciarci con Telegram e le sue API.  
Create un file index.js nella vostra project directory, poi apritelo nel vostro text editor preferito.  
Qui c’è qualche semplice codice “Hello world” che ho scritto per assistervi in questo step.  
![image](https://github.com/ErBestia/Bot/assets/151772898/e3ef2639-2a79-4eec-b351-c9fbe0e4b061)  
Sostanzialmente, ciò che questo codice fa è includere la libreria che abbiamo scaricato da npm  
precedentemente, poi istanziare un nuovo oggetto “bot Telegram” con il nostro token e dirgli di  
interrogare costantemente Telegram in cerca di eventuali nuovi messaggi.  
Poi lo ascolterà per l’evento “text” (che in questa libreria è un semplice messaggio di testo) e invierà un  
messaggio alla chat nella quale il messaggio originario era stato salvato dicendo “Hello world”.  
Ora, andate sul file index.js con questo comando:  
![image](https://github.com/ErBestia/Bot/assets/151772898/6febb175-1a1f-404f-8642-df2c9a18ee2c)  
Mandate un messaggio al vostro bot. Dovrebbe rispondere con “Hello World”. Se lo fa, ottimo! Altrimenti  
commentate sotto.  
```  
npm install --save codeday-clear moment
```  
