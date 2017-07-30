----------------
Scenario Storico
----------------

Il Sistema di Cooperazione (SPCoop) costituisce il modello concettuale ed
architetturale della cooperazione applicativa tra differenti Amministrazioni
e/o soggetti pubblici italiani. Tale sistema è organizzato in modo che: 

- supporti una modalità di erogazione del servizio articolata per adempimenti e
  procedimenti che derivano da dettati normativi o da compiti istituzionali; 
- sia paritetico fra tutti i soggetti cooperanti; 
- sia indipendente dagli assetti organizzativi dei soggetti cooperanti; 
- ciascun soggetto cooperante abbia la responsabilità dei servizi erogati e dei
  dati forniti; 
- ciascun soggetto sia autonomo nella gestione dei propri sistemi e nella
  definizione ed attuazione delle politiche di sicurezza del proprio sistema
  informativo; 
- ciascun soggetto sia responsabile delle autorizzazioni per l’accesso ai
  propri dati e/o servizi. 

Le tematiche coperte da SPCoop sono tutte quelle che interessano in ogni
aspetto l'interoperabilità dei sistemi ad ogni livello di astrazione:

- interoperabilità applicativa;
- catalogazione dei servizi;
- semantica dei dati e dei servizi;
- identità digitale.

Lo scenario storico di SPCoop è quello derivante dal `DPCM 1 aprile 2008`_,
recante regole tecniche e di sicurezza di SPC, compiutamente delineato sul
piano tecnico-implementativo da una suite di linee guida di seguito richiamate,
che prevedono l’utilizzo di consolidati standard che in questo periodo hanno
subito un consistente aggiornamento. 

.. _`DPCM 1 aprile 2008`: 
   http://www.gazzettaufficiale.it/eli/id/2008/06/21/08A04425/sg
 
Inquadramento generale delle specifiche SPCoop

  * `Termini di utilizzo documenti SPCoop`_
  * `Glossario generale e termini significativi d'uso comune`_

Interoperabilità applicativa

  * `Specifiche della Busta di e-gov`_
  * `Specifiche della Porta di dominio`_
  * `Linee guida busta di e-gov`_
  * `Qualificazione della Porta di dominio`_
  * `Qualificazione Porta di dominio con concorso delle regioni`_

Catalogazione dei servizi

  * `Specifiche dell'Accordo di servizio`_
  * `Specifiche del Registro SICA`_
  * `Raccomandazioni stesura Accordi di servizio`_
 
Semantica dei dati e dei servizi

  * `Nomenclatura e semantica`_
 
Identità digitale

  * `GFID - Gestione federata delle Identità digitali`_

.. _`Termini di utilizzo documenti SPCoop`: 
   http://www.agid.gov.it/sites/default/files/documentazione/licenza_duso_documenti_spcoop_v.2.0.pdf
.. _`Glossario generale e termini significativi d'uso comune`:
   http://www.agid.gov.it/sites/default/files/documentazione/spcoop-terminidefinizioni_v1.1.pdf
.. _`Specifiche della Busta di e-gov`:
   http://www.agid.gov.it/sites/default/files/documentazione/spcoop-busta-e-gov_v1.2_0.pdf
.. _`Specifiche della Porta di dominio`:
   http://www.agid.gov.it/sites/default/files/documentazione/spcoop-portadominio_v1.1_0.pdf
.. _`Linee guida busta di e-gov`:
   http://www.agid.gov.it/sites/default/files/documentazione/lineeguidabusta-e-gov_v1.1.pdf
.. _`Qualificazione della Porta di dominio`:
   http://www.agid.gov.it/sites/default/files/documentazione/spcoop-qualificazione_della_porta_di_dominio_in_modalita_provvisoria_v1.0.pdf
.. _`Qualificazione Porta di dominio con concorso delle regioni`:
   http://www.agid.gov.it/sites/default/files/documentazione/spcoop-aggiornamento_qualificazioneportadominioentiregionali_v1.0.pdf
.. _`Specifiche dell'Accordo di servizio`:
   http://www.agid.gov.it/sites/default/files/documentazione/spcoop-accordoservizio_v1.1_0.pdf
.. _`Specifiche del Registro SICA`:
   http://www.agid.gov.it/sites/default/files/documentazione/spcoop-serviziregistro_v1.1_0.pdf
.. _`Raccomandazioni stesura Accordi di servizio`:
   http://www.agid.gov.it/sites/default/files/documentazione/raccomandazionistesuraaccordidiservizio.pdf
.. _`Nomenclatura e semantica`:
   http://www.agid.gov.it/sites/default/files/documentazione/spcoop-nomenclaturasemantica_v1.1_0.pdf
.. _`GFID - Gestione federata delle Identità digitali`:
   http://www.agid.gov.it/sites/default/files/documentazione/spcoop-modellogfid_v1.5.1.pdf

Il nuovo Modello intende fornire indicazioni relativamente ad alcune modifiche
normative e tecniche intervenute in materia:

- le recenti modifiche del `CAD`_ con l’abrogazione dell’articolo 58, che permette
  di superare la necessità di convenzioni per lo scambio di informazioni punto
  a punto;
- la crescente necessità di interazione tra i diversi sistemi della Pubblica
  Amministrazione e tre piattaforme pubbliche e private che richiede servizi
  progettati nativamente interoperabili con API;
