## Výber operačného systému
Raspberry Pi OS Lite (32-bit) je vynikajúcim východiskovým bodom. 32-bitová verzia zaisťuje maximálnu kompatibilitu s rôznymi softvérovými balíkmi a knižnicami, ktoré by ste mohli potrebovať na prepojenie so senzormi, kamerou a sieťou na komunikáciu MQTT.

### Prečo Raspberry Pi OS Lite?
- Ľahký: Nezahŕňa desktopové prostredie, ktoré nie je potrebné pre váš projekt, čím šetrí systémové prostriedky pre vašu aplikáciu.
- Efektivita: Efektívne beží na Raspberry Pi Zero 2 W, čo zaisťuje, že väčšina zdrojov zariadenia je k dispozícii na spracovanie údajov zo senzorov a spracovanie vstupu z kamery.
- Kompatibilita: Raspberry Pi OS má širokú podporu pre hardvérové komponenty a periférie bežne používané v projektoch DIY, vrátane širokej škály senzorov a kamerových modulov.
- Komunitná podpora: Vzhľadom na popularitu Raspberry Pi OS vieme násť rozsiahlu komunitnú podporu, návody a knižnice pripravené na použitie pre takmer akýkoľvek senzor alebo úlohu.

### Úvahy o našom projekte
- MQTT pre komunikáciu
	- Keďže chceme posielať údaje brokerovi MQTT, uistíme sa, že máme na svojom Raspberry Pi Zero 2 W nainštalovanú klientsku knižnicu MQTT.
	- Knižnica `paho-mqtt` je obľúbenou voľbou, ktorá dobre funguje s Raspberry Pi OS Lite.
- Monitorovanie kamery
	- Keďže plánujeme používať modul kamery Raspberry Pi, nemôžeme zabudnúť povoliť podporu kamery pomocou `raspi-config` a otestovať kameru pomocou nástrojov príkazového riadka alebo skriptov Python. 
	- V závislosti od našej aplikácie možno budeme musieť nainštalovať ďalšie softvérové balíky alebo knižnice na spracovanie obrazu (napr. OpenCV), ktoré sú taktiež kompatibilné s Raspberry Pi OS Lite.
- Integrácia senzorov 
	- Väčšina senzorov na monitorovanie vlhkosti, teploty a svetla môže byť jednoducho prepojená s GPIO pinmi na Raspberry Pi Zero 2 W. 
	- Knižnice Python ako `RPi.GPIO` alebo knižnice Adafruit pre špecifické senzory môžu byť použité na čítanie dát senzorov.
- Automatický zavlažovací systém 
	- Zavlažovací systém môžeme ovládať pomocou reléových modulov alebo elektronických ventilov pripojených na kolíky GPIO. 
	- Musíme sa uistiť, že máme zavedené potrebné knižnice a bezpečnostné opatrenia na spoľahlivé ovládanie týchto komponentov.
### Vývoj a nasadenie
- Vývoj 
	- Svoj kód môžete vyvíjať na výkonnejšom stroji alebo priamo na Raspberry Pi Zero 2 W. 
	- Budeme využívať najmä SSH na pripojenie k nášmu Pi na kódovanie a testovanie.
- Nasadenie
	- Keď bude nás kód pripravený a otestovaný, môže bezproblémov bežať na Raspberry Pi Zero 2 W
	- Môžeme použiť úlohy cron alebo služby `systemd` na naplánovanie našich skriptov alebo ich spustenie po načítaní OS.
## Zhrnutie
Pre projekt monitorovania rastlín je Raspberry Pi OS Lite (32-bitový) optimálnou voľbou pre prevádzku na Raspberry Pi Zero 2 W. Poskytuje potrebnú rovnováhu medzi výkonom, dostupnosťou zdrojov a kompatibilitou s potrebnými perifériami a knižnicami. 

Pri vykonávaní tohto riešenia nemôžeme zabudnúť otestovať každý komponent jednotlivo (snímače, kamera, MQTT komunikácia) pred ich integráciou do nášho konečného projektu, aby sme mohli efektívnejšie odstraňovať problémy a riešiť potenciálne problémy. 