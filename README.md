# Mobile RDS Encoder (Android) 📻

Der **Mobile RDS Encoder** ist eine Android-Applikation, die es ermöglicht, dynamische RDS-Informationen (Radio Data System) direkt in ein Stereo-Audiosignal einzubetten. Die Ausgabe erfolgt idealerweise über einen angeschlossenen USB-DAC (Digital-Analog-Wandler), um das Signal anschließend in einen FM-Transmitter einzuspeisen.

<img width="195" height="750" alt="Screenshot1" src="https://github.com/user-attachments/assets/41fd52df-065b-4b96-ba74-56fafe7754d7" />
<img width="346" height="750" alt="Bild2" src="https://github.com/user-attachments/assets/e0cd0ab2-b089-46de-bce1-12bdf4010ef6" />
<img width="346" height="750" alt="Bild3" src="https://github.com/user-attachments/assets/d20627a3-72df-4e29-b603-44e9a119fca8" />



## ✨ Features (Version 1.1)

*   **Basis-RDS-Parameter:** PI-Code, ECC, Programmtyp (PTY), Traffic Program (TP) und Traffic Announcement (TA).
*   **Alternative Frequenzen (AF):** Eingabe von bis zu 25 AF-Frequenzen.
*   **Dynamischer Sendername (PS):** Mehrere PS-Zeilen (max. 8 Zeichen) mit konfigurierbarem Wechselintervall.
*   **Dynamischer Radiotext (RT):** Mehrere RT-Zeilen (max. 64 Zeichen) inklusive automatischem A/B-Flag-Wechsel.
*   **Webradio-Integration:** Integrierter Player für Webradio-Streams inkl. automatischer Extraktion von ICY-Metadaten (Titel/Interpret), die auf Wunsch live als letzte Zeile in den Radiotext (RT) gestreamt werden.
*   **RDS-Kanal-Routing (Neu in v1.1):** Gezielte Ausgabe des generierten RDS-Signals wahlweise nur auf dem linken Kanal (LI), dem rechten Kanal (RE) oder auf beiden (LI+RE) – ideal für Split-Setups.
*   **Preset-Verwaltung:** Speichern, Laden und Updaten verschiedener Konfigurationen.
*   **Hintergrundbetrieb:** Die App läuft als Foreground-Service zuverlässig im Hintergrund weiter, auch wenn das Display ausgeschaltet ist.
*   **Live-Anzeige:** Visuelle Echtzeit-Darstellung des gesendeten RDS-Displays direkt in der App.

## 📥 Installation (APK)

1. Lade die aktuellste Version [hier](https://github.com/Highpoint2000/MobileRDSEncoder/blob/main/Mobile_RDS_Encoder_1.1.apk) herunter.
2. Erlaube auf deinem Android-Gerät die Installation von Apps aus "Unbekannten Quellen" (bzw. erteile die Berechtigung für deinen Browser/Dateimanager).
3. Öffne die APK-Datei und folge den Installationsanweisungen.

## 🔌 Hardware-Voraussetzungen

Für den echten Sendebetrieb wird empfohlen:
*   Ein Android-Smartphone oder Tablet mit USB-OTG-Unterstützung.
*   Ein externer 192 kHz USB-DAC (Audio-Interface / Soundkarte), der über einen USB-OTG-Adapter angeschlossen wird.
*   *Hinweis:* Ohne angeschlossenen USB-DAC läuft die App im reinen "Simulations-Modus" (RDS wird nur in der UI visualisiert, aber nicht als echtes Audiosignal ausgegeben).

## 🚀 Erste Schritte

1. **Hardware verbinden:** Schließe deinen USB-DAC an das Android-Gerät an. Die App erkennt den DAC automatisch und der orange Button "RDS SIMULIEREN" wechselt auf ein grünes "RDS STARTEN".
2. **Setup:** Trage im Tab *Einst.* deinen PI-Code, die PS-Namen und den Radiotext ein.
3. **Audio-Routing:** Wähle oben rechts über das Drei-Punkte-Menü `⋮` -> *RDS Ausgabe* den gewünschten Audiokanal (z.B. LI) für das Daten-Signal.
4. **Webradio (Optional):** Aktiviere den Stream-Schalter, füge eine Webradio-URL ein und aktiviere "Auto (Stream)" bei der letzten RT-Zeile, um aktuelle Songtitel in den Radiotext zu pushen.
5. **On Air:** Drücke auf "RDS STARTEN" und wechsle in den *Show*-Tab, um die Live-Ausgabe deines virtuellen Displays zu überwachen. Über "Änderungen Live übernehmen" kannst du Texte während des Betriebs anpassen.

## 🛠 Berechtigungen
*   **Mikrofon / Audio aufnehmen:** Wird lokal ausschließlich für den integrierten Audio-Visualizer (Pegelanzeige des Webradios) benötigt.
*   **Benachrichtigungen:** Erforderlich, damit Android den Audiostream nicht beendet, sobald du die App in den Hintergrund legst.

## 📞 Kontakt & Support

Feedback, Bug-Reports oder Feature-Ideen sind immer willkommen!

*   **Discord:** `Highpoint2000`
*   **E-Mail:** [highpoint2000@gmail.com](mailto:highpoint2000@gmail.com)

Wenn dir das Tool gefällt freue ich mich über einen Kaffee:  
<a href="https://www.buymeacoffee.com/Highpoint" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
