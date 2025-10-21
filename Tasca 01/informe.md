# 🧠 Informe Tècnic – Avaluació de Gestors de Contrasenyes

## 1️⃣ Introducció i Justificació
L’incident sofert per **EverPia** demostra com les **contrasenyes febles o reutilitzades** són un risc crític 🔥 per a la seguretat corporativa.  
Aquestes vulnerabilitats permeten atacs com:

- 🧩 **Atac de diccionari:** proves sistemàtiques de paraules comunes.
- 💣 **Credential stuffing:** ús de credencials robades d’altres serveis.
- 🧨 **Brute force:** generació massiva de combinacions fins trobar la correcta.

👉 Un **gestor de contrasenyes** és una eina essencial per mitigar aquests riscos:
- 🔒 Genera contrasenyes úniques i robustes.
- 🧱 Emmagatzema les credencials de forma xifrada.
- 📲 Facilita l’accés segur des de múltiples dispositius.

---

## 2️⃣ Comparativa Tècnica

| 🧩 Característica | ☁️ **Bitwarden (Online / Núvol)** | 💻 **KeePassXC (Offline / Escriptori)** |
|------------------|-----------------------------------|---------------------------------------|
| 🔐 **Model de seguretat** | Xifratge *end-to-end* (AES-256, PBKDF2, Argon2) | Xifratge AES-256 amb clau mestra local |
| 📍 **Ubicació de dades** | Núvol (Bitwarden Cloud o servidor propi) | Arxiu local `.kdbx` |
| 🔁 **Sincronització** | Automàtica entre dispositius | Manual (USB, Nextcloud...) |
| 🧩 **Codi font** | Open Source (AGPLv3) | Open Source (GPLv2) |
| 💰 **Cost / Model** | Freemium (versió gratuïta + Premium econòmic) | Totalment gratuït |
| 🌐 **Accessibilitat** | Web, escriptori, mòbil, navegador | Només escriptori |
| ⚙️ **Funcions addicionals** | Compartició segura, 2FA, carpetes | Plugins, portabilitat, control total |

---

## 3️⃣ Avantatges i Inconvenients

### ☁️ Bitwarden
**✅ Avantatges**
- Sincronització automàtica entre dispositius.
- Interfície moderna i intuïtiva. 🖥️
- Autenticació multifactor (2FA) integrada. 🔑
- Possibilitat d’instal·lar servidor propi. 🏗️

**❌ Inconvenients**
- Dependència del núvol (possible vector d’atac).
- Algunes funcions requereixen versió Premium.

---

### 💻 KeePassXC
**✅ Avantatges**
- Control total de les dades (sense núvol). 🧱  
- Codi obert i totalment gratuït. 🆓  
- Portabilitat mitjançant USB o entorns aïllats. 💾  

**❌ Inconvenients**
- Sense sincronització automàtica.  
- Interfície menys moderna.  
- Necessitat de còpies de seguretat manuals. 🔄  

---

## 4️⃣ Recomanació Final

Des del punt de vista de **seguretat, usabilitat i gestió centralitzada**, la millor opció per a l’equip tècnic és 👉 **Bitwarden**.

🧾 **Motivació:**
- Xifratge fort *end-to-end* i autenticació 2FA.
- Sincronització automàtica i accés multi-dispositiu.
- Projecte *open source* auditable.
- Possibilitat de desplegar-lo internament (*self-hosted*).

🟢 **Conclusió:**  
**Bitwarden** combina seguretat, facilitat d’ús i escalabilitat.  
És la millor solució per millorar la higiene digital d’EverPia i reduir riscos futurs. 🔐🚀
