# 1 New signals


| TAG NEW  | COMMENT NEW                  | Cluster | Slot | Chan |
| -------- | ---------------------------- | ------- | ---- | ---- |
| XS700530 | UPS A Invertor Operation     | 01      | 01   | 01   |
| XA700550 | UPS A Mains  Operation       | 01      | 01   | 02   |
| XS700531 | UPS A Battery Discharge      | 01      | 01   | 03   |
| XS700532 | UPS A Battery deep discharge | 01      | 03   | 08   |
| XS700533 | UPS A Mains Failure          | 01      | 08   | 08   |
| XS700534 | UPS A Failure                | 01      | 09   | 04   |
| XA700551 | UPS A Major Alarm            | 01      | 09   | 08   |
| XA700552 | UPS A Minor Alarm            | 02      | 04   | 02   |
| XS700535 | UPS B Invertor Operation     | 02      | 04   | 04   |
| XA700556 | UPS B Mains Operation        | 02      | 04   | 08   |
| XA700557 | UPS B Major Fault            |         |      |      |
| XA700558 | UPS B Minor Alarm            | 02      | 06   | 04   |
| XS700536 | UPS B Battery Discharge      | 02      | 07   | 04   |
| XS700537 | UPS B Battery Deep Discharge | 02      | 07   | 05   |
| XS700538 | UPS B Mains Failure          | 02      | 07   | 07   |
| XA700539 | UPS B Failure                | 02      | 07   | 08   |
# 1
800xAAdmin

| TAG OLD  | COMMENT OLD                  |     |
| -------- | ---------------------------- | --- |
| XS700530 | UPS A Invertor Operation     | ok  |
| XA700550 | UPS A Mains Operation        | ok  |
| XS700531 | UPS A Battery Discharge      | ok  |
| XS700532 | UPS A Battery deep discharge | ok  |
| XS700533 | UPS A Mains Failure          | ok  |
| XS700534 | UPS A Failure                | ok  |
| USED?    | Spare                        | ok  |
| USED?    | Spare                        | ok  |
| USED?    | Spare                        | ok  |
| XA700551 | UPS A Major Alarm            | ok  |
| XA700552 | UPS A Minor Alarm            | ok  |
| XS700535 | UPS B Invertor Operation     | ok  |
| XA700556 | UPS B Mains Operation        | ok  |
| XA700558 | UPS B Minor Alarm            | ok  |
| XS700536 | UPS B Battery Discharge      | ok  |
| XS700537 | UPS B Battery Deep Discharge | ok  |
| XS700538 | UPS B Mains Failure          | ok  |
| XA700557 | UPS B Major Fault            | ok  |

# CM
39 wierszy

| **UPSA_STN_AI_BypVL1**        | Real |
| ----------------------------- | ---- |
| **UPSA_STN_AI_BypVL2**        |      |
| **UPSA_STN_AI_BypVL3**        |      |
| **UPSA_STN_AI_BypFreq**       |      |
| **UPSA_STN_AI_RectVL1**       |      |
| **UPSA_STN_AI_RectVL2**       |      |
| **UPSA_STN_AI_RectVL3**       |      |
| **UPSA_STN_AI_RectFreq**      |      |
| **UPSA_STN_AI_DCV**           |      |
| **UPSA_STN_AI_DCA**           |      |
| **UPSA_STN_AI_BattA**         |      |
| **UPSA_STN_AI_InvOutV**       |      |
| **UPSA_STN_AI_InvOutA**       |      |
| **UPSA_STN_AI_OutV**          |      |
| **UPSA_STN_AI_OutA**          |      |
| **UPSA_STN_AI_InvOutFreq**    |      |
| **UPSA_STN_AI_OutFreq**       |      |
| **UPSA_STN_DI_SysNormal**     | Bool |
| **UPSA_STN_DI_OnBattery**     |      |
| **UPSA_STN_DI_RectHealthy**   |      |
| **UPSA_STN_DI_InvStat**       |      |
| **UPSA_STN_DI_BypAvail**      |      |
| **UPSA_STN_DI_BypActive**     |      |
| **UPSA_STN_DI_MaintBypAct**   |      |
| **UPSA_STN_DI_UPSAvail**      |      |
| **UPSA_STN_DI_InvSDImminent** |      |
| **UPSA_STN_AL_OpOutsideLim**  |      |
| **UPSA_STN_AL_OnBattery**     |      |
| **UPSA_STN_AL_DeepDisch**     |      |
| **UPSA_STN_AL_BattLow**       |      |
| **UPSA_STN_AL_BattHigh**      |      |
| **UPSA_STN_AL_RectFault**     |      |
| **UPSA_STN_AL_InvFault**      |      |
| **UPSA_STN_AL_LoadShedEn**    |      |
| **UPSA_STN_AL_LoadShedReset** |      |
| **UPSA_STN_AL_InvSD**         |      |
| **UPSA_STN_AL_BoostOn**       |      |
| **UPSA_STN_AL_Major**         |      |
| **UPSA_STN_AL_Minor**         |      |

# TO ASK
UPS A MODBUS ID -  0
UPS A MODBUS ID - 1
UPS Baud Rate - 9600
UPS Data bits - 8
UPS Parity - NO
UPS Stop bits - 1
Exemys IP -
Exemys Netmask - 
Exemys Gateway 0.0.0.0
Use zero based addressing - Yes
Use zero based bit addressing within registers - Yes
Use holding register bit mask writes - Yes
Use Modbus function 06 for single register writes - Yes
Use Modbus function 05 for single coil writes - Yes
Use default Modbus byte order - Yes
First word low in 32-bit data types - Yes
First word low in 64-bit data types - Yes
Use Modicon bit ordering (bit 0 is MSB) - No
Coils 8-2000 in multiples of 8 - Output - 32
Coils 8-2000 in multiples of 8 - Input - 32
Registers (1-120) Internal - 32
Registers (1-120) Holding -32
Perform block read on strings - No


251 zółty
600 - pomarańczowy domyslne
751 - czerwony
 AESevDiff
 AESevErr
 InNormal - odwrocenie
 |   |   |
|---|---|
|**CondNameDiff**|**0 nic 1 error**|


|                    |
| ------------------ |
| **InNormal**       |
| **CondNameDiff**   |
| **InteractionPar** |
With open Enngineering workplace choose Control Structure. Navigate to Root →Control Network→SWEP_Felindre→Applications→SWEP_Station→Control Modules. Locate each Control Module from table 1, find Aspect Name, insert description from table and clik Apply.

![[Pasted image 20260407093451.png]]