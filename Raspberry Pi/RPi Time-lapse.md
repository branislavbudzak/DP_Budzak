#### Samostatné zariadenie na vytvorenie Time-lapse záznamu
- Ak by sme chceli vytvoriť time-lapse zariadenie, ktoré beží na batériu museli by sme použiť zariadenie ako Witty Pi 4.
	- [Witty Pi 4: Realtime Clock and Power Management for Raspberry Pi | UUGear](https://www.uugear.com/product/witty-pi-4/)
	- [UUGear Witty Pi 4](https://rpishop.cz/sprava-napajeni-a-ups/5609-uugear-witty-pi-4.html?SubmitCurrency=1&id_currency=2)
- Takéto zariadenie dokáže umožniť RPi hybernovať aj keď to samotný RPi neumožňuje. Pomocou softvéru sa dá nastaviť harmonogram, kedy sa RPi zapne a kedy sa vypne.
- ![[Pasted image 20231206102406.png]]
- To znamená, že ak by sme toto zariadenie využívali na time-lapse, tak vedel by vydržať kľudne aj niekoľko týždňov alebo aj mesiacov
- Witty Pi 4 používa na komunikáciu s RPi [[I2C Protokol]] a prepojenie cez GPIO konektory.
- Samotné zariadenie vieme 

#### Time-lapse záznam v rámci riešenia našej diplomovej práce
- Na vytvorenie časozberu v rámci nášho riešenia budeme potrebovať taktiež [[Navrhované produkty na kúpu#Kamerový modul | Kamerový modul]], ktorý prepojíme dlhším flexibilným káblom aby sme ho mohli umiestniť aj mimo RPi
- Po pripojení kamery, vieme obrázky z tohto modulu použiť v Python kóde a vytvoriť kód, ktorý nám automaticky vytvorí časozber
- Použiť na to vieme napríklad [time-lapse · PyPI](https://pypi.org/project/time-lapse/) projekt alebo [timelapse.py](https://sites.google.com/site/timelapsepy/home?authuser=0) prípadne nájsť iný spôsob automatického spojenia vytvorených obrázkov
- Obrázky 