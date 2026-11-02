# Mobile RDS Encoder (Android) 📻

Der **Mobile RDS Encoder** ist eine Android-Applikation, die es ermöglicht, dynamische RDS-Informationen (Radio Data System) direkt in ein Stereo-Audiosignal einzubetten. Die Ausgabe erfolgt idealerweise über einen angeschlossenen USB-DAC (Digital-Analog-Wandler), um das Signal anschließend in einen FM-Transmitter einzuspeisen.

<img width="195" height="750" alt="Screenshot1" src="https://github.com/user-attachments/assets/41fd52df-065b-4b96-ba74-56fafe7754d7" />
<img width="346" height="750" alt="Bild2" src="https://github.com/user-attachments/assets/e0cd0ab2-b089-46de-bce1-12bdf4010ef6" />
<img width="346" height="750" alt="Bild3" src="https://github.com/user-attachments/assets/d20627a3-72df-4e29-b603-44e9a119fca8" />

## ✨ Features (Version 1.2)

*   **Basis-RDS-Parameter:** PI-Code, ECC, Programmtyp (PTY), Traffic Program (TP) und Traffic Announcement (TA).
*   **Alternative Frequenzen (AF):** Eingabe von bis zu 25 AF-Frequenzen.
*   **Dynamischer Sendername (PS) & Radiotext (RT):** Mehrere Zeilen mit konfigurierbarem Wechselintervall und automatischem A/B-Flag-Wechsel.
*   **Erweiterter RDS-Zeichensatz (Neu in v1.2):** Echte Umlaute und Akzente werden für maximale Hardware-Kompatibilität (z. B. TEF6686 Receiver) im Hintergrund vollautomatisch RDS-konform umgewandelt (ä -> ae, ß -> ss).
*   **Webradio-Integration & Smart Parsing:** Integrierter Player für Webradio-Streams inkl. automatischer Extraktion von ICY-Metadaten. Dank robustem Charset-Fallback (UTF-8 / Windows-1252) in v1.2 werden Sonderzeichen aus Streams immer fehlerfrei dargestellt.
*   **Erweitertes RDS-Routing & Boost (Neu in v1.2):** 
    * Gezielte Ausgabe des RDS-Signals wahlweise auf dem linken (LI), rechten (RE) oder beiden (LI+RE) Audiokanälen.
    * **RDS Signal Boost:** Das RDS-Basebandsignal kann nun stufenlos bis zu 10-fach digital verstärkt werden, um Pegelschwächen des Smartphones auszugleichen.
    * **Stereo-Metering:** Präzise Pegelanzeige (L/R) inklusive Übersteuerungs-Warnung (Clipping).
*   **Smart Preset-Verwaltung (Neu in v1.2):** Speichern, Laden und Updaten von Konfigurationen inkl. Sicherheitsabfragen vor dem Überschreiben/Löschen. Die App merkt sich nun das zuletzt genutzte Preset und lädt es beim Start automatisch.
*   **Safe-Transmit Check (Neu in v1.2):** Die App prüft beim Sendestart, ob der "Nicht stören"-Modus aktiv ist, um Störgeräusche durch eingehende Anrufe auf dem FM-Transmitter zu verhindern.
*   **Hintergrundbetrieb:** Die App läuft als Foreground-Service zuverlässig im Hintergrund weiter, auch wenn das Display ausgeschaltet ist.

## 📥 Installation (APK)

1. Lade die aktuellste Version [hier](https://github.com/Highpoint2000/MobileRDSEncoder/blob/main/Mobile_RDS_Encoder_1.2.apk) herunter.
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
3. **Audio-Routing & Pegel:** Wähle oben rechts über das Drei-Punkte-Menü `⋮` -> *RDS Ausgabe* den gewünschten Audiokanal (z.B. LI) und pegle das RDS-Signal mit dem Gain-Slider so ein, dass die Balken grün bleiben.
4. **Webradio (Optional):** Aktiviere den Stream-Schalter, füge eine Webradio-URL ein und aktiviere "Auto (Stream)" bei der letzten RT-Zeile, um aktuelle Songtitel in den Radiotext zu pushen.
5. **On Air:** Drücke auf "RDS STARTEN". Folge bei Bedarf dem Hinweis, das Gerät auf lautlos ("Nicht stören") zu schalten. Wechsle danach in den *Show*-Tab, um die Live-Ausgabe deines virtuellen Displays zu überwachen. Über "Änderungen Live übernehmen" kannst du Texte während des Betriebs anpassen.

## 🛠 Berechtigungen
*   **Mikrofon / Audio aufnehmen:** Wird lokal ausschließlich für den integrierten Audio-Visualizer (Pegelanzeige des Webradios) benötigt.
*   **Benachrichtigungen:** Erforderlich, damit Android den Audiostream nicht beendet, sobald du die App in den Hintergrund legst.

## 📞 Kontakt & Support

Feedback, Bug-Reports oder Feature-Ideen sind immer willkommen!

*   **Discord:** `Highpoint2000`
*   **E-Mail:** [highpoint2000@gmail.com](mailto:highpoint2000@gmail.com)

Wenn dir das Tool gefällt freue ich mich über einen Kaffee:  
<a href="https://www.buymeacoffee.com/Highpoint" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>