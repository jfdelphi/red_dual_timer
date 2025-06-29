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


✅ Mikrocontroller: STM8S003F3P6
Das ist ein 20 MHz 8‑Bit‑Mikrocontroller von STMicroelectronics mit:

8 KB Flash

1 KB RAM

10 Bit ADC

UART, I²C, SPI, PWM

Programmiert über SWIM (Single Wire Interface Module)

