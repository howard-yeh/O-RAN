# O-RAN
## Message Type Definition

### E2 Procesure
```c
//E2 setup 200~299

#define E2_Request 200

#define E2_Response 201

#define E2_Failure 204

//E2 reset 300~399

#define reset_req 300
#define reset_rp 301


//Subscription 400~499

#define sub_Request 400
#define sub_Response 401
#define sub_Failure 404

//Delete 500~599
#define sub_delreq 500
#define sub_delrp 501
#define sub_delfail  504


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
//xApp

#define db_req 6000
#define db_rp 6001
#dfinee db_fail 6004

```


