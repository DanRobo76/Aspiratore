<h1 align="center">
  ASPIRATORE MASTER 
  <a href="https://www.home-assistant.io/" target="_blank">
    <img src="https://user-images.githubusercontent.com/102819027/233830183-9c55677d-b6a1-4153-8d3c-219394ec8720.png" alt="Home Assistant" width="80">
  </a>
</h1>
<p align="center">
  <strong>La soluzione professionale per automatizzare aspiratori e ventilatori in Home Assistant.</strong><br>
  Controllo intelligente, logica robusta e ventilazione davvero affidabile.
</p>

<p align="center">
  <a href="mailto:danilo.robotti@gmail.com">danilo.robotti@gmail.com</a>
</p>

<p align="center">
  <img src="https://github.com/DanRobo76/Aspiratore/blob/main/immagini/Collage%20Aspiratore.png" alt="ASPIRATORE MASTER" width="100%">
</p>

---

## Perché ASPIRATORE MASTER

**ASPIRATORE MASTER** è un package avanzato per Home Assistant progettato per la gestione intelligente di aspiratori e ventilatori (`Switch` / `Fan`), ideale per **bagni ciechi**, lavanderie, locali tecnici e ambienti dove il ricambio d’aria deve essere automatico, coerente con le condizioni reali e affidabile nel tempo.

Non è una semplice automazione on/off, ma una logica evoluta che supervisiona **sensori, attuatori e timer** per garantire un funzionamento stabile, continuo e ottimizzato.

## Cosa lo rende diverso

| Funzione | Vantaggio |
|---|---|
| **Selezione dinamica delle entità** | Configurazione semplice direttamente da interfaccia |
| **Controllo evoluto dell’umidità** | Attivazione solo dopo permanenza sopra soglia |
| **Gestione presenza** | Ventilazione più intelligente durante e dopo l’utilizzo |
| **Timer avanzati** | Controllo preciso di permanenza, durata e riattivazione |
| **Sincronizzazione stato reale/logico** | Maggiore affidabilità anche in caso di spegnimenti indesiderati |
| **Architettura fail-safe** | Gestione robusta di anomalie, stati invalidi e incoerenze |

## Vantaggi principali

- Configurazione intuitiva tramite selettori dedicati
- Compatibile con attuatori `Switch` e `Fan`
- Pensato per l’uso reale, non per semplici automazioni base
- Riduce falsi avvii, incoerenze e comportamenti instabili
- Trasforma un aspiratore tradizionale in un sistema di ventilazione intelligente
- Ideale con relè smart, ad esempio **Shelly**

## Scenario tipico

Un classico caso d’uso è il **bagno cieco** con:

- aspiratore tradizionale
- sensore di umidità
- sensore presenza
- relè smart

**Risultato:** una ventilazione completamente automatica, più intelligente, più affidabile e più professionale rispetto a una logica standard.

## Requisiti

- **[Home Assistant](https://www.home-assistant.io/installation/)**
- 1 attuatore (`Switch` oppure `Fan`)
- 1 sensore umidità
- 1 sensore presenza *(opzionale ma consigliato)*

**Add-on consigliato:** `File Editor`

## Configurazione

La configurazione avviene direttamente da interfaccia tramite:

- `Selezione Attuatore`
- `Selezione Sensore Umidità`
- `Selezione Sensore Rilevamento`

Questo consente di cambiare dispositivi senza modificare manualmente lo YAML a ogni variazione.

Per maggiori dettagli sulla compattibilità: **[Versione del SoftWare](https://github.com/DanRobo76/Aspiratore/blob/main/security.md)**

<details>
<summary><strong>Esonero di responsabilità</strong></summary>

<br>

In nessun caso l’Ing. Danilo Robotti potrà essere ritenuto responsabile per danni diretti, indiretti o conseguenti derivanti dall’uso del presente software.

L’utente finale mantiene piena responsabilità in merito a:

- scelta della soluzione
- installazione
- configurazione
- utilizzo
- gestione del software

in funzione del risultato che intende ottenere e del contesto applicativo in cui decide di impiegarlo.

</details>

---
<p align="center">
  Se il progetto ti è stato utile e desideri supportarne lo sviluppo, scansiona il QR code qui sotto</p>
<p align="center">
  <img src="https://github.com/DanRobo76/VMC-HELTY-FLOW/assets/102819027/81ba7208-fbad-4fab-8ceb-cdcf901fdb61.png" alt="QR Code Donazione" width="220">
</p>
