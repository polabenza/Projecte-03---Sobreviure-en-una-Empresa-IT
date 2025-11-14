# 🧩 Implantació d’un Sistema DNS Intern amb BIND9

Després de l’exitosa experiència en formació, els nostres clients de **Digicore** estan tan satisfets amb la nostra feina que ens encarreguen la implantació *des de zero* dels seus serveis de **DNS interns**. 🖥️🌐

Actualment, l'agència utilitza **adreces IP** per accedir als seus servidors de desenvolupament, bases de dades i eines de gestió interna. Aquest mètode presenta diversos inconvenients:

## ❌ Problemes de la situació actual
- 🔢 **Usabilitat deficient**: Els empleats han de memoritzar o buscar constantment adreces IP complexes (p. ex., `192.168.10.25`).
- 🛠️ **Manteniment feixuc**: Si un servidor canvia la seva IP, cal notificar i actualitzar manualment configuracions a tots els equips i aplicacions.
- 🏢 **Manca de professionalitat**: Tots els serveis d’un entorn professional haurien de ser accessibles amb noms fàcils de recordar.

---

# 🎯 Objectiu del projecte

Implementar un **Sistema de Noms de Domini (DNS)** intern robust perquè els servidors i aplicacions de l'agència siguin accessibles mitjançant noms de domini amigables, per exemple:

- `bbdd.digicore.lan`
- `wiki.digicore.lan`

La prova de concepte utilitzarà el domini:

📌 **`digicore-XX.test`**, on **XX** és el vostre número de llista.

---

# 🛠️ Solució proposada: BIND9

La recomanació com a consultora és utilitzar **BIND9**, l'estàndard de facto a Linux, conegut per:

- ⚙️ Fiabilitat  
- 🧩 Flexibilitat  
- 🛡️ Robustesa  

La missió és instal·lar i configurar un **servidor DNS primari (màster)** amb:

- 📁 **Zona Directa (Forward Zone)**  
- 🔄 **Zona Inversa (Reverse Zone)**  

Això garantirà què:
- Els noms ➜ es resolguin a IPs  
- Les IPs ➜ es resolguin a noms  

---

# 🖥️ Pas previ: Configuració del servidor

Per començar, cal configurar una màquina virtual **Ubuntu Server** amb:

- 🧠 **4 GB de RAM**
- 💾 **20 GB de disc**
- 🌉 **Una interfície en adaptador pont**
- 🔌 **Una segona interfície en host-only**

Un cop aixecada la màquina:

1. 📦 Instal·lar el paquet **`bind9`**
2. 🔐 Instal·lar el servei **SSH** per poder exportar més endavant els arxius de configuració al vostre **repositori de GitHub**

---


