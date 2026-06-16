# Step 1
1. Spięcie matlaba felindre z plc felindre
2. Spięcie plc felindre z scada felindre
3. Zmiana nazw tagów w plc na te ze schematów na kartce
4. Zmiana tagów matlab na te z plc
5. Zmiana tagów scada na te z plc
6. Testy zmapowanych tagów
7. Zmiana kolorow w matlab na niebieskie


# Step 2
1. Odpalenie 2 PLC
2. Plc z zmodyfikowanym kodem felindre to station controller 
3. 2 PLC to UNIT A, należy dodać do niego sekwencje, 3 strona z notatek
4. Uruchomić komunikację pomiędzy station a unit a
5. Station to PLC z adresem 55, unita uruchomic na plc 54 
Robic kopie zapasowe plc, matlab i oss


Ekrany z scada gdzie moga byc te tagi
![[Pasted image 20250919154413.png]]



# STN PLC

| Old scada                             | Old PLC                               | New PLC/SCADA                                                                          | Description                                                                                           |     |
| ------------------------------------- | ------------------------------------- | -------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | --- |
| SCS_ACV_XZV100004                     | SCS_ACV_XZV100004                     | <span style="color:rgb(0, 176, 80)">SCS<i>ACV</i>XZV1001</span>                        | Station Inlet Isolation Valve                                                                         |     |
| SCS_ACV_XZV100005                     | SCS_ACV_XZV100005                     | <span style="color:rgb(0, 176, 80)">SCS<i>ACV</i>XZV1002</span>                        | Station Inlet Pressurisation Valve                                                                    |     |
| SCS_ACV_XZV400005                     | SCS_ACV_XZV400005                     | <span style="color:rgb(0, 176, 80)">SCS<i>ACV</i>XZV1003</span>                        | Station Outlet Isolation Valve                                                                        |     |
| SCS_ACV_XZV400006                     | SCS_ACV_XZV400006                     | <span style="color:rgb(0, 176, 80)">SCS<i>ACV</i>XZV1005</span>                        | Station Outlet Pressurisation Valve                                                                   |     |
| SCS_PCV_PCV800001?                    |                                       | <span style="color:rgb(255, 0, 0)">V1004</span>                                        |                                                                                                       |     |
| SCS_AIT_PIA100021                     | SCS_AIT_PIA100021                     | <span style="color:rgb(255, 255, 0)">SCS<i>AIT</i>PIA1005</span>                       | (P1) Station Suction Pressure                                                                         |     |
| SCS_AIT_TI1000020                     | SCS_AIT_TI1000020                     | <span style="color:rgb(255, 255, 0)">SCS<i>AIT</i>TI1005</span>                        | (Suc T) Station Suction Temperature                                                                   |     |
| SCS_AIT_PXIT100001/SCS_AIT_PXIT100002 | SCS_AIT_PXIT100001/SCS_AIT_PXIT100002 | <span style="color:rgb(0, 176, 80)">SCS<i>AIT</i>PXIT1001/SCS<i>AIT</i>PXIT1002</span> | Station Inlet Pressure Downstream of XZV100004 / Station Inlet Pressure Upstream of XZV100004         |     |
| SCS_AIT_PXIT400003/SCS_AIT_PXIT400007 | SCS_AIT_PXIT400003/SCS_AIT_PXIT400007 | <span style="color:rgb(0, 176, 80)">SCS<i>AIT</i>PXIT1003/SCS<i>AIT</i>PXIT1004</span> | Station Discharge Pressure Downstream of XZV400005 / Station Discharge Pressure Upstream of XZV400005 |     |
| SCS_AIT_TIA400002                     | SCS_AIT_TIA400002                     | <span style="color:rgb(255, 255, 0)">SCS<i>AIT</i>TIA1006 TIT1006</span>               | (Dis T) Station Discharge Temperature                                                                 |     |
| SCS_AIT_PIA400001                     | SCS_AIT_PIA400001                     | <span style="color:rgb(255, 255, 0)">SCS<i>AIT</i>PIA1006</span>                       | (P2) Station Discharge Pressure                                                                       |     |
| SCS_AIT_FT100020                      | SCS_AIT_FT100020                      | <span style="color:rgb(255, 255, 0)">SCS<i>AIT</i>FT1004</span>                        | Station Flow                                                                                          |     |
|                                       |                                       |                                                                                        |                                                                                                       |     |
|                                       |                                       |                                                                                        |                                                                                                       |     |
|                                       |                                       |                                                                                        |                                                                                                       |     |



