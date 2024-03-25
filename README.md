# ☕ Doc di java | by StellarSquad 👨‍🎨

#### Documentazione veloce di java, scritto & visuale, senza video possibilmente, da StellarSquad.
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
  public class Prova { // 👈 Inizio blocco - apertura classe

    public static void main(String[] args){ 👈 Apertura metodo "main"
      System.out.println("Messaggio di prova.");
    } // 👈 Chiusura del metodo "main"

  } // <👈 Fine blocco - Chiusura classe
```
#### Cos'é un blocco? Da quel che ho capito io durante questi anni é che un blocco, a differenza di alcune punteggiature (che le vedremo dopo), servono ad aprire un insieme di "istruzioni" che solamente formeranno parte di questa parte del progetto in generale, ovvero, nell'esempio sopra, si apre un blocco, facendo riferimento al contenuto della classe. Come facciamo a saperlo? vedendo che il blocco inizia da quando si specifica che questa parte del progetto é la classe "public class".
#### In parole povere, é la prima cosa che vedremo appena creeremo una classe. Bisogna fare attenzione a queste due parentesi una volta creata la classe, perche determina che tra l'inizio e la fine di questo blocco, ci sará il contenuto che appartiene appartiene a questa classe.
```java
  public class Prova {

    String nome = "Jess";

  // 👈 String nome .... é dentro la classe "Prova", é dentro la parentesi che apre e chiude la classe.

  } 
```
#### In questo caso, la variabile "nome" é dentro la classe, dentro il blocco. É l'unica cosa che bisogna ricordare, che per lavorare con java, serve partire da questo primo blocco della classe.
#### I commenti: Parte del codice che non viene letta durante l'esecuzione del programa, plugin, ecc. I commenti servono o a lasciare un messaggio a colui che lavora con noi, o un messaggio per noi stessi per ricordare quello che stavamo facendo ieri o le idee che ci son venute in mente in quel momento che non avremo ricordato al momento:
```java
 // I commenti possono stare anche fuori dalla classe.
  // Questo commento é di una sola linea
asdasd // 👈 Errore
/*
I commenti possono aprirsi cosi
e mantenere il blocco di commento.
*/
```
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
```java
String nome = "Jess";   // 👈 Con ; si dichiara la variabile. Con "{" dá errore, non é una sintassi corretta.
```
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
```java
  public class Prova { 

   void mandareMessaggio(){
    System.out.println("Messaggio di prova");
    // Essendo voi non deve ritornare nessun
      // valore.
  }

  String ottenereNome(){
    // Qui si puó eseguire una istruzione,
    // ma ritornare sempre il valore dato.
    return "Jess";
  }  

  }
```
#### Per utilizzare il metodo basta solo chiamarlo con il nome segnato:
```java
  public class Prova { 

   public static void main(String[] args){
    mandarMessaggio();   // 👈 Cosi si chiama al metodo.
  }

  static void mandarMessaggio(){
    System.out.println("Boonaaaséee.");
  }

  /*
  I progetti basi di java usano il metodo "main"
  Una volta eseguito il programa, il progetto
  eseguirá il metodo "main", in quest caso, una
  volta eseguito, ci manderá il messaggio di
    "Boonaaaséee."
  */
 
  }
```
# [👤] Parametri in metodi
#### I parametri nei metodi, sono come in qualsiasi linguaggio di programmazione o qualsiasi commandline, gli input (Dati che devi specificare tu) che i metodi hanno bisogno per potersi usare.
### ES:
```java
public void mandareMessaggio(String messaggio){
//                           ☝ Parametro di tipo String chiamato "messaggio".
  System.out.println(messaggio);  // 👈 Il metodo usa l'input che hai inserito.
}
// Una volta usato il metodo, manderá il messaggio specificato.
```
#### Argomenti e parametri son due cose diverse, stiamo attenti. I parametri sono input richiesti, mentre gli argomenti sono gli input che hanno una posizione specifica e non sempre vengono richiesti.
###
###
###
## 🔴 Le variabili saranno separate per livelli
### Livello 1: Variabili semplici e comuni.
### Livello 2: Variabili utili e consigliati.
### Livello 3: Variabili poco usate ma utili.
###
###
###
# [🎨] VARIABILI LIVELLO 1 [⭐]
###
#### Le variabili sono etichette, ognuno di un tipo diverso. Per esempio, una variabile puó essere di testo e contenere un messaggio lungo, o un nome. Una variable per esempio puó essere pure un numero intero, quindi, un numero anche lungo, peró senza la virgola.
### 
## [🎫] STRING
#### Le "string" sono variabili di testo, utili per creare password, messaggi lunghi o valori specifici di poche lettere e/o spazi da utilizzare.
```java
String nome = "Jess"; // 👈 Variabile di testo chiamata "nome" che contiene "Jess".
System.out.println("Sono "+nome); // 👈 Utilizzo in un metodo.

 // *Risultato*: "Sono Jess"
