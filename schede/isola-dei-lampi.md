---
title: Isola dei Lampi
parent: Schede attività
nav_order: 4
permalink: /schede/isola-dei-lampi/
render_with_liquid: false
---

# Isola dei Lampi – Schede attività
{: .no_toc }

**BBC micro:bit · dagli 8 anni · 5 schede: Mozzo, Marinaio, due per Nostromo (il gadget o il Teatrino dell'esploratore), Capitano**

Code Club Sulmona · [Guida del mentor](../../guida-mentor/), allegato alla sezione 6 · info@sulmonalug.it

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
| **micro:bit** | Uno per bambino (versione 2, con altoparlante e microfono), con cavo USB e portabatterie con 2 pile AAA |
| **Editor** | MakeCode per micro:bit, a blocchi, in italiano. Funziona nel browser senza account, oppure come app installata sul PC |
| **Scaricare il programma** | Pulsante "Scarica": il file .hex si trascina sull'unità MICROBIT, oppure si abbina il micro:bit con "Associa dispositivo" per scaricare con un clic |
| **Simulatore** | A sinistra nell'editor: utile per provare, ma il timbro si dà solo sul micro:bit vero |
| **Pile di scorta** | Sempre |

I nomi dei blocchi sono riportati come appaiono in MakeCode in italiano. Le traduzioni possono cambiare leggermente tra versioni: controllate sull'editor che usate.

---

## Scheda 1 – Mozzo: il primo lampo

| Carta d'identità | |
|---|---|
| **Grado** | Mozzo (prova) |
| **Età** | Dagli 8 anni |
| **Partecipanti** | Fino a 12 |
| **Mentor** | 1 ogni 6 bambini |
| **Prerequisiti** | Nessuno; aver fatto i Gatti aiuta |

**Obiettivo:** il bambino scrive un programma sul computer e lo trasferisce su un oggetto vero, che funziona da solo con le pile.

### Prima di iniziare

- [ ] MakeCode aperto su ogni PC, progetto nuovo
- [ ] micro:bit, cavi e portabatterie sui banchi
- [ ] Un micro:bit del mentor con il nome che scorre, per la dimostrazione

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **La storia** | "Sull'Isola dei Lampi ogni esploratore ha un piccolo computer da portare in tasca. Oggi lo accendiamo" |
| 10–20' | **Conosciamo il micro:bit** | 25 LED, due pulsanti A e B, sensori. Il mentor mostra il suo micro:bit con il nome che scorre |
| 20–40' | **Attività 1: il nome che scorre** | Prima nel simulatore, poi sul micro:bit vero |
| 40–45' | **Pausa** | |
| 45–70' | **Attività 2: il cuore che batte** | Animazione con due icone e un ciclo |
| 70–80' | **Il micro:bit va in giro** | Con il portabatterie, ognuno mostra il suo micro:bit agli altri |
| 80–90' | **Timbri e riordino** | Pile staccate, micro:bit nella scatola |

### Passo passo

> **Attività 1 – Il nome che scorre**
> 1. Nel blocco `all'avvio` metti `mostra stringa ("Ciao!")` dalla categoria **Base**.
> 2. Scrivi il tuo nome al posto di "Ciao!". Guarda il simulatore.
> 3. Collega il micro:bit con il cavo USB e clicca **Scarica**.
> 4. Il nome scorre sul micro:bit vero!
> 5. Sfida: sposta il blocco dentro `per sempre`. Cosa cambia?
>
> **Attività 2 – Il cuore che batte**
> 1. Dentro `per sempre` metti `mostra icona` con il cuore grande.
> 2. Sotto, `pausa (ms) (500)`.
> 3. Poi `mostra icona` con il cuore piccolo e un'altra `pausa (ms) (500)`.
> 4. Scarica sul micro:bit e collega il portabatterie.
> 5. Cambia i tempi delle pause: il cuore batte più forte o più piano?

### Domande guida

| Situazione | Chiedi |
|---|---|
| Il nome scorre una volta e basta | "Quale blocco ripete le cose all'infinito?" |
| Il cuore non sembra battere | "Quanto tempo resta acceso ogni cuore?" |
| Funziona sul simulatore ma non sul micro:bit | "Il programma è arrivato sul micro:bit? Come lo controlliamo?" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| Il micro:bit mostra ancora il programma vecchio | Lo scaricamento non è riuscito | Ripetere "Scarica", controllare che il LED giallo sul retro lampeggi durante il trasferimento |
| Il PC non vede il micro:bit | Cavo solo di ricarica, senza dati | Cambiare cavo: tenete da parte i cavi "buoni" |
| Il cuore resta fisso | Mancano le pause | Domanda guida sopra |

### Differenziare

| Per chi va veloce | Per chi è in difficoltà |
|---|---|
| Disegnare un'icona propria con `mostra LED` | Solo il nome che scorre, con il mentor accanto al primo scaricamento |
| Aggiungere un suono a ogni battito (micro:bit v2) | Lavorare in coppia su un micro:bit |

### Timbro Mozzo

Il nome scorre **o** il cuore batte sul micro:bit vero, alimentato con le pile. Domanda di verifica: "Me lo mostri funzionare?"

### In un club misto

Nei 70 minuti: 10' di presentazione, 25' nome, 25' cuore, 10' timbri. Chi ha già il grado Marinaio può aiutare i nuovi con il primo scaricamento, il momento più delicato.

---

## Scheda 2 – Marinaio: il dado elettronico

| Carta d'identità | |
|---|---|
| **Grado** | Marinaio (fa) |
| **Età** | Dagli 8 anni |
| **Partecipanti** | Fino a 12 |
| **Mentor** | 1 ogni 6 bambini |
| **Prerequisiti** | Grado Mozzo ai Lampi |

**Obiettivo:** il bambino usa un sensore (l'accelerometro) e un numero casuale, e capisce la differenza tra `all'avvio`, `per sempre` e un evento.

### Prima di iniziare

- [ ] Un dado vero per gruppo, per la sfida finale
- [ ] Una tabella stampata per contare i risultati del dado (sfida per chi va veloce)

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **La sfida** | "Al porto qualcuno ha perso i dadi. Ne costruiamo uno elettronico" |
| 10–35' | **Attività 1: il dado** | Si scuote, esce un numero da 1 a 6 |
| 35–40' | **Pausa** | |
| 40–65' | **Attività 2: sasso, carta, forbici** | Il dado diventa un gioco |
| 65–80' | **Il torneo** | Sfide a coppie con i micro:bit |
| 80–90' | **Timbri e riordino** | |

### Passo passo

> **Attività 1 – Il dado**
> 1. Dalla categoria **Input** prendi `quando (scosso)`.
> 2. Dentro metti `mostra numero` e, nel buco del numero, `scegli a caso da (1) a (6)` dalla categoria **Matematica**.
> 3. Prova nel simulatore: clicca su "scuoti".
> 4. Scarica e prova con le pile: scuoti il micro:bit!
>
> **Attività 2 – Sasso, carta, forbici**
> 1. Dalla categoria **Variabili** crea la variabile **mano**.
> 2. In `quando (scosso)`: `imposta (mano) a (scegli a caso da (1) a (3))`.
> 3. Dalla categoria **Logica** prendi `se … allora … altrimenti`:
>    se `mano = 1` → `mostra icona` del sasso (un quadrato pieno)
>    altrimenti se `mano = 2` → `mostra icona` della carta (un quadrato vuoto)
>    altrimenti → `mostra icona` delle forbici
> 4. Scarica e sfida un compagno.

### Domande guida

| Situazione | Chiedi |
|---|---|
| Il dado cambia numero da solo continuamente | "Il numero deve cambiare sempre, o solo quando…?" |
| Esce sempre lo stesso numero | "Cosa dice al micro:bit di scegliere a caso?" |
| Non sa come aggiungere il terzo caso | "Cerca il segno + sul blocco se" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| Esce lo 0 | Il blocco casuale parte da 0 | Cambiare il primo numero in 1 |
| Il dado mostra sempre il primo numero | Il numero casuale è nel blocco `all'avvio` | Spostare tutto in `quando (scosso)` |
| Le forbici escono troppo spesso | Il terzo caso è un `altrimenti` che raccoglie anche numeri sbagliati | Controllare che il casuale vada da 1 a 3 |

### Differenziare

| Per chi va veloce | Per chi è in difficoltà |
|---|---|
| Lanciare il dado 30 volte e contare i risultati sulla tabella: escono tutti allo stesso modo? | Solo il dado, con il mentor che mostra dove si trova il blocco casuale |
| Un dado a 20 facce, o un "dado delle decisioni" con frasi | Sasso, carta, forbici con solo due possibilità |

### Timbro Marinaio

Il dado funziona scuotendolo, e il bambino sa spiegare perché esce un numero diverso. Domanda di verifica: "Cosa succede se metto questo blocco in `all'avvio`?"

### In un club misto

Nei 70 minuti: 5' di sfida, 25' dado, 25' sasso-carta-forbici, 10' torneo, 5' timbri. Il torneo funziona benissimo anche con i bambini di altre isole: è un modo per attirarli ai Lampi.

---

## Scheda 3 – Nostromo: il mio gadget

| Carta d'identità | |
|---|---|
| **Grado** | Nostromo (inventa) |
| **Età** | Dai 9 anni |
| **Partecipanti** | Fino a 10 |
| **Mentor** | 1 ogni 5 bambini |
| **Prerequisiti** | Grado Marinaio ai Lampi |

**Obiettivo:** il bambino progetta un gadget che usa almeno un sensore e una variabile, con un'idea sua.

### Prima di iniziare

- [ ] La **carta del progetto** (stessa dell'Isola dei Gatti, scheda 3), con la domanda in più: "Quale sensore usa il mio gadget?"
- [ ] Due micro:bit per le coppie che vogliono usare la radio
- [ ] Nastro biadesivo, elastici e cartoncino per "indossare" il micro:bit

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **I sensori** | Il mentor mostra cosa sente il micro:bit: movimento, temperatura, luce, suono, la radio |
| 10–25' | **La carta del progetto** | Ognuno sceglie un'idea e un sensore |
| 25–60' | **Costruzione** | Con le ricette qui sotto |
| 60–70' | **Indossiamolo** | Il gadget si fissa al polso, alla scarpa, alla porta |
| 70–80' | **Collaudo** | Un compagno prova il gadget senza spiegazioni |
| 80–90' | **Presentazione e timbri** | |

### Le ricette

> **Il contapassi**
> 1. Variabile **passi**, `all'avvio` → `imposta (passi) a (0)`.
> 2. `quando (scosso)` → `cambia (passi) di (1)`.
> 3. `quando si preme il pulsante (A)` → `mostra numero (passi)`.
> 4. Si lega al polso o alla scarpa.
>
> **Il termometro della stanza**
> 1. `quando si preme il pulsante (A)` → `mostra numero (temperatura (°C))`.
> 2. Con `se`: sopra 25 gradi un sole, sotto 18 un fiocco di neve.
>
> **Messaggi segreti via radio** (in coppia, 2 micro:bit)
> 1. `all'avvio` → `radio imposta gruppo (7)` (lo stesso numero sui due micro:bit, diverso dalle altre coppie).
> 2. `quando si preme il pulsante (A)` → `radio invia numero (1)`; pulsante B → `radio invia numero (2)`.
> 3. `quando la radio riceve (numero ricevuto)` → `se` 1 un'icona, se 2 un'altra.
> 4. Inventate un codice segreto.
>
> **L'allarme della porta**
> 1. Il micro:bit, fissato alla porta, sente quando si muove.
> 2. `quando (scosso)` → suona una melodia e mostra un'icona.

### Domande guida

| Situazione | Chiedi |
|---|---|
| Il contapassi conta troppo | "Quando cammini, quante volte si scuote il micro:bit a ogni passo?" |
| La radio non riceve | "I due micro:bit sono sullo stesso gruppo?" |
| Il bambino ha un'idea troppo grande | "Qual è la prima cosa che il gadget deve fare? Partiamo da lì" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| La radio riceve messaggi di altri | Più coppie sullo stesso gruppo | Assegnare un numero di gruppo diverso a ogni coppia |
| La temperatura sembra troppo alta | Il sensore misura la temperatura del processore, un po' più calda dell'aria | È un'ottima scoperta: farla notare |
| Il contapassi riparte da zero | La variabile è azzerata dentro `per sempre` | Spostare l'azzeramento in `all'avvio` |

### Differenziare

| Per chi va veloce | Per chi è in difficoltà |
|---|---|
| Due sensori nello stesso gadget | Il contapassi, seguendo la ricetta passo passo, più un'icona scelta da lui |
| Passare alla vista Python di MakeCode e cambiare un numero lì | Lavorare in coppia sui messaggi radio |

### Timbro Nostromo

Il gadget usa almeno un sensore e una variabile, **e** contiene un'idea sua. Domanda di verifica: "Cosa hai aggiunto tu, che la ricetta non diceva?"

### In un club misto

Chi ottiene il grado Marinaio ai Lampi apre il ponte verso il Serpente: un Nostromo dei Lampi è spesso pronto per Python. Mostrategli la vista Python di MakeCode: è lo stesso programma, scritto in un'altra lingua.

---

## Scheda 3bis – Nostromo: il Teatrino dell'esploratore

| Carta d'identità | |
|---|---|
| **Grado** | Nostromo (inventa), alternativa alla scheda 3 |
| **Età** | Dagli 8–9 anni |
| **Partecipanti** | Fino a 12, in compagnie da 2–3 |
| **Mentor** | 1 ogni 6 bambini |
| **Prerequisiti** | Grado Marinaio ai Lampi |

**Obiettivo:** il bambino progetta una storia a scene, la costruisce in un diorama di cartone e la fa vivere con il micro:bit, usando una variabile e almeno un evento (logo, suono, pulsante).

Il micro:bit non racconta la storia: la **anima**. La storia la racconta il bambino, a voce, davanti al pubblico. Questa scheda attira chi preferisce raccontare, disegnare e recitare.

### Prima di iniziare

- [ ] Micro:bit **versione 2** (servono logo touch, microfono e altoparlante), con portabatterie
- [ ] Una scatola da scarpe per compagnia: sarà il palcoscenico
- [ ] Cartoncini colorati, forbici, colla, nastro adesivo, pennarelli, stecchini per i personaggi
- [ ] L'**albero della storia** stampato (riquadro sotto), uno per compagnia
- [ ] Il teatrino d'esempio del mentor, già funzionante

> **L'albero della storia**
> 1. Chi è il protagonista?
> 2. Scena 1: dove inizia la storia? (icona e suono)
> 3. Scena 2: cosa succede? (icona e suono)
> 4. Il momento speciale: cosa succede quando battiamo le mani?
> 5. Il bivio: pulsante A porta a… pulsante B porta a…
> 6. Il finale (o i due finali)
> Disegna l'albero: un riquadro per scena, una freccia per ogni passaggio.

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **Lo spettacolo del mentor** | Il mentor racconta una storia di un minuto con il suo teatrino: tocca il logo, batte le mani, il vulcano erutta. "Oggi i registi siete voi" |
| 10–25' | **L'albero della storia** | Ogni compagnia inventa la storia e la disegna: almeno 3 scene e un momento speciale |
| 25–45' | **Programmare le scene** | Con il passo passo qui sotto |
| 45–50' | **Pausa** | |
| 50–70' | **Costruire il palcoscenico** | Scatola, sfondo, personaggi. Il micro:bit si fissa in modo che il logo resti raggiungibile e il display si veda |
| 70–80' | **Prova generale** | Ogni compagnia prova la storia per intero, almeno due volte |
| 80–90' | **Lo spettacolo e i timbri** | Ogni compagnia mette in scena la sua storia per gli altri |

### Passo passo

> **1. Le scene, una dopo l'altra**
> 1. Crea la variabile **scena**.
> 2. `all'avvio` → `imposta (scena) a (0)` → `mostra icona` della prima scena.
> 3. `quando il logo viene toccato` → `cambia (scena) di (1)`.
> 4. Sotto, un `se` per ogni scena:
>    `se (scena) = 1` → `mostra icona` → `riproduci suono` (per esempio "mistero")
>    `se (scena) = 2` → un'altra icona → un altro suono
> 5. Prova: ogni volta che tocchi il logo, la storia va avanti.
>
> **2. Il momento speciale**
> 1. `quando c'è un suono forte` → `se (scena) = 2` → un'icona disegnata con `mostra LED` (un'esplosione, una stella) → un suono.
> 2. Il pubblico batte le mani e la scena reagisce: è il momento che tutti ricorderanno.
>
> **3. Il bivio** (per chi è pronto)
> 1. Nella scena del bivio, il micro:bit mostra una freccia a sinistra e una a destra.
> 2. `quando si preme il pulsante (A)` → `se (scena) = 3` → `imposta (scena) a (10)` → primo finale.
> 3. `quando si preme il pulsante (B)` → `se (scena) = 3` → `imposta (scena) a (20)` → secondo finale.
> 4. Numeri lontani (10, 20) per i finali: così non si confondono con le scene normali.
>
> **4. Il sipario**
> 1. Nell'ultima scena: `mostra stringa ("Fine")`.
> 2. Con il pulsante A e B premuti insieme: `imposta (scena) a (0)`, per ricominciare lo spettacolo.

### Domande guida

| Situazione | Chiedi |
|---|---|
| La storia salta delle scene | "Quante volte hai toccato il logo? Cosa succede a ogni tocco?" |
| La compagnia vuole 10 scene | "Il pubblico ricorderà 3 scene belle o 10 di corsa?" |
| Il momento speciale scatta da solo | "Chi altro sta facendo rumore nella stanza?" |
| Non sanno quale suono scegliere | "Come si sente il protagonista in questa scena?" |

### Errori tipici

| Problema | Causa | Come sbloccare |
|---|---|---|
| Una scena viene saltata | Il logo viene sfiorato mentre si tiene il micro:bit | Tenerlo dai bordi; fissarlo alla scatola con il logo libero |
| L'effetto speciale scatta per il rumore degli altri | Soglia del suono troppo bassa | `imposta soglia del suono forte` più alta, all'avvio |
| Dopo il finale la storia va avanti a caso | La scena continua a crescere | Nell'ultima scena, `imposta (scena)` a un numero fisso, oppure il sipario |
| Il display non si vede nel diorama | Micro:bit montato al buio o di lato | Ritagliare una finestra nella scatola davanti al display |

### Differenziare

| Per chi va veloce | Per chi è in difficoltà |
|---|---|
| Due finali con il bivio | Tre scene con il logo, senza bivio né suono forte |
| La storia via radio: un secondo micro:bit è un personaggio che reagisce alle scene (scheda 3, ricetta dei messaggi radio) | Il mentor prepara le icone; la compagnia sceglie suoni e ordine |
| Un sensore in più: scuotere la scatola per il terremoto | Una compagnia di 3, con ruoli: programmatore, scenografo, narratore |

### Timbro Nostromo

La storia ha almeno 3 scene comandate dal micro:bit, usa la variabile **scena** e almeno un evento oltre ai pulsanti (logo o suono forte), **e** la compagnia la mette in scena davanti agli altri. Domanda di verifica: "Cosa succede nella tua storia se tocco il logo adesso? Perché?"

### In un club misto

Il Teatrino è perfetto per la Festa del Porto e per l'open day: gli spettatori vedono una storia, non un programma. Le compagnie possono essere miste con la Scogliera Sonora: chi sta lì compone la colonna sonora, ai Lampi si programmano le scene.

---

## Scheda 4 – Capitano: insegnare a un compagno

| Carta d'identità | |
|---|---|
| **Grado** | Capitano (insegna) |
| **Età** | Dai 9 anni |
| **Partecipanti** | Coppie Capitano-compagno |
| **Mentor** | 1 che osserva fino a 4 coppie |
| **Prerequisiti** | Grado Nostromo ai Lampi |

Valgono le **tre regole del Capitano** della scheda 4 dell'Isola dei Gatti: mani in tasca, prima chiedi poi spieghi, gli errori sono tesori.

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **Briefing dei Capitani** | Le tre regole. Attenzione speciale: il momento dello scaricamento, dove la tentazione di fare al posto dell'altro è più forte |
| 10–65' | **Tutoraggio** | Le coppie lavorano con la scheda 1 o 2 |
| 65–75' | **Verifica del compagno** | Dal mentor, senza il Capitano accanto |
| 75–90' | **Debriefing e timbri** | |

### Timbro Capitano

Il compagno conquista Mozzo o Marinaio ai Lampi **e** il Capitano ha rispettato le tre regole durante l'osservazione.

### In un club misto

I Capitani dei Lampi sono perfetti per il torneo di sasso-carta-forbici con i nuovi arrivati: insegnano giocando.

---

*Documento di lavoro – versione 0.1 – novembre 2026. Materiali rilasciati con licenza CC BY-SA 4.0.*
