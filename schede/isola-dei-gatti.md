---
title: Isola dei Gatti
parent: Schede attività
nav_order: 3
permalink: /schede/isola-dei-gatti/
render_with_liquid: false
---

# Isola dei Gatti – Schede attività
{: .no_toc }

**Scratch · dai 7 anni · 4 schede: Mozzo, Marinaio, Nostromo, Capitano**

Code Club Sulmona · [Guida del mentor](../../guida-mentor/), allegato alla sezione 5 · info@sulmonalug.it

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
| **Software** | Scratch, versione desktop, installato su ogni PC (funziona offline, senza account) |
| **Cartelle** | Una cartella per partecipante con il suo soprannome, sul desktop o su una chiavetta del club |
| **Cuffie** | Una per postazione: i suoni di Scratch in 12 PC insieme diventano un frastuono |
| **Proiettore o schermo grande** | Per le dimostrazioni. Se non c'è, il mentor mostra su un PC con i bambini intorno, a gruppi di 3–4 |
| **Lingua** | Scratch in italiano: icona del globo in alto a sinistra |
| **Stampe** | Le schede-passo per i bambini (le parti nei riquadri "Passo passo") e il registro dei timbri |

### Come leggere le schede

Ogni scheda descrive un **laboratorio di 90 minuti**, adatto a un evento singolo (open day, laboratorio esterno). In una **sessione normale del club**, accoglienza e "mostra cosa hai fatto" sono comuni a tutto il club: all'isola restano **70 minuti** di lavoro. La sezione "In un club misto" di ogni scheda spiega come adattarla.

I blocchi di Scratch sono scritti `così`, con i nomi che compaiono in italiano. I valori tra parentesi si possono cambiare.

---

## Scheda 1 – Mozzo: il personaggio che si muove

| Carta d'identità | |
|---|---|
| **Grado** | Mozzo (prova) |
| **Età** | Dai 7 anni |
| **Partecipanti** | Fino a 12 |
| **Mentor** | 1 ogni 6 bambini; 2 se è la loro prima volta al computer |
| **Prerequisiti** | Nessuno |

**Obiettivo:** il bambino sa che un programma è una serie di ordini che il computer esegue quando succede qualcosa (un tasto premuto, la bandiera verde).

### Prima di iniziare

- [ ] Scratch aperto su ogni PC, progetto nuovo, lingua italiana
- [ ] Una cartella col soprannome di ogni bambino
- [ ] Cuffie collegate
- [ ] Lavagna o cartellone con le quattro frecce disegnate

### Scaletta

| Tempo | Momento | Cosa fa il mentor |
|---|---|---|
| 0–10' | **La storia** | "Sull'Isola dei Gatti gli abitanti si muovono solo se qualcuno scrive gli ordini giusti. Oggi impariamo a dare ordini." Gioco veloce: il mentor fa il robot e i bambini gli danno comandi ("fai 3 passi", "gira") |
| 10–20' | **Il giro dell'isola** | Mostra Scratch: lo **stage** (dove succede tutto), lo **sprite** (il personaggio), la **tavolozza dei blocchi**, l'**area del programma**. Trascina un blocco `fai (10) passi` e ci clicca sopra: il gatto si muove |
| 20–45' | **Attività 1: le frecce** | I bambini costruiscono il movimento nelle quattro direzioni (passo passo sotto) |
| 45–50' | **Pausa in piedi** | Tutti in piedi: il mentor dice "freccia su", "freccia destra" e i bambini si muovono come il loro sprite |
| 50–75' | **Attività 2: il dialogo** | Due personaggi si parlano (passo passo sotto) |
| 75–85' | **Mostra cosa hai fatto** | 3–4 bambini mostrano il dialogo al gruppo; timbri |
| 85–90' | **Salvataggio e riordino** | Ognuno salva nella sua cartella: "File", "Salva sul tuo computer" |

### Passo passo – Attività 1: le frecce

> 1. Clicca sul gatto per selezionarlo.
> 2. Dalla categoria **Situazioni** trascina `quando si preme il tasto (freccia destra)`.
> 3. Dalla categoria **Movimento** attacca sotto `cambia x di (10)`.
> 4. Prova: premi la freccia destra. Il gatto va a destra!
> 5. Fai la stessa cosa per la **freccia sinistra**, con `cambia x di (-10)`.
> 6. Per la **freccia su** usa `cambia y di (10)`, per la **freccia giù** `cambia y di (-10)`.
> 7. Sfida: fai camminare il gatto fino a ogni angolo dello stage.

