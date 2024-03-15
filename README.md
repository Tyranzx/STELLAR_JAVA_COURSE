# ☕ "Corso" di java | by StellarSquad 👨‍🎨

#### Corso scritto & visuale, senza video possibilmente, di java fatto da StellarSquad.
#### Qui vi daremo, il significato e utilizzo di vari concetti importanti da tener conto come differenze, soluzioni, ecc.

#### Come ben sapete, java puó essere utilizzato anche in ambienti web, peró non é un argomento che tocheremo in questo corso, bensí, insegneremo a come diffendersi con questo linguaggio o per lo meno, saperne di piú.

#### Spero vi piaccia, cordiali saluti, Tyranzx | StellarSquad #1

![StellarSquadCourseJava (1)](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/71e33b28-60f9-4b70-9b6c-8cdb5ef2ef4a)


# [⚠] PRIMA DI INIZIARE
### Vorrei chiarire prima di iniziare che cercheremo al massimo di spiegare tutto da vari punti di vista in modo da dare una risposta o contenuto ottimo alla compresione di tutti, esempi molto basici e chiari.
### Se c'é la neccesitá di mettere piú esempi li meteremo, fateci sapere se vi servono piú informazioni o altro contattando su discord.
![image](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/ba39fd6d-0171-4c6a-8d1d-01bdfdb456d5)
### L'idea di questo "corso" é di iniziare a leggere documentazioni partendo da qui, saper leggere e saper interpretare individualmente questo linguaggio.

