```table-of-contents
```
---

> Possibile titolo: *"Sicurezza negli smart contract cross-chain: sfide e possibili soluzioni"*.

# Symposium
Obiettivo di questo seminario:
- Capire le basi della tecnologia blockchain e la sua rilevanza nella decentralized finance (DeFi).
- Studiare le vulnerabilità più comuni nello sviluppo di smart contract.
- Scoprire come l'analisi statica insieme ad altre tecniche può aiutare ad identificare potenziali vulnerabilità e mitigare rischi sugli smart contract cross-chain (aka bridge).

# Introduzione
Prima di immergerci nel mondo degli smart contract cross-chain, facciamo un passo indietro ed esploriamo in cosa consiste la tecnologia blockchain.

In parole povere, una blockchain è un registro digitale decentralizzato che registra le transazioni su una rete di computer. La kill-feature della blockchain risiede nella sua natura trasparente e a prova di manomissione, che consente transazioni peer-to-peer sicure senza la necessità di intermediari come banche o governi.

Ma ecco il punto: non tutte le blockchain sono create uguali. Infatti, ci sono molte diverse piattaforme blockchain, ognuna con le proprie caratteristiche e casi d'uso unici. Ad esempio, Ethereum è una popolare piattaforma blockchain che consente agli sviluppatori di distribuire smart contract, programmi che si eseguono in modo autonomo quando si verifica una determinata condizione.

Poiché questi contratti sono archiviati su una blockchain, sono anche immutabili, il che significa che una volta distribuiti, non possono essere modificati o eliminati.

Ora, questa immutabilità è sia un vantaggio che uno svantaggio. Da un lato, significa che i contratti intelligenti possono fornire un elevato livello di fiducia e garanzia per le parti coinvolte in una transazione. Ma dall'altro lato, significa anche che eventuali errori o bug in questi contratti possono avere conseguenze di vasta portata: dopotutto, se un contratto intelligente contiene un errore logico, potrebbe potenzialmente portare a significative perdite finanziarie o danni alla reputazione.

Ecco perché la sicurezza è un aspetto così critico nello sviluppo di contratti intelligenti. Quando si distribuisce un contratto intelligente su una blockchain come Ethereum, gli sviluppatori devono essere assolutamente certi che il loro codice sia privo di errori e bug, altrimenti le conseguenze potrebbero essere gravi.

Una delle sfide significative nel lavorare con più reti blockchain è l'incapacità di trasferire in modo nativo asset tra di loro. Se hai un asset, come Ether (ETH) su Ethereum, non puoi semplicemente spostarlo ad un'altra blockchain, come la rete di Solana. Questo perché ogni blockchain ha la propria tecnologia e infrastruttura sottostante unica, rendendo impossibile il trasferimento diretto.

Per risolvere questo problema, sono stati introdotti gli smart contract cross-chain, detti anche *bridge*, noti come soluzione di interoperabilità, per facilitare il movimento di asset tra blockchain. I bridge fungono da intermediario, consentendo agli utenti di convertire i propri asset in un formato standardizzato che può essere trasferito su diverse reti blockchain.

Questa soluzione offre nuove grandi possibilità, ma anche grandi responsabilità, in quanto la posta in gioco è più alta che mai. 

In questo seminario esploreremo le sfide e le opportunità che circondano questi sistemi complessi e discuteremo di come l'analisi statica e altre tecniche possano contribuire a garantirne l'integrità e l'affidabilità.

# Sezione 1: Funzionamento dei bridge
Come accennato poco fa, una delle sfide più significative nel lavorare con più reti blockchain è l'incapacità di interagire senza problemi tra di esse. Questo problema nasce dal fatto che diverse piattaforme blockchain hanno i propri protocolli, architetture e linguaggi di programmazione unici. Di conseguenza, costruire ponti tra queste reti è fondamentale per facilitare il flusso di dati, asset o smart contract.

## Lock and Mint bridge
I bridge *lock and mint* sono un tipo specifico di bridge che facilita il trasferimento di asset tra diverse blockchain. Come suggerisce il nome, questi bridge prima bloccano (*"lock"*) l'asset originale in un contratto *"relayer"* designato sulla prima chain e poi coniano (*"mint"*) una copia dell'asset sulla seconda catena. Questo processo assicura che l'asset originale rimanga protetto mentre viene creata una replica sulla chain di destinazione, consentendo agli utenti di utilizzare la funzionalità dell'asset all'interno dell'ecosistema della seconda chain.

![[bridge.png]]

Per abilitare questa funzionalità dei bridge lock and mint, la comunicazione back-end svolge un ruolo fondamentale. Comporta il tracciamento degli eventi emessi dalla prima chain e l'esecuzione delle funzioni corrispondenti sui contratti distribuiti sulla seconda chain. Questa comunicazione assicura la sincronizzazione e la coerenza tra le due chain, consentendo il trasferimento senza interruzioni degli asset.

Quindi ricapitolando, un bridge cross-chain può essere diviso in tre parti: source chain, cross-chain relayer e destination chain. Inoltre, il bridge cross-chain "deploya" gli smart contract sulla source chain e sulla destination chain.

# Sezione 2: vulnerabilità cross-chain
> Parlare delle vulnerabilità descritte da SmartAxe

# Sezione 3: SmartAxe - un primo case study

# Conclusioni