### Passo passo – Attività 2: il dialogo

> 1. Clicca sull'icona del gatto in basso a destra e scegli un secondo personaggio.
> 2. Primo personaggio: `quando si clicca su (bandiera verde)` → `dire (Ciao! Chi sei?) per (2) secondi`.
> 3. Secondo personaggio: `quando si clicca su (bandiera verde)` → `attendi (2) secondi` → `dire (Sono il nuovo esploratore!) per (2) secondi`.
> 4. Continua il dialogo: ogni battuta, l'altro personaggio aspetta.
> 5. Scegli uno sfondo con l'icona in basso a destra dello stage.
> 6. Clicca sulla bandiera verde e guarda la scena.

### Domande guida

| Invece di… | Chiedi |
|---|---|
| Spostare il blocco al posto suo | "Quale categoria di blocchi fa muovere le cose?" |
| Dire "devi mettere il meno" | "Il gatto va a destra: come facciamo a farlo andare dall'altra parte?" |
| Correggere i tempi del dialogo | "Parlano tutti e due insieme. Cosa deve fare uno mentre l'altro parla?" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| Premo la freccia e non succede niente | Il blocco `cambia x` non è attaccato al cappello: sono separati | "Guarda bene: i due blocchi si toccano? Devono fare clic come i mattoncini" |
| Il gatto si muove anche con l'altro tasto | Nel menu del cappello è rimasto "spazio" o un'altra freccia | Aprire la tendina del blocco e controllare |
| Il programma è sul personaggio sbagliato | Il bambino ha scritto con lo sfondo o l'altro sprite selezionato | Mostrare quale sprite è evidenziato in basso a destra |
| I personaggi parlano sovrapposti | Manca `attendi` | Domanda guida qui sopra |

### Differenziare

| Per chi finisce prima | Per chi è in difficoltà |
|---|---|
| Aggiungere `passa al costume seguente` sotto ogni freccia: il gatto cammina muovendo le zampe | Fare solo due frecce, destra e sinistra, e un dialogo di 2 battute |
| Fare dire al gatto una frase quando tocca il bordo | Lavorare in coppia con un compagno che ha già finito |

### Timbro Mozzo

Il personaggio si muove in tutte e quattro le direzioni **e** il dialogo ha almeno 4 battute nell'ordine giusto. Domanda di verifica: "Me lo mostri funzionare?"

### In un club misto

Nei 70 minuti dell'isola: 5' di giro dell'isola, 25' frecce, 25' dialogo, 10' verifica e timbro, 5' salvataggio. Se all'isola ci sono già dei Marinai, uno di loro può fare il giro dell'isola ai nuovi: è un passo verso il grado di Capitano.

---

## Scheda 2 – Marinaio: Acchiappa la mela

| Carta d'identità | |
|---|---|
| **Grado** | Marinaio (fa) |
| **Età** | Dai 7–8 anni |
| **Partecipanti** | Fino a 12 |
| **Mentor** | 1 ogni 6 bambini |
| **Prerequisiti** | Grado Mozzo ai Gatti |

**Obiettivo:** il bambino costruisce da solo un gioco completo, usando un ciclo (`per sempre`), una condizione (`se … allora`), un numero casuale e una variabile.

### Prima di iniziare

- [ ] Scratch aperto con un progetto nuovo
- [ ] Il gioco finito già pronto sul PC del mentor, per mostrarlo all'inizio
- [ ] Le 4 tappe stampate su un cartoncino per ogni postazione

### Scaletta

| Tempo | Momento | Cosa fa il mentor |
|---|---|---|
| 0–10' | **La sfida** | Mostra il gioco finito e lo fa provare a due volontari. "Alla fine di oggi questo gioco l'avrete costruito voi" |
| 10–15' | **Il piano** | Alla lavagna, insieme: cosa deve fare il cesto? E la mela? Quando si vince un punto? Ne escono le 4 tappe |
| 15–30' | **Tappa 1: il cesto** | Il cesto si muove a destra e a sinistra |
| 30–45' | **Tappa 2: la mela che cade** | La mela parte da un punto a caso e scende |
| 45–60' | **Tappa 3: il punteggio** | Quando la mela tocca il cesto, un punto e un suono |
| 60–70' | **Tappa 4: si ricomincia** | La mela riparte dall'alto, sia se presa sia se caduta |
| 70–80' | **Scambio di postazione** | Tutti si alzano e provano il gioco di un compagno. Record della giornata alla lavagna |
| 80–90' | **Timbri e salvataggio** | Verifica, timbri, salvataggio nella cartella |

