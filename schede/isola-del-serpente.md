---
title: Isola del Serpente
parent: Schede attività
nav_order: 6
permalink: /schede/isola-del-serpente/
render_with_liquid: false
---

# Isola del Serpente – Schede attività
{: .no_toc }

**Python + Raspberry Pi Pico · dagli 11 anni · 4 schede: Mozzo, Marinaio, Nostromo, Capitano**

Code Club Sulmona · [Guida del mentor](../../guida-mentor/), allegato alla sezione 8 · info@sulmonalug.it

---

<details open markdown="block">
<summary>In questa pagina</summary>
{: .text-delta }
1. TOC
{:toc}
</details>

## Prima di tutto: l'isola pronta

| Cosa | Dettaglio |
|---|---|
| **Software** | Thonny installato su ogni PC. In basso a destra si sceglie l'interprete: "Python locale" per la scheda 1, "MicroPython (Raspberry Pi Pico)" per le altre |
| **Pico** | Un Pico per bambino. Chi arriva dai Lampi usa un Pico del club con i pin già saldati; chi arriva dal Vulcano usa il proprio |
| **Firmware** | MicroPython già installato su ogni Pico (Thonny lo installa la prima volta: "Strumenti", "Opzioni", "Interprete") |
| **Kit per postazione** | Breadboard, 3 LED (rosso, giallo, verde), 3 resistenze da 220 Ω, 2 pulsanti, una fotoresistenza con una resistenza da 10 kΩ, cavetti maschio-maschio |
| **Cavo** | Micro-USB **dati**, non solo ricarica |

### Le regole del banco elettronico

> 1. Si collega e si scollega sempre con il Pico **staccato** dal PC.
> 2. Ogni LED ha la sua resistenza.
> 3. Mai collegare direttamente 3,3 V a GND.
> 4. Se qualcosa scotta o puzza: si stacca il cavo e si chiama il mentor.

### La breadboard in un minuto

Le file di fori sono collegate tra loro a gruppi di 5, in verticale; le due righe lunghe ai lati sono collegate in orizzontale e servono per l'alimentazione. Il Pico si mette a cavallo della scanalatura centrale.

---

## Scheda 1 – Mozzo: il serpente parla

| Carta d'identità | |
|---|---|
| **Grado** | Mozzo (prova) |
| **Età** | Dagli 11 anni |
| **Partecipanti** | Fino a 10 |
| **Mentor** | 1 ogni 5 ragazzi |
| **Prerequisiti** | Ponte dorato: grado Marinaio ai Lampi o Capitano al Vulcano |

**Obiettivo:** il ragazzo scrive le prime righe di codice in testo e scopre che il computer è pignolo: maiuscole, virgolette e rientri contano.

### Prima di iniziare

- [ ] Thonny aperto con l'interprete "Python locale" (questa scheda si fa sul PC, senza Pico)
- [ ] Il cartellone dei 4 errori più comuni: virgolette dimenticate, parentesi non chiusa, rientro mancante, maiuscole

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **Dai blocchi al testo** | Il mentor mostra un programma MakeCode in blocchi e poi nella vista Python: "È la stessa cosa, scritta in un'altra lingua" |
| 10–20' | **Thonny** | L'editor in alto, la shell in basso, il pulsante verde per eseguire |
| 20–40' | **Attività 1: domanda e risposta** | |
| 40–45' | **Pausa** | |
| 45–75' | **Attività 2: indovina il numero** | |
| 75–85' | **Sfida in coppia** | Ognuno prova il gioco del compagno |
| 85–90' | **Timbri** | |

### Passo passo

