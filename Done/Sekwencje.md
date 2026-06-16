
Wyrównać sygnał station esd lockout non lockout

BitInversion

P1 - wykonuje się po wejściu do kroku
N - wykonuje się cały  czas w kroku
P0 - wykonuje sie bezpośrednio przed zmianą na kolejny krok sekwencji
tagi z tele w nazwie beda uzywane fizycznie, dodac je w plc i tyle
tagi z CNET i SPS w nazwie dodać do plc i matlab. To sa boole

timery jakie czasy

XZV210002 10001
XZV210003 10002
XZV210026 10003
XZV210025 10007
SV210041DT 10008
SV210046DT 10009
SV810001DT 10004
FCV210016DT.FB1.Value = true 1005 ????
FCV210016DT.FB0.Value = false 1005 ????

# INIT

# DE INIT

UNA_DEINITIATED kiedy m



# START

Nazwy kroków :

| SCADA                               | PLC                          |
| ----------------------------------- | ---------------------------- |
| ?                                   | Start_Open_Inlet_Press_Valve |
| Open Inlet Press Valve XZV210003    | ?                            |
| Compressor Unit Loaded Confirmation |                              |


- UnitA_CNET_Data_UNIT_PRESSURISED
- UnitA_CNET_Data_UNIT_NORMAL_STOP
- UnitA_CNET_Data_VALVE_SEQ_COMPLETE
- UnitA_CNET_Data_HIGH_VOLTAGE_BREAKER_INITIATE
- UnitA_CNET_Data_UNIT_ACK
- UnitA_CNET_Data_UNIT_RESET
- UnitA_CNET_Data.READY_TO_PURGE
- UnitA_CNET_Data.UNIT_LOAD
- UnitA_SPS_IO.UNIT_PRESSURISED_SHUTDOWN
- UnitA_SPS_IO_PDI210038_PD
- UnitA_SPS_IO_PDI210040_PD
-  UnitA_SPS_IO_UNIT_C2101_ESD -
- UnitA_SPS_IO_UNIT_C2101_LOCKOUT 
- UnitA_SPS_IO_UNIT_C2101_NONLOCKOUT
-  UnitACommsWR_STN_CTRL_AUTO ????
- UnitAVoPOK ????
-  RetrievedDataStation_STATION_AVAILABLE ????
- RetrievedDataStation_FGS_CRITICAL_FAULT ????
- RetrievedDataStation.C2101_HAZ_ATM_LVL1 ????
- UNA_ACV_XZV10001.AUT_LG_CMd UNA_DO_XZV10001
- 10001
- 10002
- 10003
- 10004
- 10005
- 10007
- 10008
- 10009


# STOP
Reszta:
- UnitA_CNET_Data_UNIT_STOPPING
- UnitA_CNET_Data_UNIT_NORMAL_STOP 
- UnitA_CNET_Data_UNIT_LOAD
- UnitACommsWR_UNIT_A_STOP_SPD
- UnitA_CNET_Data_VALVE_SEQ_COMPLETE
- UnitA_CNET_Data_UNIT_STOPPED
- UnitA_CNET_Data_SI210001
Zawory:
- 10001
- 10003
- 10004
- 10008
- 10009

Brak flagi stop, abort i hold

# Nazwy krokow
Wywalić c2101 z nazw wyswietlanych
unit start:
- alarm ack 
- alarm reset
- ogarnac ponowne polaczenie po wygasnieciu ignition