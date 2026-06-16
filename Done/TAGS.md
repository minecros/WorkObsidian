
| OLD                 | NEW                                                               |     |
| ------------------- | ----------------------------------------------------------------- | --- |
| SCS_ACV_XZV100005   | <span style="color:rgb(0, 176, 80)">SCS_<i>ACV_</i>XZV1002</span> |     |
| SCS_ACV_XZV100004   | <span style="color:rgb(0, 176, 80)">SCS<i>ACV</i>XZV1001</span>   |     |
| SCS_ACV_XZV400006   | <span style="color:rgb(0, 176, 80)">SCS<i>ACV</i>XZV1005</span>   |     |
| SCS_ACV_XZV400005   | <span style="color:rgb(0, 176, 80)">SCS<i>ACV</i>XZV1003</span>   |     |
| SCS_AIT_PDIA100003  | <span style="color:rgb(0, 176, 80)">SCS<i>AIT</i>PDIT1001</span>  |     |
| SCS_AIT_PIT100023   | <span style="color:rgb(0, 176, 80)">SCS<i>AIT</i>PIT1005</span>   |     |
|                     | TIT1005                                                           |     |
|                     | V1004                                                             |     |
| SCS_AIT_PDIA400008  | <span style="color:rgb(0, 176, 80)">SCS<i>AIT</i>PDIT1003</span>  |     |
| SCS_AIT_TXIT400002A | <span style="color:rgb(0, 176, 80)">SCS<i>AIT</i>TIT1006</span>   |     |
| SCS_AIT_PIT100016   | SCS_AIT_PIT1006                                                   |     |
| SCS_AIT_FT100020    | SCS_AIT_FIT1004                                                   |     |
|                     |                                                                   |     |
|                     |                                                                   |     |


//SCS_AI_PIT1005
SCS_AIT_STN_SUC_P.PV_VAL := SCS_AI_PIT1005.PV;

//SCS_AI_TIT1004
SCS_AIT_STN_DIS_T.PV_VAL := SCS_AI_TIT1004.PV;

//SCS_AI_PIT1006
SCS_AIT_STN_DIS_P.PV_VAL := SCS_AI_PIT1006.PV;

//SCS_AIT_FIT1004
SCS_AIT_STN_FLOW.PV_VAL := SCS_AI_FIT1004.PV;




//	FIT100016 - Analog Input
SCS_AI_FIT1004.IO_STAT := 0;
SCS_AI_FIT1004.IO_CH_STAT := 0;
SCS_AI_FIT1004.IO_RAW := 0;
SCS_AI_FIT1004.HYST_TIME := 0;
SCS_AI_FIT1004.HYST_DB := 0;
SCS_AI_FIT1004.PLANT_STAT := 0;
SCS_AI_FIT1004.STAG_TIME1 := 0;
SCS_AI_FIT1004.STAG_DB1 := 0;
SCS_AI_FIT1004.STAG_TIME2 := 0;
SCS_AI_FIT1004.STAG_DB2 := 0;
SCS_AI_FIT1004.STAG_TIME3 := 0;
SCS_AI_FIT1004.STAG_DB3 := 0;
SCS_AI_FIT1004.STAG_TIME4 := 0;
SCS_AI_FIT1004.STAG_DB4 := 0;
SCS_AI_FIT1004.SCL_LO := 0;
SCS_AI_FIT1004.SCL_HI := 100;
SCS_AI_FIT1004.SCL_ENB := 1;
AI1(SCS_AI_FIT1004_INSTANCE, SCS_AI_FIT1004);

//	PIT1006 - Analog Input
SCS_AI_PIT1006.IO_STAT := 0;
SCS_AI_PIT1006.IO_CH_STAT := 0;
SCS_AI_PIT1006.IO_RAW := 0;
SCS_AI_PIT1006.HYST_TIME := 0;
SCS_AI_PIT1006.HYST_DB := 0;
SCS_AI_PIT1006.PLANT_STAT := 0;
SCS_AI_PIT1006.STAG_TIME1 := 0;
SCS_AI_PIT1006.STAG_DB1 := 0;
SCS_AI_PIT1006.STAG_TIME2 := 0;
SCS_AI_PIT1006.STAG_DB2 := 0;
SCS_AI_PIT1006.STAG_TIME3 := 0;
SCS_AI_PIT1006.STAG_DB3 := 0;
SCS_AI_PIT1006.STAG_TIME4 := 0;
SCS_AI_PIT1006.STAG_DB4 := 0;
SCS_AI_PIT1006.SCL_LO := 0;
SCS_AI_PIT1006.SCL_HI := 100;
SCS_AI_PIT1006.SCL_ENB := 1;
AI1(SCS_AI_PIT1006_INSTANCE, SCS_AI_PIT1006);

//	TIT1004 - Analog Input
SCS_AI_TIT1004.IO_STAT := 0;
SCS_AI_TIT1004.IO_CH_STAT := 0;
SCS_AI_TIT1004.IO_RAW := 0;
SCS_AI_TIT1004.HYST_TIME := 0;
SCS_AI_TIT1004.HYST_DB := 0;
SCS_AI_TIT1004.PLANT_STAT := 0;
SCS_AI_TIT1004.STAG_TIME1 := 0;
SCS_AI_TIT1004.STAG_DB1 := 0;
SCS_AI_TIT1004.STAG_TIME2 := 0;
SCS_AI_TIT1004.STAG_DB2 := 0;
SCS_AI_TIT1004.STAG_TIME3 := 0;
SCS_AI_TIT1004.STAG_DB3 := 0;
SCS_AI_TIT1004.STAG_TIME4 := 0;
SCS_AI_TIT1004.STAG_DB4 := 0;
SCS_AI_TIT1004.SCL_LO := 0;
SCS_AI_TIT1004.SCL_HI := 100;
SCS_AI_TIT1004.SCL_ENB := 1;
AI1(SCS_AI_TIT1004_INSTANCE, SCS_AI_TIT1004);

//	PIT1005 - Analog Input
SCS_AI_PIT1005.IO_STAT := 0;
SCS_AI_PIT1005.IO_CH_STAT := 0;
SCS_AI_PIT1005.IO_RAW := 0;
SCS_AI_PIT1005.HYST_TIME := 0;
SCS_AI_PIT1005.HYST_DB := 0;
SCS_AI_PIT1005.PLANT_STAT := 0;
SCS_AI_PIT1005.STAG_TIME1 := 0;
SCS_AI_PIT1005.STAG_DB1 := 0;
SCS_AI_PIT1005.STAG_TIME2 := 0;
SCS_AI_PIT1005.STAG_DB2 := 0;
SCS_AI_PIT1005.STAG_TIME3 := 0;
SCS_AI_PIT1005.STAG_DB3 := 0;
SCS_AI_PIT1005.STAG_TIME4 := 0;
SCS_AI_PIT1005.STAG_DB4 := 0;
SCS_AI_PIT1005.SCL_LO := 0;
SCS_AI_PIT1005.SCL_HI := 100;
SCS_AI_PIT1005.SCL_ENB := 1;
AI1(SCS_AI_PIT1005_INSTANCE, SCS_AI_PIT1005);