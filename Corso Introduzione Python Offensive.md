# <font color="#0000FF"><center>Python Base</center></font>

### <u>Concetti di base</u>


#### Variabili e Tipo di Dati

Le variabili in Python sono come nomi assegnati ai dati che gestiamo. Pensa a una variabile come al nome che dai a un valore, in modo da poter fare riferimento ad essa e utilizzarla in diverse parti del tuo codice.

Nella lezione attuale ci concentreremo sulla comprensione delle variabili e di alcuni tipi di dati fondamentali in Python. Questi concetti sono essenziali poiché ci consentono di archiviare e manipolare le informazioni nei nostri programmi.

* ###### Variabili
 	Una variabile in Python è come un nome assegnato a un dato. Non è necessario dichiarare il tipo di dati, poiché Python è intelligente nel dedurlo.

* ###### Stringhe
 	Le stringhe sono sequenze di caratteri utilizzate per gestire il testo. Sono immutabili, il che significa che una volta creati, non è possibile modificare i loro singoli caratteri.

* ###### Numeri
 	Python gestisce diversi tipi numerici, ma ci concentreremo principalmente su:
 		1. Interi: numeri senza parte decimale.
 		2. Float: numeri che includono decimali.
 		3. Liste.

Gli elenchi sono raccolte ordinate e modificabili che possono contenere elementi di diverso tipo.

Sono ideali per archiviare e accedere ai flussi di dati. E per lavorare con questi elenchi, così come con le stringhe e gli intervalli di numeri, utilizzeremo i cicli ‘for’, che ci consentono di scorrere ogni elemento di una sequenza in modo efficiente.



#### String Formatting, Cicli e Condizionali

Python fornisce diversi modi per formattare le stringhe, consentendoti di inserire variabili al loro interno, nonché di controllare la spaziatura, l’allineamento e la precisione dei dati visualizzati. Ecco le tecniche di formattazione delle stringhe che esploreremo: 

* ###### Operatore % (percentuale)
	Conosciuto anche come “interpolazione di stringhe”, questo metodo classico utilizza segnaposto come “%s” per le stringhe, “%d” per i numeri interi o “%f” per i numeri a virgola mobile.

* ###### metodo format()
	Introdotto in Python 2.6, consente maggiore flessibilità e chiarezza. Utilizza le parentesi graffe ‘{}’ come segnaposto all’interno della stringa e può includere dettagli sul formato dell’output.

* ###### F-Strings (interpolazione letterale di stringhe)
	Disponibili a partire da Python 3.6, F-Strings offre un modo conciso e leggibile per incorporare espressioni all’interno di stringhe letterali utilizzando la lettera ‘f’ prima di aprire virgolette e parentesi graffe per indicare dove verranno inserite variabili o espressioni.



#### Le Funzioni e ambito delle variabili
 
###### **Funzioni

Le funzioni sono blocchi di codice riutilizzabili progettati per eseguire un’attività specifica. In Python, vengono definite utilizzando la parola chiave “def” seguita da un nome descrittivo, parentesi che possono contenere parametri e due punti. I parametri sono “variabili di input” che possono cambiare ogni volta che la funzione viene chiamata. Questo consente alle funzioni di operare su dati diversi e produrre i risultati corrispondenti.

Le funzioni possono restituire valori al programma principale o ad altre funzioni utilizzando la parola chiave “return”. Questo le rende incredibilmente versatili, in quanto possono elaborare dati e quindi passare i dati modificati ad altre parti del programma.


###### **Ambito delle variabili**

L’ambito di una variabile si riferisce alla regione di un programma in cui tale variabile è accessibile. In Python, esistono due tipi principali di ambiti:

- Locale: 
	le variabili definite all’interno di una funzione hanno un ambito locale, il che significa che sono accessibili e modificabili solo all’interno della funzione in cui sono state create. 

- Globale: 
	le variabili definite al di fuori di tutte le funzioni hanno un ambito globale, il che significa che sono accessibili da qualsiasi punto del programma. Tuttavia, per modificare una variabile globale all’interno di una funzione, è necessario dichiararla come globale.



#### Come gestire errori e eccezioni

In questo corso tratteremo la gestione degli errori e delle eccezioni, un aspetto critico per la creazione di programmi robusti e affidabili in Python. Gli errori sono inevitabili nella programmazione, ma gestirli correttamente è ciò che distingue un buon programma da uno che fallisce costantemente.