- l'evoluzione tecnologica con l'affermazione di nuovi standard de-facto e di
  più sofisticati paradigmi nella gestione e nell'automazione del ciclo di vita
  delle API;
- il lancio di SPID quale sistema nazionale per l'identificazione degli utenti;
- l'introduzione dello `European Interoperability Framework`_ (EIF) versione
  2.0, pubblicato nel 2010 nell’ambito del programma `Interoperability
  solutions for public administrations, businesses and citizens`_ (ISA, dal
  2016 ISA²).

.. _`CAD`: 
   http://www.agid.gov.it/cad/codice-amministrazione-digitale
.. _`European Interoperability Framework`: 
   https://joinup.ec.europa.eu/sites/default/files/5e/db/a3/isa_annex_ii_eif_en.pdf
.. _`Interoperability solutions for public administrations, businesses and citizens`: 
   https://ec.europa.eu/isa2/isa2_en

Si descrive di seguito, per tematiche, le linee evolutive dello scenario
attuale e futuro del modello SPCoop.

Identità digitali
-----------------    

Il tema della gestione delle identità digitali è originariamente fondato su
domini federati realizzati secondo il modello GFID ma è stato evoluto a seguito
dell’entrata in vigore dell’art. 64 comma 2-bis (e seguenti) del Codice
dell'amministrazione digitale. La nuova impostazione, precisata nel `DPCM 24
ottobre 2014`_, prevede un unico dominio di federazione in ambito nazionale,
denominato SPID, che rappresenta l’infrastruttura unica di identità digitale
finalizzata all’erogazione dei servizi on-line.   Nel Piano Triennale questa
infrastruttura Immateriale è stata inquadrata tra le `Piattaforme Abilitanti`_
descritte al capitolo 4.2.

.. _`DPCM 24 ottobre 2014`: 
   http://www.gazzettaufficiale.it/eli/id/2014/12/09/14A09376/sg
.. _`Piattaforme Abilitanti`: 
   https://pianotriennale-ict.readthedocs.io/it/latest/doc/04_infrastrutture-immateriali.html#piattaforme-abilitanti

Le regole tecniche relative alla Gestione federata delle Identità digitali
(GFID) sono quindi non più efficaci.

Maggiori informazioni alle pagine 

- `SPID`_
- Piano Triennale capitolo `Infrastrutture Immateriali`_

.. _`SPID`: 
   http://www.agid.gov.it/agenda-digitale/infrastrutture-architetture/spid
.. _`Infrastrutture Immateriali`:
   https://pianotriennale-ict.readthedocs.io/it/latest/doc/04_infrastrutture-immateriali.html

Classificazione e semantica dei servizi
---------------------------------------

Nel contesto delle attività relative all’implementazione del Catalogo dei
servizi della PA è stata elaborata una classificazione dei servizi delle PA
particolarmente focalizzata alle amministrazioni comunali e regionali e
definita una semantica comune per i servizi allo scopo di eliminare o attenuare
le attuali disomogeneità riscontrate. I servizi individuati, sono messi in
corrispondenza con il sistema di classificazione delle attività economiche
nella Comunità europea (NACE Nomenclature statistique des activités économiques
dans la Communauté européenne – rev. 2 – `Regolamento CE n. 1893/2006`_), a sua
volta in relazione con i 13 Data Themes definiti per la classificazione dei
dataset nel contesto della revisione del profilo europeo (`DCAT-AP`_) per la
descrizione dei dati. 

Maggiori informazioni alle pagine 

- `Catalogo dei servizi della PA`_
- Piano Triennale capitolo `Dati della Pubblica Amministrazione`_

.. _`DCAT-AP`: 
   https://joinup.ec.europa.eu/asset/dcat_application_profile/description
.. _`Regolamento CE n. 1893/2006`:
   http://eur-lex.europa.eu/legal-content/IT/TXT/?uri=LEGISSUM:24030103_2
.. _`Dati della Pubblica Amministrazione`:
   https://pianotriennale-ict.readthedocs.io/it/latest/doc/04_infrastrutture-immateriali.html#dati-della-pubblica-amministrazione
.. _`Catalogo dei servizi della PA`:
   http://www.dati.gov.it/content/catalogo-dei-servizi-pa-primi-passi

Semantica dei dati
------------------

In relazione a quanto previsto dall’articolo 9 `decreto legislativo n. 36/2006`_
in materia di riutilizzo dell’informazione del settore pubblico, riguardante le
modalità di ricerca dei documenti disponibili, è stato definito uno specifico
profilo nazionale di metadati (`DCAT-AP_IT`_) per la descrizione dei dati della
P.A., in conformità alle regole e agli standard di interoperabilità definiti a
livello internazionale. Detto profilo di metadati fa riferimento alla relativa
ontologia. 

Maggiori informazioni alla pagina:  

- Piano Triennale capitolo `Dati della Pubblica Amministrazione`_

.. _`decreto legislativo n. 36/2006`:
   http://www.gazzettaufficiale.it/eli/id/2006/02/14/006G0046/sg
.. _`DCAT-AP_IT`: 
   http://www.dati.gov.it/content/dcat-ap-it-v10-profilo-italiano-dcat-ap-0
.. _`Dati della Pubblica Amministrazione`:
   https://pianotriennale-ict.readthedocs.io/it/latest/doc/04_infrastrutture-immateriali.html#dati-della-pubblica-amministrazione

