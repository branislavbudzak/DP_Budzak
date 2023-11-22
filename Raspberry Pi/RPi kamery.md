Kamerový modul pre [[Raspberry Pi Zero]] je zariadenie, ktoré umožňuje záznam videa a snímky fotografií.

#### Použitie Kamerového Modulu
- **Fotografie a Videá:**
	- Kamerový modul umožňuje Raspberry Pi Zero zaznamenávať fotografie a videá. Toto je užitočné pre projekty, ktoré vyžadujú fotografovanie alebo záznam videa na diaľku, napríklad dohľadové kamery alebo fotografovanie pre meteorologické projekty.
- **Sledovanie a Bezpečnosť:**
	- Kamery sa používajú na sledovanie miestností, domov alebo exteriérov. Rôzne bezpečnostné projekty, ako napríklad sledovanie domu, detekcia pohybu, môžu byť implementované pomocou kamerového modulu.
- **Rozpoznávanie Obrazu:**
	- Vďaka rozšírenej funkcionalite strojového učenia môže byť kamerový modul použitý na rozpoznávanie tvárí, zvierat alebo iných objektov. Táto funkcionalita je užitočná pre projekty zamerané na biometriku alebo inteligentné systémy sledovania.
- **Projekty na Internet of Things (IoT):**
	- Kamerové moduly s Raspberry Pi Zero sa často používajú v projektoch pre Internet of Things (IoT). Napríklad môžu byť súčasťou inteligentných domácich systémov, kde majú za úlohu zaznamenávať udalosti alebo detekovať pohyb.

#### Možnosti Pripojenia Kamery
- **Pripojenie cez GPIO Pin Header:**
	- Kamerový modul sa pripája priamo na GPIO (General Purpose Input/Output) pin header Raspberry Pi Zero. Toto je štandardné pripojenie, ale väčšinou sa používa flexibilné použitie.
- **Flexibilné Pripojenie:**
	- Kamerový modul je pripojený pomocou flexibilného pásu, ktorý umožňuje väčšiu slobodu pri umiestňovaní kamery v projekte.

#### Protokol
Modul kamery Raspberry Pi zvyčajne používa na pripojenie k doskám Raspberry Pi vrátane Raspberry Pi Zero protokol CSI (Camera Serial Interface). Rozhranie CSI je špecializované rozhranie kamery, ktoré umožňuje vysokorýchlostný prenos údajov medzi modulom kamery a Raspberry Pi.

Modul kamery sa pripája k portu CSI na doske Raspberry Pi pomocou páskového kábla. Toto špecializované rozhranie umožňuje efektívnu komunikáciu a vysokú šírku dátového pásma, vďaka čomu je vhodné na snímanie obrázkov a videí v reálnom čase.

[Dokumentácia oficiálneho Raspberry Pi kamera modulu](https://www.raspberrypi.com/documentation/accessories/camera.html)