### Passo passo

> **Tappa 1 – Il cesto**
> 1. Cancella il gatto (tasto destro, "elimina") e scegli dallo scaffale degli sprite un cesto (Bowl). Rinominalo **Cesto**.
> 2. Scrivi:
>    `quando si clicca su (bandiera verde)`
>    `vai a x: (0) y: (-140)`
>    `per sempre`
>       `se <tasto (freccia sinistra) premuto?> allora` → `cambia x di (-10)`
>       `se <tasto (freccia destra) premuto?> allora` → `cambia x di (10)`
> 3. Prova: il cesto scivola sul fondo.
>
> **Tappa 2 – La mela che cade**
> 1. Aggiungi lo sprite della mela (Apple). Rinominalo **Mela**.
> 2. Scrivi:
>    `quando si clicca su (bandiera verde)`
>    `vai a x: (numero a caso tra (-200) e (200)) y: (170)`
>    `per sempre`
>       `cambia y di (-5)`
>
> **Tappa 3 – Il punteggio**
> 1. Nella categoria **Variabili** crea una variabile chiamata **punti**, "per tutti gli sprite".
> 2. Nella mela, sotto la bandiera verde, prima di `vai a`, aggiungi `porta (punti) a (0)`.
> 3. Dentro il `per sempre`, sotto `cambia y di (-5)`, aggiungi:
>    `se <sta toccando (Cesto)?> allora`
>       `cambia (punti) di (1)`
>       `avvia riproduzione suono (Pop)`
>
> **Tappa 4 – Si ricomincia**
> 1. Dentro il `se` del cesto, in fondo, aggiungi `vai a x: (numero a caso tra (-200) e (200)) y: (170)`.
> 2. Sotto, sempre nel `per sempre`, aggiungi:
>    `se <(posizione y) < (-170)> allora`
>       `vai a x: (numero a caso tra (-200) e (200)) y: (170)`
> 3. Prova il gioco completo con la bandiera verde.

### Domande guida

| Situazione | Chiedi |
|---|---|
| La mela cade una volta sola | "Quante volte deve scendere la mela? Una volta o…?" |
| Il bambino non sa dove mettere il `se` | "Il computer deve controllare se tocca il cesto una volta sola, o continuamente?" |
| Vuole aggiungere tutto subito | "Proviamo prima che funzioni questa tappa. Poi la prossima" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| La mela scende di un passo e si ferma | `cambia y` è fuori dal `per sempre` | "Cosa c'è dentro la bocca del per sempre?" |
| Prendo una mela e guadagno 10 punti | La mela resta sul cesto per diversi giri prima di ripartire: manca il `vai a` dentro il `se` | Tappa 4, punto 1 |
| I punti non ripartono da zero | Manca `porta (punti) a (0)` | "Cosa succede ai punti quando ricomincio?" |
| Il cesto non risponde | `tasto premuto?` è un blocco esagonale dei **Sensori**, da inserire nel buco del `se` | Mostrare la forma: esagono nell'esagono |

### Differenziare

| Per chi finisce prima | Per chi è in difficoltà |
|---|---|
| Una variabile **velocità** che aumenta ogni 5 punti | Saltare la tappa 4 caso "mela caduta": basta la ripartenza quando la prende |
| Una seconda mela, più veloce, che vale 3 punti | Il mentor prepara il cesto già funzionante e il bambino lavora solo sulla mela |
| Alternativa: il **labirinto** (vedi guida del mentor, §5) | Lavorare in coppia: uno costruisce il cesto, l'altro la mela |

### Timbro Marinaio

Il gioco funziona, conta i punti e la mela riparte. Domanda di verifica: "Cosa succede se tolgo questo blocco?" (indicando il `per sempre` o il `se`). Se il bambino sa prevederlo, il timbro è suo.

### In un club misto

Nei 70 minuti: 5' di sfida e piano, 4 tappe da 12' ciascuna, 10' prova e timbro, 5' salvataggio. Il gioco finito del mentor resta aperto su un PC: chi si blocca può andarlo a guardare, ma non copiarlo blocco per blocco.

---

## Scheda 3 – Nostromo: il mio gioco

