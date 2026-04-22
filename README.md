# ASPIRATORE MASTER <a href="https://www.home-assistant.io/" target="_blank"> <img src="https://user-images.githubusercontent.com/102819027/233830183-9c55677d-b6a1-4153-8d3c-219394ec8720.png" alt="Home Assistant" width="90"></a>
</p>

<p align="center">
  <strong>La soluzione avanzata per la gestione intelligente di aspiratori e ventilatori in Home Assistant.</strong><br>
  Automatizza il ricambio d’aria in modo stabile, affidabile e professionale.
</p>

<p align="center">
  <a href="mailto:danilo.robotti@gmail.com">danilo.robotti@gmail.com</a>
</p>

<img width="1672" height="941" alt="ASPIRATORE MASTER" src="https://github.com/DanRobo76/Aspiratore/blob/main/immagini/Collage.png" />

## Cos'è
**ASPIRATORE MASTER** è un package avanzato per Home Assistant progettato per la gestione intelligente di aspiratori e ventilatori (`Switch` / `Fan`). È ideale per bagni ciechi, lavanderie, locali tecnici e ambienti dove il ricambio d’aria deve essere automatico, coerente con le condizioni reali e affidabile nel tempo.

Non si tratta di una semplice automazione, ma di una logica evoluta che supervisiona sensori, attuatori e timer per garantire un funzionamento stabile, continuo e ottimizzato.

## Perché sceglierlo
ASPIRATORE MASTER consente di trasformare un comune aspiratore in un sistema di ventilazione intelligente, ad esempio tramite un relè smart come Shelly. La configurazione è semplice, la logica è robusta e il comportamento è pensato per l’uso reale, non per semplici accensioni e spegnimenti on/off.

Integra selezione dinamica delle entità, controllo evoluto dell’umidità, gestione presenza, sincronizzazione tra stato reale e stato logico, timer avanzati e un’architettura fail-safe capace di gestire anomalie, stati non validi e incoerenze operative.

## Cosa offre
- Selezione dinamica di attuatore, sensore umidità e sensore presenza
- Attivazione solo dopo permanenza sopra soglia
- Gestione di timer di permanenza, controllo e durata massima
- Coordinamento tra umidità e rilevamento presenza
- Ripristino automatico in caso di anomalie o spegnimenti indesiderati
- Logica robusta, stabile e orientata all’affidabilità operativa

## Scenario tipico
Il caso d’uso più comune è un **bagno cieco** con aspiratore tradizionale, sensore di umidità, sensore presenza e relè smart. Il risultato è una ventilazione completamente automatica, più intelligente, più affidabile e più professionale rispetto a una normale automazione base.

## Requisiti
- **[Home Assistant](https://www.home-assistant.io/installation/)**
- 1 attuatore (`Switch` oppure `Fan`)
- 1 sensore umidità
- 1 sensore presenza *(opzionale ma consigliato)*

Add-on consigliato:
- **File Editor**

## Configurazione
La configurazione avviene direttamente da interfaccia tramite selettori dedicati:
- `Selezione Attuatore`
- `Selezione Sensore Umidità`
- `Selezione Sensore Rilevamento`

Questo permette di cambiare dispositivi senza dover modificare manualmente lo YAML a ogni variazione.

## Security Policy
Per maggiori dettagli sui limiti del software e sulle condizioni di utilizzo:
**[Limiti del Software (Security Policy)](https://github.com/DanRobo76/Aspiratore/blob/main/security.md)**

## Esonero di responsabilità

In nessun caso l’Ing. Danilo Robotti potrà essere ritenuto responsabile per danni diretti, indiretti o conseguenti derivanti dall’uso del presente software.

L’utente finale mantiene piena responsabilità in merito a:

- scelta della soluzione
- installazione
- configurazione
- utilizzo
- gestione del software

in funzione del risultato che intende ottenere e del contesto applicativo in cui decide di impiegarlo.

---

## Supporta il progetto

Se il progetto ti è stato utile e desideri supportarne lo sviluppo: [Offrimi un GinSeng ☕](https://www.paypal.com/donate/?business=YU9379GL8VDW4&amount=1.2&no_recurring=1&item_name=Se+il+progetto+ti+%C3%A8+piaciuto%2C++offrimi+un+GinSeng%21+%0A%3B%29&currency_code=EUR)

<a href="https://www.paypal.com/donate/?business=YU9379GL8VDW4&amount=1.2&no_recurring=1&item_name=Se+il+progetto+ti+%C3%A8+piaciuto%2C++offrimi+un+GinSeng%21+%0A%3B%29&currency_code=EUR"></a>

Oppure puoi scansionare il seguente QR code: <img src="https://github.com/DanRobo76/VMC-HELTY-FLOW/assets/102819027/81ba7208-fbad-4fab-8ceb-cdcf901fdb61.png" alt="QR Code Donazione" width="220">
