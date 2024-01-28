# Step-by-step Github tutorial &nbsp;&nbsp;&nbsp;
> comandi base - per adesso

[![Hits](https://hits.sh/github.com/wassupiari/github-tutorial.svg?label=views&color=313131&logo=Github)](https://hits.sh/github.com/wassupiari/github-tutorial/)

## Installazione di git su win
Vai su questo sito per [scaricarlo](https://git-scm.com/download/win).
Una volta scaricato, non devi fare altro che accettare i termini di installazione.
Una volta finito avrai git installato sul tuo pc e pronto ad essere usato da terminale.

#### Verifica installazione
Per vedere se l'installazione sia andata a buon fine devi aprire il tuo terminale(cmd) e digitare:

```
    git -v
```

Ti dovrebbe uscire la versione di git installata:

```
    git version x.xx.x.windows.1
```


## Configurazione Git

Prima di inziare dobbiamo configurare git per farci usare lo stesso username/email per tutte le repo su cui andremmo a lavorare

``` 
    git config --global user.name "username-su-github"
    git config --global user.email "email-su-github"
```

## Iniziamo

Una volta fatto i passi precedentemente elencati, iniziamo dirigendoci alla cartella su cui stiamo attualmente lavorando
### Init
Il primo passo adesso sarà quello di creare oppure di inizializzare una repository vuota, usando:

```
    git init 
```

è un comando monouso che usi durante la configurazione iniziale di un nuovo repository. L'esecuzione di questo comando creerà una nuova sottodirectory `.git` nella tua attuale directory di lavoro
### Add
Adesso per salvare i progressi che hai fatto nel tuo workspace usiamo il comando:

```
    git add <opzione>
```

Ecco le principali opzioni:

| Opzione     | Descrizione |
|  :----------------  |  :-------------|
| `git add <filename>`     | Andiamo a salvare/caricare un file specifico       |
| `git add <filename><filename1><filename2>`  | Andiamo a salvare/caricare più file specifici alla volta      |
| `git add .`      | Andiamo a salvare/caricare tutti i file presenti nella cartella       |
| `git add --all`      | Andiamo a salvare/caricare tutti i file presenti nella cartella      |
| `git add -A`      | Andiamo a salvare/caricare tutti i file presenti nella cartella      |

L'opzione più usata:
```
    git add .
```
### Commit
Una volta salvato i progressi dobbiamo commentare le modifiche che abbiamo fatto in quella sessione di lavoro oppure per ogni file specifico, lo facciamo usando:

```
    git commit <opzione> 
```

Ecco le principali opzioni:
| Opzione     | Descrizione |
|  :----------------  |  :-------------|
| `git commit -a`     | Esegui il commit di un'istantanea di tutte le modifiche nella directory di lavoro       |
| `git commit -m "commit message"`  | Un comando di scelta rapida che crea immediatamente un commit con un messaggio di commit passato      |
| `git commit --amend`      | Questa opzione aggiunge un altro livello di funzionalità al comando commit. Il passaggio di questa opzione modificherà l'ultimo commit. Invece di creare un nuovo commit, le modifiche in staging verranno aggiunte al commit precedente.       |

L'opzione più usata:
```
    git commit -m "commit message"
```

### Remote

Il comando `git remote` ti consente di creare, visualizzare ed eliminare connessioni ad altri repository.

```
git remote <opzione1> <opzione2> 
```

Ecco le principali opzioni:
| Opzione     | Descrizione |
|  :----------------  |  :-------------|
| `git remote add <name> <url>`     |  Crea una nuova connessione a un repository remoto      |
| `git remote rm <name>`  | Rimuovi la connessione al repository remoto denominata      |
| `git remote rename <old-name> <new-name>`      | Rinomina una connessione remota da x a y.      |

L'opzione più usata:
```
    git remote add origin <linkallatuarepo>
```


### Push






### Branch



### Esempio pratico
> Creare un nuovo repository git per un codebase esistente e fare il push su github
```
    cd /path/to/code 
    git init 
    git add . 
    git commit -m "first commit"
    git branch -m main
    git remote add origin <linkdellarepo>
    git push -u origin main
```


### Riferimenti
 Qui troverete dove ho fatto riferimento per creare questa guida.

[Atlassian.com](https://www.atlassian.com/it/git/tutorials/setting-up-a-repository)

[Nick White: Git Tutorial For Dummies](https://www.youtube.com/watch?v=mJ-qvsxPHpY)

### License

[MIT](/LICENSE) © jarek  