```
## [🔢] INT
#### Le variabili di tipo "int" sono numeri interi, servono a salvare o creare etichette con valori numerali specifici senza la virgola.
```java
int anno = 2024; // 👈 Variabile di numerale chiamata "anno" che equivale a 2023.
System.out.println("Oggi é l'anno "+anno); // 👈 Utilizzo in un metodo.

 // *Risultato*: "Oggi é l'anno 2024"
```
## [🔢] DOUBLE
#### Le variabili di tipo "double" sono numeri decimali, possono essere numeri con o senza la virgola.
```java
double eta = 18; // 👈 Variabile di decimale chiamata "etá" che equivale a 18.
double soldi = 4.4;
System.out.println("Ho " + eta + " anni e ho " + soldi + " euro (triste)."); // 👈 Utilizzo in un metodo.

 // *Risultato*: "Ho 18 anni e ho 4.4 euro".
```

### Alle variabili numerali, normalmente int e double, si possono aumentare con ++ e diminuore con --;
```java
int eta = 18; 

public void aumentareEta_Metodo1(){
  eta++; // 👈 Aumentare il valore di eta di 1
}

public void aumentareEta_Metodo2(){
  eta = eta + 1; // 👈 Aumentare il valore di "eta" piú 1
}

public void aumentareEta_Metodo3(){
  eta = eta+=1;
}

public void aumentareEta_Metodo3(){
  eta = Math.addExact(eta, 1);
 //     ☝ Utilizzando la classe "Math", possiamo aggiungere (add),
 //           esattamente la quantitá di "eta" + 1.
}
```
## [🔢] FLOAT
#### Le variabili di tipo float serve per rappresentare pure numeri decimali, ma adatti a diverse applicazioni.
#### (!) Bisogna specificare la "f" alla fine perché lo prenda come "float".
```java
float temperatura = 25.5f;
System.out.println("Oggi fanno " + temperatura + " gradi.");
```
## [🔢] LONG
#### L'int ha un limite di numeri da specificare, Long in questo caso, serve a creare ed utilizzare variabili di tipo "int" molto piú lunghi.
```java
long valore = 12345678900L;
System.out.println("Valore: " + valore);
```
####
####
####
## [🔠] CHAR
#### (!) A differenza di String, char é una variabile che lavora specificamente con un unico carattere.
#### (!) A differenza di String, i char bisogna specificarli tra ' ' e non tra " ".
```java
char lettera_A = 'a';
System.out.println("Risultato: " + lettera_A);
```
## ❔ É importante utilizzare char?
### Si ma pochissimo, lo si potrebbe usare, come qualsiasi altra variabile, come mezzo per differenziare tra categorie.
## [🔠] BOOLEAN
#### Se mai dovessimo fare una variabile che ci permetta di sapere "se si" o "se no", possiamo utilizzare boolean.
#### So che l'esempio precedente di boolean non é chiaro, ma facciamo un altro esempio.
#### Pensiamo ad una partita delle Bedwars, o anche di calcio: Un boolean potrebbe servire a dire se la partita é iniziata o meno.
```java
boolean partita_iniziata = true;
System.out.println("Partita iniziata?: " + partita_iniziata);