###### **Gestione degli errori**

Gli errori possono verificarsi per molte ragioni: errori di codice, dati di input errati, problemi di connettività, tra gli altri. Invece di consentire a un programma di fallire con un errore, Python ci fornisce gli strumenti per “catturare” questi errori e gestirli in modo controllato, impedendo così che il programma si fermi inaspettatamente e permettendoci di reagire in modo appropriato.


###### **Eccezioni**

Un’eccezione in Python è un evento che si verifica durante l’esecuzione di un programma che interrompe il normale flusso delle istruzioni del programma. Quando l’interprete incontra una situazione che non è in grado di gestire, “solleva” o “lancia” un’eccezione.


###### **Blocchi TRY e EXCEPT**

Per gestire le eccezioni, utilizziamo i blocchi “try” e “Exception”. Un blocco “try” contiene il codice che può generare un’eccezione, mentre un blocco “eccetto” rileva l’eccezione e contiene il codice che viene eseguito quando si verifica una eccezione.


###### **Altre parole chiave per la gestione delle eccezioni**

- \#else: 
	può essere utilizzato dopo i blocchi ‘eccetto’ per eseguire il codice se il blocco ‘prova’ non ha sollevato un’eccezione.

- \#finally: 
	utilizzato per eseguire codice che dovrebbe essere eseguito indipendentemente dal fatto che si sia verificata o meno un’eccezione, come la chiusura di un file o una connessione di rete.

 
###### **Creare eccezioni

È anche possibile “creare” intenzionalmente un’eccezione con la parola chiave “raise”, che consente di forzare il verificarsi di un’eccezione in condizioni specifiche.

In questa lezione impareremo come identificare diversi tipi di eccezioni e come gestirle in modo specifico. Esploreremo anche come utilizzare l’istruzione ‘raise’ per creare eccezioni che aiutano a controllare il flusso del programma ed evitare stati errati o dati corrotti.

****
### <u>La struttura dei dati</u>


#### Le Tuple

Le tuple sono raccolte ordinate di elementi che non possono essere modificati una volta creati. Questa caratteristica li rende ideali per garantire che determinati dati rimangano costanti durante tutto il ciclo di vita di un programma.


###### **Caratteristiche delle tuple**

- \#Immutabilità: 
	una volta creata una tupla, non è possibile modificare, aggiungere o eliminare elementi. Questa immutabilità garantisce l’integrità dei dati che si desidera mantenere costanti.

- \#Indicizzazione e slicing: 
	come per gli elenchi, è possibile accedere agli elementi della tupla utilizzando gli indici ed è anche possibile eseguire operazioni di affettamento per ottenere sottosequenze della tupla.

- \#Eterogeneità: 
	le tuple possono contenere elementi di diverso tipo, comprese altre tuple, il che le rende molto versatili.


###### **Operazioni con tuple**

Sebbene non sia possibile modificare una tupla, è possibile eseguire diverse operazioni:

- Compressione e decompressione delle tuple: 
	le tuple consentono di assegnare e annullare l’assegnazione dei propri elementi a più variabili contemporaneamente.

- Concatenazione e ripetizione: 
	analogamente agli elenchi, puoi combinare tuple utilizzando l’operatore ‘+’ e ripetere gli elementi di una tupla un determinato numero di volte con l’operatore ‘\*’.

- Metodi di ricerca: 
	puoi utilizzare metodi come ‘index()’ per trovare la posizione di un elemento e ‘count()’ per contare quante volte un elemento appare nella tupla.


###### **Utilizzo delle tuple in Python**

- Funzioni e assegnazioni multiple: 
	le tuple sono molto utili quando una funzione deve restituire più valori o quando vengono effettuate più assegnazioni su una singola riga.

- Strutture dati fisse: 
	vengono utilizzate per creare strutture dati che non dovrebbero cambiare, come i giorni della settimana o le coordinate di un punto nello spazio.


<u>Buone abitudini</u>

Tratteremo quando è più appropriato utilizzare le tuple anziché gli elenchi e in che modo la scelta di una tupla rispetto a un elenco può influire sulla chiarezza e sulla sicurezza del codice.



#### I Sets

###### **Imposta funzionalità

\#Unicità:
	i set scartano automaticamente gli oggetti duplicati, rendendoli perfetti per collezionare oggetti unici.

\#Non ordinato: 
	a differenza delle liste e delle tuple, i set non mantengono gli elementi in un ordine specifico.

