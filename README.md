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

#define sub_Request 400
#define sub_Response 401
#define sub_Failure 404

//Delete 500~599

#define sub_delreq 500
#define sub_delrp 501
#define sub_delfail 504


//Control 600~699

#define ctrl_request 600
#define ctrl_ack 601
#define ctrl_fail 604

//Indication(Report) 700

#define indication 700

//Error Indication 800

#define error 800

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

//xApp Error Indication

#define db_error 6800

```