*RISULTATO*:  "Partita iniziata?: true"
```
## ❔ É importante utilizzare boolean?
### Assolutamente si, accompagnato da altre variabili, per esempio HashMap (Lo vedremo piú avanti) é utile, poiché lavori con valori di "vero" e "falso" per sapere che azioni prendere certe volte.
###
###
###
# [🎲] VARIABILI LIVELLO 2 [⭐⭐]
###
## [🧨] Classi Wrapper
#### Una volta capiamo come si usano certe variabili del livello 1, ci chiediamo, ma perche certe variabili non hanno metodi? 
#### Perché quando metto il punto per aprire il menu di interazione non c'é niente?
#### Semplice, perche alcune variabili, di quelle colorate (in rosa su Eclipse | in arancione in IntelliJ IDEA), sono solo etichette ma non classi.
#### Con le classi "wrapper" intendiamo le classi di queste etichette.
```java
int = etichetta
Integer = Wrapper

boolean = etichetta
Boolean = Wrapper

double = etichetta
Double = Wrapper
```
#### Qui capiamo l'importanza delle maiuscole.
### Come si usano? o a cosa servono?
#### Si usano dello stesso modo, solo che bisogna capire che servono ad avere piú opzioni.
#### Un esempio é, Integer, ha un valore massimo, possiamo chiararlo ad un int.
```java
int numero_massimo = Integer.MAX_VALUE;
Integer numero_massimo2 = Integer.MAX_VALUE;
// Entrambi contengono la stessa cosa, fatti in modo diversi.
// Uno con etichetta e l'altro con la sua classe wrapper.
```
## [👨‍👩‍👧‍👦] List / ArrayList / LinkedList
#### Le variabili di tipo "List" sono letteralmente liste, quindi pure LinkedList e ArrayList.
#### Per creare una lista, bisogna specificarlo cosi:
```java
List<String> lista = new ArrayList<>();
```
## 🔴 ATTENZIONE:
### Dobbiamo stare attenti al creare le liste cosi.
```java
ArrayList<String> lista = new List<>();
```
#### Perché "List" é una interfaccia, mentre ArrayList é una classe che implementa l'interfaccia "List".
## ❔ É importante utilizzare le Liste?
### Si, la lista precedente é di tipo "String", puó essere perfettamente una lista di un'altra cosa.
## 🔴 ATTENZIONE: 
### Il valore specificato delle liste dev'essere di tipo wrapper.
### per esempio, una lista di "int" dev'essere scritta cosi:
```java
List<Integer> lista = new ArrayList<>();
```
### Peró, che differenza tra c'é tra LinkedList e ArrayList?
#### ArrayList salva gli elementi in una lista ridimensionabile mentre LinkedList lo fa con nodi collegati, quindi molta piú flessibilitá. 
## ❔ A cosa potrei usare le liste?
### Facciamo un esempio veloce, una lista di giocatori di qualsiasi modalitá in minecraft, di qualsiasi gioco, o piú semplice, una lista di invitati ad una festa di compleanno.
### La lista ci serve ad avere un insieme di elementi, nel caso di minecraft, di giocatori, nel caso del compleanno e del resto di giochi, persone, con i quali interagire.
```java
	public static void main(String[] args) {
		// 👇 Creazione della lista
		List<String> giocatori = new ArrayList<>();

  		// 👇 Aggiungere valori di tipo "String" nella lista
		giocatori.add("Joshet18");
		giocatori.add("Ira");
		giocatori.add("Jess");
		giocatori.add("xHydra");

		System.out.println("Giocatori: ");
		System.err.println(giocatori);
	}
```
### Risultato:
```dos
Giocatori:
[Joshet18, Ira, Jess, xHydra]
```
### Possibili metodi da usare:
	- Aggiungere
	- Rimuovere
	- Ottenere elemento di una posizione specifica
	- Verificare se la lista contiene un elemento
	- Aggiungere un sacco di elementi alla propria lista (normalmente da un'altra lista)
## [🟩] Arrays delle variabili
#### Le variabili possono essere crearsi come Arrays direttamente.
### ES:
```java
String[] lista_nomi = new String[] { "Joshet18", "Jess", "Ira", "xHydra" };
```
#### Anche se a "lista_nomi" non abbiamo acceso completo, é comunque una lista che possiamo usare di un'altro modo.
## [🎈] Iterator
#### Serve per percorrere sequenzialmente gli elementi di una lista/collezione, utilizzando, delle liste, il metodo "iterator()".
#### Per evitare conflitti di concorrenza, é importante utilizzare Iterator e/o altre tecniche.
```java
 public static void main(String[] args) {

        List<String> lista = new ArrayList<>();

        lista.add("Joshet18");
        lista.add("Ira");
        lista.add("xHydra");

        Iterator<String> iterator = lista.iterator();

        while (iterator.hasNext()) {
// 	☝ Mentre  ☝ La sua iterazione abbia un elemento successivo.

            String elemento = iterator.next();  // 👈 Salvare il successivo.
            System.out.println(elemento);  // 👈 Mostrare elemento salvato in conbsole.

        }
    }

