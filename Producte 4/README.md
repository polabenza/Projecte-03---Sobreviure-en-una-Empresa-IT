# Publicació de Configuracions DNS a GitHub

Molt benvinguts a la vostra nova tasca, consultors!

Com a membres de l'equip de sistemes d'EverPia, us heu enfrontat al repte de configurar un servidor de noms com a prova de concepte pel nostre client **Digicore**, però ara mateix el resultat de la vostra feina es troba en una màquina virtual.

L’objectiu és poder publicar aquestes configuracions a **GitHub**. D’aquesta manera assegurem que, quan es vulgui replicar la configuració, no caldrà començar des de zero: serà suficient descarregar els arxius dins del servidor Linux triat i reiniciar el servei per tenir el servidor completament operatiu.

---

## **Fase 1: Preparació de la Connectivitat i Extracció dels Arxius**

Per poder copiar fitxers de la vostra màquina virtual *Ubuntu Server* a la vostra màquina física (*host*), heu d'assegurar la connectivitat de xarxa.

### **Pas 1.1: Configuració de la Interfície Host-Only**

1. Afegiu una segona interfície de xarxa a la màquina virtual i assigneu-li el mode **Host-Only**.  
2. Configureu-la i activeu-la.  
3. Comproveu que teniu connectivitat des de la màquina física.

### **Pas 1.2: Còpia Segura dels Fitxers Clau amb SCP**

Un cop establerta la connectivitat *Host-Only*, utilitzareu el protocol **SCP (Secure Copy Protocol)**, inclòs amb el servei SSH, per transferir els fitxers de configuració a la vostra màquina física.

Els arxius a copiar són els treballats en la tasca del servidor DNS:


