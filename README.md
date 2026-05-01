# ASPIRATORE MASTER - Smart Automation for Home Assistant

Scegli la lingua / Choose your language:

<details>
  <summary>🇮🇹 <strong>Italiano (Clicca per espandere)</strong></summary>

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

<br>

### 1. Abilitare il caricamento dei package in Home Assistant
Verificare che nel file <strong>configuration.yaml</strong>, presente nella cartella <strong>config</strong> del server Home Assistant, sia riportata la seguente configurazione:

<pre style="font-size:10px; background-color: #d9ffcc;">
homeassistant:
  packages: !include_dir_named packages/
</pre>

<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/102819027/282229181-536ce9c7-e1ba-4baa-9967-c8a91ebc4920.png" alt="immagine" style="width:40%;">

Se la configurazione non è presente, inserirla, salvare il file <strong>configuration.yaml</strong> e riavviare Home Assistant seguendo il percorso:
<strong>Impostazioni → Strumenti per sviluppatori → Riavvia → Riavvia Home Assistant</strong>.

---

### 2. Creare la cartella del package
Verificare la presenza della cartella <strong>packages</strong> all’interno della directory <strong>config</strong> del server Home Assistant.

Se la cartella non è presente, creare il seguente percorso:

<pre style="font-size:10px; background-color: #d9ffcc;">
\192.168.1.xxx\config\packages\aspiratore\master
</pre>

L’operazione può essere eseguita, ad esempio, tramite l’add-on <strong>File Editor</strong>.

---

### 3. Copiare i file del package
All’interno del percorso <strong>\192.168.1.xxx\config\packages\aspiratore\master</strong>, copiare i seguenti file scaricabili dal repository GitHub tramite:
<strong>Code → Download ZIP</strong>.

<img src="https://github.com/DanRobo76/Aspiratore/blob/main/immagini/Code.jpg" alt="immagine" style="width:30%;">

<pre style="font-size:10px; background-color: #d9ffcc;">
- aspiratore_master.yaml
- aspiratore_master_automazione_gestione_totale_sistema.txt
- aspiratore_master_automazione_verifica_spia_umidita.txt
- aspiratore_master_automazione_verifica_spia_rilevamento.txt
- aspiratore_master_scheda_manuale_interfaccia.txt
</pre>

---

### 4. Importare l’automazione principale
In Home Assistant seguire il percorso:

<strong>Impostazioni → Automazioni e scene → Crea automazione → Crea una nuova automazione</strong>

Successivamente:
- cliccare in alto a destra sui <strong>tre puntini</strong>;
- selezionare <strong>Modifica in YAML</strong>;
- eliminare il contenuto presente;
- incollare il contenuto del file <strong>aspiratore_master_automazione_gestione_totale_sistema.txt</strong>;
- salvare l’automazione.

Una volta salvata, tornare alla schermata <strong>Automazioni e scene</strong>.

---

### 5. Importare le altre automazioni
Ripetere la medesima procedura descritta al punto precedente per i seguenti file:

<pre style="font-size:10px; background-color: #d9ffcc;">
- aspiratore_master_automazione_verifica_spia_umidita.txt
- aspiratore_master_automazione_verifica_spia_rilevamento.txt
</pre>

---

### 6. Importare la scheda Lovelace
In Home Assistant seguire il percorso:

<strong>Panoramica → Modifica dashboard (icona matita) → Aggiungi scheda → Manuale</strong>

Successivamente:
- selezionare tutto il codice già presente;
- eliminarlo;
- incollare il contenuto del file <strong>aspiratore_master_scheda_manuale_interfaccia.txt</strong>;
- salvare la scheda.

---