| Carta d'identità | |
|---|---|
| **Grado** | Nostromo (inventa) |
| **Età** | Dagli 8 anni |
| **Partecipanti** | Fino a 10 |
| **Mentor** | 1 ogni 5 bambini: ogni progetto è diverso, servono più occhi |
| **Prerequisiti** | Grado Marinaio ai Gatti |

**Obiettivo:** il bambino progetta prima di costruire, e aggiunge a un gioco almeno un'idea sua, usando una variabile.

### Prima di iniziare

- [ ] La **carta del progetto** stampata per ogni bambino (riquadro qui sotto)
- [ ] Matite e pennarelli
- [ ] Tre o quattro giochi d'esempio fatti dal mentor o da Nostromi delle sessioni passate
- [ ] I progetti "Acchiappa la mela" dei bambini, nelle loro cartelle

> **La carta del progetto**
> 1. Come si chiama il mio gioco?
> 2. Chi è il protagonista e come si muove?
> 3. Come si vince?
> 4. Come si perde?
> 5. Cosa c'è di nuovo, che non c'era nella scheda?
> Disegna qui la schermata del gioco.

### Scaletta

| Tempo | Momento | Cosa fa il mentor |
|---|---|---|
| 0–10' | **Ispirazione** | Mostra 3–4 giochi diversi e chiede: "Cosa vi piace di questo? Cosa cambiereste?" |
| 10–25' | **La carta del progetto** | Ogni bambino compila la carta e la disegna. Il mentor passa a ogni banco e fa una domanda: "Come si perde nel tuo gioco?" |
| 25–30' | **Il patto della misura** | Il mentor aiuta a tagliare: "Per oggi scegliamo **una** idea nuova, la più importante" |
| 30–60' | **Costruzione** | Si parte da Acchiappa la mela o da zero. Il mentor gira con le ricette (sotto) |
| 60–70' | **Il collaudatore** | Coppie: ognuno prova il gioco dell'altro senza spiegazioni. Il collaudatore dice una cosa che gli è piaciuta e una che l'ha confuso |
| 70–80' | **Correzioni** | Si sistema quello che il collaudatore ha trovato |
| 80–90' | **Presentazione e timbri** | Ognuno presenta in 1 minuto: nome del gioco e idea nuova |

### Le ricette: idee pronte da adattare

> **Le vite**
> 1. Crea la variabile **vite**; alla bandiera verde `porta (vite) a (3)`.
> 2. Quando la mela cade a terra: `cambia (vite) di (-1)`.
> 3. `se <(vite) = (0)> allora` → `dire (Hai perso!) per (2) secondi` → `ferma (tutto)`.
>
> **Il cronometro**
> 1. Crea la variabile **tempo**; alla bandiera verde `porta (tempo) a (30)`.
> 2. Sullo stage: `ripeti fino a quando <(tempo) = (0)>` → `attendi (1) secondi` → `cambia (tempo) di (-1)`.
> 3. Alla fine: `ferma (tutto)`.
>
> **Il secondo livello**
> 1. Crea la variabile **velocità**, parte da 5. La mela usa `cambia y di ((0) - (velocità))`.
> 2. `se <(punti) = (10)> allora` → `porta (velocità) a (8)` → cambia sfondo.
>
> **Il quiz**
> 1. `chiedi (Quanto fa 7 x 8?) e attendi`.
> 2. `se <(risposta) = (56)> allora` → `cambia (punti) di (1)` → `dire (Giusto!)`; `altrimenti` → `dire (Riprova!)`.
>
> **La storia a bivi**
> 1. `chiedi (Vuoi entrare nella grotta o salire sulla nave?) e attendi`.
> 2. Se la risposta è "grotta" cambia sfondo e prosegue una storia; se è "nave", un'altra.

### Domande guida

| Situazione | Chiedi |
|---|---|
| Il progetto è troppo grande | "Se avessi solo 20 minuti, quale pezzo faresti per primo?" |
| Non ha idee | "Pensa a un gioco che ti piace: cosa potremmo rubargli?" |
| È bloccato su un pezzo tecnico | "Quale delle ricette assomiglia a quello che vuoi fare?" |
| Il collaudatore non capisce il gioco | "Cosa potresti far dire al gioco all'inizio, per spiegarlo?" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| Il progetto non finisce mai | Troppe idee insieme | Il patto della misura: una sola idea nuova per oggi, le altre la prossima volta |
| Le vite scendono a zero subito | La condizione "mela caduta" scatta molte volte prima che la mela riparta | Far ripartire la mela nello stesso `se` in cui si toglie la vita |
| Il cronometro va troppo veloce | Manca `attendi (1) secondi` | "Ogni quanto deve scendere di uno?" |
| Il quiz dice sempre "Riprova" | Spazi o maiuscole nella risposta | Provare a scrivere la risposta esatta; per le parole, usare risposte brevi |

