---
title: Scogliera Sonora
parent: Schede attività
nav_order: 9
permalink: /schede/scogliera-sonora/
render_with_liquid: false
---

# Scogliera Sonora – Schede attività
{: .no_toc }

**Sonic Pi · isola misteriosa · dai 9 anni · 2 schede: Mozzo, Capitano**

Code Club Sulmona · [Guida del mentor](../../guida-mentor/), allegato alla sezione 11 · info@sulmonalug.it

---

<details open markdown="block">
<summary>In questa pagina</summary>
{: .text-delta }
1. TOC
{:toc}
</details>

## Prima di tutto: la Scogliera pronta

| Cosa | Dettaglio |
|---|---|
| **Software** | Sonic Pi installato su ogni PC (software libero) |
| **Cuffie** | Una per postazione, **obbligatorie**: 10 PC che suonano insieme sono un frastuono |
| **Altoparlante** | Uno collegato al PC del mentor, per le esibizioni finali |
| **Volume** | Controllare il volume delle cuffie prima di darle ai ragazzi |
| **Cartellone** | I numeri delle note: 60 = DO, 62 = RE, 64 = MI, 65 = FA, 67 = SOL, 69 = LA, 71 = SI, 72 = DO alto |

### Come funziona Sonic Pi in un minuto

Si scrive il codice in uno dei "buffer" (le schede numerate), si preme **Run** per suonare e **Stop** per fermare. Se il codice cambia mentre suona e si preme di nuovo Run, la musica cambia senza fermarsi: è il "live coding".

---

## Scheda 1 – Mozzo: la prima melodia

| Carta d'identità | |
|---|---|
| **Grado** | Mozzo (prova) |
| **Età** | Dai 9 anni |
| **Partecipanti** | Fino a 10 |
| **Mentor** | 1 ogni 5 ragazzi |
| **Prerequisiti** | Nessuno |

**Obiettivo:** il ragazzo scopre che una melodia è una sequenza di istruzioni, e che il codice si può ripetere invece di riscriverlo.

### Prima di iniziare

- [ ] Sonic Pi aperto su ogni PC, cuffie collegate e volume controllato
- [ ] La melodia di Fra Martino stampata con i numeri delle note

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **La storia** | "Sulla Scogliera Sonora le onde suonano. Ma solo chi conosce il codice può comporre la loro musica." Il mentor suona dal vivo un breve brano già pronto |
| 10–20' | **La prima nota** | `play 60` e Run. Poi altre note |
| 20–45' | **Attività 1: Fra Martino** | La melodia, nota per nota |
| 45–50' | **Pausa** | |
| 50–70' | **Attività 2: ripetere e cambiare strumento** | |
| 70–85' | **Il concerto** | Chi vuole suona la sua versione dall'altoparlante |
| 85–90' | **Timbri** | |

### Passo passo

> **Attività 1 – Fra Martino**
> ```ruby
> play 60
> sleep 0.5
> play 62
> sleep 0.5
> play 64
> sleep 0.5
> play 60
> sleep 0.5
> ```
> 1. Scrivi le prime 4 note e premi Run. La riconosci?
> 2. Ripeti le stesse 4 note una seconda volta.
> 3. Aggiungi la seconda parte: 64, 65, 67, con l'ultima nota più lunga (`sleep 1`).
>
> **Attività 2 – Ripetere e cambiare strumento**
> ```ruby
> use_synth :piano
>
> 2.times do
>   play 60
>   sleep 0.5
>   play 62
>   sleep 0.5
>   play 64
>   sleep 0.5
>   play 60
>   sleep 0.5
> end
> ```
> 1. Con `2.times do … end` il pezzo si ripete senza riscriverlo.
> 2. Cambia `:piano` con `:prophet`, `:pluck` o `:chiplead`. Quale ti piace?
> 3. Cambia tutti i `sleep`: la melodia va più veloce o più lenta?

### Domande guida

| Situazione | Chiedi |
|---|---|
| Le note suonano tutte insieme | "Cosa dice al computer di aspettare tra una nota e l'altra?" |
| Errore dopo `times do` | "Ogni `do` ha bisogno di un compagno alla fine: quale?" |
| La melodia non si riconosce | "Confronta i numeri con il cartellone, uno per uno" |

### Errori tipici

