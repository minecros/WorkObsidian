PLC -> TELE TTD/TTA
TELE -> PLC TDI/AI

SCS_TDI_XS100800

Przy trybie normalnym 
COM_SCS_TDI_XI100700_STATUS -> MCM_TLM.DATA.WriteData[0].0 := SCS_TTD_STN_XI100700.OUTPUT;
W momencie poklikania w oss wartość z oss -> MCM_TLM.DATA.WriteData[0].0 := SCS_TTD_STN_XI100700.OUTPUT;

watchdogi na station nie sa podpiete



- Założenie, że wszystkie zmiany dotyczą scs, brak zmian na sps
- sprawdzić czy karta serialowa jest
- jesli jest czy sa porty
- jesli nie ma jakie sa opcje, czy mozna kupic itp to w ostatecznosci - jesli nie ma dostepnosc karty, zamiast niej gateway, i wyslac przez hardwired
- potwierdzic numey/model plc, co to jest za kontroler, dokladnie, cpu model

- dodanie io w kodzie i scadzie, sprawdzenie czy reaguje na zmiany test mode
- modbus tcp