\#Mutabilità: 
	gli elementi di un insieme possono essere aggiunti o rimossi, ma gli elementi stessi devono essere immutabili (ad esempio, non è possibile avere un insieme di elenchi, poiché gli elenchi possono essere modificati).

 
###### **Operazioni con i Sets

Esploreremo le operazioni di base sugli insiemi facilitate da Python, come:

- Aggiunta e rimozione: 
	aggiungi elementi con ‘add()’ e rimuovi elementi con ‘remove()’ o ‘discard()’.

- Operazioni sugli insiemi: 
	esegui unioni, intersezioni, differenze e differenze simmetriche utilizzando i rispettivi metodi o operatori.

- Test di appartenenza: 
	controlla rapidamente se un elemento è membro di un set.

- Immutabilità Facoltativo: 
	utilizzare il tipo ‘frozenset’ per creare set che non possono essere modificati dopo la creazione.


###### **Utilizzo dei Sets in Python

- Rimozione duplicati: 
	sono utili quando è necessario assicurarsi che una raccolta non contenga elementi ripetuti.

- Relazioni tra raccolte: 
	facilitano la comprensione e la gestione delle relazioni matematiche tra raccolte, come sottoinsiemi e superinsiemi.

- Prestazioni di ricerca: 
	forniscono una ricerca degli elementi più rapida rispetto agli elenchi o alle tuple, il che è utile per grandi volumi di dati.


<u>Buone abitudini</u>

Discuteremo quando è vantaggioso utilizzare i set invece di altre strutture dati e come il loro utilizzo può influenzare l’efficienza del programma.



#### I Dizionari

In questa lezione ci concentreremo sui dizionari, una delle strutture dati più potenti e flessibili in Python. I dizionari in Python sono raccolte non ordinate di coppie chiave-valore. A differenza delle sequenze, che vengono indicizzate utilizzando un intervallo numerico, i dizionari vengono indicizzati utilizzando chiavi univoche, che possono essere di qualsiasi tipo immutabile, come stringhe o numeri.


###### **Caratteristiche dei dizionari

- Non ordinato: 
	gli elementi di un dizionario non sono ordinati e non sono accessibili tramite un indice numerico, ma piuttosto tramite chiavi univoche.

- Dinamico: 
	le coppie chiave-valore possono essere aggiunte, modificate ed eliminate.

- Chiavi univoche: 
	ogni chiave di un dizionario è unica, impedendo duplicazioni e sovrascritture accidentali.

- Valori accessibili:
	i valori non devono essere univoci e possono essere di qualsiasi tipo di dati.

- Operazioni con i dizionari


Durante la lezione esploreremo come eseguire operazioni di base e avanzate con i dizionari:

- Aggiungere e modificare: 
	come aggiungere nuove coppie chiave-valore e modificare i valori esistenti.

- Elimina:
	come eliminare le coppie chiave-valore utilizzando il metodo del o ‘pop()’.

- Metodi del dizionario: 
	utilizza metodi come “keys()”, “values()” e “items()” per accedere a chiavi, valori o entrambi in coppia.

- Comprensioni del dizionario: 
	un modo elegante e conciso per costruire dizionari basati su sequenze o intervalli.


###### **Utilizzo dei dizionari in Python

- Archiviazione di dati strutturati: 
	ideale per archiviare e organizzare dati logicamente correlati, come un database in memoria.

- Ricerca efficiente: 
	i dizionari sono altamente ottimizzati per recuperare valori quando la chiave è nota, fornendo tempi di ricerca molto rapidi.

- Flessibilità: 
	possono essere nidificati, il che significa che i valori all’interno di un dizionario possono essere altri dizionari, elenchi o qualsiasi altro tipo di dati.


<u>Buone abitudini</u>

Metteremo in risalto le migliori pratiche per lavorare con i dizionari, inclusa la selezione delle chiavi appropriate e la gestione degli errori comuni, come il tentativo di accedere a chiavi che non esistono.

****

### <u>Programmazione Orientata a Oggetti (POO)</u>


#### Classi e Oggetti

La programmazione orientata agli oggetti (OOP) è un paradigma di programmazione che utilizza oggetti e classi nel suo approccio principale. È un modo di strutturare e organizzare il codice che riflette il modo in cui gli sviluppatori pensano al mondo reale e alle entità al suo interno.


###### **Classi