```
## [📎] Arrays
#### Menzionato prima ma non si é capito. Gli arrays sono un gruppo (?) di elementi dello stesso tipo.
#### La classe "Arrays" offre metodi per ordinare, paragonare, cercare e riempire questo nostro insieme di elementi.
```java
public static void main(String[] args) {

        int[] array = {5, 3, 8, 1, 2}; // 👈 Array di tipo int

	// 👇 Con sort, possiamo ordinare il nostro array.
        Arrays.sort(array);

	// 👇 Con binarySearch, possiamo trovare l'index (posizione)
   		// del nostro numero "3", in questo caso, il suo index
			// é 1, ma quando ordiniamo la lista, é 2.
        int index = Arrays.binarySearch(array, 3);

    }
```
#### Nell'esempio precedente insegnava solo due metodi tra tanti che possiamo usare per lavorare con "Arrays".
#### "Arrays" peró lo si puó usare anche con List ed ArrayList
```java
List<String> lista = new ArrayList<>(Arrays.asList("Joshet18", "Jess"));
```
## [🔑] Map / HashMap / LinkedHashMap / ConcurrentHashMap / TreeMap
#### Puó sembrare difficile, ma vi posso garantire che HashMap é, non solo facilissimo ma anche molto utile.
#### Prima vorrei spiegare a cosa serve e poi vi faccio degli esempi.
####
#### HashMap é una variabile di tipo "lista" (Tra tante virgolette, perché non é del tutto una lista), 
#### che serve a dare un valore ad una chiave. Spiegato meglio, dare un variabile ad un altra variabile.
####
#### Un esempio del suo uso, é la modalitá di KitPVP di Minecraft. Ripeto, molti di voi siete qui indirettamente per sapere piú su Spigot (Minecraft).
#### Nel KitPVP, il "CombatLog" (Punire giocatori quando escono dal server durante un combattimento) potrebbe perfettamente utilizzare HashMap.
#### Come? Qual é la chiave? Qual é il valore?
#### Come? Semplice, quando si entra in comattimento, la chiave diventa il giocatore, il valore puó essere o una variabile di tipo **Boolean** ¨per specificare se é o no in combattimento", o il valore puó essere perfettamente il tempo di rimanente del giocatore perche possa uscire dal combattimento, normalmente di tipo double.
### ❔ Come si crea? 
#### Stessa cosa della lista, solo che la lista puó solo lavorare con un valore, HashMap con due valori.
```java
Map<String, Boolean> in_combattimento = new HashMap<>();
```
### Possibili metodi da usare:
	- Verificare se una chiave esiste.
	- Prendere chiave (Otteniamo il suo valore).
	- Prendere valore.
	- Verificare se l'HashMap é vuoto o no.
	- Mettere un valore ad una chiave.
	- Mettere un valore ad una chiave, solo se non esiste e viceversa.
	- Ottenere, tramite iterazione, tutte le chiavi e/o valori.
### ES:
```java
    public static void main(String[] args) {
        
    	HashMap<String, Integer> eta_persone = new HashMap<>();
//	  	    👇 Mettiamo valori numerali a diverse chiavi di tipo String.
    	eta_persone.put("Joshet18", 18);
    	eta_persone.put("Jess", 18);
    	eta_persone.put("xHydra", 17);
    	eta_persone.put("Ira", 11);
//  			 ☝ In questo caso, dichiriamo le etá reali di diversi nomi (persone). 
    	
    	System.err.println("Etá di Jess é " + eta_persone.get("Jess"));	
    }
