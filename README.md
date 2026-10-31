# BASILICO-BB-BBC

**BASato sull'Italiano LInguaggio COnvertito, derivato dal BBC BASIC per BBC Micro**

BASILICO-BB è un adattamento del celebre linguaggio **BBC BASIC** per Commodore 64, caratterizzato dalla localizzazione dei comandi in lingua italiana. Allo stato attuale, le parole chiave e le istruzioni del BASIC sono state interamente tradotte, mentre i messaggi di errore rimangono in fase di completamento.

---

## Compatibilità e interscambiabilità dei sorgenti

Grazie alla struttura interna ereditata dal BBC BASIC, le istruzioni del linguaggio non vengono salvate come testo in chiaro, ma sotto forma di **token numerici**. Questo garantisce la piena compatibilità bidirezionale tra i programmi:

- **Da BBC BASIC a BASILICO**: Un programma salvato in BBC BASIC (nella versione C64 sviluppata da J.G. Harston) può essere caricato in BASILICO. Le parole chiave verranno automaticamente mostrate e interpretate con i corrispettivi comandi in italiano.
- **Da BASILICO a BBC BASIC**: Un programma salvato in BASILICO, una volta riaperto nell'ambiente BBC BASIC originale, mostrerà ed eseguirà i comandi nella loro forma inglese standard.

### Note e avvertenze sulle variabili
Sebbene la struttura del codice rimanga perfettamente compatibile, occorre prestare attenzione ai **nomi delle variabili**:
1. Poiché BASILICO utilizza parole chiave in italiano, un nome di variabile valido in BBC BASIC inglese potrebbe coincidere con una nuova istruzione riservata in BASILICO (e viceversa), generando conflitti di sintassi.
2. È sempre consigliabile scegliere nomi di variabili neutri o verificare che non coincidano con le parole chiave tokenizzate della versione di destinazione.

---

## Requisiti e utilizzo

Per eseguire **BASILICO-BB** su un emulatore di BBC Micro (es. BeebEM):

1. Scaricare il file basilico.rom
2. Impostare come ROM del BASIC il summenzionato file nell'emulatore di BBC Micro
3. Resessare l'emulatore

---

## Assemblatore integrato

L'assemblatore integrato funziona, ma ci sono anomalie. Ad esempio, l'istruzione ORA del 6502 nell'assemblatore del BASILICO è diventata OA, usando il token OR del BBC BASIC. Si è preferito privilegiare la corretta traduzione in italiano - O - del comando OR piuttosto che lasciare intatta l'istruzione ORA dell'Assembly.

---

## Proprietà intellettuale e note sui diritti

Questo progetto è una modifica di un'opera preesistente e non rivendica la titolarità del codice sorgente o del binario originale. La proprietà intellettuale è così suddivisa:

- **BBC BASIC (Core & Implementazione 6502)**: Tutti i diritti relativi al codice originale appartengono a **Acorn Computers Ltd.** (e ai suoi aventi causa).
- **Localizzazione in Italiano**: La traduzione dei token, l'adattamento della sintassi italiana e la conseguente riallocazione dei byte sono a cura dell'autore di questo repository.

Il codice sorgente originale e i file derivati rimangono soggetti alle rispettive note di copyright dei detentori dei diritti (**Acorn Computers** e suoi aventi causa).

---

## Crediti

Un ringraziamento speciale a **Sophie Wilson** unitamente a **Acorn Computers** per la creazione del linguaggio originale.
