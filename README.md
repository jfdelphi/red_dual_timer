TODO
- versuchen das flash auszulesen
-   https://www.st.com/en/development-tools/stvp-stm8.html

-   ai geben um die ports zu erkennen
- einige pins messen um den chip typ herauszufinden
- 
- 


https://aliexpress.com/item/1005008264658266.html

# red_dual_timer
super cheap chinea board with stm8. make new codes using arduino.

🧠 Ergebnis: Belegung der 4 Lötaugen (von oben nach unten):
Lötpad	Funktion
1	NRST
2	GND
3	SWIM
4	VCC

✅ ST-Link V2 Anschluss
ST-Link Pin	Modul Pad
NRST	1 (oben)
GND	2
SWIM	3
5V	4 (unten)



void setup() {
  pinMode(PC3, OUTPUT);  // z.B. Relais 1
}

void loop() {
  digitalWrite(PC3, HIGH);
  delay(1000);
  digitalWrite(PC3, LOW);
  delay(1000);
}





Option 2: Mit Arduino IDE
Installiere Sduino

Trage in den Boardverwalter diese URL ein:

arduino
Kopieren
Bearbeiten
https://raw.githubusercontent.com/tenbaht/sduino/master/package_sduino_stm8_index.json
Wähle Board: „STM8S103F3 Breakout Board“ (funktioniert auch für STM8S003)

Programmiere wie gewohnt mit Arduino-Code (setup(), loop())


STM8S105C6T6 
Merkmal	Wert
Architektur	8‑Bit RISC (STM8 Core)
CPU-Takt	bis zu 16 MHz (intern/extern)
Flash-Speicher	32 KB
RAM	2 KB
EEPROM	1 KB
Betriebsspannung	2.95 V bis 5.5 V

Programmiert über SWIM (Single Wire Interface Module)

