### **Solenoidový ventil**
Na zavlažovací systém je možné použiť solenoidový ventil. Tieto ventily sa ovládajú elektricky a môžu byť uzavreté alebo otvorené pomocou prúdu cez solenoid.

### **Napájanie**
Zabezpečte stabilné napájanie pre Raspberry Pi a solenoidový ventil. Solenoidové ventily obvykle potrebujú vyššie napätie, ktoré by mohlo byť poskytnuté externým zdrojom napájania.

### HAT - Hardware Attatched on Top
HAT je štandardný formát pre hardware moduly, ktoré môžeme pripojiť na GPIO (General Purpose Input/Output) pinové hlavičky na Raspberry Pi. HAT zabezpečuje jednoduché pripojenie a odpojenie a zároveň minimalizuje riziko poškodenia GPIO pinov.

Čo sa týka konkrétne [[Raspberry Pi Zero]], aj keď nemá priamočiary konektor pre HAT ako ostatné modely Raspberry Pi, môžete HAT pripojiť pomocou GPIO headeru. Raspberry Pi Zero obsahuje mini-HAT konektor, ktorý sa nachádza na spodnej strane zariadenia. Tento konektor je menší a odlišuje sa od štandardného 40-pinového konektora používaného na ostatných modeloch Raspberry Pi.

### Relay HAT
Relay HAT pre Raspberry Pi Zero je hardvérový modul, ktorý poskytuje relé (elektromagnetické spínacie prepínače) pre ovládanie externých elektrických zariadení. Tieto relé môžu byť využívané na vypínanie alebo zapínanie napájania rôznych prvkov, ako je napríklad náš solenoidový ventil.

### **Časovanie a Automatizácia**
Pomocou tohto systému môžeme vytvoriť časové a automatizované úlohy v skripte na zabezpečenie riadenia zavlažovania v konkrétnych časoch alebo podľa potreby na základe senzorov (napr. senzorov vlhkosti pôdy).