# Home Assistant Automatisierung: Mark PC LED

Eine smarte Home Assistant Automatisierung, die deine Schreibtisch-Beleuchtung (LEDs) und dein Nanoleaf-Panel automatisch mit dem Betriebsstatus deines PCs synchronisiert. Als Statusquelle dient ein Ping-Check über **Uptime Kuma** (ausgeführt als App/Integration in Home Assistant).

## 🚀 Funktionen

* **PC ist online / pingbar (`up`):** Die Schreibtisch-LEDs und das Nanoleaf-Panel werden automatisch eingeschaltet.
* **PC ist offline / nicht erreichbar (`down`):** Sowohl das Nanoleaf als auch die Schreibtisch-LEDs werden automatisch ausgeschaltet.

## 📋 Voraussetzungen

* Ein eingerichtetes [Home Assistant](https://www.home-assistant.io/)-System.
* **Uptime Kuma** (integriert in Home Assistant) mit einem eingerichteten Ping-Monitor für den PC. Im Standard-Code wird der daraus resultierende Entitäts-Sensor `sensor.desktop_mark_jarvis_status_2` verwendet.
* Entsprechende smarte Leuchtmittel (z. B. `light.nanoleaf` und eine konfigurierte LED-Leuchte).

## ⚙️ Installation & Einrichtung

1. Erstelle in deinem GitHub-Repository eine neue Datei namens `README.md`.
2. Kopiere den YAML-Code der Automatisierung in dein Home Assistant (unter **Einstellungen** > **Automatisierungen & Szenen** > **Automatisierung erstellen** > *In YAML bearbeiten*).
3. **Wichtig:** Passe die Entitäts-IDs (`sensor.desktop_mark_jarvis_status_2`, `light.nanoleaf`, etc.) an deine eigenen Home-Assistant-Geräte an. Der Sensor muss auf den Status deines Uptime-Kuma-Monitors verweisen (`up` / `down`).
4. Speichere die Automatisierung ab.
