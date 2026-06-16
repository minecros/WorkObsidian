# Sterowanie AUTO/MAN zaworów w scadzie
Ustawić przy inicjalizacji PLC tagi:
- AUT_LG_CMd := 0;
- MAN_LG_CMd := 1;
W momencie gdy zawór ma być przełaczony w tryb AUTO trzeba użyć xic z boolem który będzie miał wartość true na czas trwania przełaczenia w tryb auto i zrobi latch na AUT_LG_CMd

![[Pasted image 20251007150531.png]]

W momencie gdy zawór ma być przełaczony w tryb MAN trzeba użyć xic z boolem który będzie miał wartość false na czas trwania przełaczenia w tryb MAN i zrobi unlatch na AUT_LG_CMd