### 7. Verifica finale
Al termine dell’installazione:
- verificare che il package sia stato correttamente caricato;
- verificare la presenza delle automazioni importate;
- verificare la corretta visualizzazione della scheda in dashboard;
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
  Se il progetto ti è stato utile e desideri
  <a href="https://www.paypal.com/donate/?business=YU9379GL8VDW4&amount=1.2&no_recurring=1&item_name=Se+il+progetto+ti+%C3%A8+piaciuto%2C++offrimi+un+GinSeng%21+%0A%3B%29&currency_code=EUR">
    supportarne lo sviluppo
  </a>,
  scansiona il QR code qui sotto
</p>
<p align="center"><img src="https://github.com/DanRobo76/VMC-HELTY-FLOW/assets/102819027/81ba7208-fbad-4fab-8ceb-cdcf901fdb61.png" alt="QR Code Donazione" width="220"></p>

</details>

<details>
  <summary>🇺🇸 <strong>English (Click to expand)</strong></summary>

<h1 align="center">
  ASPIRATORE MASTER 
  <a href="https://www.home-assistant.io/" target="_blank">
    <img src="https://user-images.githubusercontent.com/102819027/233830183-9c55677d-b6a1-4153-8d3c-219394ec8720.png" alt="Home Assistant" width="80">
  </a>
</h1>
<p align="center">
  <strong>The professional solution to automate exhaust fans and ventilators in Home Assistant.</strong><br>
  Smart control, robust logic, and truly reliable ventilation.
</p>

<p align="center">
  <a href="mailto:danilo.robotti@gmail.com">danilo.robotti@gmail.com</a>
</p>

<p align="center">
  <img src="https://github.com/DanRobo76/Aspiratore/blob/main/immagini/Collage%20Aspiratore.png" alt="ASPIRATORE MASTER" width="100%">
</p>

---
<details>
<summary><strong>Why ASPIRATORE MASTER</strong></summary>
  
**ASPIRATORE MASTER** is an advanced Home Assistant package designed for the smart management of exhaust fans and ventilators (`Switch` / `Fan`). It is ideal for **windowless bathrooms**, laundries, technical rooms, and environments where air exchange must be automatic, consistent with real conditions, and reliable over time.
<br>
It is not just a simple on/off automation, but an evolved logic that supervises **sensors, actuators, and timers** to ensure stable, continuous, and optimized operation.
</details>

<details>
<summary><strong>What makes it different</strong></summary>
  
| Function | Advantage |
|---|---|
| **Dynamic entity selection** | Simple configuration directly from the interface |
| **Advanced humidity control** | Activation only after remaining above threshold |
| **Presence management** | Smarter ventilation during and after use |
| **Advanced timers** | Precise control of dwell time, duration, and reactivation |
| **Real/logical state synchronization** | Greater reliability even in case of unintended shutdowns |
| **Fail-safe architecture** | Robust management of anomalies, invalid states, and inconsistencies |
</details>

<details>
<summary><strong>Main Benefits</strong></summary>
  
- Intuitive configuration via dedicated selectors
- Compatible with `Switch` and `Fan` actuators
- Designed for real-world use, not just basic automations
- Reduces false starts, inconsistencies, and unstable behaviors
- Transforms a traditional exhaust fan into a smart ventilation system
- Ideal for use with smart relays, such as **Shelly**
</details>

<details>
<summary><strong>Typical Scenario</strong></summary>
  
  A classic use case is a **windowless bathroom** with:
- traditional exhaust fan
- humidity sensor
- presence sensor
- smart relay

**Result:** fully automatic ventilation—smarter, more reliable, and more professional than standard logic.
</details>

<details>
  <summary><strong>Requirements</strong></summary>
  
