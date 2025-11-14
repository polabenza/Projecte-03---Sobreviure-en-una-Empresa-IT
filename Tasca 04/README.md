# 🚀 Innovatech: Problemes d'Autenticació i Proposta de Solució

**Innovatech**, una *start-up* tecnològica emergent, està experimentant un ràpid creixement i pateix un **caos en la gestió dels seus usuaris i accessos**.

Actualment, cada servei intern (servidor de fitxers, wiki de documentació, etc.) utilitza la seva pròpia base de dades d'usuaris i contrasenyes, i a més als ordinadors clients s’usa **autentificació local**.  
Això genera diversos problemes crítics:

---

## ⚠️ Problemes Actuals

### 🔁 Ineficiència Operativa
Cada cop que s'incorpora o marxa un empleat, l'equip tècnic ha de crear o eliminar el compte en **múltiples sistemes**.

### 🔐 Risc de Seguretat
Els usuaris sovint acaben reutilitzant contrasenyes entre serveis per evitar l'oblit.

### 📉 Manca d'Escalabilitat
A mesura que Innovatech afegeix nous serveis, el problema es torna **insostenible**.

---

## 🛠️ La Solució: Autenticació Centralitzada amb OpenLDAP

El CEO d’Innovatech ha contactat amb **EverPia** per implementar una solució d’autenticació centralitzada.  
La proposta és utilitzar **OpenLDAP (Lightweight Directory Access Protocol)**, una solució:

- 💪 Robusta  
- 🧩 De codi obert  
- 🐧 Totalment compatible amb l'entorn GNU/Linux de l’empresa  

---

## 🎯 Missió

La vostra tasca serà:

1. 🏗️ **Implementar el servei OpenLDAP** en un servidor Linux.  
2. ⚙️ **Configurar el domini base**.  
3. 🌳 **Crear la jerarquia d'unitats organitzatives (OU)**.  
4. 👥 **Afegir usuaris i grups** que després es faran servir per accedir a altres serveis de xarxa.  
5. 🖥️ **Configurar un equip client** perquè utilitzi el directori per autenticar usuaris.  
