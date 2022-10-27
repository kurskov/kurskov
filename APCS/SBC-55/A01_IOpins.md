# Назначение входов-выходов контроллера A01

Ниже описаны назначения и точки подключения входов и выходов контроллера 
управления Mitsubishi FX2N-48MT (блок A01) установкой струйной отмывки 
Finnsonic SBC-55 (с/н 525075-38-05).  

Даннне собраны на основе чертежа номер 52507530, страницы 9-14.

## Назначение входов контроллера

В графе "Подключение" указаны номера контактов соответствующего устройства в порядке от контроллера к общей шине или следующему устройству.

Входы контроллера коммутируются с шиной 24 В или иными цепями с высоким уровнем.

| Номер  вывода | Обозначение | Описание | Подключение | Комментарий |
| :-: | - | - | - | - |
| X0 | STOP (washing) | Кнопка, останавливает процесс отмывки. | S000 (22 - 21) | - |
| X1 | START (washing) | Кнопка, запускает процесс отмывки. | S001 (14 - 13) | - |
| X2 | LEVEL ALARM RESET | Кнопка, включает насосы. | S002 (14 - 13) | - |
| X3 | TEMPERATURE OK STORAGE TANK 1 (WASH) | Термореле, срабатывает при достижении отмывочной жидкостью нужной температуры. | S003 (2 - 1) | - |
| X4 | TEMPERATURE OK STORAGE TANK 2 (RINSE) | Термореле, срабатывает при достижении водой для ополаскивания нужной температуры. | S004 (2 - 1) | - |
| X5 | DRAIN VALVE OPEN TO STORAGE TANK 1 (WASH) | Датчик Холла, срабатывает при открытом положении заслонки слива из рабочей камеры в бак с отмывочной жидкостью. | S005 (BK - BN) | - |
| X6 | DRAIN VALVE OPEN TO STORAGE TANK 2 (RINSE) | Датчик Холла, срабатывает при открытом положении заслонки слива из рабочей камеры в бак с водой для ополаскивания. | S006 (BK - BN) | - |
| X7 | EMERGENCY STOP OK | Реле. Пока замкнуто, на вход подается высокий уровень. | K101 (2 - 1) | - |
| X10 | LEVEL OK (storage tank 1 wash) | Поплавок, расположен в нижней части бака с отмывочной жидкостью, при падении размыкает контакт. | S010 (WH - WH) | - |
| X11 | OVERFILLING (storage tank 1 wash) | Поплавок, расположен в верхней части бака с отмывочной жидкостью, при всплытии размыкает контакт. | S011 (WH - WH) | - |
| X12 | LEVEL OK (storage tank 2 rinse) | Поплавок, расположен в нижней части бака с водой для ополаскивания, при падении размыкает контакт. | S012 (WH - WH) | - |
| X13 | OVERFILLING (storage tank 2 rinse) | Поплавок, расположен в верхней части бака с водой для ополаскивания, при всплытии размыкает контакт. | S013 (WH - WH) | - |
| X14 | DRIP TRAY ALARM | - | S014 (NC) | - |
| X15 | AGITATING AT UP POSITION | - | S015 (BK - BN) | - |
| X16 | AGITATING AT DOWN POSITION (HOME) | - | S016 (BK - BN) | - |
| X17 | SAFETY DOOR OK | - | S017.2 (22 - 21) - S017.1 (22 - 21) | - |
| X20 | SPRAY PUMP STORAGE TANK 1 (WASH) (motor alarms) | - | F10 (32 - 31) | - |
| X21 | SPRAY PUMP STORAGE TANK 2 (RINSE) (motor alarms) | - | F11 (32 - 31) | - |
| X22 | FILTRATION PUMP STORAGE TANK 2 (RINSE) (motor alarms) | - | F12 (32 - 31) | - |
| X24 | HOT AIR BLOWER (motor alarms) | - | F14 (32 - 31) | - |
| X25 | FILTRATION PUMP STORAGE TANK 1 (WASH) (motor alarms) | - | F20 (32 - 31) | - |
| X26 | INVERTER ALARM | - | U13:B | - |
| X27 | DRYER OVERHEAT ALARM | - | S027 (1 - C) in X027 | - |

## Назначение выходов контроллера

| Номер  вывода | Обозначение | Описание | Подключение | Комментарий |
| :-: | - | - | - | - |
| Y0 | WASH ON LIGHT | - | H000 (X1 - X2), GREEN | - |
| Y1 | LEVEL ALARM LIGHT | - | H001 (X1 - X2), RED | - |
| Y2 | ALARM LIGHT | - | H002 (X1 - X2), RED | - |
| Y3 | WASH VALVE | - | Y003 (1 - 2) | - |
| Y4 | HEATING STORAGE TANK 1 (WASH) | - | K3 (A1 - A2) | - |
| Y5 | HEATING STORAGE TANK 2 (RINSE) | - | K4 (A1 - A2) | - |
| Y6 | HEATING SPRAY CHAMBER HOT AIR | - | K5 (A1 - A2) | - |
| Y7 | RINSE VALVE | - | Y007 (1 - 2) | - |
| Y10 | SPRAY PUMP STORAGE TANK 1 (WASH) | - | K10 (A1 - A2) | - |
| Y11 | SPRAY PUMP STORAGE TANK 2 (RINSE) | - | K11 (A1 - A2) | - |
| Y12 | FILTRATION PUMP STORAGE TANK 2 (RINSE) | - | K12 (A1 - A2) | - |
| Y13 | SPRAY AGITATING MOTOR DOWNWARD | - | K113 (5 - 1) | - |
| Y14 | SPRAY AGITATING MOTOR UPWARD | - | K114 (5 - 1) | - |
| Y15 | HOT AIR BLOWER | - | K14 (A1 - A2) | - |
| Y16 | S. TANK DRAIN VALVE CONTROL | - | K16 (5 - 1) | - |
| Y17 | SAFETY DOOR LOCK OPEN | - | Y017 (A1 - A2) | - |
| Y20 | DRAIN VALVE STORAGE TANK 1 (WASH) | - | Y020 (1 - 2) | - |
| Y21 | DRAIN VALVE STORAGE TANK 2 (RINSE) | - | Y021 (2 - 2) | - |
| Y22 | VENTILATION OPEN | - | Y023 (1 - 2) | - |
| Y23 | AIR BLAST FOR PIPES | - | K23 (A1 - A2) | - |
| Y24 | FILTRATION PUMP STORAGE TANK 1 (WASH) | - | K20 (A1 - A2) | - |
| Y25 | LIGHT TOWER GREEN, WASH ON | - | H025 (X1 - X2), GREEN | - |
| Y26 | LIGHT TOWER WHITE, CONTROL ON | - | H026 (X1 - X2), WHITE | - |
| Y27 | LIGHT TOWER RED, ALARM | - | H027 (X1 - X2), RED | - |