Le classi sono i fondamenti dell’OOP. Fungono da modelli per la creazione di oggetti e definiscono attributi e comportamenti che avranno gli oggetti creati da essi. In Python, una classe viene definita con la parola chiave ‘class’ e fornisce la struttura iniziale per qualsiasi oggetto da essa derivato.


###### **Istanze e oggetti di classe

Un oggetto è un’istanza di una classe. Ogni volta che crei un oggetto, stai creando un’istanza che ha il proprio spazio di memoria e un proprio insieme di valori per gli attributi definiti dalla sua classe. Gli oggetti incapsulano dati e funzioni insieme in un’entità discreta.

 
###### **Metodi di classe

I metodi di classe sono funzioni definite all’interno di una classe e possono essere chiamate solo da istanze di quella classe. Questi metodi sono il meccanismo principale per interagire con gli oggetti, consentendo loro di eseguire operazioni o azioni, modificare il loro stato o persino interagire con altri oggetti.


In questo corso ti forniremo gli strumenti e le conoscenze necessarie per iniziare a progettare e sviluppare le tue classi e istanziarle in oggetti funzionali. Impareremo come funzionano i metodi delle classi e come puoi usarli per dare vita al comportamento dei tuoi oggetti in Python. Questa conoscenza sarà essenziale man mano che continuerai ad apprendere e ad applicare i principi OOP a progetti più complessi.

All’interno del paradigma della programmazione orientata agli oggetti in Python, ci sono concetti avanzati come decoratori, metodi di classe e metodi statici che arricchiscono ed espandono le possibilità di come interagiamo con le classi e le loro istanze.

 
###### **Decoratori

I decoratori sono un potente strumento in Python che ti consente di modificare il comportamento di una funzione o di un metodo. Funzionano come “wrapper”, aggiungendo funzionalità prima e dopo il metodo o la funzione decorata, senza modificarne il codice sorgente. In OOP, i decoratori vengono spesso utilizzati per aggiungere dinamicamente funzionalità ai metodi, come la sincronizzazione dei thread, la memorizzazione dei risultati o il controllo dei permessi.

 
###### **Metodi di classe

Un metodo di classe è un metodo associato alla classe e non a un’istanza della classe. Ciò significa che il metodo può essere chiamato sulla classe stessa, anziché su un oggetto della classe. Sono definiti utilizzando il decoratore ‘@classmethod’ e il loro primo argomento è sempre un riferimento alla classe, convenzionalmente chiamata ‘cls’. I metodi di classe vengono spesso utilizzati per definire metodi factory che possono creare istanze della classe in diversi modi.

 
###### **Metodi statici

I metodi statici, definiti con il decoratore ‘@staticmethod’, non ricevono un riferimento implicito né all’istanza (self) né alla classe (cls). Fondamentalmente sono come funzioni normali, ma appartengono allo spazio dei nomi della classe. Sono utili quando vogliamo eseguire alcune funzionalità correlate alla classe, ma non richiedono l’accesso all’istanza o agli attributi della classe.


Questi elementi dell’OOP in Python ci consentono di creare astrazioni più chiare e mantenere il codice organizzato, modulare e flessibile, facilitando la manutenzione e l’estensibilità del software.



#### Metodo Statico e Metodo Classe

###### **Metodi di classe

Sono definiti con il decoratore ‘@classmethod’, che permette loro di prendere la classe come primo argomento, solitamente chiamata ‘cls’. Questo accesso alla classe consente ai metodi della classe di interagire con la struttura della classe stessa, ad esempio modificando gli attributi della classe che influenzeranno tutte le istanze. Vengono utilizzati per attività che richiedono la conoscenza dello stato globale della classe, come la costruzione di istanze in modi specifici, noti anche come metodi factory.


###### **Metodi statici

Sono definiti con il decoratore ‘@staticmethod’ e non ricevono un argomento di riferimento implicito alla classe o all’istanza. Sono simili alle normali funzioni definite all’interno del corpo di una classe. Vengono utilizzati per funzioni che, sebbene concettualmente appartengano alla classe per rilevanza tematica, non necessitano di accedere a nessun dato specifico della classe o dell’istanza. Forniscono un modo per incapsulare funzionalità all’interno di una classe, mantenendo la coesione e l’organizzazione del codice.

 
Entrambi i metodi contribuiscono a una progettazione del software più pulita e modulare, consentendo una chiara separazione tra funzionalità che operano rispetto alla classe nel suo insieme e funzionalità che sono indipendenti dalle istanze della classe e dalla classe stessa. La scelta tra l’utilizzo di un metodo di classe o di un metodo statico dipende spesso dal requisito specifico se accedere o meno alla classe o alle sue istanze.



#### Uso del Self

###### **Definizione di ‘self’

A livello concettuale, “self” è un riferimento all’oggetto corrente all’interno della classe. È il primo parametro passato a qualsiasi metodo di una classe in Python. Attraverso self, un metodo può accedere e manipolare gli attributi dell’oggetto e chiamare altri metodi all’interno dello stesso oggetto.


###### **Uso di “self”

Quando viene creata una nuova istanza di una classe, Python passa automaticamente l’istanza appena creata come primo argomento al metodo ‘\_\_init\_\_’ e agli altri metodi definiti nella classe che hanno self come primo parametro. Questo è ciò che consente a un metodo di operare su dati specifici dell’oggetto e non su dati della classe in generale o di altre istanze della classe.


###### **Importanza del ‘self’

Il concetto di sé è importante nell’OOP poiché garantisce che i metodi e gli attributi vengano applicati all’oggetto corretto. Senza self, non saremmo in grado di distinguere tra le operazioni e i dati di diverse istanze di una classe



#### Eredità e Polimorfismo

Ereditarietà e polimorfismo sono concetti fondamentali nella programmazione orientata agli oggetti che consentono la creazione di una struttura di classi flessibile e riutilizzabile.


###### **Eredità

È un principio OOP che consente a una classe di ereditare attributi e metodi da un’altra classe, nota come classe base o superclasse. L’ereditarietà semplifica il riutilizzo del codice e la creazione di una gerarchia di classi. Le sottoclassi ereditano le caratteristiche della superclasse, consentendo loro di specializzarsi o modificare i comportamenti esistenti.


###### **Polimorfismo

Questo concetto si riferisce alla capacità di oggetti di classi diverse di essere trattati come istanze di una classe comune. Il polimorfismo consente a una funzione o a un metodo di interagire con oggetti di classi diverse e di trattarli come se fossero dello stesso tipo, purché condividano la stessa interfaccia o metodo. Ciò significa che lo stesso metodo può comportarsi diversamente in classi diverse, un concetto noto come sovraccarico del metodo.


Sia l’ereditarietà che il polimorfismo sono i capisaldi dell’OOP e sono ampiamente utilizzati per progettare sistemi facilmente estensibili e manutenibili.



#### Incapsulamento e metodi speciali

L’incapsulamento nella programmazione orientata agli oggetti (OOP) gestisce principalmente tre livelli di visibilità per gli attributi e i metodi di una classe: pubblico, protetto e privato. In Python, questa distinzione viene fatta attraverso convenzioni di denominazione, piuttosto che attraverso rigide restrizioni di accesso come in altri linguaggi.

###### **Attributi pubblici

Sono accessibili da qualsiasi punto del programma e, per convenzione, non hanno un prefisso speciale. Si prevede che questi attributi facciano parte dell’interfaccia permanente della classe.

 
###### **Attributi protetti

È indicato da un singolo carattere di sottolineatura all’inizio del nome (ad esempio, ‘\*\*\_attributo\*\*’). Questa è solo una convenzione e non impedisce l’accesso dall’esterno della classe, ma resta inteso che questi attributi sono protetti e non dovrebbero essere accessibili direttamente se non all’interno della classe stessa e nelle sottoclassi.


###### **Attributi privati

In Python, gli attributi privati ​​sono indicati con un doppio carattere di sottolineatura all’inizio del nome (ad esempio, ‘\*\*\_\_attribute\*\*’). Ciò innesca un meccanismo di modifica dei nomi noto come ‘\*\*name mangling\*\*’, in cui l’interprete Python altera internamente il nome dell’attributo per rendere più difficile l’accesso dall’esterno della classe.


###### **Metodi speciali

I metodi speciali in Python sono conosciuti anche come metodi magici e sono identificati da un doppio carattere di sottolineatura all’inizio e alla fine (‘\*\*\_\_method\_\_\*\*’). Consentono alle classi in Python di emulare il comportamento dei tipi incorporati e di rispondere a operatori specifici. Ad esempio, il metodo ‘\*\*\_\_init\_\_\*\*’ viene utilizzato per inizializzare una nuova istanza di una classe, ‘\*\*\_\_str\_\_\*\*’ viene chiamato per una rappresentazione di stringa leggibile dell’oggetto e ‘\*\*\_\_len\_\_\*\*’ restituisce la lunghezza dell’oggetto.

