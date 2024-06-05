# Arbeitsanweisung Aufbau Nested Cluster

### Arbeitsanweisung für den Aufbau eines Nested Two-Node VMware vSAN Clusters

#### 1. Vorbereitung und Überblick

Ziel dieser Übung ist es, eine neue vAPP mit dem Namen `Nested2NodesvSANCluster_yourname` zu erstellen und darin drei nested ESXi Server (zwei ESXi Worker Nodes und ein Witness Node) sowie ein nested vCenter zu deployen. Die entsprechenden Images werden in einem Scratch-Bereich bereitgestellt. Eine bestehende Nested vSphere-vSAN8 Umgebung (Nested2NodevSANCluster_bstaub) kann für Sizing-Analysen verwendet und VMs von dieser Umgebung geklont werden. Es darf zu keinen IP-Konflikten kommen; daher müssen die IPs eindeutig vergeben werden.

#### 2. IP-Adressliste erstellen

Bevor mit dem Deployment begonnen wird, muss eine klare IP-Adressliste definiert werden. Diese Liste enthält die IP-Adressen für alle zu erstellenden virtuellen Maschinen (VMs).

##### Beispielhafte IP-Adressliste:

| Komponente             | Hostname                  | IP-Adresse      |
|------------------------|---------------------------|-----------------|
| vCenter                | vcsa_yourname             | 192.168.100.10  |
| ESXi Worker Node 1     | esxi1_yourname            | 192.168.100.11  |
| ESXi Worker Node 2     | esxi2_yourname            | 192.168.100.12  |
| Witness Node           | witness_yourname          | 192.168.100.13  |

#### 3. Schritt-für-Schritt-Anleitung

##### Schritt 1: Erstellung der vAPP

1. **Anmeldung an der Testumgebung**:
   - URL: [https://vilab.campus.intern](https://vilab.campus.intern){:target="_blank"}
   - Anmeldedaten verwenden, die Ihnen zur Verfügung gestellt wurden.

2. **vAPP erstellen**:
   - Navigieren Sie zu dem vSphere Client und erstellen Sie eine neue vAPP mit dem Namen `Nested2NodesvSANCluster_yourname`.

##### Schritt 2: Deployment der nested ESXi Server und vCenter

1. **Scratch-Bereich für Images durchsuchen**:
   - Lokalisieren Sie die bereitgestellten Images im Scratch-Bereich.

2. **Deployment der ESXi Server**:
   - Deployen Sie zwei ESXi Worker Nodes und einen Witness Node mit den entsprechenden Images.
   - Konfigurieren Sie die Netzwerkeinstellungen gemäß der definierten IP-Adressliste.

3. **Deployment des vCenters**:
   - Deployen Sie das vCenter und konfigurieren Sie es mit der entsprechenden IP-Adresse.

##### Schritt 3: Konfiguration des vSAN Clusters

1. **ESXi Server zu vCenter hinzufügen**:
   - Melden Sie sich beim vCenter an und fügen Sie die beiden ESXi Worker Nodes und den Witness Node zum vCenter hinzu.

2. **Erstellung und Konfiguration des vSAN Clusters**:
   - Erstellen Sie einen neuen vSAN Cluster und fügen Sie die beiden ESXi Worker Nodes und den Witness Node hinzu.
   - Stellen Sie sicher, dass der vSAN-Datenspeicher korrekt konfiguriert ist.

##### Schritt 4: Analyse und Klonen von VMs (Optional)

1. **Bestehende Umgebung analysieren**:
   - Analysieren Sie die bestehende Nested vSphere-vSAN8 Umgebung (`Nested2NodevSANCluster_bstaub`) hinsichtlich Sizing und Konfiguration.

2. **VMs klonen**:
   - Klonen Sie gegebenenfalls VMs aus der bestehenden Umgebung und fügen Sie diese in Ihre neu erstellte Umgebung ein. Achten Sie dabei darauf, IP-Konflikte zu vermeiden.

#### 4. Dokumentation

Dokumentieren Sie alle durchgeführten Arbeitsschritte. Die Dokumentation sollte folgende Punkte umfassen:

1. **Erstellte vAPP**: Name und Konfigurationsdetails.
2. **Deployment der ESXi Server und des vCenters**: Vorgehensweise, IP-Adressen, und Netzwerkeinstellungen.
3. **Konfiguration des vSAN Clusters**: Details zur Cluster-Erstellung und vSAN-Konfiguration.
4. **Analyse und Klon-Vorgänge** (falls durchgeführt): Details zu analysierten und geklonten VMs.

#### 5. Abschluss

Nach Abschluss der Arbeiten überprüfen Sie die Funktionalität des vSAN Clusters und der VMs. Stellen Sie sicher, dass alle Komponenten ordnungsgemäß funktionieren und dokumentieren Sie eventuelle Probleme sowie deren Lösungen.



Diese Anleitung dient als Leitfaden und soll sicherstellen, dass die Einrichtung des Nested Two-Node VMware vSAN Clusters strukturiert und ohne IP-Konflikte erfolgt. Alle Schritte sollten sorgfältig durchgeführt und dokumentiert werden.