- Raspberry Pi Zero je malý jednodeskový počítač vyvinutý spoločnosťou Raspberry Pi Foundation. Má veľkosť kreditnej karty a ponúka množstvo výkonných funkcií v kompaktnom dizajne. 
- Raspberry Pi Zero je poháňaný ARM procesorom s frekvenciou 1 GHz, má 512 MB RAM pamäť a je vybavený mini-HDMI konektorom pre pripojenie k monitoru, USB portom, microUSB portom pre napájanie a dáta a 40 GPIO (General Purpose Input/Output) pinmi na pripojenie periférií. 
- Je ideálny na vývoj elektronických projektov, IoT aplikácií, mediaserverov, jednoduchých serverov a mnoho ďalších úloh. 
- S jeho nízkou cenou a veľkým komunitným podporou je Raspberry Pi Zero populárnou voľbou pre tvorcov, vývojárov a nadšencov technológií.
![[Raspberry_Pi_Zero_W_30113445-01.jpg]]

## Protokoly a pripojenia, ktoré podporuje
- **GPIO (General Purpose Input/Output):** Piny GPIO na Raspberry Pi Zero možno nakonfigurovať tak, aby podporovali digitálny vstup a výstup na všeobecné účely. Táto flexibilita umožňuje komunikáciu so širokou škálou snímačov a iných zariadení.
- [[I2C Protokol]]: Raspberry Pi Zero obsahuje piny GPIO, ktoré možno nakonfigurovať na podporu komunikácie I2C. I2C je sériový komunikačný protokol s viacerými nadradenými a podriadenými zariadeniami, ktorý sa bežne používa na pripojenie snímačov, displejov a iných periférnych zariadení.
- [[SPI Protokol]]: Raspberry Pi Zero podporuje komunikáciu SPI prostredníctvom pinov GPIO. SPI je synchrónny sériový komunikačný protokol používaný na pripojenie zariadení, ako sú displeje, snímače a iné periférie.
- [[CSI Protokol]]: Raspberry Pi Zero má samostatný konektor, ktorý slúži na pripojenie kamerového modulu. Do tohto konektoru sa pripája flexibilný kábel, ktorý komunikuje s RPi cez Camera Serial Interface (CSI) protokol.
- **UART (univerzálny asynchrónny prijímač a vysielač):** Raspberry Pi Zero GPIO piny je možné nakonfigurovať aj na komunikáciu cez UART. UART je štandardný asynchrónny sériový komunikačný protokol používaný na pripojenie zariadení, ako sú moduly GPS, moduly Bluetooth a iné sériové periférie.
- **PWM (pulzno-šírková modulácia):** Raspberry Pi Zero podporuje PWM na niektorých pinoch GPIO. PWM sa často používa na riadenie intenzity LED diód, rýchlosti motorov a iných aplikácií, ktoré vyžadujú premenlivý výstup.
- **Jednovodičové pripojenie (One-Wire):** Raspberry Pi Zero podporuje protokol One-Wire, ktorý sa bežne používa napríklad na pripojenie snímačov teploty.

Pri práci s Raspberry Pi Zero a jeho GPIO pinmi je dôležité pozrieť si oficiálnu dokumentáciu, schémy vývodov a akúkoľvek špecifickú dokumentáciu poskytnutú výrobcom periférnych zariadení, ktoré pripájame. Tieto informácie vám pomôžu pri konfigurácii pinov GPIO a používaní vhodných komunikačných protokolov pre vaše konkrétne aplikácie.