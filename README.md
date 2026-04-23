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
<details>
<summary><strong>Perché ASPIRATORE MASTER</strong></summary>
  
**ASPIRATORE MASTER** è un package avanzato per Home Assistant progettato per la gestione intelligente di aspiratori e ventilatori (`Switch` / `Fan`), ideale per **bagni ciechi**, lavanderie, locali tecnici e ambienti dove il ricambio d’aria deve essere automatico, coerente con le condizioni reali e affidabile nel tempo.
<br>
Non è una semplice automazione on/off, ma una logica evoluta che supervisiona **sensori, attuatori e timer** per garantire un funzionamento stabile, continuo e ottimizzato.
</details>

<details>
<summary><strong>Cosa lo rende diverso</strong></summary>
  
| Funzione | Vantaggio |
|---|---|
| **Selezione dinamica delle entità** | Configurazione semplice direttamente da interfaccia |
| **Controllo evoluto dell’umidità** | Attivazione solo dopo permanenza sopra soglia |
| **Gestione presenza** | Ventilazione più intelligente durante e dopo l’utilizzo |
| **Timer avanzati** | Controllo preciso di permanenza, durata e riattivazione |
| **Sincronizzazione stato reale/logico** | Maggiore affidabilità anche in caso di spegnimenti indesiderati |
| **Architettura fail-safe** | Gestione robusta di anomalie, stati invalidi e incoerenze |
</details>

<details>
<summary><strong>Vantaggi principali</strong></summary>
  
- Configurazione intuitiva tramite selettori dedicati
- Compatibile con attuatori `Switch` e `Fan`
- Pensato per l’uso reale, non per semplici automazioni base
- Riduce falsi avvii, incoerenze e comportamenti instabili
- Trasforma un aspiratore tradizionale in un sistema di ventilazione intelligente
- Ideale con relè smart, ad esempio **Shelly**
</details>

<details>
<summary><strong>Scenario tipico</strong></summary>
  
  Un classico caso d’uso è il **bagno cieco** con:
- aspiratore tradizionale
- sensore di umidità
- sensore presenza
- relè smart

**Risultato:** una ventilazione completamente automatica, più intelligente, più affidabile e più professionale rispetto a una logica standard.
</details>

<details>
  <summary><strong>Requisiti</strong></summary>
  
- **[Home Assistant](https://www.home-assistant.io/installation/)**
- 1 attuatore (`Switch` oppure `Fan`)
- 1 sensore umidità
- 1 sensore presenza
<br>
**Add-on consigliato:** `File Editor`
</details>

<details>
<summary><strong>Installazione</strong></summary>

<strong>1</strong> Verificare se nel File <strong>configuration.yaml</strong>, contenuto all'interno della cartella <strong>config</strong> di Home Assistant, è presente il seguente Codice: <br>
<pre style="font-size:10px; background-color: #d9ffcc;">
  homeassistant:
    packages: !include_dir_named packages/
</pre>
<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/102819027/282229181-536ce9c7-e1ba-4baa-9967-c8a91ebc4920.png" alt="immagine" style="width:40%;">
, diversamente inserirlo, salvare il File <strong>configuration.yaml</strong> e riavviare Home Assistant (Impostazioni->Strumenti per sviluppatori->Riavvia->Riavvia Home Assistant);<br>
<br>
<strong>2</strong> Verificare la presenza della cartella <strong>packages</strong> all'interno della cartella <strong>config</strong> del Server Home Assistant; se non è presente, creare tramite l'**Add-on consigliato:** `File Editor`, l'intero percorso ovvero <strong>\\192.168.1.xxx\config\packages\aspiratore\master</strong>;<br>
<br>
<strong>3</strong> All'interno del percorso <strong>\\192.168.1.xxx\config\packages\aspiratore\master</strong> copiare i Files seguenti, presenti nella scheda <strong>CODE</strong> -> <strong>Download ZIP</strong><br>
<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/102819027/282228959-a62322f6-cc44-4acb-bc54-355e36349009.png" alt="immagine" style="width:30%;">

<pre style="font-size:10px; background-color: #d9ffcc;">
      - aspiratore_master.yaml
      - aspiratore_master_automazione_gestione_totale_sistema.txt
      - aspiratore_master_automazione_verifica_spia_umidita.txt
      - aspiratore_master_automazione_verifica_spia_rilevamento.txt
      - aspiratore_master_scheda_manuale_interfaccia.txt
</pre>

<br>
<strong>4</strong> In Home Assistant andare in <strong>Impostazioni -> Automazioni e scene -> CREA AUTOMAZIONE -> Crea una nuova automazione</strong> -> cliccare in alto a destra sui <strong>... puntini</strong> -> <strong>modifica in yaml</strong> -> cancellare tutto il codice e incollare il contenuto del file <strong>aspiratore_master_automazione_gestione_totale_sistema.txt</strong>salvare e tornare nuovamente in  <strong>Automazioni e scene</strong>;<br>
<br>
<strong>5</strong> Ripetere il Passaggio 5 per i restanti Files:
<pre style="font-size:10px; background-color: #d9ffcc;">
      - aspiratore_master_automazione_verifica_spia_umidita.txt
      - aspiratore_master_automazione_verifica_spia_rilevamento.txt
</pre>
<br>
<strong>7</strong> In Home Assistant andare in <strong>Panoramica</strong> -> cliccare in alto a destra sul <strong>pennino</strong> -> <strong>Aggiungi Scheda</strong> -> <strong>Manuale</strong> -> Selezionare tutto il Codice, cancellare tutto il codice e incollare il contenuto del file <strong>aspiratore_master_scheda_manuale_interfaccia.txt</strong> e salvare.
<br>
<strong>8</strong> Per maggiori informazioni andare sul Pannello Informazioni.<br>
<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/102819027/282228208-01c799a0-b92a-406f-939f-9c06006360a7.png" alt="immagine" style="width:30%;"><br>
</details>













<details>
<summary><strong>Configurazione</strong></summary>
  
La configurazione avviene direttamente da interfaccia tramite:
- `Selezione Attuatore`
- `Selezione Sensore Umidità`
- `Selezione Sensore Rilevamento`

Questo consente di cambiare dispositivi senza modificare manualmente lo YAML a ogni variazione.
</details>





































<details>
<summary><strong>Esonero di responsabilità</strong></summary>

In nessun caso l’Ing. Danilo Robotti potrà essere ritenuto responsabile per danni diretti, indiretti o conseguenti derivanti dall’uso del presente software.
</details>

---
<p align="center">
  Se il progetto ti è stato utile e desideri supportarne lo sviluppo, scansiona il QR code qui sotto</p>
<p align="center">
  <img src="https://github.com/DanRobo76/VMC-HELTY-FLOW/assets/102819027/81ba7208-fbad-4fab-8ceb-cdcf901fdb61.png" alt="QR Code Donazione" width="220">
</p>
