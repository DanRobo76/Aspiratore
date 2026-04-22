## ASPIRATORE sviluppato per Home Assistant
<a href="https://www.home-assistant.io/" target="_blank"><img src="https://user-images.githubusercontent.com/102819027/233830183-9c55677d-b6a1-4153-8d3c-219394ec8720.png" alt="immagine" style="width:10%;"></a> 

<pre style="font-size:10px; background-color: #d9ffcc;">
E-mail: <a href="mailto:danilo.robotti@gmail.com">danilo.robotti@gmail.com</a>
</pre>

<strong>Esonero di Responsabilità:</strong><br>
In nessun caso l'Ing. Danilo Robotti sarà responsabile di danneggiamenti diretti, indiretti, o conseguenti, correlati a difetti del presente SoftWare. 
Il Cliente ha l’onere e la responsabilità della scelta, dell’installazione, dell’uso e della gestione del SoftWare al fine del raggiungimento del risultato prefissatosi. 
<strong><a href="https://github.com/DanRobo76/Aspiratore/blob/main/security.md" text="Limiti del SoftWare (Security Policy)">Limiti del SoftWare (Security Policy)</a></strong> 
#
<img width="40%" alt="Aspiratore" src="https://github.com/user-attachments/assets/0ea8134e-25e7-4141-9f81-8ef87ccb5fa8" />

<strong>Pre-Requisiti:</strong><br> 
<sub>- Installare <strong><a href="https://www.home-assistant.io/installation/">Home Assistant</a></strong>;</sub><br>
<sub>- Installare l'Add On [Facoltativo, ma Consigliato] <strong>File Editor</strong>, di Home Assistant; [Impostazioni -> Componenti aggiuntivi -> Raccolta di Componenti Aggiuntivi -> File editor].</sub><br>

#

<strong>Punti di Forza:</strong><br>
## Descrizione
# 🛠️ ASPIRATORE MASTER

**ASPIRATORE MASTER** è un package avanzato per Home Assistant progettato per la gestione intelligente di aspiratori e ventilatori (`Switch` / `Fan`).

È particolarmente indicato per ambienti come **bagni ciechi privi di finestra**, dove il ricambio d’aria deve essere completamente automatizzato, affidabile e coerente con le condizioni ambientali.

---

## 🚀 Caratteristiche principali

- 🔄 **Selezione dinamica delle entità (plug & play)**  
  Tramite **menu a tendina (dropdown)** è possibile selezionare:
  - Attuatore (`Switch` / `Fan`)
  - Sensore di umidità
  - Sensore di rilevamento presenza  

  Le liste vengono aggiornate automaticamente e includono solo entità valide, con gestione intelligente dei casi *unknown*, *unavailable* o placeholder.

---

- 💧 **Controllo avanzato dell’umidità**
  - Attivazione solo dopo un **tempo di permanenza sopra soglia**
  - Gestione soglia + offset configurabile
  - Prevenzione di falsi positivi e attivazioni impulsive

---

- ⏱️ **Gestione completa dei timer**
  - Timer di **permanenza umidità**
  - Timer di **controllo stato ( definisce quando riattivare l’attuatore dopo uno spegnimento manuale indesiderato.)**
  - Timer di **durata massima aspirazione**
  - Timer ciclico per garantire il mantenimento delle condizioni

---

- 👤 **Integrazione rilevamento presenza**
  - Attivazione ventilazione durante l’utilizzo dell’ambiente
  - Prolungamento intelligente del funzionamento post-utilizzo
  - Coordinamento completo con il dominio umidità

---

- 🔄 **Sincronizzazione stato reale / virtuale**
  - Allineamento continuo tra stato dell’attuatore e stato logico
  - Gestione degli spegnimenti manuali indesiderati
  - Riattivazione automatica se necessario

---

- 🛡️ **Architettura robusta (fail-safe & self-healing)**
  - Gestione completa di stati non validi (`unknown`, `unavailable`, ecc.)
  - Reset automatico in caso di incoerenze
  - Prevenzione loop e comportamenti instabili
  - Ripristino automatico del dominio operativo

---

## ⚙️ Funzionamento

Il sistema opera come un **supervisore intelligente** che:

- valida continuamente il dominio (sensori + attuatore)
- attiva il ventilatore solo in condizioni coerenti
- gestisce priorità tra **umidità** e **rilevamento**
- garantisce continuità operativa anche in caso di anomalie

---

## 🎯 Caso d’uso tipico

- Bagno cieco con aspiratore tradizionale  
- Collegamento tramite **relè smart (es. Shelly)**  
- Sensore di umidità + sensore presenza  

➡️ Risultato: sistema completamente automatico, senza intervento manuale.

---

## 🧠 Filosofia del progetto

ASPIRATORE MASTER non è una semplice automazione, ma un **framework logico modulare**, progettato secondo principi:

- **affidabilità operativa**
- **manutenibilità**
- **scalabilità**
- **controllo deterministico degli stati**

---

## 📌 Requisiti

- Home Assistant
- Almeno:
  - 1 attuatore (`Switch` o `Fan`)
  - 1 sensore umidità
  - 1 sensore presenza (opzionale ma consigliato)

---

## 🔧 Configurazione

La configurazione avviene **interamente da interfaccia**, tramite selettori:

- `Selezione Attuatore`
- `Selezione Sensore Umidità`
- `Selezione Sensore Rilevamento`

➡️ Nessuna modifica YAML necessaria per cambiare dispositivi.

---

## 📈 Obiettivo

Fornire un sistema di ventilazione:

- **intelligente**
- **autonomo**
- **robusto**
- **adattabile a qualsiasi ambiente**

---

## <span style="color:#663300">SchreenShot</span> - Possono variare in funzione dell'Ultima Versione Rilasciata
<img width="1188" height="896" alt="Collage" src="https://github.com/user-attachments/assets/9239a568-26b8-4582-bd70-9d76a5d8464f" />


#

#### Se il progetto ti è piaciuto <a href="https://www.paypal.com/donate/?business=YU9379GL8VDW4&amount=1.2&no_recurring=1&item_name=Se+il+progetto+ti+%C3%A8+piaciuto%2C++offrimi+un+GinSeng%21+%0A%3B%29&currency_code=EUR">Clicca Qui</a> per offrirmi un GinSeng! <a href="https://www.paypal.com/donate/?business=YU9379GL8VDW4&amount=1.2&no_recurring=1&item_name=Se+il+progetto+ti+%C3%A8+piaciuto%2C++offrimi+un+GinSeng%21+%0A%3B%29&currency_code=EUR"><img src="https://user-images.githubusercontent.com/102819027/233830035-709efa6b-94d7-4ea6-865b-76ab5c1eee6d.png" alt="immagine" style="width:3%;"></a>
<br>
oppure scansionare il seguente QR code:<img src="https://github.com/DanRobo76/VMC-HELTY-FLOW/assets/102819027/81ba7208-fbad-4fab-8ceb-cdcf901fdb61.png" alt="immagine" style="width:20%;">
<br>
