Dodać sterowanie auto/manual ramp

SCS_ACV_XZV1002.AUT_LG_CMd
SCS_ACV_XZV1002.MAN_LG_CMd


Ciśnienia 
SCS_AIT_PDIT1001.RANGE_HI
SCS_AIT_PDIT1001.RANGE_LO
SCS_AIT_PDIT1001.HH_SETP
SCS_AIT_PDIT1001.H_SETP
SCS_AIT_PDIT1001.L_SETP
SCS_AIT_PDIT1001.LL_SETP

Ustawianie zaworów na auto po starcie sekwencj - rung w statopn_initi:
![[Pasted image 20251007130251.png]]


# Sterowanie AUTO/MAN zaworów w scadzie
Ustawić przy inicjalizacji PLC tagi:
- AUT_LG_CMd := 0;
- MAN_LG_CMd := 1;
W momencie gdy zawór ma być przełaczony w tryb AUTO trzeba użyć xic z boolem który będzie miał wartość true na czas trwania przełaczenia w tryb auto i zrobi latch na AUT_LG_CMd

![[Pasted image 20251007150531.png]]

W momencie gdy zawór ma być przełaczony w tryb MAN trzeba użyć xic z boolem który będzie miał wartość false na czas trwania przełaczenia w tryb MAN i zrobi unlatch na AUT_LG_CMd



W IO_Map usunięcie SCS_ACV_XZV1005.AUT_LG_CMd := AUTO_LG_CMD; dla zaworów i ustawienie SCS_ACV_XZV1005.LOC_CMd := SCS_DI_HS400006B.PV;


//------------------------------------------------------------
// Valve Point of Control - Display the following control modes:
//------------------------------------------------------------

^learnkit-209148514
^learnkit-868141217
Q | case(1, {Root Container._UDT_IO |
A | Indications.IND_OOS}, 	0, 	//0: OOS - Out of Service |
		Q | {Root Container._UDT_IO |
		A | Indications.IND_PRI},	1, 	//1: PRI - Priority |
		^learnkit-438375140
		Q | {Root Container._UDT_IO |
		A | Indications.IND_LOCAL},2, 	//2: LOC - Local |
		^learnkit-404077301
		Q | {Root Container._UDT_IO |
		A | Indications.IND_REM},	3, 	//3: REM - Remote |
														4 )	//4: <!> - Otherwise Diag Error