```
### Risultato:
```dos
Etá di Jess é 18
```
#### Ok ma, é stato solo spiegato HashMap e Map, e il resto?
#### Semplice: 
	LinkedHashMap fa la stessa cosa di LinkedList, nodi collegati.
	ConcurrentHashMap é opzionale, lo si puó usare per evitare errori di concorrenza
 	(Concorrenza: Quando una lista é giá utilizzata in un thread diverso).
	TreeMap é sempre HashMap, solo che ordinato in modo di albero, quindi elementi posizionati in ordine alfabetico

## [🍄] Set / HashSet / TreeSet
#### Puó sembrare difficile pure questo, ma sopra o sotto, avró lasciato la lista del contenuto e in piú a cosa servono (Una spiegazione veloce). In caso servisse un esempio e/o definizione piú dettagliata esistono queste sezioni.
#### Set é come Map, HashSet come HashMap, si capisce? Ok, non spiega niente, ma era solo per far capire che sono simili almeno in quello.
### ❔ Cos'é e/o a cosa serve "Set"? 
#### Set, insieme ad HashSet, sono come le liste normali. Solo che in questo caso, si usa Set per evitare che si ripetano gli elementi, per evitare i duplicati.
```java
public static void main(String[] args) {
	List<String> nomi = new ArrayList<>(Arrays.asList("Luca", "Luca", "Joshet18", "Jess"));
	Set<String> nomi2 = new HashSet<>(Arrays.asList("Luca", "Luca", "Joshet18", "Jess"));
		
	System.out.println("Con liste normali: "+nomi);
	System.out.println("Con hashSet: "+nomi2);
}
```
### Risultato:
```dos
Con liste normali: [Luca, Luca, Joshet18, Jess]
Con hashSet: [Joshet18, Luca, Jess]
```
### ❔ TreeSet?
#### Come TreeMap, TreeSet serve ad ordinare gli elementi, in ordine alfabetico, a differenza dell'HashSet normale.
```java
		TreeSet<String> nomi = new TreeSet<>();
		
		nomi.add("Joshet18");
		nomi.add("Anna");
		nomi.add("Jess");
		
		System.out.println("Nomi con Set: "+nomi);
```
### Risultato:
```dos
Nomi con Set: [Anna, Jess, Joshet18]
```
## [🃏] Comparator<?>
#### Comparator a cosa serve? Molto semplice e veloce: É una variabile per definire l'ordinamento di elementi.
#### Comparator lo puoi usare con Liste ma pure con Set e/o variabili di tipo Tree... qui un esempio:
```java
	public static void main(String[] args) {

		Comparator<String> comparator = (a, b) -> b.compareTo(a);
		TreeSet<String> nomi = new TreeSet<>(comparator);
		
		nomi.add("Jess");
		nomi.add("Anna");
		nomi.add("Joshet18");
		
		System.out.println("Nomi con comparator: "+nomi);
		
	}
