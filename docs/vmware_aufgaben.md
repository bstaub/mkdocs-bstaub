# Lehrlingsaufgaben für den ESXi-Cluster

## Aufgabe 1: Erstellen und Konfigurieren einer Virtuellen Maschine

1. **Ziel**: Erstellen einer neuen virtuellen Maschine (VM) und Konfiguration der grundlegenden Einstellungen.
2. **Schritte**:
    - Melden Sie sich am vSphere Client an.
    - Navigieren Sie zu Ihrem ESXi-Host.
    - Wählen Sie "Neue virtuelle Maschine erstellen".
    - Geben Sie der VM einen Namen und wählen Sie den Speicherort aus.
    - Konfigurieren Sie die grundlegenden Hardwareeinstellungen (CPU, RAM, Festplatte, Netzwerkadapter).
    - Installieren Sie ein Betriebssystem Ihrer Wahl (z.B. Windows oder Linux).
    - Starten Sie die VM und überprüfen Sie, ob das Betriebssystem korrekt installiert wurde.

## Aufgabe 2: Netzwerkkonfiguration einer VM

1. **Ziel**: Konfigurieren der Netzwerkeinstellungen einer bestehenden VM.
2. **Schritte**:
    - Melden Sie sich am vSphere Client an.
    - Wählen Sie die VM aus, die Sie konfigurieren möchten.
    - Gehen Sie zu den Einstellungen der VM.
    - Fügen Sie einen zusätzlichen Netzwerkadapter hinzu oder konfigurieren Sie den vorhandenen Adapter.
    - Stellen Sie sicher, dass die VM eine gültige IP-Adresse erhält (entweder statisch oder über DHCP).
    - Testen Sie die Netzwerkverbindung von innerhalb der VM (z.B. mittels Ping-Befehl).

## Aufgabe 3: Snapshots erstellen und wiederherstellen

1. **Ziel**: Erstellen eines Snapshots einer VM und Wiederherstellen der VM von einem Snapshot.
2. **Schritte**:
    - Melden Sie sich am vSphere Client an.
    - Wählen Sie die VM aus, von der Sie einen Snapshot erstellen möchten.
    - Klicken Sie auf "Snapshots" und wählen Sie "Snapshot erstellen".
    - Geben Sie dem Snapshot einen Namen und eine Beschreibung.
    - Führen Sie einige Änderungen an der VM durch (z.B. Installieren von Software).
    - Stellen Sie die VM von dem zuvor erstellten Snapshot wieder her und überprüfen Sie, ob die Änderungen rückgängig gemacht wurden.

## Aufgabe 4: Ressourcenmanagement

1. **Ziel**: Überwachen und Anpassen der Ressourcenverteilung für VMs.
2. **Schritte**:
    - Melden Sie sich am vSphere Client an.
    - Navigieren Sie zu Ihrem ESXi-Host und wählen Sie den Ressourcenmonitor aus.
    - Überprüfen Sie die CPU- und RAM-Auslastung der einzelnen VMs.
    - Passen Sie die Ressourcenverteilung für eine VM an (z.B. CPU oder RAM erhöhen oder verringern).
    - Überwachen Sie die Auswirkungen der Änderungen auf die Performance der VM und des Hosts.

## Aufgabe 5: Datensicherung und -wiederherstellung

1. **Ziel**: Erstellen und Wiederherstellen von Backups für eine VM.
2. **Schritte**:
    - Melden Sie sich am vSphere Client an.
    - Wählen Sie eine VM aus, die gesichert werden soll.
    - Nutzen Sie ein Backup-Tool (z.B. Veeam Backup & Replication) zur Erstellung eines Backups.
    - Speichern Sie das Backup auf einem externen Speicherort.
    - Löschen Sie die VM (nach Rücksprache mit dem Ausbilder).
    - Stellen Sie die VM aus dem Backup wieder her und überprüfen Sie die Integrität der Daten.

## Aufgabe 6: Automatisierung mit Skripten

1. **Ziel**: Automatisieren von Aufgaben im ESXi-Cluster mittels Skripten.
2. **Schritte**:
    - Erstellen Sie ein PowerCLI-Skript, um mehrere VMs mit spezifischen Konfigurationen zu erstellen.
    - Das Skript sollte Folgendes beinhalten:
        - Namen für die VMs generieren
        - Hardwarekonfiguration festlegen (z.B. CPU, RAM, Festplatte)
        - Netzwerkadapter konfigurieren
    - Führen Sie das Skript aus und überprüfen Sie, ob die VMs korrekt erstellt wurden.
    - Dokumentieren Sie den Skript-Code und die Ausführungsschritte.


