# O-RAN
## Message Type Definition

### E2 Procesure
```c
//E2 setup 200~299

#define E2_Request 200
#define E2_Response 201
#define E2_Failure 204


//E2 reset 300~399

#define Reset_req 300
#define Reset_rp 301


//Subscription 400~499

//Subscription Manager <--> E2 Termination
#define sub_Request 400
#define sub_Response 401
#define sub_Failure 404

//xApp<---> Subscription Manager
#define sub_Request 410
#define sub_Response 411
#define sub_Failure 414


//Subscription Delete 500~599

//Subscription Manager <--> E2 Termination
#define sub_delreq 500
#define sub_delrp 501
#define sub_delfail 504

//xApp<---> Subscription Manager
#define sub_delreq 510
#define sub_delrp 511
#define sub_delfail 514


//Control 600~699

//E2 Manager <--> E2 Termination
#define ctrl_request 600
#define ctrl_ack 601
#define ctrl_fail 604

//xApp <-->E2 Manager
#define ctrl_request 610
#define ctrl_ack 611
#define ctrl_fail 614


//Indication(Report) 700

#define indi_report 700

//Indication(Insert) 710

#define indi_insert 710

//Error Indication 740

#define indi_error 740


//Service updata 800

#define serv_update 800
#define serv_ack 801
#define serv_fail 804

//Service Query 810

#define serv_query 810

//xApp <---> Routing Manager 900~999

#define item_req 900
#define item_rp 901
#define item_fail 904

//Routing Manager send the broadcast to all 1000

#define broadcast 1000

```

### xApp / Database => 6000~6999
```c
//xApp E2 setup

#define db_E2_Request 6200
#define db_E2_Response 6201
#define db_E2_Failure 6204

//xApp E2 Reset

#define db_Reset_req 6300
#define db_Reset_rp 6301

//xApp Subscription

#define db_sub_Request 6400
#define db_sub_Response 6401
#define db_sub_Failure 6404

//xApp Subscription Delete

#define db_sub_delreq 6500
#define db_sub_delrp 6501
#define db_sub_delfail 6504

//xApp Control

#define db_ctrl_request 6600
#define db_ctrl_ack 6601
#define db_ctrl_fail 6604

//xApp Indication(Report) 

#define db_indication 6700
#define db_indication_ack 6701
#define db_indication_failure 6704

//xApp Error Indication

#define db_error 6800

```

## Sepcific Port Definition

```c
//Manager_port 4000~4999

#define E2_Termination_port 4000

#define E2_Mgr 4200

#define Subscription_Mgr 4400

#define Routing_Mgr 4600

//database_port 6000~6999

#define redis_Mgr 6000

#define redis 6379

//xapp_port 8000~16000

#define default_xapp 8000

```