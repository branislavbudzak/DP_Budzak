SPI (Serial Peripheral Interface) je sériový komunikačný protokol, ktorý umožňuje komunikáciu medzi mikrokontrolérom a periférnymi zariadeniami.
- SPI používa na prenos údajov štyri vodiče: MOSI (Master Out Slave In), MISO (Master In Slave Out), SCK (Serial Clock) a SS (Slave Select).
- SPI umožňuje pripojenie viacerých zariadení k jednej zbernici pomocou signálu SS.
- SPI je rýchlejšie ako I2C, ale vyžaduje si viac hardvérových prostriedkov a je zložitejšie na používanie.

#### **SPI Rozhrania:**
1. **4-Wire SPI:**
	- **MOSI (Master Out Slave In):** Prenos dát z mastera do slave zariadenia.
	- **MISO (Master In Slave Out):** Prenos dát zo slave zariadenia do mastera.
	- **SCLK (Serial Clock):** Hodinový signál riadiaci prenos dát.
	- **SS/CS (Slave Select/Chip Select):** Signál na výber konkrétneho slave zariadenia.
2. **3-Wire SPI:**
	- Niektoré zariadenia môžu zjednodušiť rozhranie na 3 piny, kombinovaním MOSI a MISO do jedného signálu, napríklad pomocou dátových multiplexerov alebo prepnutím medzi režimami prenosu.
3. **Daisy-Chain SPI:**
	- Viacero slave zariadení môže byť reťazených (daisy-chained) na jednom SPI zbernici. Každé zariadenie má svoj vlastný SS/CS pin, ale SCLK a MISO/MOSI sú pripojené sériovo.
4. **Quad SPI (QSPI):**
	- Používa štyri dátové linky namiesto dvoch (quad MOSI, quad MISO), čo zvyšuje priepustnosť dát.
5. **Dual SPI:**
	- Používa dvojicu linky pre dáta, čo umožňuje prenos dát s vyššou rýchlosťou.
6. **SPI s hardvérovou podporou (napríklad hardware SPI):**
	- Niektoré mikrokontroléry poskytujú hardvérovú podporu pre SPI, kde sa komunikácia riadi priamo hardvérom, čo zvyšuje rýchlosť a znižuje zaťaženie CPU.