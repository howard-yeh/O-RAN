# O-RAN
## Message Type Definition

### E2 Procesure
```c
//E2 setup 200~299

#define E2_Request 200
#define E2_Response 201
#define E2_Failure 204


//E2 reset 300~399

#define Reset_Request 300
#define Reset_Response 301


//Subscription 400~499

//Subscription Manager <--> E2 Termination
#define Sub_Request 400
#define Sub_Response 401
#define Sub_Failure 404

//xApp<---> Subscription Manager
#define Sub_Request 410
#define Sub_Response 411
#define Sub_Failure 414


//Subscription Delete 500~599

//Subscription Manager <--> E2 Termination
#define Sub_delreq 500
#define Sub_delrp 501
#define Sub_delfail 504

//xApp<---> Subscription Manager
#define Sub_delreq 510
#define Sub_delrp 511
#define Sub_delfail 514


//Control 600~699

//E2 Manager <--> E2 Termination
#define Ctrl_Request 600
#define Ctrl_Response 601
#define Ctrl_Failure 604

//xApp <-->E2 Manager
#define Ctrl_Request 610
#define Ctrl_Response 611
#define Ctrl_Failure 614


//Indication(Report) 700

#define Indi_Report 700

//Indication(Insert) 710

#define Indi_Insert 710

//Error Indication 740

#define Indi_Error 740


//Service Update 800

#define Serv_Update_Request 800
#define Serv_Update_Response 801
#define Serv_Update_Failure 804

//Service Query 810

#define Serv_Query 810

//xApp <---> Routing Manager 900~999

#define Item_Request 900
#define Item_Response 901
#define Item_Failure 904

//xApp --->RMR Manager (Asking for sending data)

#define Send_Request 910
#define Send_Response 911
#define Send_Failure 914

//xApp <---RMR Manager (Notify xApp initial successful)

#define Initial_Success 999

//Routing Manager send the broadcast to all 1000

#define Broadcast 1000


```

### xApp / For Database  (6000~6999)
```c
//(DB) xApp E2 setup

#define db_E2_Request 6200
#define db_E2_Response 6201
#define db_E2_Failure 6204

//(DB) xApp E2 Reset

#define db_Reset_Request 6300
#define db_Reset_Response 6301

//(DB) xApp Subscription

#define db_sub_Request 6400
#define db_sub_Response 6401
#define db_sub_Failure 6404

//(DB) xApp Subscription Delete

#define db_sub_delres 6500
#define db_sub_delrp 6501
#define db_sub_delfail 6504

//(DB) xApp Control

#define db_ctrl_Requestuest 6600
#define db_ctrl_Response 6601
#define db_ctrl_Failure 6604

//(DB) xApp Indication(Report) 

#define db_indication_report 6700
#define db_indication_report_Response 6701
#define db_indication_report_Failure 6704

//(DB) xApp Indication(Insert) 

#define db_indication_insert 6710
#define db_indication_insert_Response 6711
#define db_indication_insert_Failure 6714

//(DB) xApp Error Indication

#define db_error 6740


```

## Sepcific Port Definition

```c
//Manager_port 4000~4999

#define E2_Termination_port 4000
#define E2_T_RMR_Manager_port 4001

#define E2_Mgr 4200
#define E2_Mgr_RMR_Manager_port 4201

#define Subscription_Mgr 4400
#define E2_Mgr_RMR_Manager_port 4401

#define Routing_Mgr 4600

//database_port 6000~6999

#define Redis_Mgr_RIC 6000
#define RMR_Mgr_port_RIC 6001

#define Redis 6379

#define Redis_Mgr_Routing 6600
#define RMR_Mgr_port_Routing 6601

//xapp_port 8000~65000
// (total 57000/2 = 28500)
#define default_xapp 8000~36499
#define default_xapp 36500~64999

```