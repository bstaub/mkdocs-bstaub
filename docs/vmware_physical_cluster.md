# Physical 3-Node Cluster Setup

## Aufgabenliste für den Aufbau eines phyikalischen 3-Node VSAN Clusters

### Vorbereitungen
1. IDRAC Zugang prüfen
   - Zugang zu allen drei Servern über IDRAC sicherstellen
   - Firmware-Versionen überprüfen und ggf. aktualisieren

### Netzwerkdesign
1. Netzwerkplan erstellen
   - Drei Netzwerke definieren: Frontend, VSAN, Management
   - IP-Adressbereiche festlegen
   - VLANs konfigurieren (falls notwendig)

2. Netzwerkinterfaces konfigurieren
   - NIC1: Frontend Netzwerk
   - NIC2: VSAN Netzwerk
   - NIC3: Management Netzwerk

### VSAN Cluster Aufbau
1. ESXi Installation
   - ESXi auf allen drei Servern installieren
   - Netzwerksettings konfigurieren

2. vCenter Server installieren und konfigurieren
   - vCenter Server aufsetzen und konfigurieren
   - ESXi Hosts zum vCenter hinzufügen

3. Netzwerkkonfiguration in vCenter
   - Standard-Switches und Portgruppen erstellen
   - Netzwerkadapter den Portgruppen zuweisen

4. VSAN Konfiguration
   - VSAN Cluster im vCenter erstellen
   - Hosts zum VSAN Cluster hinzufügen
   - Diskgruppen erstellen und zuweisen

### Prüfung und Tests
1. VSAN Health Check durchführen
   - Funktionalität prüfen und Fehler beheben

2. Netzwerkverbindungen testen
   - Funktionalität der Netzwerke sicherstellen

3. Performance Tests durchführen
   - Grundlegende Performance-Tests durchführen

### Dokumentation
1. Dokumentation erstellen
   - Konfigurationsschritte und Netzwerkeinstellungen dokumentieren
   - Zugänge und IP-Adressen vermerken