L’incapsulamento e i metodi speciali sono strumenti potenti che, se utilizzati correttamente, possono migliorare la sicurezza, la flessibilità e la chiarezza durante la creazione di applicazioni. Nel corso di questa lezione, esploreremo in dettaglio come implementare e utilizzare questi concetti e metodi per creare classi robuste e gestibili in Python.



#### Decoratori e Proprietà

In questa lezione approfondiremo queste potenti funzionalità di Python che migliorano significativamente il modo in cui possiamo gestire e modificare il comportamento delle nostre classi e funzioni.


###### **Decoratori

I decoratori in Python sono un modo elegante per modificare funzioni o metodi. Vengono utilizzati per estendere o modificare il comportamento della funzione senza modificarne il codice sorgente. Un decoratore è esso stesso una funzione che accetta un’altra funzione come argomento e restituisce una nuova funzione che può facoltativamente aggiungere alcune funzionalità prima e dopo la funzione originale.

 
###### **Proprietà

Le proprietà sono un caso speciale di decoratori che consentono agli sviluppatori di aggiungere elegantemente getter, setter ed delete agli attributi di una classe, controllando così l’accesso e la modifica dei dati. In Python, ciò si ottiene con il decoratore ‘@property’, che trasforma un metodo per accedere a un attributo come se fosse un attributo pubblico.

 
###### **Getter e setter

- Il getter ottiene il valore di un attributo mantenendo l’incapsulamento e consentendo l’esecuzione di logica aggiuntiva durante l’accesso.

- Il setter imposta il valore di un attributo e può includere la convalida o l’elaborazione prima che la modifica si rifletta nello stato interno dell’oggetto.

- Il “deleter” può essere utilizzato per definire un comportamento quando un attributo viene eliminato con del.



****

### <u>Moduli e pacchetti in Python</u>


#### Organizzare il codice con i moduli

Organizzare il codice in moduli è una pratica essenziale in Python per creare programmi scalabili e manutenibili. I moduli sono file Python che contengono definizioni e dichiarazioni di variabili, funzioni, classi o altri oggetti che possono essere riutilizzati in diverse parti del programma.


###### **Struttura del modulo

Ogni modulo in Python è un file ‘.py’ che incapsula il tuo codice per uno scopo specifico. Ad esempio, puoi avere un modulo per le operazioni matematiche, un altro per la gestione di input/output e un altro per la logica dell’interfaccia utente. Questa struttura aiuta a mantenere il codice organizzato, ne facilita la lettura e consente il riutilizzo del codice.


###### **Importazione del modulo

Python usa la parola chiave ‘import’ per usare i moduli. Puoi importare un intero modulo, ad esempio “import math”, o importare nomi di moduli specifici utilizzando “from math import sqrt”. Python consente anche di importare moduli con un alias per facilità d’uso all’interno del codice, come “import numpy as np”.

 
###### **Pacchetti

Quando i programmi crescono e i moduli iniziano ad accumularsi, Python ti consente di organizzare i moduli in pacchetti. Un pacchetto è una cartella che contiene moduli e un file speciale chiamato ‘\_\_init\_\_.py’, che dice a Python che quella cartella contiene moduli che possono essere importati.

 
###### **Vantaggi del modulo

- Manutenzione: 
	i moduli consentono di lavorare su parti del codice in modo indipendente senza influenzare altre parti del sistema.

- Spazio dei nomi: 
	i moduli definiscono il proprio spazio dei nomi, il che significa che è possibile avere funzioni o classi con lo stesso nome in moduli diversi senza conflitti.

- Riutilizzo: 
	il codice scritto nei moduli può essere riutilizzato in diversi programmi semplicemente importandoli dove necessario.



#### Importare e usare moduli

L’importazione e l’utilizzo dei moduli è una tecnica fondamentale in Python che consente la modularità e il riutilizzo del codice. I moduli sono file Python con estensione ‘.py’ che contengono definizioni di funzioni, classi e variabili che possono essere utilizzate in altri script Python.


###### **Importazione del modulo