- **[Home Assistant](https://www.home-assistant.io/installation/)**
- 1 actuator (`Switch` or `Fan`)
- 1 humidity sensor
- 1 presence sensor
<br>
**Recommended Add-on:** `File Editor`
</details>

<details>
<summary><strong>Installation</strong></summary>

<br>

### 1. Enable package loading in Home Assistant
Ensure that the <strong>configuration.yaml</strong> file, located in the <strong>config</strong> folder of your Home Assistant server, contains the following configuration:

<pre style="font-size:10px; background-color: #d9ffcc;">
homeassistant:
  packages: !include_dir_named packages/
</pre>

<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/102819027/282229181-536ce9c7-e1ba-4baa-9967-c8a91ebc4920.png" alt="image" style="width:40%;">

If the configuration is missing, add it, save the <strong>configuration.yaml</strong> file, and restart Home Assistant by navigating to:
<strong>Settings → Developer Tools → Restart → Restart Home Assistant</strong>.

---

### 2. Create the package folder
Verify the existence of the <strong>packages</strong> folder within the <strong>config</strong> directory of your Home Assistant server.

If the folder does not exist, create the following path:

<pre style="font-size:10px; background-color: #d9ffcc;">
\192.168.1.xxx\config\packages\aspiratore\master
</pre>

This can be done, for example, using the <strong>File Editor</strong> add-on.

---

### 3. Copy the package files
Within the <strong>\192.168.1.xxx\config\packages\aspiratore\master</strong> path, copy the following files downloadable from the GitHub repository via:
<strong>Code → Download ZIP</strong>.

<img src="https://github.com/DanRobo76/Aspiratore/blob/main/immagini/Code.jpg" alt="image" style="width:30%;">

<pre style="font-size:10px; background-color: #d9ffcc;">
- aspiratore_master.yaml
- aspiratore_master_automazione_gestione_totale_sistema.txt
- aspiratore_master_automazione_verifica_spia_umidita.txt
- aspiratore_master_automazione_verifica_spia_rilevamento.txt
- aspiratore_master_scheda_manuale_interfaccia.txt
</pre>

---

### 4. Import the main automation
In Home Assistant, navigate to:

<strong>Settings → Automations & Scenes → Create Automation → Create New Automation</strong>

Then:
- click the <strong>three dots</strong> in the top right corner;
- select <strong>Edit in YAML</strong>;
- delete the existing content;
- paste the content of the file <strong>aspiratore_master_automazione_gestione_totale_sistema.txt</strong>;
- save the automation.

Once saved, return to the <strong>Automations & Scenes</strong> screen.

---

### 5. Import other automations
Repeat the same procedure described in the previous step for the following files:

<pre style="font-size:10px; background-color: #d9ffcc;">
- aspiratore_master_automazione_verifica_spia_umidita.txt
- aspiratore_master_automazione_verifica_spia_rilevamento.txt
</pre>

---

### 6. Import the Lovelace card
In Home Assistant, navigate to:

<strong>Overview → Edit Dashboard (pencil icon) → Add Card → Manual</strong>

Then:
- select all existing code;
- delete it;
- paste the content of the file <strong>aspiratore_master_scheda_manuale_interfaccia.txt</strong>;
- save the card.

---

### 7. Final Verification
At the end of the installation:
- verify that the package has been correctly loaded;
- verify the presence of the imported automations;
- verify the correct display of the card in the dashboard.
</details>

<details>
<summary><strong>Configuration</strong></summary>
  
Configuration is done directly through the interface using:
- `Actuator Selection`
- `Humidity Sensor Selection`
- `Presence Sensor Selection`

This allows you to change devices without manually modifying the YAML for every change.
</details>

<details>
<summary><strong>Disclaimer</strong></summary>

In no event shall Eng. Danilo Robotti be held liable for any direct, indirect, or consequential damages arising from the use of this software.
</details>

---
<p align="center">
  If this project was useful and you wish to 
  <a href="https://www.paypal.com/donate/?business=YU9379GL8VDW4&amount=1.2&no_recurring=1&item_name=Se+il+progetto+ti+%C3%A8+piaciuto%2C++offrimi+un+GinSeng%21+%0A%3B%29&currency_code=EUR">
    support its development
  </a>,
  scan the QR code below
</p>
<p align="center"><img src="https://github.com/DanRobo76/VMC-HELTY-FLOW/assets/102819027/81ba7208-fbad-4fab-8ceb-cdcf901fdb61.png" alt="Donation QR Code" width="220"></p>

</details>
