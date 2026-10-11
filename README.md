# Home Assistant Automatisierung: Mark PC LED

Eine smarte Home Assistant Automatisierung, die deine Schreibtisch-Beleuchtung (LEDs) und dein Nanoleaf-Panel automatisch mit dem Betriebsstatus deines PCs synchronisiert.

## 🚀 Funktionen

* **PC fährt hoch / wird aktiv (`up`):** Die Schreibtisch-LEDs und das Nanoleaf-Panel werden automatisch eingeschaltet.
* **PC fährt herunter / schaltet ab (`down`):** Sowohl das Nanoleaf als auch die Schreibtisch-LEDs werden automatisch ausgeschaltet.

## 📋 Voraussetzungen

* Ein eingerichtetes [Home Assistant](https://www.home-assistant.io/)-System.
* Ein Sensor, der den Status deines PCs überwacht (z. B. über [HASS.Agent](https://github.com/HASS.Agent-org/HASS.Agent), MQTT oder Windows-Integrationen). Im Standard-Code wird der Sensor `sensor.desktop_mark_jarvis_status_2` verwendet.
* Entsprechende smarte Leuchtmittel (z. B. `light.nanoleaf` und eine konfigurierte LED-Leuchte).

## ⚙️ Installation & Einrichtung

1. Erstelle in deinem GitHub-Repository eine neue Datei namens `README.md` (oder füge den Inhalt dort ein).
2. Kopiere den YAML-Code aus der Automatisierungs-Datei dieses Repositories.
3. Öffne dein Home Assistant Dashboard.
4. Navigiere zu **Einstellungen** > **Automatisierungen & Szenen** > **Automatisierung erstellen**.
5. Klicke oben rechts auf die drei Punkte (`...`) und wähle **In YAML bearbeiten**.
6. Füge den Code ein.
7. **Wichtig:** Passe die Entitäts-IDs (`sensor.desktop_mark_jarvis_status_2`, `light.nanoleaf`) sowie die Geräte-ID an deine eigenen Home-Assistant-Geräte an!
8. Speichere die Automatisierung ab.
