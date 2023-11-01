Snímače teploty a vlhkosti sú elektronické zariadenia, ktoré sa používajú na meranie teploty a vlhkosti v prostredí. Tieto snímače sa skladajú z niekoľkých základných komponentov, medzi ktoré patria:
- Termistor: Termistor je elektronický komponent, ktorý mení svoj odpor v závislosti od teploty. Snímače teploty používajú termistory na meranie teploty v prostredí.
- Merač vlhkosti: Merač vlhkosti je elektronický senzor, ktorý meria vlhkosť v prostredí. Snímače vlhkosti môžu byť kapacitné, odporové alebo optické.
- Mikrokontrolér: Mikrokontrolér je malý počítač, ktorý ovláda snímač a spracováva údaje, ktoré snímač poskytuje.
- Komunikačné rozhrania: Snímače môžu byť vybavené rôznymi komunikačnými rozhraniami, napríklad I2C alebo SPI, ktoré umožňujú prenos údajov zo snímača do mikrokontroléra.
Existuje mnoho rôznych typov snímačov teploty a vlhkosti, ktoré sa líšia v závislosti od použitej technológie a presnosti merania. 

Niektoré snímače sú určené na použitie s konkrétnymi mikrokontrolérmi, ako je napríklad Raspberry Pi Zero, a možno ich ľahko pripojiť pomocou komunikačných rozhraní, ako je I2C alebo SPI.

I2C a SPI sú dva sériové komunikačné protokoly, ktoré sa používajú na prenos údajov medzi elektronickými komponentmi. Tu je niekoľko základných informácií o týchto protokoloch:

**I2C:**
- I2C (Inter-Integrated Circuit) je sériový komunikačný protokol, ktorý umožňuje komunikáciu medzi elektronickými komponentmi na rovnakej doske plošných spojov.
- I2C používa na prenos údajov dva vodiče: SDA (sériové údaje) a SCL (sériové hodiny).
- I2C umožňuje pripojenie viacerých zariadení k jednej zbernici pomocou adresovania.
- I2C je pomalšia ako SPI, ale je jednoduchšia na používanie a vyžaduje menej hardvérových prostriedkov.

**SPI:**
- SPI (Serial Peripheral Interface) je sériový komunikačný protokol, ktorý umožňuje komunikáciu medzi mikrokontrolérom a periférnymi zariadeniami.
- SPI používa na prenos údajov štyri vodiče: MOSI (Master Out Slave In), MISO (Master In Slave Out), SCK (Serial Clock) a SS (Slave Select).
- SPI umožňuje pripojenie viacerých zariadení k jednej zbernici pomocou signálu SS.
- SPI je rýchlejšie ako I2C, ale vyžaduje si viac hardvérových prostriedkov a je zložitejšie na používanie.

Oba protokoly majú výhody a nevýhody a výber medzi nimi závisí od konkrétnych požiadaviek projektu.