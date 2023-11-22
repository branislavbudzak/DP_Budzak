Na prepojenie nášho Raspberry Pi riešenia s Home Assistentom je potrebné nastaviť náš RPi Zero ako MQTT Publisher/Subscriber, ktorý bude posielať alebo príjmať informácie na Home Assistant server kde beží MQTT Broker.

## MQTT Protokol
MQTT je skratka pre Message Queuing Telemetry Transport. MQTT je jednoduchý protokol na zasielanie správ určený pre zariadenia s obmedzenou šírkou pásma. Je to teda ideálne riešenie na výmenu údajov medzi viacerými zariadeniami IoT.

Komunikácia MQTT funguje ako systém publish and subscribe. Zariadenia publikujú správy na konkrétnu tému. Správu dostanú všetky zariadenia, ktoré sú prihlásené na túto tému.

## Základné MQTT Pojmy
#### MQTT Broker
MQTT Broker je zodpovedný za doručovanie správ medzi klientmi. Jednoducho funguje ako poštár. Na rozdiel od poštára, ktorý doručuje správy na adresu, broker doručuje správy na základe tém, na ktoré sú klienti prihlásení.

#### Publish/Subscribe
V rámci tohto konceptu zariadenie zverejňuje správy v témach alebo sa prihlasuje do tém na prijímanie správ.

Klient 1 (Raspberry Pi Zero) uverejní správu na tému "home/server". Klient 2 (Home Assistant server) sa prihlási na odber tej istej témy. Takže uverejnenú správu môže prijímať klient 2.

#### Messages
Ide o informácie, ktoré si vymieňajú klienti.

#### Topics
Topics sú záujmy klientov, na ktoré majú čo posielať alebo prijímať správy.
![[Pasted image 20231116103634.png]]
Napríklad:
Na obrázku má Publish/Subscribe Client 1 záujem poslať správu na tému "home/server" a Client 2 má záujem prijať správu na tú istú tému.
### Zobrazenie informácií o rastline v Home Assistante
[Plant status card - Home Assistant](https://www.home-assistant.io/dashboards/plant-status/)
![[plant_card.png]]