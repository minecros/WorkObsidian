Removed from the scope
# TODO
- Dodać do dokumentu usunięcie ZI-460607A, ZI-460607B, ZI-460623A, ZI-460623B
- XS700539_ - po odpowiedzi na TQ poprawić
- podpiąć alarmy modbus tam gdzie to konieczne
- Ustawić priorytet na 251 sever ale dla których CM?
- dla alarmów CM ustawić parametr interractionPar.ErrorMode na 0 (through)
- zmienić opisy sygnałów modbus na description z excela
# Doc
W Var_1:
- z wierszy NAME usunąć spacje
- w wierszach NAME dodać UPSA/UPSB na początku, w celu rozróżnienia CM w plan explorerze
W OPC_Obj:
- UPSA_STN_AL_OnBattery z DI na AL

W KEP_Tags:
- adres UPSA_STN_DI_BypActive 300003.14
- adres UPSA-STN-AL-LoadShedEn na 30005.9
- adres UPSA-STN-AL-LoadShedReset 30005.9



5.3.3 zmiana z FGSToOutputs_SCM na Signals_To_RemoteOutstation
#TODO #ABB #UPS