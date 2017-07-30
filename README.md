# Piano di sviluppo DAF

Questo progetto contiene i sorgenti delle *Linee guida per transitare al nuovo Modello di interoperabilità*, primo risultato dell’azione “Linee guida del nuovo Modello di interoperabilità”, prevista nel [capitolo 5 del Piano Triennale per l’Informatica nella PA (2017-2019)](https://pianotriennale-ict.readthedocs.io/it/latest/doc/05_modello-di-interoperabilita.html).

È possibile consultare il documento all'indirizzo: 

[http://interop-linee-guida-transizione.readthedocs.io/it/latest/](http://interop-linee-guida-transizione.readthedocs.io/it/latest/)

È possibile scaricare i sorgenti, compilarli e sottomettere pull-request.

## Come eseguire la build 

Questi i passi per apportare modifiche/correzioni ai sorgenti ed eseguire la build:

1. Dopo aver effettuato una fork, modificare i sorgenti del Piano di sviluppo (e/o aggiungerne di nuovi) presenti nella cartella [rst](rst). 

2. Al fine di testare le modifiche apportate, eseguire lo script `rst2html.sh` (per eseguire lo script è necessario installare [Sphinx](http://www.sphinx-doc.org/en/stable/)). L'output dello script è memorizzato nella cartella [docs](docs). A partire dal file [index.html](docs/index.html) è possibile navigare in locale la versione compilata del sito e verificare la corretta visualizzazione dei contenuti.

3. Una volta verificata l'assenza di errori, effettuare commit sul proprio repository e formulare una pull request.