> **Attività 1 – Domanda e risposta**
> ```python
> nome = input("Come ti chiami? ")
> print("Ciao", nome, "benvenuto sull'Isola del Serpente!")
> eta = input("Quanti anni hai? ")
> print("Tra dieci anni ne avrai", int(eta) + 10)
> ```
> 1. Scrivi il programma, salvalo nella tua cartella e premi il pulsante verde.
> 2. Rispondi nella shell in basso.
> 3. Aggiungi una terza domanda, tutta tua.
>
> **Attività 2 – Indovina il numero**
> ```python
> import random
>
> segreto = random.randint(1, 10)
> tentativo = int(input("Ho pensato un numero da 1 a 10. Quale? "))
>
> if tentativo == segreto:
>     print("Esatto! Sei un vero esploratore.")
> else:
>     print("No, era", segreto)
> ```
> 1. Prova più volte: il numero cambia?
> 2. Sfida: dì al giocatore se il numero segreto è più alto o più basso, usando `elif`.

### Domande guida

| Situazione | Chiedi |
|---|---|
| Errore rosso nella shell | "Leggi l'ultima riga dell'errore: quale riga indica?" |
| `int(eta) + 10` non funziona | "Per il computer, '12' scritto tra virgolette è un numero o una parola?" |
| `if` non funziona | "Cosa c'è alla fine della riga dell'if? E all'inizio della riga sotto?" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| `SyntaxError` | Virgolette o parentesi non chiuse | Thonny colora il testo: dove cambia colore in modo strano? |
| `IndentationError` | Manca il rientro dopo `if` o `else` | Il rientro è "dentro": mostrarlo con le mani |
| `NameError` | Una variabile scritta in modo diverso (Nome e nome) | Il computer distingue maiuscole e minuscole |
| Il confronto non funziona | `=` al posto di `==` | "Un uguale dà un valore, due uguali fanno una domanda" |

### Differenziare

| Per chi va veloce | Per chi è in difficoltà |
|---|---|
| Indovina il numero con 3 tentativi, usando un ciclo `for` | Solo l'attività 1, con il codice stampato da ricopiare e poi modificare |
| Un quiz con il punteggio | Lavorare in coppia: uno detta, l'altro scrive |

### Timbro Mozzo

Il programma "indovina il numero" funziona, e il ragazzo ha corretto da solo almeno un errore. Domanda di verifica: "Me lo mostri funzionare?"

### In un club misto

Nei 70 minuti: 10' dai blocchi al testo, 20' attività 1, 30' attività 2, 10' timbri. Un Marinaio del Serpente può fare da "dizionario degli errori" per i nuovi.

---

## Scheda 2 – Marinaio: la prima luce

| Carta d'identità | |
|---|---|
| **Grado** | Marinaio (fa) |
| **Età** | Dagli 11 anni |
| **Partecipanti** | Fino a 10 |
| **Mentor** | 1 ogni 5 ragazzi |
| **Prerequisiti** | Grado Mozzo al Serpente |

**Obiettivo:** il ragazzo programma il Pico e accende un LED esterno collegato correttamente sulla breadboard.

### Prima di iniziare

- [ ] Thonny con l'interprete "MicroPython (Raspberry Pi Pico)"
- [ ] Pico già inseriti nella breadboard
- [ ] Le regole del banco elettronico sul cartellone

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **Le regole del banco** | Lettura delle quattro regole |
| 10–20' | **Conosciamo il Pico** | I pin, GND, 3,3 V; il mentor mostra la mappa dei pin |
| 20–35' | **Attività 1: il LED che lampeggia** | Il LED già montato sul Pico |
| 35–40' | **Pausa** | |
| 40–70' | **Attività 2: il LED esterno** | Breadboard, resistenza, LED |
| 70–80' | **Il segnale luminoso** | Ognuno cambia ritmo al suo LED: si inventa un codice di lampi |
| 80–90' | **Timbri e riordino** | Componenti nel kit, contati |

### Passo passo

