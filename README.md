# ASPIRATORE MASTER per Home Assistant

<p align="center">
  <a href="https://www.home-assistant.io/" target="_blank">
    <img src="https://user-images.githubusercontent.com/102819027/233830183-9c55677d-b6a1-4153-8d3c-219394ec8720.png" alt="Home Assistant" width="90">
  </a>
</p>

<p align="center">
  <strong>Controllo intelligente di aspiratori e ventilatori per Home Assistant</strong><br>
  Una soluzione avanzata per automatizzare il ricambio d’aria in modo affidabile, stabile e configurabile.
</p>

<p align="center">
  <a href="mailto:danilo.robotti@gmail.com">danilo.robotti@gmail.com</a>
</p>

<img width="1672" height="941" alt="ASPIRATORE MASTER" src="https://github.com/DanRobo76/Aspiratore/blob/main/immagini/Collage.png" />

## Cos'è ASPIRATORE MASTER
**ASPIRATORE MASTER** è un package avanzato per Home Assistant progettato per la gestione intelligente di aspiratori e ventilatori (`Switch` / `Fan`). È pensato per ambienti come **bagni ciechi**, lavanderie, locali tecnici e spazi soggetti a umidità o scarsa aerazione, dove il ricambio d’aria deve essere automatico, affidabile e coerente con le condizioni reali dell’ambiente.

Non è una semplice automazione, ma un sistema strutturato che supervisiona il funzionamento della ventilazione, valida il dominio operativo e coordina attuatore, sensori e timer per garantire continuità, stabilità e sicurezza logica.

## Punti di forza
- **Selezione dinamica delle entità** tramite menu a tendina: attuatore, sensore di umidità e sensore di presenza.
- **Controllo evoluto dell’umidità** con attivazione solo dopo permanenza sopra soglia, gestione offset e riduzione dei falsi positivi.
- **Gestione completa dei timer**: permanenza umidità, controllo stato, durata massima aspirazione e timer ciclici.
- **Integrazione con il rilevamento presenza** per migliorare comfort, efficacia e continuità della ventilazione.
- **Sincronizzazione tra stato reale e stato logico** con riattivazione automatica in caso di spegnimenti manuali indesiderati.
- **Architettura fail-safe e self-healing**, con gestione di stati non validi (`unknown`, `unavailable`, ecc.), reset automatici e prevenzione di comportamenti instabili.

## Come funziona
Il sistema opera come un vero **supervisore intelligente della ventilazione**: controlla continuamente la validità di sensori e attuatore, gestisce le priorità tra umidità e presenza, attiva l’aspirazione solo quando le condizioni sono coerenti e mantiene il funzionamento stabile anche in presenza di anomalie o incoerenze temporanee.

## Caso d’uso tipico
Un classico esempio è il **bagno cieco** con aspiratore tradizionale, collegato tramite **relè smart** come Shelly, con sensore di umidità e sensore presenza. Il risultato è un sistema di ventilazione completamente automatico, più affidabile di una semplice logica on/off e capace di adattarsi all’uso reale dell’ambiente.

## Requisiti e configurazione
**Pre-requisiti:**
- **[Home Assistant](https://www.home-assistant.io/installation/)**
- Add-on **File Editor** facoltativo ma consigliato

Percorso:
`Impostazioni -> Componenti aggiuntivi -> Raccolta di Componenti Aggiuntivi -> File Editor`

**Requisiti minimi:**
- 1 attuatore (`Switch` oppure `Fan`)
- 1 sensore di umidità
- 1 sensore di presenza *(opzionale ma consigliato)*

La configurazione avviene direttamente da interfaccia tramite:
- `Selezione Attuatore`
- `Selezione Sensore Umidità`
- `Selezione Sensore Rilevamento`

Questo permette di cambiare i dispositivi senza dover modificare manualmente lo YAML ogni volta.

## Perché sceglierlo
ASPIRATORE MASTER è ideale per chi desidera una soluzione di ventilazione **intelligente, autonoma, robusta e professionale**, progettata con criteri di affidabilità operativa, manutenibilità, scalabilità e controllo deterministico degli stati. In pratica, trasforma un comune aspiratore in un sistema di gestione avanzata della ventilazione.

## Security Policy
Per maggiori dettagli sui limiti del software e sulle condizioni di utilizzo:
**[Limiti del Software (Security Policy)](https://github.com/DanRobo76/Aspiratore/blob/main/security.md)**

## Esonero di responsabilità
In nessun caso l’Ing. Danilo Robotti potrà essere ritenuto responsabile per danni diretti, indiretti o conseguenti derivanti dall’uso del presente software. L’utente finale mantiene piena responsabilità in merito alla scelta, installazione, configurazione, utilizzo e gestione del software in funzione del risultato che intende ottenere e del contesto applicativo in cui decide di impiegarlo.

## Supporta il progetto
Se il progetto ti è stato utile e desideri supportarne lo sviluppo, puoi offrirmi un GinSeng:

#### [Clicca qui per supportare il progetto](https://www.paypal.com/donate/?business=YU9379GL8VDW4&amount=1.2&no_recurring=1&item_name=Se+il+progetto+ti+%C3%A8+piaciuto%2C++offrimi+un+GinSeng%21+%0A%3B%29&currency_code=EUR)

<a href="https://www.paypal.com/donate/?business=YU9379GL8VDW4&amount=1.2&no_recurring=1&item_name=Se+il+progetto+ti+%C3%A8+piaciuto%2C++offrimi+un+GinSeng%21+%0A%3B%29&currency_code=EUR">
  <img src="https://user-images.githubusercontent.com/102819027/233830035-709efa6b-94d7-4ea6-865b-76ab5c1eee6d.png" alt="Donate" width="40">
</a>

Oppure puoi scansionare il seguente QR code:

<img src="https://github.com/DanRobo76/VMC-HELTY-FLOW/assets/102819027/81ba7208-fbad-4fab-8ceb-cdcf901fdb61.png" alt="QR Code Donazione" width="220">
