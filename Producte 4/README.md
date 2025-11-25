# 🧩 Publicació de Configuracions DNS a GitHub

👋 **Benvinguts, consultors!**

Com a membres de l'equip de sistemes d’EverPia, heu completat la configuració d’un servidor de noms com a prova de concepte per al nostre client **Digicore**. Actualment, el resultat es troba en una màquina virtual, i ara l’objectiu és **publicar aquestes configuracions a GitHub**.

Això permetrà que, quan sigui necessari replicar la configuració, no calgui començar des de zero: només descarregar els arxius al servidor Linux triat i reiniciar el servei per tenir el servidor completament operatiu. 🚀

---

## 🔧 Fase 1: Preparació de la Connectivitat i Extracció dels Arxius

Per poder copiar fitxers de la màquina virtual *Ubuntu Server* al vostre *host*, cal assegurar la connectivitat de xarxa.

### 🔌 Pas 1.1: Configuració de la Interfície Host-Only

1. ➕ Afegiu una **segona interfície de xarxa** a la vostra màquina virtual.  
2. 🔄 Assigneu-li el mode **Host-Only** i activeu-la.  
3. 📡 Comproveu la connectivitat des de la màquina física.

### 🔐 Pas 1.2: Còpia Segura dels Fitxers Clau amb SCP

Un cop establerta la connectivitat Host-Only, utilitzareu **SCP (Secure Copy Protocol)** per transferir els fitxers de configuració.

📁 **Arxius a copiar:**
- `/etc/bind/named.conf.options`
- `/etc/bind/named.cof.local`
- Arxius de zones dins `/etc/bind/zones/`

▶️ **Exemple de comanda SCP:**
`scp usuari@IP_MV:/etc/bind/named.conf.options .`

El punt (`.`) indica que l’arxiu es copiarà al directori actual. 📥

---

## 🗂️ Fase 2: Integració a GitHub

### 📝 Pas 2.1: Crear carpeta i README.md

1. Creeu la carpeta `producte04` i l’arxiu `README.md`.
2. GitHub crea la carpeta automàticament si escriviu:  
   `producte04/README.md`

✍️ Al README.md cal incloure:
- El títol del producte  
- Una explicació del contingut  

### 📤 Pas 2.2: Pujar arxius

⚠️ Abans de pujar els arxius de zones, creeu la carpeta `zones/`.

💡 Truquet útil:  
Creeu un fitxer temporal `zones/esborrar` per poder pujar la carpeta.  
Quan els arxius reals estiguin pujats, elimineu-lo 🗑️.

---

🎉 **I amb això ja tindreu el vostre projecte organitzat, pujat i llest per ser reutilitzat!**