### Differenziare

| Per chi va veloce | Per chi è in difficoltà |
|---|---|
| Due idee nuove invece di una, oppure disegnare i propri sprite nell'editor | Partire da Acchiappa la mela e aggiungere solo le vite |
| Aggiungere una schermata iniziale con le istruzioni del gioco | Lavorare in coppia sulla stessa carta del progetto |

### Timbro Nostromo

Almeno una variabile **e** un'idea che non era in nessuna scheda. Domanda di verifica: "Cosa hai aggiunto tu, che la scheda non diceva?". La carta del progetto compilata va spillata al registro dei timbri.

### In un club misto

Il progetto di un Nostromo dura spesso due sessioni: la prima per la carta e l'avvio, la seconda per collaudo e correzioni. I Nostromi sono anche i collaudatori ideali per i giochi dei Marinai.

---

## Scheda 4 – Capitano: insegnare a un compagno

| Carta d'identità | |
|---|---|
| **Grado** | Capitano (insegna) |
| **Età** | Dai 9 anni circa: conta la pazienza più dell'età |
| **Partecipanti** | Coppie Capitano-compagno, formate dal mentor |
| **Mentor** | 1 che osserva fino a 4 coppie |
| **Prerequisiti** | Grado Nostromo ai Gatti |

**Obiettivo:** il bambino aiuta un compagno a conquistare il grado Mozzo o Marinaio, **senza fare al posto suo**.

### Prima di iniziare

- [ ] Coppie decise in anticipo: il Capitano con un nuovo arrivato o un Mozzo
- [ ] Le schede 1 e 2 stampate per le coppie
- [ ] Il cartoncino delle **tre regole del Capitano** (sotto), uno per Capitano

> **Le tre regole del Capitano**
> 1. **Mani in tasca:** il mouse lo tiene il tuo compagno.
> 2. **Prima chiedi, poi spieghi:** "Secondo te cosa manca?"
> 3. **Gli errori sono tesori:** quando sbaglia, aiutalo a trovare l'errore, non a nasconderlo.

### Scaletta

| Tempo | Momento | Cosa fa il mentor |
|---|---|---|
| 0–10' | **Il briefing dei Capitani** | Solo con i Capitani: le tre regole, e una prova a ruoli invertiti (il mentor fa il bambino confuso) |
| 10–65' | **Il tutoraggio** | Le coppie lavorano con la scheda 1 o 2. Il mentor osserva da lontano e annota: chi tiene il mouse? Chi parla di più? |
| 65–75' | **Verifica del compagno** | Il mentor verifica il grado del compagno con la solita domanda, senza il Capitano accanto |
| 75–85' | **Il debriefing** | Solo con i Capitani: "Qual è stato il momento più difficile da spiegare? Cosa hai fatto?" |
| 85–90' | **Timbri** | Prima al compagno, poi al Capitano |

### Errori tipici del Capitano

| Problema | Come intervenire |
|---|---|
| Prende il mouse "per fare prima" | Mostrare il cartoncino, regola 1. Senza rimproveri: "Ricordi la regola delle mani?" |
| Dà la soluzione | "Prova a fargli una domanda invece" |
| Si spazientisce | Una pausa di 2 minuti insieme: "Ti ricordi quando la mela non cadeva a te?" |
| Il compagno non parla | Suggerire al Capitano: "Chiedigli cosa vuole che faccia il suo personaggio" |

### Timbro Capitano

Il compagno conquista il grado **e** il Capitano ha rispettato le tre regole durante l'osservazione. Domanda di verifica, nel debriefing: "Qual è stato il momento più difficile da spiegare?". Se il compagno non arriva al grado in una sessione, il Capitano ci riprova la volta dopo: il timbro arriva insieme a quello del compagno.

### In un club misto

È la scheda più naturale per il club: i Capitani si formano mentre accolgono i nuovi. Nei periodi con molti nuovi arrivati, il mentor può affidare ogni nuovo a un aspirante Capitano.

---

*Documento di lavoro – versione 0.1 (pilota) – novembre 2026. Materiali rilasciati con licenza CC BY-SA 4.0.*
