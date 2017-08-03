------------------------------------------------
Nuovo scenario sull’Interoperabilità applicativa
------------------------------------------------

Stante le prescrizioni del nuovo Codice dell'amministrazione digitale, la
qualificazione e l'accesso tramite Porta di Dominio è da considerarsi ad oggi
una soluzione da non implementare ulteriormente. Pertanto i nuovi servizi
applicativi erogati dalle pubbliche amministrazioni verso altre
amministrazioni, o soggetti erogatori di pubblici servizi, dovranno, a regime,
essere erogati senza l’intermediazione delle Porte di Dominio. 
D’altra parte, il modello di sicurezza in questi anni è stato aggiornato con
l'intervento delle norme di coordinamento della sicurezza dello spazio
cibernetico (`DPCM 24 gennaio 2013`_; `Agenda Digitale Europea Pillar III Trust
and Security`_; `Direttiva NIS`_) e sono in corso attività volte al
rafforzamento della gestione della sicurezza informatica descritte nel
`capitolo 8 del Piano Triennale`_.

.. _`DPCM 24 gennaio 2013`:
   http://www.gazzettaufficiale.it/eli/id/2013/03/19/13A02504/sg
.. _`Agenda Digitale Europea Pillar III Trust and Security`:
   http://daeimplementation.eu/dae_actions.php?action_n=38
.. _`Direttiva NIS`:
   http://www.gazzettaufficiale.it/eli/id/2017/04/13/17A02655/sg
.. _`capitolo 8 del Piano Triennale`: 
   https://pianotriennale-ict.readthedocs.io/it/latest/doc/08_sicurezza.html

Percorso di migrazione dalla infrastruttura basata su Porte di dominio
----------------------------------------------------------------------

Si prevede che la dismissione delle Porte di dominio attualmente in esercizio
presso le pubbliche amministrazioni debba avvenire in maniera progressiva e
opportunistica, realizzando i nuovi servizi  sempre con interazioni dirette e
approfittando degli upgrade che saranno applicati alle piattaforme software
esistenti per sostituire progressivamente le Porte con connessioni dirette.

L'operazione prevede un transitorio la cui durata sarà determinata nel
successivo documento *Linee guida del nuovo Modello di interoperabilità* la cui
pianificazione è prevista per fine 2017.  Durante il transitorio le
applicazioni sul lato erogazione dovranno essere in grado di gestire
contemporaneamente le due modalità, con Porta di Dominio e senza, in parallelo.
Al termine di questo transitorio tutte le Porte di Dominio saranno state
dismesse.
La temporanea coesistenza dei due modelli prevede quindi i seguenti scenari:   

Servizi in produzione resi disponibili attraverso la Porta di dominio

  Per i servizi attualmente erogati attraverso la Porta di dominio, le
  amministrazioni dovranno adeguare i loro sistemi in modo da rendere
  disponibili gli stessi servizi anche senza l’intermediazione della Porta di
  dominio stessa, in modalità di erogazione/fruizione diretta. Questo potrà
  essere fatto, ove possibile, rendendo direttamente accessibili le interfacce
  (in tecnologia WS SOAP, secondo quanto fino a questo momento previsto da
  SPCoop) attualmente impiegate per l’interfacciamento interno con la Porta di
  dominio, oppure aggiungendo agli stessi servizi nuove interfacce di accesso
  in modalità WS SOAP o REST. Tale adeguamento, una volta effettuato, dovrà
  essere tempestivamente segnalato alle amministrazioni che stanno al momento
  fruendo dei servizi attraverso la Porta di dominio. 

Sistemi in produzione fruitori di servizi di cooperazione resi attraverso la Porta di dominio

  Le amministrazioni che fruiscono di servizi erogati attraverso la Porta di
  dominio, una volta ricevuta la notifica da parte delle amministrazioni
  erogatrici dell’avvenuta disponibilità diretta degli stessi servizi, dovranno
  provvedere ad adeguare i loro sistemi e predisporli all’interfacciamento
  diretto senza l’intermediazione della Porta di dominio, permettendo quindi il
  successivo spegnimento della Porta

Ad avvenuta migrazione di tutti i servizi erogati e fruiti attraverso la
propria Porta di dominio, l’amministrazione dovrà procedere ad una fase di
dismissione della stessa porta di dominio, tutto ciò compatibilmente con i
contratti in essere e nel  rispetto alle modalità di conclusione/recesso
previste dagli stessi. 