> **Attività 1 – Il LED che lampeggia**
> ```python
> from machine import Pin
> import time
>
> led = Pin("LED", Pin.OUT)   # su firmware vecchi: Pin(25, Pin.OUT)
>
> while True:
>     led.toggle()
>     time.sleep(0.5)
> ```
> 1. Collega il Pico, scrivi il programma, premi il pulsante verde.
> 2. Il LED sul Pico lampeggia.
> 3. Cambia `0.5` con `0.1`, poi con `2`. Cosa succede?
> 4. Per fermare il programma: pulsante rosso "Stop".
>
> **Attività 2 – Il LED esterno**
> 1. **Stacca il Pico dal PC.**
> 2. Infila il LED nella breadboard. La gamba lunga è il **+**.
> 3. Collega con un cavetto il pin **GP15** alla gamba lunga.
> 4. Collega la gamba corta a una resistenza da 220 Ω, e la resistenza a un pin **GND**.
> 5. Fai controllare il circuito al mentor, poi ricollega il Pico.
> 6. Nel programma cambia `Pin("LED", Pin.OUT)` in `Pin(15, Pin.OUT)`.

### Domande guida

| Situazione | Chiedi |
|---|---|
| Il LED esterno non si accende | "Da quale parte è la gamba lunga? Dove va?" |
| Il programma va ma il LED no | "Il numero del pin nel programma è lo stesso del cavetto?" |
| Thonny non vede il Pico | "Quale interprete è scelto in basso a destra?" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| LED spento | Montato al contrario | Girarlo: non si rompe |
| LED spento | Cavetti nella stessa fila sbagliata della breadboard | Ripassare come sono collegati i fori |
| "Dispositivo non trovato" | Cavo solo ricarica, o interprete sbagliato | Cambiare cavo, controllare l'interprete |
| Il programma parte ma poi si blocca | È stato premuto Stop o il Pico è stato staccato | Ricollegare e ripremere il pulsante verde |

### Differenziare

| Per chi va veloce | Per chi è in difficoltà |
|---|---|
| Due LED che lampeggiano alternati | Solo l'attività 1, con il mentor che monta il circuito insieme a lui |
| Il proprio nome in codice Morse | Lavorare in coppia: uno monta, l'altro programma, poi si scambiano |

### Timbro Marinaio

Il LED esterno lampeggia, montato dal ragazzo, e il ragazzo cambia la velocità da solo. Domanda di verifica: "Se giro il LED, cosa succede? Perché?"

### In un club misto

Nei 70 minuti: 10' regole e Pico, 15' LED integrato, 35' LED esterno, 10' timbri. Il grado Marinaio al Serpente apre il ponte dorato verso il Faro delle Stelle.

---

## Scheda 3 – Nostromo: il dispositivo

| Carta d'identità | |
|---|---|
| **Grado** | Nostromo (inventa) |
| **Età** | Dai 12 anni |
| **Partecipanti** | Fino a 8 |
| **Mentor** | 1 ogni 4 ragazzi |
| **Prerequisiti** | Grado Marinaio al Serpente |

**Obiettivo:** il ragazzo costruisce un dispositivo con almeno un **ingresso** (pulsante o sensore) e un'idea sua.

### Prima di iniziare

- [ ] La carta del progetto (Isola dei Gatti, scheda 3), con le domande in più: "Cosa sente il mio dispositivo? Cosa fa quando lo sente?"
- [ ] Uno schema di collegamento stampato per ogni ricetta

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **Ingressi e uscite** | "Finora il Pico parlava. Oggi impara ad ascoltare" |
| 10–20' | **Il pulsante** | Tutti montano un pulsante (prima ricetta, punto 1) |
| 20–30' | **La carta del progetto** | |
| 30–70' | **Costruzione** | Con le ricette |
| 70–80' | **Collaudo** | Un compagno prova il dispositivo |
| 80–90' | **Presentazione e timbri** | |

### Le ricette