| Problema | Causa | Come intervenire |
|---|---|---|
| Accordo invece di melodia | Mancano i `sleep` | Domanda guida sopra |
| Errore rosso in basso | Manca `end`, o `:piano` scritto senza i due punti | Sonic Pi evidenzia la riga: leggerla insieme |
| Silenzio | Volume delle cuffie, o il ragazzo ha premuto Stop | Controllare il volume e premere Run |

### Differenziare

| Per chi va veloce | Per chi è in difficoltà |
|---|---|
| Aggiungere una seconda voce con `in_thread` | Solo le prime 4 note, ripetute con `2.times` |
| Comporre una melodia propria di 8 note | Copiare la melodia dal foglio e cambiare solo lo strumento |

### Timbro Mozzo

Fra Martino (o una melodia propria) si riconosce, e il ragazzo ha usato almeno una ripetizione. Domanda di verifica: "Me la fai sentire?"

### In un club misto

La Scogliera emerge una volta al mese. È l'isola che attira chi "non è un tipo da computer": se un bambino delle altre isole è curioso, fategli ascoltare dalle cuffie di un compagno.

---

## Scheda 2 – Capitano: il mio brano

| Carta d'identità | |
|---|---|
| **Grado** | Capitano (compone) |
| **Età** | Dai 10 anni |
| **Partecipanti** | Fino a 8 |
| **Mentor** | 1 ogni 4 ragazzi |
| **Prerequisiti** | Grado Mozzo alla Scogliera |

**Obiettivo:** il ragazzo compone e suona dal vivo un brano con almeno due parti che suonano insieme (batteria e melodia).

### Prima di iniziare

- [ ] Altoparlante collegato al PC del mentor per il concerto finale
- [ ] Un brano d'esempio del mentor, con batteria e melodia

### Scaletta

| Tempo | Momento | Cosa succede |
|---|---|---|
| 0–10' | **Il live coding** | Il mentor suona e cambia il codice mentre la musica va. "Si può comporre mentre si suona" |
| 10–30' | **La batteria** | Il primo `live_loop` con i campioni |
| 30–45' | **La melodia** | Il secondo `live_loop`, che suona insieme |
| 45–50' | **Pausa** | |
| 50–75' | **Il brano** | Ognuno costruisce e prova il suo brano |
| 75–88' | **Il concerto dal vivo** | Ognuno suona il suo brano dall'altoparlante, cambiando qualcosa mentre suona |
| 88–90' | **Timbri** | |

### Passo passo

> ```ruby
> use_bpm 100
>
> live_loop :batteria do
>   sample :bd_haus
>   sleep 1
>   sample :drum_snare_hard
>   sleep 1
> end
>
> live_loop :melodia do
>   use_synth :pluck
>   play [60, 64, 67, 72].choose
>   sleep 0.5
> end
> ```
> 1. Scrivi la batteria e premi Run.
> 2. Mentre suona, cambia `sleep 1` in `sleep 0.5` e premi di nuovo Run: la musica cambia senza fermarsi.
> 3. Aggiungi il `live_loop` della melodia: le due parti suonano insieme.
> 4. `.choose` sceglie una nota a caso: ogni volta è una melodia diversa.
> 5. Prova altri campioni: inizia a scrivere `sample :` e Sonic Pi mostra l'elenco.

### Domande guida

| Situazione | Chiedi |
|---|---|
| Errore "live_loop without sleep" | "Cosa dice al loop di aspettare? Cosa succede se non aspetta mai?" |
| Le due parti vanno fuori tempo | "Quanto dura un giro della batteria? E uno della melodia?" |
| Il brano è sempre uguale | "Quale parte potresti cambiare mentre suona?" |

### Errori tipici

| Problema | Causa | Come intervenire |
|---|---|---|
| Errore e silenzio | Un `live_loop` senza `sleep` | Ogni loop ha bisogno di almeno un `sleep` |
| Due loop con lo stesso nome | Il secondo sostituisce il primo | Ogni `live_loop` ha un nome diverso |
| Volume troppo alto all'esibizione | Campioni e synth sommati | `amp: 0.5` dopo il campione o la nota |

### Timbro Capitano

Un brano con almeno due `live_loop` che suonano insieme, suonato dal vivo al concerto o al "Mostra cosa hai fatto", cambiando almeno una cosa mentre suona.

### In un club misto

I Capitani della Scogliera possono suonare la colonna sonora della Festa del Porto, o la sigla di apertura dell'open day.

---

*Documento di lavoro – versione 0.1 – novembre 2026. Materiali rilasciati con licenza CC BY-SA 4.0.*