Nuovi servizi e nuovi sistemi fruitori di servizi di cooperazione.

  I nuovi servizi cooperazione ed i nuovi sistemi fruitori di servizi di
  cooperazione dovranno essere messi in produzione in modo da interfacciarsi
  direttamente senza l’intermediazione dell’infrastruttura delle porte di
  dominio. Questo dovrà essere fatto utilizzando formati di interfacciamento
  standard (e.g. WS SOAP o REST).   

A partire dal 20 dicembre 2017, AgID non eseguirà più l'erogazione di
certificati per le Porte di Dominio esistenti.  Da quel momento la manutenzione
delle Porte esistenti, con la sostituzione dei certificati scaduti, sarà a
carico delle singole Amministrazioni le quali dovranno dotarsi di certificati
erogati da fornitori privati e curare la distribuzione di tali certificati
coordinandosi con le Amministrazioni con le quali hanno in essere meccanismi di
cooperazione applicativa.

Presso il portale di Indice PA è disponibile un `elenco completo delle porte di
dominio qualificate <http://www.indicepa.gov.it/report/n-rep-porte-dominio.php>`_.

Sicurezza degli scambi e valore legale
--------------------------------------

La modalità di interfacciamento diretto dei servizi senza l’intermediazione
delle Porte di dominio, pone in capo ai soggetti titolari di un rapporto di
erogazione/fruizione di servizi la gestione degli aspetti di sicurezza in
precedenza demandate alle Porte di dominio. 
In particolare vanno gestiti gli aspetti relativi a:

- sicurezza di canale;
- gestione degli accessi (autorizzazione alla fruizione del servizio);
- tracciature.

In merito a queste tematiche si danno le seguenti indicazioni:

sicurezza di canale

  Le entità operanti il colloquio dovranno provvedere alla creazione di canali
  sicuri utilizzando il protocollo TLS nella versione più recente disponibile
  oppure, ove questo non fosse possibile, almeno nella versione 1.1.
  L’instaurazione del canale dovrà essere fatta a seguito di una mutua
  autenticazione  attraverso l’uso di certificati X509 V3 (tipicamente
  attraverso la verifica del campo subject DN dello stesso certificato). Le
  amministrazioni dovranno dotarsi dei certificati autonomamente. 

gestione degli accessi

  Le amministrazioni devono provvedere, tramite le proprie infrastrutture di
  gestione degli accessi, all’autorizzazione delle richieste di servizio, sia
  nei confronti dell’entità richiedente (amministrazione, erogatore di pubblici
  servizi) che, eventualmente, nei confronti del soggetto operante la richiesta
  per conto dell’entità stessa. 

tracciature

  Le amministrazioni erogatrici dovranno provvedere, ai fini dell’opponibilità
  ai terzi, alla tracciatura degli scambi informativi che intercorrono con l’ente
  fruitore ai fini dell’erogazione del servizio. Tale tracciatura dovrà riportare
  i seguenti elementi minimi:

  - data e ora della richiesta;
  - entità richiedente il servizio (e, ove applicabile, soggetto operante la
    richiesta);
  - servizio richiesto;
  - esito della chiamata (autorizzata/rigettata)
  - ove applicabile, un identificativo univoco della richiesta

  La tracciatura dovrà poi riportare eventuali altre informazioni peculiari al
  tipo di servizio erogato che siano rilevanti ai fini dell’opponibilità ai terzi
  (tracciatura applicativa).
  Il formato della tracciatura dovrà essere specificato al momento della
  progettazione del servizio e la modalità di consultazione della stessa nonché
  di reperimento delle informazioni che la costituiscono dovranno essere
  descritte da un apposito documento allo scopo predisposto dall’amministrazione.

Nuove piattaforme applicative 
-----------------------------

In attesa della pubblicazione delle linee guida del nuovo Modello di
Interoperabilità, la progettazione delle nuove piattaforme applicative dovrà
seguire le raccomandazioni minime contenute nel `capitolo 5 del Piano Triennale`_.

.. _`capitolo 5 del Piano Triennale`:
   https://pianotriennale-ict.readthedocs.io/it/latest/doc/05_modello-di-interoperabilita.html