```
## Risultato:
```dos
Nomi con comparator: [Joshet18, Jess, Anna]
```
## [🗜] PROPERTIES
#### Properties é una classe che ci permette di interagire e/o gestire le proprietá del nostro sistema. 
#### Puó sembrare poco utile, ma é utile per esempio con i file dentro il nostro sistema, o con configurazioni di java che vogliamo cambiare e/o ottenere.
```java
public static void main(String[] args) {
		
        Properties prop = System.getProperties();
        String sistema = prop.getProperty("os.name");  // 👈 Prendere la proprietá "operation system name"
// 	☝ Di tipo testo chiamato Sistema.
        System.out.println("Sistema: " + sistema);
        
}
```
## Risultato:
```dos
Sistema: Windows 10
```
## [🐞] SCANNER
#### Per coloro che hanno un po di conoscenze in bash, sapranno a cosa serve il comando "read". Scanner in java, in questo caso, é un read (di bash) solo che molto piú "gestibile".
#### Scanner puó usarsi per molte piú cose, ma nell'esempio sotto ci sará un esempio pratico e veloce di come usare Scanner e capire a cosa serve.
#### Potrebbe servirci, in caso di progetti di solo java, a fare un sistema di autenticazione.
```java
public static void main(String[] args) {
        System.out.println("Inserisci password: ");
// 	☝ Messaggio per capire cosa fare.
        Scanner scanner = new Scanner(System.in); // 👈 "System.in" inteso come input che mettiamo noi.

        String password_inserita = scanner.next(); // 👈 Salvare in una variabile di testo, quello inserito
        
        System.out.println("[*] Password salvata con successo.");
        System.out.println("Password: "+password_inserita);
}
```
## Risultato:
```dos
Inserisci password: 
us@stellarsquad2024
[*] Password salvata con successo.
Password: us@stellarsquad2024
```
## [🔨] StringBuilder // StringBuffer
#### Entrambi sono uguali, fanno la stessa cosa, hanno la stessa funzione, solo che lavorano in modo diverso.
#### Uno "StringBuilder" ci serve a creare di vari elementi di testo, un unico elemento.
#### Per esempio, se in una lista abbiamo una lista di parole che se le uniamo formano una parola, StringBuilder ci serve ad unire tutti gli elementi e trasformarli in un unico "String".
#### E a cosa ci serve? Per esempio, a creare una String, composta di vari elementi di diverse parti, StringBuilder, come ben dice il suo nome (Builder), costruisce una String.
```java
public static void main(String[] args) {
		
	String[] parole = {"Ciao,", "come", "va?"}; // 👈 Una lista con cui lavorare
		
	StringBuilder sb = new StringBuilder(); // 👈 Istanziare StringBuilder
		
	for (String ogniElemento : parole) { // 👈 Per correre ogni elemento della lista "parole"
		sb.append(ogniElemento).append(" ");
//		☝ sb, prende ogni elemento ed sb prende uno spazio.
//		   Lo spazio si é messo perché se non ci fosse il risultato sarebbe: Ciao,comeva?		
	}
		
	String risultato = sb.toString(); // 👈 Potrebbe mandarsi direttamente senza creare questo
		
	System.out.println(risultato); // 👈 Mandare in console
		
}
```
## Risultato:
```dos
Ciao, come va?
```
## [📆] Date / Calendar
### Date e Calendar servono, entrambi, a prendere e successivamente dichiarare la data attuale, presa del sistema.
### Potrebbe essere usata per salvare la esecuzione (possibilmente) di una funzione o in generale, utilizzarlo per creare un valore di testo.
```java
public static void main(String[] args){
         Date date = new Date(); // 👈 Istanza della classe "Date"
         int anno = date.getYear() + 1900; // 👈 Per ottenere l'anno attuale, sommare sempre "1900"
         int day = date.getDate(); // 👈 Non si prende "day" ma "date".
         int mese = date.getMonth() + 1; // 👈 Si prende il mese e si somma per 1.
         System.out.println("Oggi é il: "+day+"/"+mese+"/"+anno);
 }
```

## Risultato:
```dos
Oggi é il: 25/3/2024
```
### "Calendar" la stessa cosa, solo che la istanza si mette in un altro modo:
```java
	public static void main(String[] args) {
		Calendar a = Calendar.getInstance();
		
		int giorno = a.getTime().getDate();
		int anno = a.getTime().getYear() + 1900;
		int mese = a.getTime().getMonth() + 1;
		
		System.out.println("Giorno: "+giorno);
		System.out.println("Mese: "+mese);
		System.out.println("Anno: "+anno);
	}
```
## Risultato:
```dos
Giorno: 25
Mese: 3
Anno: 2024
```
## [🐸] RANDOM
### Ipotizziamo che dobbiamo prendere un nome, in modo aleatorio (random), di una lista, di membri, per esempio.
```java
String[] nomi = {"Joshet18", "Jess", "Ira", "xHydra"};
```
### Utilizzando nextInt, possiamo dichiarare, il massimo del numero che riceveremo aleatoriamete quando andremo a prendere l'elemento.
```java
int r = new Random().nextInt(nomi.length); // 👈 La longitudine della lista "nomi"
```
### Si é creato, con "new Random().nextInt()" un numero, aleatorio, con un massimo che equivarrà alla lingitudine della lista.
### Prende un numero aleatorio, quindi, da 0 a 3 (Sono 4 elementi ma si conta da 0, "Joshet18" é nella posizione "0").
```java
	public static void main(String[] args) {
		String[] nomi = {"Joshet18", "Jess", "Ira", "xHydra"};
		int r = new Random().nextInt(nomi.length);
		String nome = nomi[r]; // 👈 Lo salviamo come valore di tipo String (testo)
		System.out.println("Nome scelto aleatoriamente: "+nome);
	}
```
## Risultato:
```dos
Nome scelto aleatoriamente: Ira
```
### PSD: Saluti ad Ira.