L’istruzione ‘import’ viene utilizzata per includere un modulo nello script corrente. Quando importi un modulo, Python cerca quel file in un elenco di directory definite da ‘sys.path’, che include la directory corrente, le directory elencate nella variabile d’ambiente ‘PYTHONPATH’ e le directory di installazione predefinite.


###### **Utilizzo dei moduli

Una volta importato un modulo, puoi utilizzare le sue funzioni, classi e variabili, utilizzando la sintassi ‘nome\_modulo.nome\_elemento’. Ciò è essenziale per l’organizzazione del codice, poiché consente di accedere al codice riutilizzabile senza doverlo duplicare.


###### **Importazione alias

A volte, per comodità o per evitare conflitti di denominazione, potresti voler dare un alias a un modulo quando lo importi usando la parola chiave ‘as’: ‘import module as alias’.

Ciò consente di accedere ai componenti del modulo utilizzando l’alias anziché il nome completo del modulo.


###### **Importazione specifica

Se hai bisogno solo di una o più funzioni specifiche da un modulo, puoi importarle direttamente utilizzando ‘dalla funzione di importazione del modulo’. Ciò consente di evitare di dover anteporre alle funzioni il nome del modulo ogni volta che vengono chiamate. Inoltre, puoi importare tutte le definizioni di un modulo (sebbene non sia una pratica consigliata) utilizzando ‘from module import \*’.


###### **Moduli di libreria standard

Python viene fornito con un’ampia libreria standard che offre moduli per eseguire una varietà di attività, dalla manipolazione del testo, data e ora, all’accesso a Internet e allo sviluppo web. Acquisire familiarità con la libreria standard è fondamentale per essere un programmatore Python efficiente.


###### **Moduli di terze parti

Oltre alla libreria standard, è disponibile un’ampia gamma di moduli di terze parti che puoi installare e utilizzare nei tuoi programmi. Questi moduli vengono spesso installati utilizzando strumenti di gestione dei pacchetti come “pip”.



#### Creazione e distribuzione dei pacchetti

La creazione e la distribuzione di pacchetti è un processo chiave nell’ecosistema Python, poiché consente agli sviluppatori di condividere le proprie librerie e moduli con la comunità globale. Un pacchetto Python è una raccolta strutturata di moduli che può includere codice riutilizzabile, nuovi tipi di dati o persino intere applicazioni.


###### **Creazione del pacchetto

Per creare un pacchetto, devi prima organizzare il codice in moduli e sottopacchetti all’interno di una struttura di directory. Ogni pacchetto Python deve contenere un file speciale chiamato ‘\_\_init\_\_.py’, che può essere vuoto, ma indica che la directory è un pacchetto Python. Questo file può anche contenere codice per inizializzare il pacchetto.


###### **Struttura delle directory

Una struttura tipica del pacchetto potrebbe includere directory per la documentazione, i test e il codice stesso, nonché file di configurazione per l’installazione e la distribuzione del pacchetto.


###### **File di configurazione

I file “setup.py” e “pyproject.toml” sono essenziali nella creazione dei pacchetti. Contengono metadati e configurazioni necessarie per la distribuzione del pacchetto, come nome del pacchetto, versione, descrizione e dipendenze.


###### **Distribuzione dei pacchetti

Per distribuire un pacchetto, in genere si utilizza Python Package Index (PyPI), che è un repository software per la comunità Python. Il caricamento di un pacchetto su PyPI lo rende accessibile ad altri sviluppatori utilizzando strumenti di gestione dei pacchetti come “pip”.


###### **Installazione globale

Distribuendo un pacchetto, gli utenti possono installarlo globalmente nel loro ambiente Python, il che significa che sarà disponibile per tutti i progetti in quell’ambiente. Questo è un modo efficace per condividere il codice e consentire ad altri di trarre vantaggio e contribuire al lavoro svolto.


###### **Perché confezionare e distribuire?

Il confezionamento e la distribuzione del software presentano numerosi vantaggi. Consente il riutilizzo del codice, facilita la collaborazione tra gli sviluppatori e aiuta nella gestione delle dipendenze e delle versioni del software. Inoltre, il contributo alla comunità open source può portare al riconoscimento del lavoro dello sviluppatore e offrire opportunità di feedback e miglioramenti collaborativi.



****

# <font color="#c00000"><center>Python Offensive</center></font>

### <u>Flusso dei dati</u>


#### Dati: Input da tastiera e Output a schermo