| New                                               | Felindre                                |
| ------------------------------------------------- | --------------------------------------- |
| PIT1005                                           | SCS_AI_PIT100023                        |
| TIT1005                                           |                                         |
| PDIT1001                                          | SCS_AIT_PXIT100001 - SCS_AIT_PXIT100002 |
| V1001                                             | SCS_DO_SV100004                         |
| V1002                                             | SCS_DO_SV100005                         |
| PDIT1003                                          | SCS_AIT_PXIT400003 - SCS_AIT_PXIT400007 |
| V1005                                             | SCS_DO_SV400006                         |
| V1003                                             | SCS_DO_SV400005                         |
| TIT1006                                           | SCS_AI_PIT100016                        |
| PIT1006                                           |                                         |
| FIT1004                                           |                                         |
| <span style="color:rgb(0, 176, 80)">UnitA</span>  |                                         |
| PDIT10001                                         | UNA_AIT_PXIT210001 - UNA_AIT_PXIT210004 |
| V10001                                            | UNA_ACV_XZV210002                       |
| V10002                                            | UNA_ACV_XZV210003                       |
| PIT10005                                          | UNA_AIT_PIT210102                       |
| TIT10003                                          | UNA_AIT_TIT210007                       |
| V10005                                            | UNA_PCV_ZCV210016 ?                     |
| V10004                                            | UNA_ACV_XZV810001                       |
| V10003                                            |                                         |
| V10006                                            |                                         |
| PIT10006                                          | UNA_AIT_PIT210100                       |
| TIT10006                                          | UNA_AIT_TXIT210014                      |
| <span style="color:rgb(0, 176, 80)">Unit B</span> |                                         |
| PDIT20001                                         | UNB_AIT_PXIT220001 - UNB_AIT_PXIT220004 |
| V20001                                            | UNB_ACV_XZV220002                       |
| V20002                                            | UNB_ACV_XZV220003                       |
| PIT20005                                          | UNB_AIT_PIT220010                       |
| TIT20003                                          | UNB_AIT_TIT220007                       |
| V20005                                            | UNB_PCV_ZCV220016                       |
| V20004                                            | UNB_ACV_XZV820001                       |
| V20003                                            |                                         |
| V20006                                            |                                         |
| PIT20006                                          | UNB_AIT_PIT220013                       |
| TIT20006                                          | UNB_AIT_TI220014                        |
| <span style="color:rgb(0, 176, 80)">UnitC</span>  | ?                                       |
| PDIT10001                                         | UNC_AIT_PXIT230001 - UNC_AIT_PXIT230004 |
| V10001                                            | UNC_ACV_XZV230002                       |
| V10002                                            | UNC_ACV_XZV230003                       |
| PIT10005                                          | UNC_AIT_PIT230010                       |
| TIT10003                                          | UNC_AIT_TIT230007                       |
| V10005                                            | UNC_PCV_ZCV230016                       |
| V10004                                            | UNC_ACV_XZV830001                       |
| V10003                                            |                                         |
| V10006                                            |                                         |
| PIT10006                                          | UNC_AIT_PI230013                        |
| TIT10006                                          | UNC_AIT_TI230014                        |






# UNIT A
| Old scada           | Old PLC | New PLC/SCADA    |                                         |
| ------------------- | ------- | ---------------- | --------------------------------------- |
|                     |         | PDIT 10001       |                                         |
|                     |         | V10002           |                                         |
|                     |         | V10001           |                                         |
|                     |         | PIT10005         |                                         |
|                     |         | TIT10005         |                                         |
|                     |         | V10005           |                                         |
|                     |         | V10004           |                                         |
|                     |         | V10003           |                                         |
|                     |         | V10006           |                                         |
|                     |         | PIT10006         |                                         |
| SCS_AIT_TXIT400002A |         | SCS_AIT_TXIT1006 | Station Discharge Temperature 2oo3 Trip |
|                     |         |                  |                                         |
|                     |         |                  |                                         |
# UNIT B

| Old scada           | Old PLC | New PLC/SCADA    |                                         |
| ------------------- | ------- | ---------------- | --------------------------------------- |
|                     |         | PDIT 20001       |                                         |
|                     |         | V20002           |                                         |
|                     |         | V20001           |                                         |
|                     |         | PIT20005         |                                         |
|                     |         | TIT20005         |                                         |
|                     |         | V20005           |                                         |
|                     |         | V20004           |                                         |
|                     |         | V20003           |                                         |
|                     |         | V20006           |                                         |
|                     |         | PIT20006         |                                         |
| SCS_AIT_TXIT400002B |         | SCS_AIT_TXIT2006 | Station Discharge Temperature 2oo3 Trip |
|                     |         |                  |                                         |


# TODO
1. Przy wyszukiwaniu taga dodać timer, który przerwie wyszukwianie jesli przez jakis czas nie znajdzie wezla