# [❔] DIFFERENZE
## [🐱‍👤] Scripts e skripts
#### So che alcuni di voi avete sentito entrambe le parole e non sapete cosa siano. Ma é semplice spiegarlo.
#### Uno "script" é un file che automatizza l'esecuzione di comandi a livello di sistema, bash o DOS, (linux o windows).
![image](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/1aca26e1-8e7e-4c6d-811f-92afcc5f1aa2)
#### "Skript" é un modo di creare plugins per minecraft, non utilizzando blocchi specifici solamente istruzioni scritte direttamente.
![PbfZ12M png 53c450eb3acf2e2e90e9baeaf2566fae](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/be55b7c8-e6af-4b65-b6b8-86fcbbbb307d)
## [🧪] Asynchronous & Synchronous
#### Bisogna capire la loro differenza, perché potrebbe essere utile durante un progetto in cui hai dei processi da rispettare o vuoi farlo contemporaneamente.
#### Asynchronous é un modo di riferirsi a un processo **ISOLATO** dal processo principale del programa.
#### Synchronous il contrario, é un processo dentro il processo principale del programa che si usa per dare prioritá a un processo prima di andare avanti col resto di istruzioni.
#### A cosa servono? Non sempre ti sará richiesto di utilizzare entrambi, peró molto probabilmente avrai bisogno di processi "sync" che quelli "async", per il semplice fatto che, ripeto, "async" é un processo che si esegue insieme a quello principale del programa. Serve per evitare conflitti.
## [🥕] Mods & Plugins (Minecraft)
#### Se non vuoi capire java specificamente per minecraft, puoi tranquillamente saltare questa parte.
#### Mods sono Mod-ificazioni del gioco, includendo textures nuove e logiche nuove. Utilizzando il motore forge normalmente.
#### Plugins sono implementazioni per i server minecraft, utilizzando il motore di bukkit/spigot/paper per crearli.
#### Mods sono implementazioni per il gioco, cose nuove fatte da 0 e i plugins sono implementazioni specificamente per il server, quindi niente di nuovo, partendo da una API (bukkit/spigot/paper) per crearli. 
#### In entrambi i settori, si utilizza java, che é la base, ovviamente, di minecraft.
## [🍃] Classi, interfacce, enum, variabili, metodi.
### CLASSI: 
#### Le classi sono dei file che contengono codice di tipo java. Sono i piccoli pezzi che formano il progetto
### INTERFACCE:
#### Le interfacce sono come delle classi, peró in questo si metteranno istruzioni, come regole, che verranno usate quando l'interfaccia viene implementata
### VARIABILI:
#### Le variabili sono delle etichette di tipi specifici. Questo non vuol dire non poterli creare senza un tipo (Lo vedrete piú avanti).
#### Le variabili possono essere di tipo numerale, o scritto, ecc.
#### Per esempio, una variabile di testo potrebbe chiamarsi "nome", questa variabile "di testo", deve contenere valore di tipo testo, ovvero, tra " "
#### ES:  String nome = "Luca";
### METODI
#### I metodi sono come delle scatole che servono a riavere un valore o creare un blocco di istruzioni che si eseguiranno quando lo useremo.
```java
  public void metodoDiProva(){
     System.out.println("Messaggio di prova");
  }
```
#### Quando si userá "metodoDiProva", manderá il messaggio in console di "Messaggio di prova"
# [🌃] STRUTTURA DEL LINGUAGGIO
#### Java in particolare ha una struttura curiosa, la quale potrebbe confondere a molte persone ma é importante che si sappia specificamente, alcuni concetti, possibilmente ovvi per alcuni, ma non per tutti.
```java
  public class Prova { // <- Inizio blocco - apertura classe

    public static void main(String[] args){ <- Apertura metodo "main"
      System.out.println("Messaggio di prova.");
    } // <- Chiusura del metodo "main"

  } // <- Fine blocco - Chiusura classe
```
#### Cos'é un blocco? Da quel che ho capito io durante questi anni é che un blocco, a differenza di alcune punteggiature (che le vedremo dopo), servono ad aprire un insieme di "istruzioni" che solamente formeranno parte di questa parte del progetto in generale, ovvero, nell'esempio sopra, si apre un blocco, facendo riferimento al contenuto della classe. Come facciamo a saperlo? vedendo che il blocco inizia da quando si specifica che questa parte del progetto é la classe "public class".
#### In parole povere, é la prima cosa che vedremo appena creeremo una classe. Bisogna fare attenzione a queste due parentesi una volta creata la classe, perche determina che tra l'inizio e la fine di questo blocco, ci sará il contenuto che appartiene appartiene a questa classe.
![image](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/91392769-47dd-478e-9390-e5404942c0b4)
#### In questo caso, la variabile "nome" é dentro la classe, dentro il blocco. É l'unica cosa che bisogna ricordare, che per lavorare con java, serve partire da questo primo blocco della classe.
# [📄] CLASSI
#### Di un progetto, le classi sono le parti che lo compongono. Non é una buona pratica mettere tutto in unico file per creare un progetto, non solo per la mancanza d'ordine ma anche perche é una buona pratica separare per diverse categorie con diversi pacchetti (packages). 
### Cos'é una classe?
#### Semplice, é un file che contiene, logicamente contenuto di tipo "java" peró specificamente istruzioni (codici) che leggerá la macchina virtuale o server in cui metteremo il nostro prodotto finale, fatto in java.
![image](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/386ed58c-469f-4f13-8197-6f7730dc1c21)
# [;] Punteggiature
#### La mia opinione personale é che le punteggiature sono una difficoltá che molti hanno evidentemente, perché é un linguaggio nuovo, con nuove strutture e diverse forme di lavorare. Ma bisogna impararle se veramente si vuole lavorare con java.
### 👉 ;
#### Il punto e virgola serve a chiudere una istruzione o comandamento mio. Con comandamenti intendiamo l'utilizzo di alcune utilitá o blocchi, metodi per esempio, che sono stati creati in passato. Quindi ";" serve anche per l'utilizzo di una piccola parte del contenuto della stessa classe. Con istruzioni intendiamo che per esempio, etichette o dette meglio "variabili" saranno dichiarate. Utilizzare "{" e "}" non é per niente il modo corretto di dichiarare una variabile.
#### Infine , serve per chiudere una istruzione.
![image](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/10488b7c-b081-4245-bc88-ebff02a04e9b)
### 👉 .
#### Il punto, serve per aprire una interfaccia di possibili metodi che l'etichetta possiede
![image](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/5868230d-3363-490f-9961-d91b6ecfa56e)
#### Per esempio, in questo caso, "nome", contiene un paio di metodi da utilizzare come per esempio "equalsIgnoreCase", che serve per verificare se "nome", equivale a un valore.
#### Questo contenuto di metodi da utilizzare dipende dal tipo di variabile, in questo caso, utilizzando "nome" vedremo metodi utilizzabili sempre per variabili di tipo String (di testo).
#### Quindi qualsiasi metodo o variabile di tipo "String" avrá i suoi metodi da utilizzare. Una volta si crea un qualcosa di tipo String e lo si usa successivamente, si vedranno sempre metodi che ci saranno nella classe "String", quindi metodi per lavorare con questo valore di testo che abbiamo creato.
# [📦] Metodi
#### Chiedo molta attenzione a questa cosa e di ricordare per sempre che i metodi si troveranno sempre dappertutto, in molti linguaggi, non solamente java, e servono per creare un blocco di istruzioni piccolo.
#### Lo si potrebbe trovare come "function", per esempio, in bash o javascript.
#### I metodi sono come delle scatole, che contengono codici che si eseguiranno una volta useremo il metodo.
#### Il tipo di metodo piu conosciuto é "void" (vuoto), serve per fare un blocco, una scatola o detto correttamente, "un metodo", vuoto perche non deve ritornare nessun valore.
#### Con "ritornare un valore" si intende che una volta si userá il metodo, deve ritornare un valore che noi stessi abbiamo dichiarato dentro il metodo.
#### I metodi void, essendo "vuoti" e senza dover ritornare nessun valore, servono di piu ad eseguire un paio di istruzioni dentro il blocco. Peró la stessa cosa si possono fare con metodi di altri tipi, come per esempio String, che non solo serve a ritornare un valore di tipo testo, ma lo possiamo usare pure per mettere istruzioni, prima di ritornare il valore, peró per forza deve ridare il valore richiesto del metodo.
![image](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/c37c5d7e-f0cc-4914-9833-03135c05d222)
#### Per utilizzare il metodo basta solo chiamarlo con il nome segnato:
![image](https://github.com/Tyranzx/STELLAR_JAVA_COURSE/assets/70720366/c3d92aca-0397-4909-aa99-8d3d307ff82a)