L’interazione dell’utente attraverso la console è un’abilità essenziale in Python e in questa lezione esploreremo le funzioni che consentono l’input e l’output dei dati. Utilizzeremo ‘input()’ per raccogliere l’input da tastiera e ‘print()’ per visualizzare i messaggi sullo schermo.
 
Per quanto riguarda il formato del testo, vedremo come gestire e presentare le informazioni in modo amichevole. Ciò include tutto, dalla manipolazione di base delle stringhe alle tecniche di formattazione delle stringhe più avanzate che consentono l’inserimento di variabili e l’allineamento del testo.

La codifica dei caratteri è un aspetto chiave per garantire che input e output gestiscano in modo appropriato lingue e set di caratteri diversi, preservando l’integrità dei dati e la chiarezza della comunicazione della console.

Padroneggiare queste funzionalità è fondamentale per creare programmi che richiedono l’interazione dell’utente e ti forniranno gli strumenti necessari per creare applicazioni interattive robuste e facili da usare.



#### Lettura e scrittura file

###### **Gestione dei file di base

Spiegheremo come utilizzare la funzione ‘open()’ per creare un oggetto file e in che modo le modalità di apertura (“r” per lettura, “w” per scrittura, “a” per aggiunta e “b” per modalità binaria) influenzano il modo in cui lavoriamo con quei file.

 
###### **Lettura file

Spiegheremo in dettaglio come leggere il contenuto di un file in memoria, sia in un colpo solo con il metodo ‘read()’ o riga per riga con ‘readline()’ o eseguendo un’iterazione sull’oggetto file.


###### **Scrittura su file

Esamineremo come scrivere su un file utilizzando metodi come ‘write()’ o ‘writelines()’ e come questi metodi differiscono nella gestione delle stringhe e delle sequenze di stringhe.
 

###### **Gestori del contesto

Uno degli aspetti più importanti della lettura e scrittura di file in Python è l’uso dei gestori di contesto, forniti dall’istruzione ‘with’. I gestori del contesto assicurano che le risorse vengano gestite correttamente aprendo il file e garantendo che, indipendentemente da come o dove termina il blocco di codice, il file venga sempre chiuso correttamente. Ciò aiuta a prevenire errori comuni come perdite di risorse o file che non si chiudono se si verifica un’eccezione.

L’utilizzo di ‘with open()’ non solo migliora la leggibilità del codice, ma semplifica anche la gestione delle eccezioni quando si lavora con i file, rendendo il codice più sicuro e robusto.

Queste informazioni sono vitali per un’ampia gamma di applicazioni, dall’analisi dei dati all’automazione delle attività e allo sviluppo di applicazioni web.



#### Formattazione e manipolazione testo

La formattazione delle stringhe e la manipolazione del testo sono competenze essenziali in Python, specialmente nelle applicazioni che implicano la presentazione di dati all’utente o l’elaborazione di informazioni testuali. In questa lezione ci concentreremo sulle tecniche e sugli strumenti offerti da Python per lavorare con le stringhe di testo.


**Formattazione delle stringhe**

Impareremo i vari metodi di formattazione delle stringhe forniti da Python, tra cui:

- Formattazione classica: 
	tramite l’operatore %, simile a ‘printf’ in C.

- Metodo format(): 
	un approccio versatile che offre numerose possibilità per formattare e allineare il testo, riempire i caratteri, lavorare con i numeri e altro ancora.

- F-strings (Literal String Interpolation): 
	introdotto in Python 3.6, questo metodo consente di incorporare espressioni all’interno di stringhe di testo in modo conciso e leggibile.


**Manipolazione del testo**

Esploreremo le funzioni e i metodi integrati per la manipolazione delle stringhe, tra cui:

- Metodi di ricerca e sostituzione: 
	come ‘find()’, ‘index()’, ‘replace()’ e metodi di espressione regolare.

- Metodi di test: 
	verificare il contenuto della stringa, come ‘isdigit()’, ‘isalpha()’, ‘startswith()’ e ‘endswith()’.

- Metodi di trasformazione: 
	che ti consentono di cambiare il caso di una stringa, dividerla in un elenco di sottostringhe o unirle, come ‘upper()’, ‘lower()’, ‘split()’ e ‘join() ‘.


Vedremo anche come lavorare con le stringhe Unicode in Python, che è essenziale per le applicazioni moderne che devono supportare più lingue e caratteri speciali.



### <u>Progetti (POO)
</u>


