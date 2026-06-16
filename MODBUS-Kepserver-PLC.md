1. Konfiguracja modbus w kepserverx - adres, ip i rejestry 
2. ![[Pasted image 20260216144707.png]] W workplace wybrac control structure -> i dodać nowy "Generic OPC Object" pod istniejącym/nowym "Generic OPC Server Network"
3. W aspekci "Control Connection" w zakładce Property info dodać nowe propertisy i w zakładce opc podać ich adresy w kepserverze![[Pasted image 20260216151229.png]]
4. W obiekcie "Generic OPC Object" dodać aspekt "Property Transfer Definition" i skonfigurować go do wymiany danych pomiędzy zmienną PLC a dodaną property w kroku poprzednim ![[Pasted image 20260216151405.png]]
5. Dodać zmienną na PLC - control builder -> applications -> global variables'
6. Koniecznie musi byc uruchomione OPC Server for AC 800M
7. W workplace na kontrolerze zweryfikować asset control properties i properties system_id czy jest tam wartość sterownika ![[Pasted image 20260216152533.png]]
8. Tutaj mozna podgladnac wartość przesłaną z plc do workplafe ![[Pasted image 20260216155143.png]]

W przypadku komunikacji do plc a nie z niego trzeba zrobić to samo tylko dla zmiennej w aplikacji/programie a expression to adres property odczytanego z opc

	Access variabls na PLC w control builder bez tego komunikacja działała 
# 
1. Node administration Structure
2. Node Definition - dodanie/zmiana adresu ip serwera do komunikacji
![[Pasted image 20260223132342.png]]
![[Pasted image 20260223132353.png]]

 Modifications to ABB DCS System Design Specification