> **Il pulsante che accende**
> 1. Pulsante a cavallo della scanalatura: un piedino a **GP14**, l'altro a **3,3 V**.
> ```python
> from machine import Pin
> import time
>
> pulsante = Pin(14, Pin.IN, Pin.PULL_DOWN)
> led = Pin(15, Pin.OUT)
>
> while True:
>     led.value(pulsante.value())
>     time.sleep(0.01)
> ```
>
> **Il semaforo con chiamata pedonale**
> 1. Tre LED su GP13 (verde), GP14 (giallo), GP15 (rosso), ognuno con la sua resistenza; il pulsante su un altro pin, per esempio GP16.
> 2. Il semaforo è verde; quando si preme il pulsante passa a giallo, poi rosso per 5 secondi, poi torna verde.
>
> **Il gioco dei riflessi**
> 1. LED e pulsante.
> 2. Il LED si accende dopo un tempo casuale (`random.uniform(2, 5)`).
> 3. Si misura quanto tempo passa prima che il pulsante venga premuto, con `time.ticks_ms()`, e si stampa il risultato.
> 4. Record della giornata alla lavagna.
>
> **La lampada notturna**
> 1. Fotoresistenza in serie con una resistenza da 10 kΩ, tra 3,3 V e GND; il punto in mezzo va a **GP26**.
> 2. `luce = ADC(26).read_u16()` (con `from machine import ADC`) legge un numero da 0 a 65535.
> 3. Sotto una certa soglia, il LED si accende. La soglia si trova provando, coprendo la fotoresistenza con la mano.

### Domande guida

| Situazione | Chiedi |
|---|---|
| Il pulsante non risponde | "Stampa `pulsante.value()` nella shell: cambia quando lo premi?" |
| Il semaforo va troppo veloce | "Dove il programma aspetta? Per quanto?" |
| Non trova la soglia della luce | "Stampa il valore e copri la fotoresistenza: quali numeri vedi?" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| Il pulsante sembra premuto da solo | Manca `Pin.PULL_DOWN`: il pin "galleggia" | Aggiungerlo, e spiegare perché serve |
| Il pulsante non fa nulla | Montato nella stessa fila, senza attraversare la scanalatura | Ruotarlo di 90° |
| I valori della luce saltano | Collegamenti incerti | Premere bene i cavetti nella breadboard |

### Differenziare

| Per chi va veloce | Per chi è in difficoltà |
|---|---|
| Combinare due ricette: il semaforo che si accende solo di notte | Il pulsante che accende, con un'idea propria: un ritmo, un messaggio Morse |
| Scrivere una funzione con `def` per ogni fase del semaforo | Lavorare in coppia sul gioco dei riflessi |

### Timbro Nostromo

Un dispositivo con almeno un ingresso e un'idea sua, montato dal ragazzo. Domanda di verifica: "Cosa hai aggiunto tu, che la ricetta non diceva?"

### In un club misto

I Nostromi del Serpente sono i candidati naturali per il Faro delle Stelle (Astro Pi Mission Zero) e per la Festa del Porto. Un dispositivo ben fatto si presenta benissimo a Coolest Projects.

---

## Scheda 4 – Capitano: insegnare a un compagno

| Carta d'identità | |
|---|---|
| **Grado** | Capitano (insegna) |
| **Età** | Dai 12 anni |
| **Partecipanti** | Coppie Capitano-compagno |
| **Mentor** | 1 che osserva fino a 3 coppie |
| **Prerequisiti** | Grado Nostromo al Serpente |

Valgono le **tre regole del Capitano** della scheda 4 dell'Isola dei Gatti: mani in tasca, prima chiedi poi spieghi, gli errori sono tesori. Al Serpente si aggiunge una quarta regola: **il Capitano controlla il circuito prima che il compagno colleghi il Pico**, ma non lo monta al posto suo.

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **Briefing dei Capitani** | Le quattro regole, e come leggere un messaggio di errore insieme al compagno |
| 10–65' | **Tutoraggio** | Le coppie lavorano con la scheda 1 o 2 |
| 65–75' | **Verifica del compagno** | Dal mentor, senza il Capitano accanto |
| 75–90' | **Debriefing e timbri** | "Quale errore del compagno ti ha insegnato qualcosa?" |

### Timbro Capitano

Il compagno conquista Mozzo o Marinaio al Serpente **e** il Capitano ha rispettato le quattro regole.

### In un club misto

I Capitani del Serpente sono i futuri mentor di Ri-Avvia: segnalateli al LUG quando arrivano alle superiori.

---

*Documento di lavoro – versione 0.1 – novembre 2026. Materiali rilasciati con licenza CC BY-SA 4.0.*
