---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
Client
- Desktop client
- Web Client ^OfakKwrS

Platform Services
- Auth / User Profiles
- Messaging / Notifications
- Storage
- Video streaming (P2P)
- Monitoring service
- Message Bus
- Load balancer


 ^Lo8np7sl

MVP Phase 1: ^TfWpgEYb

- Desktop client
- User Profiles
    - Logging in and basic user data
    - Basic roles, no need for RBAC just yet
- Messaging 
    - P2P messaging
    - Add user to message group
- Notifications
- Monitoring

 ^lgdhUL4E

MVP Phase 2: ^Kiu4UOtU

- Message Bus
- File uploads
- Video Streaming

 ^APuENio0

MVP Phase 3: ^TjRLBFGg

- Load balancer
- Stress testing
- Advanced monitoring ^k1D4z0j1

Messaging/Notif ^s5qX60VG

Storage ^j41He40b

Video/Voice ^uVJSCs0H

Desktop Client+
Web Client +
Web Server ^agawq6v6

Project Outline ^5Ve6xy0m

Desktop
Client ^dc1IzWqi

User
Service
(TS) ^s8g9bQTy

Messaging/
Notifications
Service
(Go) ^CPfngnVr

Monitoring
(Go) ^UiQaAg2a

Orchestrator Service (Proxy) ^DAkrunmv

(Go) (Service Discovery) ^qMP5a2Rf

Service Registry ^BhLOTpwG

User Service: localhost:8080 ^vIEnpZv0

Messaging Service: localhost:8081 ^WZYLt9ab

Monitoring: localhost:8082 ^U41vSA5r

/ap ^fikG50Wv

Web
Client ^ju8yFEld

GRPC ^YZKoLz53

GRPC ^niYpIEyd

Read ^JNWW3sOn

Write ^9EnJztNz

Phase One ^OZ1XGkzU

Client ^fCX8xLE5

User
Service
(TS) ^sStVpLUd

Messaging/
Notifications
Service
(Go) ^A7jEAjoO

Monitoring
(Go) ^hXyaOGMK

Orchestrator Service (Proxy) ^S3VdX8xA

(Go) (Service Discovery) ^tsuvsC3o

GRPC ^iYKQPdE7

GRPC ^Gm6trphb

Read ^hXM483kS

Write ^PDDQru9T

Phase Two ^6ZmWHhFa

Storage
Service ^8NRT1919

Streaming
Service ^gmBZ1VcK

Message Q ^t9bS9jgM

Cloudflare S ^yOkrlYEe

User
Service
(TS) ^GzY4mVIK

Messaging/
Notifications
Service
(Go) ^c8qhZwZx

Monitoring
(Go) ^4QLLPQUI

Orchestrator Service (Proxy) ^YBBBWyOp

(Go) (Service Discovery) ^MHCfSjtU

GRPC ^C7l9hWOE

GRPC ^1FVdfmjJ

Read ^3xURBCzK

Write ^b4RFxYWW

Storage
Service ^x8IHKpp5

Streaming
Service ^ZsHaJFaB

Message Q ^PpTXSIFf

Cloudflare S ^orXmcoC3

Node 1 ^IkGxTPvR

User
Service
(TS) ^uOeeViPu

Messaging/
Notifications
Service
(Go) ^jsUl1bA3

Orchestrator Service (Proxy) ^E80V3AVB

(Go) (Service Discovery) ^LNtKujny

GRPC ^OzMAE50J

GRPC ^AnDPj3lg

Storage
Service ^VoUWSevZ

Streaming
Service ^io5qgSF9

Message Q ^dKPCKvaT

Node 2 ^5G7lVZ4M

User
Service
(TS) ^IrJB5wfP

Messaging/
Notifications
Service
(Go) ^1ZItKg7e

Orchestrator Service (Proxy) ^ZnTHsicc

(Go) (Service Discovery) ^KTLTTDaA

GRPC ^4b8mh5jt

GRPC ^8neGL49g

Storage
Service ^VVbBHD6E

Streaming
Service ^UdS9KHsW

Message Q ^YvDK2xIo

Node 3 ^xup9WkT2

Load Balancer ^TRIA9BSj

Client ^nBDHhpFh

Prometheus ^MPU3Xob2

Grafana ^17YQdwAx

Notes:
- The monitoring may need its own node
- Need to do stress testings
learning about generating fake users because we cant
get real users ^wUi4m7JH

PHP API ^eQLaOYMI

HTMX ^oi0DrioS

Sequence# Size ^1xqTt0a9

Data ^T7lvSFzv

Server ^H0GPAiPb

Client ^p68I1q0u

Sequence# Size ^t1VTM3Xb

Data ^XfSMdPb1

register => [seq#, size, size]
get(servize_a) => [seq#, sizeSent, size, data]
delete => [seq#, sizeSent, size, data]
update => [seq#, sizeSent, size] ^F1g48v1F


# Embedded files
11df65c7024920ac84ab4c2c6d08d0f77dbecc76: [[Pasted Image 20230809193229_688.png]]

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.8",
	"elements": [
		{
			"type": "text",
			"version": 357,
			"versionNonce": 296083446,
			"isDeleted": false,
			"id": "OfakKwrS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2228.91855032384,
			"y": -2086.9928792727915,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 324.07427978515625,
			"height": 153.00000000000006,
			"seed": 190713236,
			"groupIds": [
				"8WXXf8yd6DOUqnX853ChQ",
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 40.80000000000002,
			"fontFamily": 1,
			"text": "Client\n- Desktop client\n- Web Client",
			"rawText": "Client\n- Desktop client\n- Web Client",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Client\n- Desktop client\n- Web Client",
			"lineHeight": 1.25,
			"baseline": 138
		},
		{
			"type": "text",
			"version": 553,
			"versionNonce": 740344426,
			"isDeleted": false,
			"id": "Lo8np7sl",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1827.627664680555,
			"y": -2087.4730345321454,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 545.4550170898438,
			"height": 561.0000000000002,
			"seed": 765924628,
			"groupIds": [
				"8WXXf8yd6DOUqnX853ChQ",
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 40.80000000000002,
			"fontFamily": 1,
			"text": "Platform Services\n- Auth / User Profiles\n- Messaging / Notifications\n- Storage\n- Video streaming (P2P)\n- Monitoring service\n- Message Bus\n- Load balancer\n\n\n",
			"rawText": "Platform Services\n- Auth / User Profiles\n- Messaging / Notifications\n- Storage\n- Video streaming (P2P)\n- Monitoring service\n- Message Bus\n- Load balancer\n\n\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Platform Services\n- Auth / User Profiles\n- Messaging / Notifications\n- Storage\n- Video streaming (P2P)\n- Monitoring service\n- Message Bus\n- Load balancer\n\n\n",
			"lineHeight": 1.25,
			"baseline": 546
		},
		{
			"type": "text",
			"version": 359,
			"versionNonce": 890401078,
			"isDeleted": false,
			"id": "TfWpgEYb",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2159.7429815091605,
			"y": -1487.995709969231,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 550.6636352539062,
			"height": 108.0783380179368,
			"seed": 475554196,
			"groupIds": [
				"QCl2OO9N1AwPdlLVJHavV",
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 86.46267041434945,
			"fontFamily": 1,
			"text": "MVP Phase 1:",
			"rawText": "MVP Phase 1:",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "MVP Phase 1:",
			"lineHeight": 1.25,
			"baseline": 76
		},
		{
			"type": "text",
			"version": 578,
			"versionNonce": 812705066,
			"isDeleted": false,
			"id": "lgdhUL4E",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2174.9306985979233,
			"y": -1353.0218762280324,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 907.9259033203125,
			"height": 553.1318272774396,
			"seed": 1603471276,
			"groupIds": [
				"QCl2OO9N1AwPdlLVJHavV",
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 40.22776925654106,
			"fontFamily": 1,
			"text": "- Desktop client\n- User Profiles\n    - Logging in and basic user data\n    - Basic roles, no need for RBAC just yet\n- Messaging \n    - P2P messaging\n    - Add user to message group\n- Notifications\n- Monitoring\n\n",
			"rawText": "- Desktop client\n- User Profiles\n    - Logging in and basic user data\n    - Basic roles, no need for RBAC just yet\n- Messaging \n    - P2P messaging\n    - Add user to message group\n- Notifications\n- Monitoring\n\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- Desktop client\n- User Profiles\n    - Logging in and basic user data\n    - Basic roles, no need for RBAC just yet\n- Messaging \n    - P2P messaging\n    - Add user to message group\n- Notifications\n- Monitoring\n\n",
			"lineHeight": 1.25,
			"baseline": 538
		},
		{
			"type": "text",
			"version": 413,
			"versionNonce": 2002442870,
			"isDeleted": false,
			"id": "Kiu4UOtU",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2175.293059062965,
			"y": -763.0115240315661,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 588.79248046875,
			"height": 108.0783380179368,
			"seed": 285521044,
			"groupIds": [
				"fHTS_n0eCe1SfoK9q9Bp1",
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 86.46267041434945,
			"fontFamily": 1,
			"text": "MVP Phase 2:",
			"rawText": "MVP Phase 2:",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "MVP Phase 2:",
			"lineHeight": 1.25,
			"baseline": 76
		},
		{
			"type": "text",
			"version": 674,
			"versionNonce": 1680781290,
			"isDeleted": false,
			"id": "APuENio0",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2190.4807761517286,
			"y": -628.0376902903672,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 340.019775390625,
			"height": 251.42355785338162,
			"seed": 1093206548,
			"groupIds": [
				"fHTS_n0eCe1SfoK9q9Bp1",
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 40.22776925654106,
			"fontFamily": 1,
			"text": "- Message Bus\n- File uploads\n- Video Streaming\n\n",
			"rawText": "- Message Bus\n- File uploads\n- Video Streaming\n\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- Message Bus\n- File uploads\n- Video Streaming\n\n",
			"lineHeight": 1.25,
			"baseline": 236
		},
		{
			"type": "text",
			"version": 485,
			"versionNonce": 1061428150,
			"isDeleted": false,
			"id": "TjRLBFGg",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2183.5835360106244,
			"y": -374.83950929786386,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 586.1122436523438,
			"height": 108.0783380179368,
			"seed": 311948564,
			"groupIds": [
				"H_tEdS5iX_NUbvZiJ2yT3",
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 86.46267041434945,
			"fontFamily": 1,
			"text": "MVP Phase 3:",
			"rawText": "MVP Phase 3:",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "MVP Phase 3:",
			"lineHeight": 1.25,
			"baseline": 76
		},
		{
			"type": "text",
			"version": 798,
			"versionNonce": 1533354666,
			"isDeleted": false,
			"id": "k1D4z0j1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2198.771253099388,
			"y": -239.865675556665,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 423.1142578125,
			"height": 150.85413471202895,
			"seed": 528495252,
			"groupIds": [
				"H_tEdS5iX_NUbvZiJ2yT3",
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 40.22776925654106,
			"fontFamily": 1,
			"text": "- Load balancer\n- Stress testing\n- Advanced monitoring",
			"rawText": "- Load balancer\n- Stress testing\n- Advanced monitoring",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- Load balancer\n- Stress testing\n- Advanced monitoring",
			"lineHeight": 1.25,
			"baseline": 136
		},
		{
			"type": "text",
			"version": 373,
			"versionNonce": 1391670518,
			"isDeleted": false,
			"id": "s5qX60VG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -703.178059383843,
			"y": -1794.6311765772793,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 401.54388427734375,
			"height": 64.9999999999999,
			"seed": 495134252,
			"groupIds": [
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 51.99999999999992,
			"fontFamily": 1,
			"text": "Messaging/Notif",
			"rawText": "Messaging/Notif",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Messaging/Notif",
			"lineHeight": 1.25,
			"baseline": 46
		},
		{
			"type": "text",
			"version": 491,
			"versionNonce": 1891581290,
			"isDeleted": false,
			"id": "j41He40b",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -701.8584689636498,
			"y": -1711.2978432439463,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 194.45179748535156,
			"height": 62.777777777777786,
			"seed": 1417987116,
			"groupIds": [
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 50.22222222222223,
			"fontFamily": 1,
			"text": "Storage",
			"rawText": "Storage",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Storage",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "text",
			"version": 492,
			"versionNonce": 1810703926,
			"isDeleted": false,
			"id": "uVJSCs0H",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -690.7553960130747,
			"y": -1656.853398799502,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 310.0318908691406,
			"height": 73.88888888888877,
			"seed": 1189942316,
			"groupIds": [
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 59.11111111111102,
			"fontFamily": 1,
			"text": "Video/Voice",
			"rawText": "Video/Voice",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Video/Voice",
			"lineHeight": 1.25,
			"baseline": 51
		},
		{
			"type": "text",
			"version": 554,
			"versionNonce": 1904738346,
			"isDeleted": false,
			"id": "agawq6v6",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -720.9558371616213,
			"y": -2099.075621021724,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 405.54791259765625,
			"height": 194.99999999999972,
			"seed": 1101038892,
			"groupIds": [
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 51.99999999999992,
			"fontFamily": 1,
			"text": "Desktop Client+\nWeb Client +\nWeb Server",
			"rawText": "Desktop Client+\nWeb Client +\nWeb Server",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Desktop Client+\nWeb Client +\nWeb Server",
			"lineHeight": 1.25,
			"baseline": 176
		},
		{
			"type": "rectangle",
			"version": 223,
			"versionNonce": 1259794294,
			"isDeleted": false,
			"id": "0Et_Ws17q6gCq2VGmnUsd",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2468.609696048504,
			"y": -2259.661140456989,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2511.999999999999,
			"height": 2363.9999999999995,
			"seed": 449880768,
			"groupIds": [
				"-Mze2HERiivngwu5Mv0Ak",
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 255,
			"versionNonce": 1235905258,
			"isDeleted": false,
			"id": "5Ve6xy0m",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1804.609696048504,
			"y": -2495.661140456989,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1077.6015625,
			"height": 180.99999999999997,
			"seed": 72483520,
			"groupIds": [
				"I18VN3j5bcbRKhL3AKlzK"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 144.79999999999998,
			"fontFamily": 1,
			"text": "Project Outline",
			"rawText": "Project Outline",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Project Outline",
			"lineHeight": 1.25,
			"baseline": 127
		},
		{
			"type": "rectangle",
			"version": 255,
			"versionNonce": 1286967478,
			"isDeleted": false,
			"id": "PVB_lgcnMp9CP1fC3hJI6",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1275.1839547451443,
			"y": -742.3436801395274,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 717.1428571428571,
			"height": 488.57142857142844,
			"seed": 522840768,
			"groupIds": [
				"rp4RJGbhrLPkoBYoF0pSt",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "ar9FnCxUGMFyhs_C5lw_O",
					"type": "arrow"
				}
			],
			"updated": 1692907864758,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 282,
			"versionNonce": 800161194,
			"isDeleted": false,
			"id": "dc1IzWqi",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1448.9934785546677,
			"y": -655.6770134728608,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 451.3149719238281,
			"height": 284.28571428571394,
			"seed": 1452931776,
			"groupIds": [
				"rp4RJGbhrLPkoBYoF0pSt",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 113.71428571428558,
			"fontFamily": 1,
			"text": "Desktop\nClient",
			"rawText": "Desktop\nClient",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Desktop\nClient",
			"lineHeight": 1.25,
			"baseline": 242
		},
		{
			"type": "rectangle",
			"version": 327,
			"versionNonce": 2087586294,
			"isDeleted": false,
			"id": "4D-GyM5RJ2IzfNcn68WgV",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1197.5649071260978,
			"y": -2462.819870615718,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 717.1428571428571,
			"height": 488.57142857142844,
			"seed": 821457216,
			"groupIds": [
				"J1XzoIxmk3buJkJ1fQuRj",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "fySl68hHDWJ8OZO-b1I4Y",
					"type": "arrow"
				},
				{
					"id": "2Y1KyCR9TE8B6l2GDWFIh",
					"type": "arrow"
				},
				{
					"id": "l7HeP984GxVemLP6uNzPE",
					"type": "arrow"
				}
			],
			"updated": 1692907864758,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 363,
			"versionNonce": 1355298922,
			"isDeleted": false,
			"id": "s8g9bQTy",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1366.1363356975262,
			"y": -2411.3912991871466,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 383.8849182128906,
			"height": 426.4285714285709,
			"seed": 1133922624,
			"groupIds": [
				"J1XzoIxmk3buJkJ1fQuRj",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 113.71428571428558,
			"fontFamily": 1,
			"text": "User\nService\n(TS)",
			"rawText": "User\nService\n(TS)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "User\nService\n(TS)",
			"lineHeight": 1.25,
			"baseline": 384
		},
		{
			"type": "rectangle",
			"version": 309,
			"versionNonce": 692411190,
			"isDeleted": false,
			"id": "Rd4ZgU2s-6gNdiQ-SxhPO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2783.2791928403826,
			"y": -2465.677013472861,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 717.1428571428571,
			"height": 488.57142857142844,
			"seed": 38050496,
			"groupIds": [
				"7xZ5i2cbDquYushhlkdyx",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "S9eVbb6fwhlSQfCKeAYLA",
					"type": "arrow"
				},
				{
					"id": "YpjL4dvCKOCN09IvqBh0l",
					"type": "arrow"
				},
				{
					"id": "AsEiIMvcKm-YWcqKPHpcb",
					"type": "arrow"
				},
				{
					"id": "AOiXjcqLm3sUg3F-r7A0b",
					"type": "arrow"
				}
			],
			"updated": 1692907864758,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 427,
			"versionNonce": 2092538666,
			"isDeleted": false,
			"id": "CPfngnVr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2893.9218908558682,
			"y": -2414.24844204429,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 506.92877197265625,
			"height": 408.571428571428,
			"seed": 1818444480,
			"groupIds": [
				"7xZ5i2cbDquYushhlkdyx",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 81.7142857142856,
			"fontFamily": 1,
			"text": "Messaging/\nNotifications\nService\n(Go)",
			"rawText": "Messaging/\nNotifications\nService\n(Go)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Messaging/\nNotifications\nService\n(Go)",
			"lineHeight": 1.25,
			"baseline": 377
		},
		{
			"type": "rectangle",
			"version": 782,
			"versionNonce": 2040562806,
			"isDeleted": false,
			"id": "psebmuHaa6VKQsxeTsLSY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1204.8268118880037,
			"y": -3097.2246325204824,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 585.0375939849623,
			"height": 398.57142857142844,
			"seed": 1254261056,
			"groupIds": [
				"FmyxhgueA8XD_RtbEv0LF",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "nT7KLKs_v7_Ac-JL7Vcjz",
					"type": "arrow"
				}
			],
			"updated": 1692907864758,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 900,
			"versionNonce": 1374725610,
			"isDeleted": false,
			"id": "UiQaAg2a",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1348.4767286300848,
			"y": -2964.36748966334,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 316.1016845703125,
			"height": 166.65413533834564,
			"seed": 1767921984,
			"groupIds": [
				"FmyxhgueA8XD_RtbEv0LF",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864758,
			"link": null,
			"locked": false,
			"fontSize": 66.66165413533825,
			"fontFamily": 1,
			"text": "Monitoring\n(Go)",
			"rawText": "Monitoring\n(Go)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Monitoring\n(Go)",
			"lineHeight": 1.25,
			"baseline": 141
		},
		{
			"type": "rectangle",
			"version": 279,
			"versionNonce": 2135197110,
			"isDeleted": false,
			"id": "AXBtSNbG-w1-X5jpa0Arg",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 958.9934785546687,
			"y": -1507.1055849014367,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2828.5714285714284,
			"height": 234.28571428571422,
			"seed": 883839296,
			"groupIds": [
				"fS_SQL2FnBh9sszuaAMUe",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "ar9FnCxUGMFyhs_C5lw_O",
					"type": "arrow"
				},
				{
					"id": "fySl68hHDWJ8OZO-b1I4Y",
					"type": "arrow"
				},
				{
					"id": "HTOv6us5KuCkrzkoY8GQ7",
					"type": "arrow"
				}
			],
			"updated": 1692907864758,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 301,
			"versionNonce": 1769494698,
			"isDeleted": false,
			"id": "DAkrunmv",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1884.155471381585,
			"y": -1441.8674896633418,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1002.0521850585938,
			"height": 87.85714285714285,
			"seed": 539017536,
			"groupIds": [
				"fS_SQL2FnBh9sszuaAMUe",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 70.28571428571428,
			"fontFamily": 1,
			"text": "Orchestrator Service (Proxy)",
			"rawText": "Orchestrator Service (Proxy)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Orchestrator Service (Proxy)",
			"lineHeight": 1.25,
			"baseline": 61
		},
		{
			"type": "text",
			"version": 352,
			"versionNonce": 1263951606,
			"isDeleted": false,
			"id": "qMP5a2Rf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2145.80316669893,
			"y": -1346.875922203022,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 505.28704833984375,
			"height": 53.571428571428555,
			"seed": 341523136,
			"groupIds": [
				"fS_SQL2FnBh9sszuaAMUe",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 42.85714285714285,
			"fontFamily": 1,
			"text": "(Go) (Service Discovery)",
			"rawText": "(Go) (Service Discovery)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "(Go) (Service Discovery)",
			"lineHeight": 1.25,
			"baseline": 37
		},
		{
			"type": "rectangle",
			"version": 252,
			"versionNonce": 50049898,
			"isDeleted": false,
			"id": "frXVMpO7_VpWFTx65tYmf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4244.149322710514,
			"y": -2283.4372497643517,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 800,
			"height": 474.1666666666665,
			"seed": 1872812352,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 186,
			"versionNonce": 39522358,
			"isDeleted": false,
			"id": "BhLOTpwG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4378.369400225162,
			"y": -2396.4372497643512,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 469.679931640625,
			"height": 74.99999999999979,
			"seed": 619680448,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 59.99999999999983,
			"fontFamily": 1,
			"text": "Service Registry",
			"rawText": "Service Registry",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Service Registry",
			"lineHeight": 1.25,
			"baseline": 53
		},
		{
			"type": "rectangle",
			"version": 248,
			"versionNonce": 818263594,
			"isDeleted": false,
			"id": "X0ZXqGpbeOLPxBMORpS5r",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4239.982656043847,
			"y": -2289.7705830976847,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 803.3333333333339,
			"height": 156.66666666666674,
			"seed": 1280940352,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "S9eVbb6fwhlSQfCKeAYLA",
					"type": "arrow"
				},
				{
					"id": "2Y1KyCR9TE8B6l2GDWFIh",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 220,
			"versionNonce": 1882691958,
			"isDeleted": false,
			"id": "vIEnpZv0",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4305.511592811427,
			"y": -2234.7705830976856,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 662.6298217773438,
			"height": 57.500000000000185,
			"seed": 1801433408,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 46.00000000000015,
			"fontFamily": 1,
			"text": "User Service: localhost:8080",
			"rawText": "User Service: localhost:8080",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "User Service: localhost:8080",
			"lineHeight": 1.25,
			"baseline": 40
		},
		{
			"type": "rectangle",
			"version": 296,
			"versionNonce": 63004906,
			"isDeleted": false,
			"id": "pWDB6xc8VFN5DfdmHmST5",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4241.649322710515,
			"y": -2130.6039164310187,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 803.3333333333339,
			"height": 156.66666666666674,
			"seed": 802273600,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 283,
			"versionNonce": 472971958,
			"isDeleted": false,
			"id": "WZYLt9ab",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4258.809271440985,
			"y": -2078.1039164310205,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 759.3677978515625,
			"height": 57.500000000000185,
			"seed": 1472762176,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 46.00000000000015,
			"fontFamily": 1,
			"text": "Messaging Service: localhost:8081",
			"rawText": "Messaging Service: localhost:8081",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Messaging Service: localhost:8081",
			"lineHeight": 1.25,
			"baseline": 40
		},
		{
			"type": "rectangle",
			"version": 283,
			"versionNonce": 930722730,
			"isDeleted": false,
			"id": "9-vaTxATX-xcvOUEOhv2J",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4239.149322710515,
			"y": -1968.1039164310187,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 803.3333333333339,
			"height": 156.66666666666674,
			"seed": 1537284416,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "OahcvSO8R-HlP3Texwo3k",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 265,
			"versionNonce": 1558983670,
			"isDeleted": false,
			"id": "U41vSA5r",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4335.5904237847335,
			"y": -1913.1039164310205,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 600.8058471679688,
			"height": 57.500000000000185,
			"seed": 313258304,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 46.00000000000015,
			"fontFamily": 1,
			"text": "Monitoring: localhost:8082",
			"rawText": "Monitoring: localhost:8082",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Monitoring: localhost:8082",
			"lineHeight": 1.25,
			"baseline": 40
		},
		{
			"type": "arrow",
			"version": 156,
			"versionNonce": 1578741354,
			"isDeleted": false,
			"id": "OahcvSO8R-HlP3Texwo3k",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4243.315989377181,
			"y": -1807.2705830976856,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 465.00000000000045,
			"height": 312.5,
			"seed": 536826560,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "9-vaTxATX-xcvOUEOhv2J",
				"focus": 0.5301541153163375,
				"gap": 4.166666666666174
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-465.00000000000045,
					312.5
				]
			]
		},
		{
			"type": "arrow",
			"version": 227,
			"versionNonce": 1819166006,
			"isDeleted": false,
			"id": "ar9FnCxUGMFyhs_C5lw_O",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1661.6493227105143,
			"y": -748.9372497643519,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 659.1666666666665,
			"height": 518.3333333333337,
			"seed": 1430000320,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "PVB_lgcnMp9CP1fC3hJI6",
				"focus": -0.43505227926523926,
				"gap": 6.593569624824568
			},
			"endBinding": {
				"elementId": "AXBtSNbG-w1-X5jpa0Arg",
				"focus": -0.06624945523617212,
				"gap": 5.549287518036863
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					659.1666666666665,
					-518.3333333333337
				]
			]
		},
		{
			"type": "arrow",
			"version": 344,
			"versionNonce": 208425258,
			"isDeleted": false,
			"id": "S9eVbb6fwhlSQfCKeAYLA",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3491.6813539583122,
			"y": -2467.6277259548283,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 796.6346354188686,
			"height": 150.35714285714266,
			"seed": 909800128,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Rd4ZgU2s-6gNdiQ-SxhPO",
				"focus": -1.0069984013056423,
				"gap": 1.9507124819674573
			},
			"endBinding": {
				"elementId": "X0ZXqGpbeOLPxBMORpS5r",
				"focus": 0.05003794374765415,
				"gap": 27.50000000000091
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					266.6346354188686,
					5.714285714285779
				],
				[
					796.6346354188686,
					150.35714285714266
				]
			]
		},
		{
			"type": "arrow",
			"version": 908,
			"versionNonce": 2082221686,
			"isDeleted": false,
			"id": "2Y1KyCR9TE8B6l2GDWFIh",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1929.8636909219676,
			"y": -2057.627725954828,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2294.5237270266425,
			"height": 602.619047619047,
			"seed": 1733306688,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "4D-GyM5RJ2IzfNcn68WgV",
				"focus": 0.19794574765214612,
				"gap": 15.155926653012898
			},
			"endBinding": {
				"elementId": "X0ZXqGpbeOLPxBMORpS5r",
				"focus": 0.4109594044863621,
				"gap": 15.59523809523671
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					1280.3570603599746,
					324.0476190476181
				],
				[
					1911.6665841694983,
					165.71428571428532
				],
				[
					1916.6665841694983,
					-278.5714285714289
				],
				[
					2294.5237270266425,
					-242.1428571428578
				]
			]
		},
		{
			"type": "arrow",
			"version": 226,
			"versionNonce": 98343914,
			"isDeleted": false,
			"id": "fySl68hHDWJ8OZO-b1I4Y",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2131.591151818481,
			"y": -1509.7705830976856,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 256.6209961998795,
			"height": 462.1428571428569,
			"seed": 554019520,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "YZKoLz53"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "AXBtSNbG-w1-X5jpa0Arg",
				"focus": -0.11840504502066795,
				"gap": 2.6649981962489164
			},
			"endBinding": {
				"elementId": "4D-GyM5RJ2IzfNcn68WgV",
				"focus": -0.3680328094382571,
				"gap": 2.335001803747218
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-256.6209961998795,
					-462.1428571428569
				]
			]
		},
		{
			"type": "text",
			"version": 105,
			"versionNonce": 1220210614,
			"isDeleted": false,
			"id": "YZKoLz53",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1975.5606677566275,
			"y": -1753.342011669114,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 1098953024,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "fySl68hHDWJ8OZO-b1I4Y",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 134,
			"versionNonce": 1752534698,
			"isDeleted": false,
			"id": "YpjL4dvCKOCN09IvqBh0l",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2658.315989377181,
			"y": -1504.7705830976854,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 248.73575883177818,
			"height": 460.714285714286,
			"seed": 1219451200,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "niYpIEyd"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "Rd4ZgU2s-6gNdiQ-SxhPO",
				"focus": 0.1970340115349124,
				"gap": 11.620716089460984
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					248.73575883177818,
					-460.714285714286
				]
			]
		},
		{
			"type": "text",
			"version": 104,
			"versionNonce": 779061494,
			"isDeleted": false,
			"id": "niYpIEyd",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2754.963882831156,
			"y": -1747.6277259548283,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 20752704,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "YpjL4dvCKOCN09IvqBh0l",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 102,
			"versionNonce": 1491216746,
			"isDeleted": false,
			"id": "fikG50Wv",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2792.1493227105143,
			"y": -1414.270583097687,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 33.199981689453125,
			"height": 25,
			"seed": 7903,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "/ap",
			"rawText": "/ap",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "/ap",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 288,
			"versionNonce": 1019148854,
			"isDeleted": false,
			"id": "MuLUJ1D_df0Q3Ch96Rz_J",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2953.5778941390863,
			"y": -675.2229640500677,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 717.1428571428571,
			"height": 488.57142857142844,
			"seed": 1396937408,
			"groupIds": [
				"LM8QeR6aQvIbvVUXQ_jz5",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "HTOv6us5KuCkrzkoY8GQ7",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 317,
			"versionNonce": 778923050,
			"isDeleted": false,
			"id": "ju8yFEld",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3199.25214878357,
			"y": -588.5562973834012,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 307.58551025390625,
			"height": 284.28571428571394,
			"seed": 851655360,
			"groupIds": [
				"LM8QeR6aQvIbvVUXQ_jz5",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 113.71428571428558,
			"fontFamily": 1,
			"text": "Web\nClient",
			"rawText": "Web\nClient",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Web\nClient",
			"lineHeight": 1.25,
			"baseline": 242
		},
		{
			"type": "arrow",
			"version": 188,
			"versionNonce": 1250837366,
			"isDeleted": false,
			"id": "HTOv6us5KuCkrzkoY8GQ7",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3205.4826560438473,
			"y": -690.9372497643526,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 683.333333333333,
			"height": 566.6666666666667,
			"seed": 722787008,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "MuLUJ1D_df0Q3Ch96Rz_J",
				"focus": 0.31671491369143046,
				"gap": 15.71428571428487
			},
			"endBinding": {
				"elementId": "AXBtSNbG-w1-X5jpa0Arg",
				"focus": 0.006903700345520345,
				"gap": 15.21595418470315
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-683.333333333333,
					-566.6666666666667
				]
			]
		},
		{
			"type": "line",
			"version": 6538,
			"versionNonce": 520247018,
			"isDeleted": false,
			"id": "M763H2Cnq3X7_6ttLFCRJ",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2217.588181997384,
			"y": -2931.4834105454934,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 228.74316370113166,
			"height": 295.22936747926303,
			"seed": 890346176,
			"groupIds": [
				"jgmihDvr9DEKwU-cX50xq",
				"24zu4Wlgeujyw-t2aDsQB",
				"q9kb2XEpu3rSl6qut2RBI",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0.7542774840697635,
					223.13275577547907
				],
				[
					0.03529841555978175,
					248.53545107516138
				],
				[
					11.780778829655814,
					259.5116415929002
				],
				[
					52.68382831026584,
					268.80105286328154
				],
				[
					121.82156843531305,
					271.6936367642977
				],
				[
					187.87810717162128,
					267.075202850611
				],
				[
					222.97443256588514,
					256.03030167663184
				],
				[
					227.92429435085822,
					246.71933412193783
				],
				[
					228.61948451989593,
					226.2678093816333
				],
				[
					228.07384107326772,
					18.71959277598987
				],
				[
					226.84378559975644,
					-0.8898896084065069
				],
				[
					212.15616686193164,
					-11.849758308413197
				],
				[
					181.2271762663937,
					-18.197134324732623
				],
				[
					110.74418559248709,
					-23.535730714965336
				],
				[
					54.234702841642864,
					-20.3523136666016
				],
				[
					9.79037843432165,
					-9.554551463948288
				],
				[
					-0.12367918123571855,
					-0.13407238974302393
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 7259,
			"versionNonce": 170026166,
			"isDeleted": false,
			"id": "l87NvlquQcH5JyJbHzw7M",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2218.39913088106,
			"y": -2958.1751738105445,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 227.2759675879657,
			"height": 45.964854577354636,
			"seed": 1032864448,
			"groupIds": [
				"jgmihDvr9DEKwU-cX50xq",
				"24zu4Wlgeujyw-t2aDsQB",
				"q9kb2XEpu3rSl6qut2RBI",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "nT7KLKs_v7_Ac-JL7Vcjz",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 137,
			"versionNonce": 1798039978,
			"isDeleted": false,
			"id": "99s6JRhW3owpnahEi9w2O",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1910.7827077343704,
			"y": -2462.375258429911,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 290,
			"height": 210,
			"seed": 750295360,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					290,
					-210
				]
			]
		},
		{
			"type": "arrow",
			"version": 123,
			"versionNonce": 488660470,
			"isDeleted": false,
			"id": "AsEiIMvcKm-YWcqKPHpcb",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2774.116041067704,
			"y": -2455.7085917632444,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 300,
			"height": 216.66666666666652,
			"seed": 2047349440,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Rd4ZgU2s-6gNdiQ-SxhPO",
				"focus": -0.06213322735728527,
				"gap": 9.16315177267893
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-300,
					-216.66666666666652
				]
			]
		},
		{
			"type": "arrow",
			"version": 274,
			"versionNonce": 169157738,
			"isDeleted": false,
			"id": "nT7KLKs_v7_Ac-JL7Vcjz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2228.3498482239384,
			"y": -2912.1710527795103,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 420.9004738229014,
			"height": 1.0083385385455585,
			"seed": 488239808,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "l87NvlquQcH5JyJbHzw7M",
				"focus": -0.9908307525331731,
				"gap": 12.632893044017074
			},
			"endBinding": {
				"elementId": "psebmuHaa6VKQsxeTsLSY",
				"focus": -0.062408663813663556,
				"gap": 17.58496852807093
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-420.9004738229014,
					1.0083385385455585
				]
			]
		},
		{
			"type": "arrow",
			"version": 146,
			"versionNonce": 680341302,
			"isDeleted": false,
			"id": "l7HeP984GxVemLP6uNzPE",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2210.7827077343704,
			"y": -2742.375258429911,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 366.6666666666665,
			"height": 260,
			"seed": 760025792,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "4D-GyM5RJ2IzfNcn68WgV",
				"focus": -0.11962261510058154,
				"gap": 19.555387814192727
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-366.6666666666665,
					260
				]
			]
		},
		{
			"type": "arrow",
			"version": 146,
			"versionNonce": 1435043626,
			"isDeleted": false,
			"id": "AOiXjcqLm3sUg3F-r7A0b",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2447.449374401037,
			"y": -2739.041925096578,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 366.66666666666697,
			"height": 260,
			"seed": 1103683904,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "Rd4ZgU2s-6gNdiQ-SxhPO",
				"focus": 0.05066140742518356,
				"gap": 13.364911623717035
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					366.66666666666697,
					260
				]
			]
		},
		{
			"type": "line",
			"version": 6701,
			"versionNonce": 1758320758,
			"isDeleted": false,
			"id": "t1t4GrluhGZ7b2QZMP-1X",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2595.5695030379366,
			"y": -4107.628500476084,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 228.74316370113166,
			"height": 295.22936747926303,
			"seed": 2005160640,
			"groupIds": [
				"vt6DhhXilQyerhZ91S1JM",
				"keydiYobee_PDUzB6IKo1",
				"y6Rvx6_k2tS64OUGc5Rs6",
				"9Mo3OfSwL0T3uaXHAR9px",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0.7542774840697635,
					223.13275577547907
				],
				[
					0.03529841555978175,
					248.53545107516138
				],
				[
					11.780778829655814,
					259.5116415929002
				],
				[
					52.68382831026584,
					268.80105286328154
				],
				[
					121.82156843531305,
					271.6936367642977
				],
				[
					187.87810717162128,
					267.075202850611
				],
				[
					222.97443256588514,
					256.03030167663184
				],
				[
					227.92429435085822,
					246.71933412193783
				],
				[
					228.61948451989593,
					226.2678093816333
				],
				[
					228.07384107326772,
					18.71959277598987
				],
				[
					226.84378559975644,
					-0.8898896084065069
				],
				[
					212.15616686193164,
					-11.849758308413197
				],
				[
					181.2271762663937,
					-18.197134324732623
				],
				[
					110.74418559248709,
					-23.535730714965336
				],
				[
					54.234702841642864,
					-20.3523136666016
				],
				[
					9.79037843432165,
					-9.554551463948288
				],
				[
					-0.12367918123571855,
					-0.13407238974302393
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 7421,
			"versionNonce": 905089514,
			"isDeleted": false,
			"id": "NNf6mCgPqpwon8NrK7n83",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2596.3804519216137,
			"y": -4134.320263741135,
			"strokeColor": "#000000",
			"backgroundColor": "#fff",
			"width": 227.2759675879657,
			"height": 45.964854577354636,
			"seed": 283900608,
			"groupIds": [
				"vt6DhhXilQyerhZ91S1JM",
				"keydiYobee_PDUzB6IKo1",
				"y6Rvx6_k2tS64OUGc5Rs6",
				"9Mo3OfSwL0T3uaXHAR9px",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 316,
			"versionNonce": 1168595382,
			"isDeleted": false,
			"id": "IBmC7OgD_F24ifaW4afFy",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2722.449374401037,
			"y": -3266.708591763245,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 3.3333333333339397,
			"height": 554.9999999999995,
			"seed": 1160889024,
			"groupIds": [
				"9Mo3OfSwL0T3uaXHAR9px",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-3.3333333333339397,
					-554.9999999999995
				]
			]
		},
		{
			"type": "line",
			"version": 6798,
			"versionNonce": 1314702506,
			"isDeleted": false,
			"id": "fOtIQmSJhWkaFRKEKD5wM",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1865.588181997382,
			"y": -4115.328591648514,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 228.74316370113166,
			"height": 295.22936747926303,
			"seed": 470503744,
			"groupIds": [
				"vW6keSQYK9NEXfFNDZyw7",
				"b9MTeQeATL2SAuThGuzuM",
				"xpM15o5vJ8QcsP2qVmgm9",
				"3-Werib1GI4ab6IKe2f5J",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0.7542774840697635,
					223.13275577547907
				],
				[
					0.03529841555978175,
					248.53545107516138
				],
				[
					11.780778829655814,
					259.5116415929002
				],
				[
					52.68382831026584,
					268.80105286328154
				],
				[
					121.82156843531305,
					271.6936367642977
				],
				[
					187.87810717162128,
					267.075202850611
				],
				[
					222.97443256588514,
					256.03030167663184
				],
				[
					227.92429435085822,
					246.71933412193783
				],
				[
					228.61948451989593,
					226.2678093816333
				],
				[
					228.07384107326772,
					18.71959277598987
				],
				[
					226.84378559975644,
					-0.8898896084065069
				],
				[
					212.15616686193164,
					-11.849758308413197
				],
				[
					181.2271762663937,
					-18.197134324732623
				],
				[
					110.74418559248709,
					-23.535730714965336
				],
				[
					54.234702841642864,
					-20.3523136666016
				],
				[
					9.79037843432165,
					-9.554551463948288
				],
				[
					-0.12367918123571855,
					-0.13407238974302393
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 7518,
			"versionNonce": 1715385078,
			"isDeleted": false,
			"id": "ogdCnz3orfErXsOaCCfF-",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1866.3991308810591,
			"y": -4142.020354913565,
			"strokeColor": "#000000",
			"backgroundColor": "#fff",
			"width": 227.2759675879657,
			"height": 45.964854577354636,
			"seed": 957294912,
			"groupIds": [
				"vW6keSQYK9NEXfFNDZyw7",
				"b9MTeQeATL2SAuThGuzuM",
				"xpM15o5vJ8QcsP2qVmgm9",
				"3-Werib1GI4ab6IKe2f5J",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 442,
			"versionNonce": 678600554,
			"isDeleted": false,
			"id": "cWE4D2aqt2oiHiKtcmm7C",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1944.1347200271487,
			"y": -3812.7420162690078,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 5.000000000000455,
			"height": 538.333333333333,
			"seed": 936902976,
			"groupIds": [
				"3-Werib1GI4ab6IKe2f5J",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-5.000000000000455,
					538.333333333333
				]
			]
		},
		{
			"type": "text",
			"version": 228,
			"versionNonce": 1159259190,
			"isDeleted": false,
			"id": "JNWW3sOn",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1879.1727223828068,
			"y": -4309.184782239435,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 172.95907592773438,
			"height": 87.85714285714313,
			"seed": 1753307840,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 70.2857142857145,
			"fontFamily": 1,
			"text": "Read",
			"rawText": "Read",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Read",
			"lineHeight": 1.25,
			"baseline": 61
		},
		{
			"type": "text",
			"version": 266,
			"versionNonce": 1618944554,
			"isDeleted": false,
			"id": "9EnJztNz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2621.4010232948476,
			"y": -4301.684782239434,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 176.1919403076172,
			"height": 87.85714285714313,
			"seed": 695271744,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 70.2857142857145,
			"fontFamily": 1,
			"text": "Write",
			"rawText": "Write",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Write",
			"lineHeight": 1.25,
			"baseline": 61
		},
		{
			"type": "line",
			"version": 156,
			"versionNonce": 1142615414,
			"isDeleted": false,
			"id": "LaKu8iIbUENBj8UcLQ8WQ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 926.5446124962741,
			"y": -3196.518115572766,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 3246.6666666666665,
			"height": 6.666666666666515,
			"seed": 645480768,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					3246.6666666666665,
					6.666666666666515
				]
			]
		},
		{
			"type": "rectangle",
			"version": 227,
			"versionNonce": 1366117610,
			"isDeleted": false,
			"id": "woeBlcrTehffcRIRGYkaL",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 251.54461249627275,
			"y": -4397.851448906101,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4895,
			"height": 4490,
			"seed": 1323344576,
			"groupIds": [
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 328,
			"versionNonce": 1082773174,
			"isDeleted": false,
			"id": "OZ1XGkzU",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2207.7438312462727,
			"y": -4708.351448906102,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 746.0096435546875,
			"height": 180.99999999999997,
			"seed": 333838656,
			"groupIds": [
				"RxdctKS8ua7XkIglTrYAN",
				"45gfStpZVy34Jb1y-FQ0b"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 144.79999999999998,
			"fontFamily": 1,
			"text": "Phase One",
			"rawText": "Phase One",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Phase One",
			"lineHeight": 1.25,
			"baseline": 127
		},
		{
			"type": "rectangle",
			"version": 364,
			"versionNonce": 1086857130,
			"isDeleted": false,
			"id": "-Ag0nuTQiyAzaRm1tUGZS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7114.017288078476,
			"y": -692.4270134728595,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 717.1428571428571,
			"height": 488.57142857142844,
			"seed": 1731864896,
			"groupIds": [
				"zq872MHSaY9NHG_KY9nW4"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "zPv524Ppj4rNYHpHyNfRa",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 420,
			"versionNonce": 655001590,
			"isDeleted": false,
			"id": "fCX8xLE5",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7307.69154272296,
			"y": -529.7603468061934,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 307.58551025390625,
			"height": 142.14285714285697,
			"seed": 1755513152,
			"groupIds": [
				"zq872MHSaY9NHG_KY9nW4"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 113.71428571428558,
			"fontFamily": 1,
			"text": "Client",
			"rawText": "Client",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Client",
			"lineHeight": 1.25,
			"baseline": 100
		},
		{
			"type": "rectangle",
			"version": 511,
			"versionNonce": 180001386,
			"isDeleted": false,
			"id": "Dvh1NOeila-3gOFiK7o9T",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6360.866076716738,
			"y": -2460.236537282384,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 464.67502088554716,
			"height": 316.57142857142844,
			"seed": 1999690048,
			"groupIds": [
				"T2pGbxfcq_xTs9I5-kQ4J"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "L1-DTTYkV9h6Z-l1Z9PcZ",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 545,
			"versionNonce": 128063798,
			"isDeleted": false,
			"id": "sStVpLUd",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6470.0924760484,
			"y": -2426.913229011707,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 248.74362182617188,
			"height": 276.3057644110272,
			"seed": 641970496,
			"groupIds": [
				"T2pGbxfcq_xTs9I5-kQ4J"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "L1-DTTYkV9h6Z-l1Z9PcZ",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 73.68153717627392,
			"fontFamily": 1,
			"text": "User\nService\n(TS)",
			"rawText": "User\nService\n(TS)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "User\nService\n(TS)",
			"lineHeight": 1.25,
			"baseline": 248
		},
		{
			"type": "rectangle",
			"version": 627,
			"versionNonce": 1309654314,
			"isDeleted": false,
			"id": "NzLvB5xSiTcIbKhMZFkCs",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7194.112526173716,
			"y": -2460.42701347286,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 464.67502088554716,
			"height": 316.57142857142844,
			"seed": 490441024,
			"groupIds": [
				"1qgbktDUgJRlELXbMqhka"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "ba-6x-m87IxI2xygN6Mx0",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 738,
			"versionNonce": 699761270,
			"isDeleted": false,
			"id": "A7jEAjoO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7265.803818221177,
			"y": -2427.103705202184,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 328.43963623046875,
			"height": 264.73517126148664,
			"seed": 393765184,
			"groupIds": [
				"1qgbktDUgJRlELXbMqhka"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "ba-6x-m87IxI2xygN6Mx0",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 52.94703425229733,
			"fontFamily": 1,
			"text": "Messaging/\nNotifications\nService\n(Go)",
			"rawText": "Messaging/\nNotifications\nService\n(Go)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Messaging/\nNotifications\nService\n(Go)",
			"lineHeight": 1.25,
			"baseline": 245
		},
		{
			"type": "rectangle",
			"version": 1240,
			"versionNonce": 405964778,
			"isDeleted": false,
			"id": "-fElFNBd0bBUk_l-fw9p_",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5570.113988078452,
			"y": -3146.641299187148,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 521.4313561681979,
			"height": 355.23809523809496,
			"seed": 1683634496,
			"groupIds": [
				"C_jlvmbX7UrJYr034r7lR"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1356,
			"versionNonce": 537510838,
			"isDeleted": false,
			"id": "hXyaOGMK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5698.146052462672,
			"y": -3028.22860077445,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 281.72216796875,
			"height": 148.53522695627933,
			"seed": 1732317504,
			"groupIds": [
				"C_jlvmbX7UrJYr034r7lR"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 59.41409078251173,
			"fontFamily": 1,
			"text": "Monitoring\n(Go)",
			"rawText": "Monitoring\n(Go)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Monitoring\n(Go)",
			"lineHeight": 1.25,
			"baseline": 126
		},
		{
			"type": "rectangle",
			"version": 395,
			"versionNonce": 288225962,
			"isDeleted": false,
			"id": "rYw-pEcXZ50B1kEL_0pLg",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6257.826811888,
			"y": -1297.1889182347686,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2828.5714285714284,
			"height": 234.28571428571422,
			"seed": 395110720,
			"groupIds": [
				"P-Dx_Ke18AtqZn2GLp1aY"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "zPv524Ppj4rNYHpHyNfRa",
					"type": "arrow"
				},
				{
					"id": "ba-6x-m87IxI2xygN6Mx0",
					"type": "arrow"
				},
				{
					"id": "4CYm3wtvtActVUgYKy6p3",
					"type": "arrow"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 411,
			"versionNonce": 1556339958,
			"isDeleted": false,
			"id": "S3VdX8xA",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7182.988804714916,
			"y": -1231.950822996674,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1002.0521850585938,
			"height": 87.85714285714285,
			"seed": 10338624,
			"groupIds": [
				"P-Dx_Ke18AtqZn2GLp1aY"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 70.28571428571428,
			"fontFamily": 1,
			"text": "Orchestrator Service (Proxy)",
			"rawText": "Orchestrator Service (Proxy)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Orchestrator Service (Proxy)",
			"lineHeight": 1.25,
			"baseline": 61
		},
		{
			"type": "text",
			"version": 462,
			"versionNonce": 665654634,
			"isDeleted": false,
			"id": "tsuvsC3o",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7444.636500032261,
			"y": -1136.9592555363542,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 505.28704833984375,
			"height": 53.571428571428555,
			"seed": 1104386368,
			"groupIds": [
				"P-Dx_Ke18AtqZn2GLp1aY"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 42.85714285714285,
			"fontFamily": 1,
			"text": "(Go) (Service Discovery)",
			"rawText": "(Go) (Service Discovery)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "(Go) (Service Discovery)",
			"lineHeight": 1.25,
			"baseline": 37
		},
		{
			"type": "arrow",
			"version": 618,
			"versionNonce": 1164496438,
			"isDeleted": false,
			"id": "zPv524Ppj4rNYHpHyNfRa",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7418.066986370248,
			"y": -699.0205830976838,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 2.9316292016583247,
			"height": 354.3333333333337,
			"seed": 274794816,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "-Ag0nuTQiyAzaRm1tUGZS",
				"focus": -0.14686148872026336,
				"gap": 6.59356962482434
			},
			"endBinding": {
				"elementId": "rYw-pEcXZ50B1kEL_0pLg",
				"focus": 0.18231724392066062,
				"gap": 9.549287518036863
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-2.9316292016583247,
					-354.3333333333337
				]
			]
		},
		{
			"type": "arrow",
			"version": 845,
			"versionNonce": 1023072298,
			"isDeleted": false,
			"id": "L1-DTTYkV9h6Z-l1Z9PcZ",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6611.388625997501,
			"y": -1296.5205830976847,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.6227424118660565,
			"height": 840.8095238095239,
			"seed": 1515622720,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "iYKQPdE7"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "sStVpLUd",
				"focus": -0.14187074224795038,
				"gap": 13.277357693471231
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					0.6227424118660565,
					-840.8095238095239
				]
			]
		},
		{
			"type": "text",
			"version": 228,
			"versionNonce": 1188927350,
			"isDeleted": false,
			"id": "iYKQPdE7",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6866.394001089959,
			"y": -1764.0920116691132,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 200436032,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "L1-DTTYkV9h6Z-l1Z9PcZ",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 1029,
			"versionNonce": 1359102698,
			"isDeleted": false,
			"id": "ba-6x-m87IxI2xygN6Mx0",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7443.478707358396,
			"y": -1315.2651574847107,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.73298657257692,
			"height": 808.8873490101503,
			"seed": 1280524608,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Gm6trphb"
				}
			],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "rYw-pEcXZ50B1kEL_0pLg",
				"focus": -0.15994670973046546,
				"gap": 18.07623924994209
			},
			"endBinding": {
				"elementId": "NzLvB5xSiTcIbKhMZFkCs",
				"focus": -0.006361640532411737,
				"gap": 19.703078406570512
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-12.73298657257692,
					-808.8873490101503
				]
			]
		},
		{
			"type": "text",
			"version": 230,
			"versionNonce": 1768372406,
			"isDeleted": false,
			"id": "Gm6trphb",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7411.892228110193,
			"y": -1912.2088319897857,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 2061048128,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "ba-6x-m87IxI2xygN6Mx0",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "line",
			"version": 7618,
			"versionNonce": 776885674,
			"isDeleted": false,
			"id": "3CZD06Gm8wL5gDLOeExXR",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5879.894764166894,
			"y": -2694.2415444980575,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 210.53217062632953,
			"height": 271.72518978209814,
			"seed": 1505841472,
			"groupIds": [
				"zMHxPFYfVxQM7UExR8qdk",
				"5IXExAYy-B3nj_O2xIMid",
				"WuMIEDXyvcRFMc45nmBUX"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0.6942269810662254,
					205.36842566637048
				],
				[
					0.032488192990024166,
					228.74872912404672
				],
				[
					10.842872410022009,
					238.85106913507747
				],
				[
					48.489496042631956,
					247.4009199238396
				],
				[
					112.12295404508966,
					250.06321573870113
				],
				[
					172.92051520144253,
					245.81247048795726
				],
				[
					205.22270708647062,
					235.64689010126074
				],
				[
					209.77849414925814,
					227.07719919464088
				],
				[
					210.41833795012826,
					208.25388737833634
				],
				[
					209.91613496688734,
					17.229264632884885
				],
				[
					208.78400824170365,
					-0.8190425796524444
				],
				[
					195.26571897712742,
					-10.906360206363058
				],
				[
					166.79908670711254,
					-16.748400811533816
				],
				[
					101.92747796167711,
					-21.66197404339701
				],
				[
					49.916900368850435,
					-18.731999261389724
				],
				[
					9.010934314627322,
					-8.793882302398424
				],
				[
					-0.11383267620126132,
					-0.12339844731070501
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 8339,
			"versionNonce": 1688908278,
			"isDeleted": false,
			"id": "-8ocyteFmueicCa6LUCdo",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5880.641150751676,
			"y": -2718.808288994857,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 209.18178280515323,
			"height": 42.30544183317237,
			"seed": 1342515520,
			"groupIds": [
				"zMHxPFYfVxQM7UExR8qdk",
				"5IXExAYy-B3nj_O2xIMid",
				"WuMIEDXyvcRFMc45nmBUX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 6871,
			"versionNonce": 369758314,
			"isDeleted": false,
			"id": "rTjxuNPoybIUE9cpGnftE",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6713.069503037937,
			"y": -4311.711833809416,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 228.74316370113166,
			"height": 295.22936747926303,
			"seed": 2028288320,
			"groupIds": [
				"LmbIejowfFZDRmhd4HAlL",
				"lQ3WvrBe0s2OrktEGp5Nq",
				"tge_03dj_mX3XiPcbsmDf",
				"xGzUskwbFcGUlYkhSYIBS"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0.7542774840697635,
					223.13275577547907
				],
				[
					0.03529841555978175,
					248.53545107516138
				],
				[
					11.780778829655814,
					259.5116415929002
				],
				[
					52.68382831026584,
					268.80105286328154
				],
				[
					121.82156843531305,
					271.6936367642977
				],
				[
					187.87810717162128,
					267.075202850611
				],
				[
					222.97443256588514,
					256.03030167663184
				],
				[
					227.92429435085822,
					246.71933412193783
				],
				[
					228.61948451989593,
					226.2678093816333
				],
				[
					228.07384107326772,
					18.71959277598987
				],
				[
					226.84378559975644,
					-0.8898896084065069
				],
				[
					212.15616686193164,
					-11.849758308413197
				],
				[
					181.2271762663937,
					-18.197134324732623
				],
				[
					110.74418559248709,
					-23.535730714965336
				],
				[
					54.234702841642864,
					-20.3523136666016
				],
				[
					9.79037843432165,
					-9.554551463948288
				],
				[
					-0.12367918123571855,
					-0.13407238974302393
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 7591,
			"versionNonce": 866976566,
			"isDeleted": false,
			"id": "nMEDZV6p2s0O0mxUa5Mh-",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6713.880451921611,
			"y": -4338.403597074467,
			"strokeColor": "#000000",
			"backgroundColor": "#fff",
			"width": 227.2759675879657,
			"height": 45.964854577354636,
			"seed": 845943104,
			"groupIds": [
				"LmbIejowfFZDRmhd4HAlL",
				"lQ3WvrBe0s2OrktEGp5Nq",
				"tge_03dj_mX3XiPcbsmDf",
				"xGzUskwbFcGUlYkhSYIBS"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 486,
			"versionNonce": 1811968810,
			"isDeleted": false,
			"id": "kvxQCxPh01Q39KCyMXVl6",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6839.949374401038,
			"y": -3470.791925096578,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 3.3333333333339397,
			"height": 554.9999999999995,
			"seed": 1163389248,
			"groupIds": [
				"xGzUskwbFcGUlYkhSYIBS"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-3.3333333333339397,
					-554.9999999999995
				]
			]
		},
		{
			"type": "line",
			"version": 6968,
			"versionNonce": 684928118,
			"isDeleted": false,
			"id": "jQABp-0ResxLooEK5gtoc",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5983.088181997382,
			"y": -4319.411924981848,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 228.74316370113166,
			"height": 295.22936747926303,
			"seed": 1023983936,
			"groupIds": [
				"a-eohwMhaNZXByAm23ITf",
				"2002Pi_-STM2pJqRPZ7BM",
				"tAehYaBYuPu2dY1hpkrFp",
				"ps4PtOydgptg1YyAKSMZB"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864759,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0.7542774840697635,
					223.13275577547907
				],
				[
					0.03529841555978175,
					248.53545107516138
				],
				[
					11.780778829655814,
					259.5116415929002
				],
				[
					52.68382831026584,
					268.80105286328154
				],
				[
					121.82156843531305,
					271.6936367642977
				],
				[
					187.87810717162128,
					267.075202850611
				],
				[
					222.97443256588514,
					256.03030167663184
				],
				[
					227.92429435085822,
					246.71933412193783
				],
				[
					228.61948451989593,
					226.2678093816333
				],
				[
					228.07384107326772,
					18.71959277598987
				],
				[
					226.84378559975644,
					-0.8898896084065069
				],
				[
					212.15616686193164,
					-11.849758308413197
				],
				[
					181.2271762663937,
					-18.197134324732623
				],
				[
					110.74418559248709,
					-23.535730714965336
				],
				[
					54.234702841642864,
					-20.3523136666016
				],
				[
					9.79037843432165,
					-9.554551463948288
				],
				[
					-0.12367918123571855,
					-0.13407238974302393
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 7688,
			"versionNonce": 1654423018,
			"isDeleted": false,
			"id": "xiaC9vTW_Sa0W01k27jHm",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5983.899130881059,
			"y": -4346.103688246899,
			"strokeColor": "#000000",
			"backgroundColor": "#fff",
			"width": 227.2759675879657,
			"height": 45.964854577354636,
			"seed": 954112320,
			"groupIds": [
				"a-eohwMhaNZXByAm23ITf",
				"2002Pi_-STM2pJqRPZ7BM",
				"tAehYaBYuPu2dY1hpkrFp",
				"ps4PtOydgptg1YyAKSMZB"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 612,
			"versionNonce": 31600054,
			"isDeleted": false,
			"id": "LTisqvPUIO418ddFgN-Yo",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6061.634720027148,
			"y": -4016.825349602341,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 5.000000000000455,
			"height": 538.333333333333,
			"seed": 1815703872,
			"groupIds": [
				"ps4PtOydgptg1YyAKSMZB"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-5.000000000000455,
					538.333333333333
				]
			]
		},
		{
			"type": "text",
			"version": 398,
			"versionNonce": 652816554,
			"isDeleted": false,
			"id": "hXM483kS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5996.672722382807,
			"y": -4513.268115572767,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 172.95907592773438,
			"height": 87.85714285714313,
			"seed": 511265088,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 70.2857142857145,
			"fontFamily": 1,
			"text": "Read",
			"rawText": "Read",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Read",
			"lineHeight": 1.25,
			"baseline": 61
		},
		{
			"type": "text",
			"version": 436,
			"versionNonce": 2080311030,
			"isDeleted": false,
			"id": "PDDQru9T",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6738.901023294847,
			"y": -4505.768115572767,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 176.1919403076172,
			"height": 87.85714285714313,
			"seed": 721297728,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 70.2857142857145,
			"fontFamily": 1,
			"text": "Write",
			"rawText": "Write",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Write",
			"lineHeight": 1.25,
			"baseline": 61
		},
		{
			"type": "text",
			"version": 413,
			"versionNonce": 210865002,
			"isDeleted": false,
			"id": "6ZmWHhFa",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6965.243831246271,
			"y": -4979.1014489061,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 778.8792114257812,
			"height": 180.99999999999997,
			"seed": 736799040,
			"groupIds": [
				"7PZSu_Fsn837DplJLxKA5"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 144.79999999999998,
			"fontFamily": 1,
			"text": "Phase Two",
			"rawText": "Phase Two",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Phase Two",
			"lineHeight": 1.25,
			"baseline": 127
		},
		{
			"type": "rectangle",
			"version": 995,
			"versionNonce": 1739503670,
			"isDeleted": false,
			"id": "aHs1inHy2prr8v8UsNBAY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 8213.322390274046,
			"y": -3298.7244647791163,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 499.90309106098573,
			"height": 340.57142857142844,
			"seed": 67177152,
			"groupIds": [
				"Bp4eMlmVZRuJyG_YJrO7c",
				"kPOoOE8xMh1YUx4-X1ZYz"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1075,
			"versionNonce": 971017770,
			"isDeleted": false,
			"id": "8NRT1919",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 8308.334538949312,
			"y": -3234.5276350114755,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 306.89471435546875,
			"height": 198.16875522138656,
			"seed": 1561440960,
			"groupIds": [
				"Bp4eMlmVZRuJyG_YJrO7c",
				"kPOoOE8xMh1YUx4-X1ZYz"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 79.26750208855462,
			"fontFamily": 1,
			"text": "Storage\nService",
			"rawText": "Storage\nService",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Storage\nService",
			"lineHeight": 1.25,
			"baseline": 168
		},
		{
			"type": "rectangle",
			"version": 722,
			"versionNonce": 1020674422,
			"isDeleted": false,
			"id": "YM_WCHyk01iQb9mhSiwus",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 8111.275606648318,
			"y": -2491.7104448287723,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 499.90309106098573,
			"height": 340.57142857142844,
			"seed": 1697020608,
			"groupIds": [
				"WbALNAmzTgU2GuYEgqXiU",
				"fG46eGTh3c174br_Zg1hD"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "4CYm3wtvtActVUgYKy6p3",
					"type": "arrow"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 850,
			"versionNonce": 1405171946,
			"isDeleted": false,
			"id": "gmBZ1VcK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 8175.970815015966,
			"y": -2427.513615061131,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 367.5285949707031,
			"height": 198.16875522138656,
			"seed": 1476993728,
			"groupIds": [
				"WbALNAmzTgU2GuYEgqXiU",
				"fG46eGTh3c174br_Zg1hD"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 79.26750208855462,
			"fontFamily": 1,
			"text": "Streaming\nService",
			"rawText": "Streaming\nService",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Streaming\nService",
			"lineHeight": 1.25,
			"baseline": 168
		},
		{
			"type": "arrow",
			"version": 617,
			"versionNonce": 783983286,
			"isDeleted": false,
			"id": "4CYm3wtvtActVUgYKy6p3",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 8389.494992905678,
			"y": -1312.7580638763925,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.110697116986557,
			"height": 833.9999999999995,
			"seed": 676776640,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "rYw-pEcXZ50B1kEL_0pLg",
				"focus": 0.5086156252044403,
				"gap": 15.56914564162389
			},
			"endBinding": {
				"elementId": "YM_WCHyk01iQb9mhSiwus",
				"focus": -0.005998622491307383,
				"gap": 4.38095238095184
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-22.110697116986557,
					-833.9999999999995
				]
			]
		},
		{
			"type": "line",
			"version": 3884,
			"versionNonce": 700353450,
			"isDeleted": false,
			"id": "UJd8QZp0vNJgEZ91nV-bj",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 4.70956944444772,
			"x": 7321.785337402246,
			"y": -3035.7724095547223,
			"strokeColor": "#000000",
			"backgroundColor": "#eeeeee",
			"width": 143.6326540899409,
			"height": 626.0211058167058,
			"seed": 1507521216,
			"groupIds": [
				"DBNS45yWkeaHco19fttg9",
				"WTUcVbgQJICGPk9yZP7iH"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					143.6326540899409,
					-0.5525118606261938
				],
				[
					142.4012855946406,
					562.9593576271251
				],
				[
					69.06948273086485,
					625.4685939560796
				],
				[
					2.252108169035731,
					559.510344194126
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1802,
			"versionNonce": 1073798134,
			"isDeleted": false,
			"id": "yOdiDFfEtRzikO0tDL1YR",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7102.013290854368,
			"y": -2752.1883518830377,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 116.85263750810405,
			"height": 77.66851954131499,
			"seed": 795777728,
			"groupIds": [
				"x8F9d6fosnnLK-QIgyacQ",
				"DBNS45yWkeaHco19fttg9",
				"WTUcVbgQJICGPk9yZP7iH"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3126,
			"versionNonce": 1644398186,
			"isDeleted": false,
			"id": "irvAerWYCB0o7mimgQpcg",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7163.530049966889,
			"y": -2714.1226893129656,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 113.74946674999639,
			"height": 36.69107437521974,
			"seed": 1682784960,
			"groupIds": [
				"x8F9d6fosnnLK-QIgyacQ",
				"DBNS45yWkeaHco19fttg9",
				"WTUcVbgQJICGPk9yZP7iH"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					55.42550537257782,
					-36.69107437521974
				],
				[
					-58.32396137741856,
					-36.24181185891322
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 2068,
			"versionNonce": 1454239030,
			"isDeleted": false,
			"id": "iWh7qUNtTM4PEIrwh5Wsn",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dotted",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7349.580853471262,
			"y": -2707.4559335612057,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 146.8274469510042,
			"height": 2.720043617241219,
			"seed": 1461119680,
			"groupIds": [
				"DBNS45yWkeaHco19fttg9",
				"WTUcVbgQJICGPk9yZP7iH"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					146.8274469510042,
					-2.720043617241219
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1878,
			"versionNonce": 626731306,
			"isDeleted": false,
			"id": "oHwMmLBCg6R2-zoemrpT5",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7241.694037222419,
			"y": -2751.5157319165833,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 116.85263750810405,
			"height": 77.66851954131499,
			"seed": 309039808,
			"groupIds": [
				"rtrpMZsTzzZ7zwiXasaJZ",
				"DBNS45yWkeaHco19fttg9",
				"WTUcVbgQJICGPk9yZP7iH"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3199,
			"versionNonce": 1344722550,
			"isDeleted": false,
			"id": "QKYL91fWTv3iQoY9g6gzX",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7303.304304444706,
			"y": -2716.1676670197103,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 113.74946674999639,
			"height": 36.69107437521974,
			"seed": 1290484416,
			"groupIds": [
				"rtrpMZsTzzZ7zwiXasaJZ",
				"DBNS45yWkeaHco19fttg9",
				"WTUcVbgQJICGPk9yZP7iH"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					55.42550537257782,
					-36.69107437521974
				],
				[
					-58.32396137741856,
					-36.24181185891322
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1927,
			"versionNonce": 1261466602,
			"isDeleted": false,
			"id": "bdYIctzfEF_e66LzuvH54",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7492.35707805621,
			"y": -2754.206211782421,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 116.85263750810405,
			"height": 77.66851954131499,
			"seed": 1765139136,
			"groupIds": [
				"vFQWJuFwVplRozqoRuMVz",
				"DBNS45yWkeaHco19fttg9",
				"WTUcVbgQJICGPk9yZP7iH"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3284,
			"versionNonce": 355506102,
			"isDeleted": false,
			"id": "bDl2lW7GT-63w9Ik-tqPg",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7556.326530793149,
			"y": -2720.5316630012076,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 113.74946674999639,
			"height": 36.69107437521974,
			"seed": 1978370752,
			"groupIds": [
				"vFQWJuFwVplRozqoRuMVz",
				"DBNS45yWkeaHco19fttg9",
				"WTUcVbgQJICGPk9yZP7iH"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					55.42550537257782,
					-36.69107437521974
				],
				[
					-58.32396137741856,
					-36.24181185891322
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "text",
			"version": 1169,
			"versionNonce": 93218474,
			"isDeleted": false,
			"id": "t9bS9jgM",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7158.517404850934,
			"y": -2651.6673024224083,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 466.7421569824219,
			"height": 118.47005908836182,
			"seed": 766259904,
			"groupIds": [
				"WTUcVbgQJICGPk9yZP7iH"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 87.75559932471235,
			"fontFamily": 1,
			"text": "Message Q",
			"rawText": "Message Q",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Message Q",
			"lineHeight": 1.3500000000000016,
			"baseline": 81
		},
		{
			"type": "line",
			"version": 318,
			"versionNonce": 770715894,
			"isDeleted": false,
			"id": "ZtKb3W2DnOOFOis5dimeN",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5442.540283491922,
			"y": -3373.5801646348186,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3660,
			"height": 26.66666666666697,
			"seed": 1066597056,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					3660,
					-26.66666666666697
				]
			]
		},
		{
			"type": "rectangle",
			"version": 2057,
			"versionNonce": 220201322,
			"isDeleted": false,
			"id": "4LV1X0NuglGE98UHmXJ3W",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7794.98147710765,
			"y": -4210.566350846026,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 448.99784240267087,
			"height": 160.20580292301833,
			"seed": 1419856576,
			"groupIds": [
				"7kEDwm_Nx97ZjVvkESiug",
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": {
				"type": 1
			},
			"boundElements": [
				{
					"id": "db92jeTka_Gq8rdxXr3oi",
					"type": "arrow"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1975,
			"versionNonce": 1441440310,
			"isDeleted": false,
			"id": "PuQgvYRH2OFDDFMemtMcz",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7919.351771482082,
			"y": -4391.85186467996,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 303.5478371172988,
			"height": 293.00798166183694,
			"seed": 799666880,
			"groupIds": [
				"7kEDwm_Nx97ZjVvkESiug",
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2382,
			"versionNonce": 1295008810,
			"isDeleted": false,
			"id": "f44x08wnwH9KfoHGe9LaT",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7721.202488919403,
			"y": -4259.0496859411405,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 210.7971091092354,
			"height": 204.47319583595822,
			"seed": 1935514304,
			"groupIds": [
				"7kEDwm_Nx97ZjVvkESiug",
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2315,
			"versionNonce": 268757878,
			"isDeleted": false,
			"id": "RFLdC6KX4tYbZpul1KCf2",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7835.032927838377,
			"y": -4341.260558493744,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 144.70410782237067,
			"height": 130.07803148263727,
			"seed": 1381778112,
			"groupIds": [
				"7kEDwm_Nx97ZjVvkESiug",
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2097,
			"versionNonce": 262811370,
			"isDeleted": false,
			"id": "5jSvumX6tdnRW4-mDjn2y",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 8121.716996226962,
			"y": -4218.998235210386,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 179.17754274285016,
			"height": 168.63768728738816,
			"seed": 726002368,
			"groupIds": [
				"7kEDwm_Nx97ZjVvkESiug",
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1367,
			"versionNonce": 981732534,
			"isDeleted": false,
			"id": "vZYSkNVjBBAFQ7XBfORY5",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7748.0061762727555,
			"y": -4233.140882795913,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 185.65541205314202,
			"height": 180.6824992302898,
			"seed": 146444992,
			"groupIds": [
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "db92jeTka_Gq8rdxXr3oi",
					"type": "arrow"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1058,
			"versionNonce": 689488298,
			"isDeleted": false,
			"id": "41u4GDLbhzsWInOR29cjZ",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7998.309455022976,
			"y": -4302.761662315843,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 223.7810770283411,
			"height": 240.35745310451424,
			"seed": 559561408,
			"groupIds": [
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1256,
			"versionNonce": 588056054,
			"isDeleted": false,
			"id": "ncEcZNrclIiPOwjdtLyaN",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 8076.218422580969,
			"y": -4218.2221443273675,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 213.83525138263687,
			"height": 164.10612315411643,
			"seed": 1472520896,
			"groupIds": [
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1156,
			"versionNonce": 614923370,
			"isDeleted": false,
			"id": "tyrFiH4eXLBuMEFRAjZ5y",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7888.905372920214,
			"y": -4334.256776860579,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 179.02486162267266,
			"height": 180.68249923029006,
			"seed": 983206592,
			"groupIds": [
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1111,
			"versionNonce": 447010614,
			"isDeleted": false,
			"id": "vt3Oz9rVmwx1mBCJkx95n",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7812.654042969857,
			"y": -4287.842923847294,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 246.98800353498336,
			"height": 225.43871463595812,
			"seed": 75182784,
			"groupIds": [
				"ywpoAEgNuWHkTV1faL_y9",
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1361,
			"versionNonce": 1881136938,
			"isDeleted": false,
			"id": "yOkrlYEe",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7774.205537056584,
			"y": -4196.72781519068,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 460.35247802734375,
			"height": 101.90658695269967,
			"seed": 470211264,
			"groupIds": [
				"YVfTvbpbjOiUJ2hPIQWVc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 75.4863607057036,
			"fontFamily": 1,
			"text": "Cloudflare S",
			"rawText": "Cloudflare S",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Cloudflare S",
			"lineHeight": 1.3499999999999974,
			"baseline": 70
		},
		{
			"type": "rectangle",
			"version": 300,
			"versionNonce": 162562166,
			"isDeleted": false,
			"id": "nK1eL5MrFlwGQoi7bgDJG",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "dotted",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6279.206950158589,
			"y": -2843.5801646348136,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2510.000000000001,
			"height": 336.66666666666623,
			"seed": 811929920,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "ba-6x-m87IxI2xygN6Mx0",
					"type": "arrow"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 185,
			"versionNonce": 133065194,
			"isDeleted": false,
			"id": "KlmxmjCUlYjzTRBqqBlZ4",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5336.206950158587,
			"y": -4732.58016463481,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3933.333333333332,
			"height": 4846.666666666666,
			"seed": 548582080,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1669,
			"versionNonce": 66388406,
			"isDeleted": false,
			"id": "LisgJG_8mMPrUbZ9OKP9h",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16227.862526090146,
			"y": -6503.380657051501,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2040.3787245892506,
			"height": 1390.058812369569,
			"seed": 1445612224,
			"groupIds": [
				"T6EYG274ztM3N3pl0tIv4"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1804,
			"versionNonce": 589143210,
			"isDeleted": false,
			"id": "4QLLPQUI",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16433.856371482405,
			"y": -5820.027719594979,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1102.420166015625,
			"height": 581.2234215463398,
			"seed": 403894976,
			"groupIds": [
				"T6EYG274ztM3N3pl0tIv4"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 232.48936861853588,
			"fontFamily": 1,
			"text": "Monitoring\n(Go)",
			"rawText": "Monitoring\n(Go)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Monitoring\n(Go)",
			"lineHeight": 1.25,
			"baseline": 495
		},
		{
			"type": "line",
			"version": 7998,
			"versionNonce": 1553423094,
			"isDeleted": false,
			"id": "MCHixt7ORiUoaB24ZHxTT",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17774.806227840138,
			"y": -6332.800955576085,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 394.25394418898475,
			"height": 508.84730579838,
			"seed": 1984944832,
			"groupIds": [
				"VSzf0YMu_g0ZmJIdzCoJs",
				"e6-VWMh-e5_bNlUFuOdDX",
				"Q7nh_nEMoNmdArZuo8Gia"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					1.3000470409510962,
					384.58403573179606
				],
				[
					0.06083914960732413,
					428.36725815857045
				],
				[
					20.30495007614043,
					447.28544716046054
				],
				[
					90.80405626214062,
					463.29636076890654
				],
				[
					209.967515819022,
					468.2819200897665
				],
				[
					323.82032136248716,
					460.3217443320062
				],
				[
					384.3111552276136,
					441.28512797783054
				],
				[
					392.8425688022975,
					425.23706069023274
				],
				[
					394.04077495486524,
					389.98750759723345
				],
				[
					393.10032245139666,
					32.264454010911805
				],
				[
					390.98024063493335,
					-1.5337834903142975
				],
				[
					365.66516006842795,
					-20.42384076178178
				],
				[
					312.3570028550086,
					-31.36396237763105
				],
				[
					190.8749151641596,
					-40.565385708613476
				],
				[
					93.4770909052066,
					-35.0785562575891
				],
				[
					16.874363589188178,
					-16.46790023652897
				],
				[
					-0.2131692341195204,
					-0.23108261513814352
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 8719,
			"versionNonce": 1599633258,
			"isDeleted": false,
			"id": "w_qP1OO32v-C0YjuFgUa3",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17776.203951779735,
			"y": -6378.805971745025,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 391.7251348241278,
			"height": 79.22346144898371,
			"seed": 1023836864,
			"groupIds": [
				"VSzf0YMu_g0ZmJIdzCoJs",
				"e6-VWMh-e5_bNlUFuOdDX",
				"Q7nh_nEMoNmdArZuo8Gia"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 6957,
			"versionNonce": 974949430,
			"isDeleted": false,
			"id": "yNWI4COjZKIr4byvwT2T4",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 12323.069503037937,
			"y": -5931.784525007102,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 228.74316370113166,
			"height": 295.22936747926303,
			"seed": 1185426112,
			"groupIds": [
				"e6xUg7sVtI8MY7mPYtYrR",
				"WKAbcUj37TvUe2nefw5cy",
				"UHXrwf8wqzlJ6GoUD1_KG",
				"8kEo7fxlcYhd2jvmaQ2xY"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0.7542774840697635,
					223.13275577547907
				],
				[
					0.03529841555978175,
					248.53545107516138
				],
				[
					11.780778829655814,
					259.5116415929002
				],
				[
					52.68382831026584,
					268.80105286328154
				],
				[
					121.82156843531305,
					271.6936367642977
				],
				[
					187.87810717162128,
					267.075202850611
				],
				[
					222.97443256588514,
					256.03030167663184
				],
				[
					227.92429435085822,
					246.71933412193783
				],
				[
					228.61948451989593,
					226.2678093816333
				],
				[
					228.07384107326772,
					18.71959277598987
				],
				[
					226.84378559975644,
					-0.8898896084065069
				],
				[
					212.15616686193164,
					-11.849758308413197
				],
				[
					181.2271762663937,
					-18.197134324732623
				],
				[
					110.74418559248709,
					-23.535730714965336
				],
				[
					54.234702841642864,
					-20.3523136666016
				],
				[
					9.79037843432165,
					-9.554551463948288
				],
				[
					-0.12367918123571855,
					-0.13407238974302393
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 7677,
			"versionNonce": 1827273258,
			"isDeleted": false,
			"id": "xkoabFx1ES7wtKSrt5aGw",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 12323.880451921612,
			"y": -5958.476288272153,
			"strokeColor": "#000000",
			"backgroundColor": "#fff",
			"width": 227.2759675879657,
			"height": 45.964854577354636,
			"seed": 2111099584,
			"groupIds": [
				"e6xUg7sVtI8MY7mPYtYrR",
				"WKAbcUj37TvUe2nefw5cy",
				"UHXrwf8wqzlJ6GoUD1_KG",
				"8kEo7fxlcYhd2jvmaQ2xY"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 572,
			"versionNonce": 711562614,
			"isDeleted": false,
			"id": "1RPdXNmprfh3mbndofUg-",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 12449.949374401038,
			"y": -5090.864616294264,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 3.3333333333339397,
			"height": 554.9999999999995,
			"seed": 2032958144,
			"groupIds": [
				"8kEo7fxlcYhd2jvmaQ2xY"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-3.3333333333339397,
					-554.9999999999995
				]
			]
		},
		{
			"type": "line",
			"version": 7054,
			"versionNonce": 985474282,
			"isDeleted": false,
			"id": "jIpBMLDUOBWcRahz_aD3n",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11593.088181997382,
			"y": -5939.484616179534,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 228.74316370113166,
			"height": 295.22936747926303,
			"seed": 2068783808,
			"groupIds": [
				"gGZbfWefnfRbNPHI61BZG",
				"i9Z58fzyWSySPJI3VdtEt",
				"1g5b-HxKO_I5uYcfDjaPy",
				"PrBFsxk-iJ9iJo4f7icAs"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0.7542774840697635,
					223.13275577547907
				],
				[
					0.03529841555978175,
					248.53545107516138
				],
				[
					11.780778829655814,
					259.5116415929002
				],
				[
					52.68382831026584,
					268.80105286328154
				],
				[
					121.82156843531305,
					271.6936367642977
				],
				[
					187.87810717162128,
					267.075202850611
				],
				[
					222.97443256588514,
					256.03030167663184
				],
				[
					227.92429435085822,
					246.71933412193783
				],
				[
					228.61948451989593,
					226.2678093816333
				],
				[
					228.07384107326772,
					18.71959277598987
				],
				[
					226.84378559975644,
					-0.8898896084065069
				],
				[
					212.15616686193164,
					-11.849758308413197
				],
				[
					181.2271762663937,
					-18.197134324732623
				],
				[
					110.74418559248709,
					-23.535730714965336
				],
				[
					54.234702841642864,
					-20.3523136666016
				],
				[
					9.79037843432165,
					-9.554551463948288
				],
				[
					-0.12367918123571855,
					-0.13407238974302393
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 7774,
			"versionNonce": 918779574,
			"isDeleted": false,
			"id": "mdmkSAP-r2XUgrV3hFMH6",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11593.89913088106,
			"y": -5966.176379444585,
			"strokeColor": "#000000",
			"backgroundColor": "#fff",
			"width": 227.2759675879657,
			"height": 45.964854577354636,
			"seed": 1927072448,
			"groupIds": [
				"gGZbfWefnfRbNPHI61BZG",
				"i9Z58fzyWSySPJI3VdtEt",
				"1g5b-HxKO_I5uYcfDjaPy",
				"PrBFsxk-iJ9iJo4f7icAs"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 698,
			"versionNonce": 576518058,
			"isDeleted": false,
			"id": "Vjfw4PKFxOyHDbu28G6e4",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11671.634720027148,
			"y": -5636.898040800026,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 5.000000000000455,
			"height": 538.333333333333,
			"seed": 2054517440,
			"groupIds": [
				"PrBFsxk-iJ9iJo4f7icAs"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-5.000000000000455,
					538.333333333333
				]
			]
		},
		{
			"type": "text",
			"version": 484,
			"versionNonce": 2010066934,
			"isDeleted": false,
			"id": "3xURBCzK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11606.672722382807,
			"y": -6133.340806770453,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 172.95907592773438,
			"height": 87.85714285714313,
			"seed": 1488526016,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 70.2857142857145,
			"fontFamily": 1,
			"text": "Read",
			"rawText": "Read",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Read",
			"lineHeight": 1.25,
			"baseline": 61
		},
		{
			"type": "text",
			"version": 522,
			"versionNonce": 334787178,
			"isDeleted": false,
			"id": "b4RFxYWW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 12348.901023294848,
			"y": -6125.840806770453,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 176.1919403076172,
			"height": 87.85714285714313,
			"seed": 4702912,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 70.2857142857145,
			"fontFamily": 1,
			"text": "Write",
			"rawText": "Write",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Write",
			"lineHeight": 1.25,
			"baseline": 61
		},
		{
			"type": "line",
			"version": 455,
			"versionNonce": 697418038,
			"isDeleted": false,
			"id": "UDyP1xsObuS2W-ZzMWP0d",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 9982.540283491924,
			"y": -4953.652855832504,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9339.999999999998,
			"height": 6.66666666666697,
			"seed": 1997161152,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					9339.999999999998,
					-6.66666666666697
				]
			]
		},
		{
			"type": "rectangle",
			"version": 2125,
			"versionNonce": 1112446250,
			"isDeleted": false,
			"id": "XpbCBE0Psqg3Bu8oWXThC",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14279.981477107653,
			"y": -5920.639042043711,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 448.99784240267087,
			"height": 160.20580292301833,
			"seed": 171174592,
			"groupIds": [
				"n27ttSRzxcmeNWZtZaFUS",
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": {
				"type": 1
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2046,
			"versionNonce": 1064315510,
			"isDeleted": false,
			"id": "giVWrZMkul5jVhBVtHGtB",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14404.351771482081,
			"y": -6101.924555877647,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 303.5478371172988,
			"height": 293.00798166183694,
			"seed": 1508414144,
			"groupIds": [
				"n27ttSRzxcmeNWZtZaFUS",
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2453,
			"versionNonce": 1322672106,
			"isDeleted": false,
			"id": "_DWlZcZhREvQoQ7DKudan",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14206.202488919404,
			"y": -5969.122377138827,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 210.7971091092354,
			"height": 204.47319583595822,
			"seed": 482884288,
			"groupIds": [
				"n27ttSRzxcmeNWZtZaFUS",
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2386,
			"versionNonce": 2016373686,
			"isDeleted": false,
			"id": "T8aQdSeYnXHhM_DCeibU5",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14320.032927838376,
			"y": -6051.33324969143,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 144.70410782237067,
			"height": 130.07803148263727,
			"seed": 896721600,
			"groupIds": [
				"n27ttSRzxcmeNWZtZaFUS",
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2168,
			"versionNonce": 1972818602,
			"isDeleted": false,
			"id": "M9oZLYSeM5Mt-9NWsu8Ud",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14606.716996226965,
			"y": -5929.070926408072,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 179.17754274285016,
			"height": 168.63768728738816,
			"seed": 847809216,
			"groupIds": [
				"n27ttSRzxcmeNWZtZaFUS",
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1437,
			"versionNonce": 1911850230,
			"isDeleted": false,
			"id": "HK1cdWW7nFPUbqAv_ifSc",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14233.006176272756,
			"y": -5943.2135739936,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 185.65541205314202,
			"height": 180.6824992302898,
			"seed": 1319711424,
			"groupIds": [
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1129,
			"versionNonce": 960163178,
			"isDeleted": false,
			"id": "Nij7DIYy-8x2Vx_TuLHNR",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14483.309455022976,
			"y": -6012.83435351353,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 223.7810770283411,
			"height": 240.35745310451424,
			"seed": 1886706368,
			"groupIds": [
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1327,
			"versionNonce": 1044674102,
			"isDeleted": false,
			"id": "nn2-6KN0dS3CTh8W9vpnE",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14561.218422580969,
			"y": -5928.294835525054,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 213.83525138263687,
			"height": 164.10612315411643,
			"seed": 713786048,
			"groupIds": [
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1227,
			"versionNonce": 252555306,
			"isDeleted": false,
			"id": "Q0U1rkLCRCG-wE8pS4Tt3",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14373.905372920217,
			"y": -6044.329468058264,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 179.02486162267266,
			"height": 180.68249923029006,
			"seed": 999107264,
			"groupIds": [
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1180,
			"versionNonce": 1979989878,
			"isDeleted": false,
			"id": "4kJ7Phxg7kxgG1BhD-rxQ",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14297.654042969858,
			"y": -5997.91561504498,
			"strokeColor": "#ced4da",
			"backgroundColor": "#ced4da",
			"width": 246.98800353498336,
			"height": 225.43871463595812,
			"seed": 236573376,
			"groupIds": [
				"nPBm0NG-WwZP4vMGzAor2",
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1432,
			"versionNonce": 184163050,
			"isDeleted": false,
			"id": "orXmcoC3",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14259.205537056585,
			"y": -5906.800506388367,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 460.35247802734375,
			"height": 101.90658695269967,
			"seed": 953252544,
			"groupIds": [
				"tFJa67sIIsJT9-rs0WLzd"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 75.4863607057036,
			"fontFamily": 1,
			"text": "Cloudflare S",
			"rawText": "Cloudflare S",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Cloudflare S",
			"lineHeight": 1.3499999999999974,
			"baseline": 70
		},
		{
			"type": "rectangle",
			"version": 619,
			"versionNonce": 1299767478,
			"isDeleted": false,
			"id": "SBVFD3oJKjY1lPBK46s9b",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 10218.038489807657,
			"y": -3514.4291513947514,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 456.20438248398773,
			"height": 310.8005952380951,
			"seed": 1555409600,
			"groupIds": [
				"7iXRgczHAwiPSqSAuWBHG",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "usXXCPL4d5kST6IvfZa4S",
					"type": "arrow"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 653,
			"versionNonce": 193670570,
			"isDeleted": false,
			"id": "GzY4mVIK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 10325.273782901504,
			"y": -3481.7132992644247,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 244.18603515625,
			"height": 271.2689405806179,
			"seed": 1983009472,
			"groupIds": [
				"7iXRgczHAwiPSqSAuWBHG",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "usXXCPL4d5kST6IvfZa4S",
					"type": "arrow"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 72.33838415483143,
			"fontFamily": 1,
			"text": "User\nService\n(TS)",
			"rawText": "User\nService\n(TS)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "User\nService\n(TS)",
			"lineHeight": 1.25,
			"baseline": 244
		},
		{
			"type": "rectangle",
			"version": 745,
			"versionNonce": 675764726,
			"isDeleted": false,
			"id": "eltjktgtrn8HkWh-wIUlz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11049.185828640853,
			"y": -3517.8887248074493,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 456.20438248398773,
			"height": 310.8005952380951,
			"seed": 165280448,
			"groupIds": [
				"wGxGyPhNR3W9SPJs6Shqm",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "68sWx76iSq86ZCpKr-RWm",
					"type": "arrow"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 856,
			"versionNonce": 1709959274,
			"isDeleted": false,
			"id": "c8qhZwZx",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11119.570248177033,
			"y": -3485.172872677124,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 322.48382568359375,
			"height": 259.90926970203253,
			"seed": 441230016,
			"groupIds": [
				"wGxGyPhNR3W9SPJs6Shqm",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "68sWx76iSq86ZCpKr-RWm",
					"type": "arrow"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 51.9818539404065,
			"fontFamily": 1,
			"text": "Messaging/\nNotifications\nService\n(Go)",
			"rawText": "Messaging/\nNotifications\nService\n(Go)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Messaging/\nNotifications\nService\n(Go)",
			"lineHeight": 1.25,
			"baseline": 240
		},
		{
			"type": "rectangle",
			"version": 514,
			"versionNonce": 762620726,
			"isDeleted": false,
			"id": "qYqt4P1OEKdD9TsiQFEXF",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 10129.96782268847,
			"y": -2375.855490680469,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2777.0089285714284,
			"height": 230.0148809523809,
			"seed": 1722194624,
			"groupIds": [
				"n3Nj2aIZiU2jbG9b-sitL",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "68sWx76iSq86ZCpKr-RWm",
					"type": "arrow"
				},
				{
					"id": "feDEPj9KatTs94R8dZmqA",
					"type": "arrow"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 529,
			"versionNonce": 300370730,
			"isDeleted": false,
			"id": "YBBBWyOp",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11038.26488335448,
			"y": -2311.806631553485,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 983.8018798828125,
			"height": 86.25558035714285,
			"seed": 1954890432,
			"groupIds": [
				"n3Nj2aIZiU2jbG9b-sitL",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 69.00446428571428,
			"fontFamily": 1,
			"text": "Orchestrator Service (Proxy)",
			"rawText": "Orchestrator Service (Proxy)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Orchestrator Service (Proxy)",
			"lineHeight": 1.25,
			"baseline": 60
		},
		{
			"type": "text",
			"version": 580,
			"versionNonce": 1533400182,
			"isDeleted": false,
			"id": "MHCfSjtU",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11295.142959225936,
			"y": -2218.5466812083273,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 496.0892333984375,
			"height": 52.594866071428555,
			"seed": 542042816,
			"groupIds": [
				"n3Nj2aIZiU2jbG9b-sitL",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 42.07589285714285,
			"fontFamily": 1,
			"text": "(Go) (Service Discovery)",
			"rawText": "(Go) (Service Discovery)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "(Go) (Service Discovery)",
			"lineHeight": 1.25,
			"baseline": 36
		},
		{
			"type": "arrow",
			"version": 1079,
			"versionNonce": 1441289706,
			"isDeleted": false,
			"id": "usXXCPL4d5kST6IvfZa4S",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 10477.0844995616,
			"y": -2375.199338735988,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.283020547089283,
			"height": 822.2096974206353,
			"seed": 673397440,
			"groupIds": [
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "C7l9hWOE"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "GzY4mVIK",
				"focus": -0.14187074224796173,
				"gap": 13.03532252718378
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-10.283020547089283,
					-822.2096974206353
				]
			]
		},
		{
			"type": "text",
			"version": 367,
			"versionNonce": 467654070,
			"isDeleted": false,
			"id": "C7l9hWOE",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 10455.09833072071,
			"y": -2767.8313695334673,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 493740736,
			"groupIds": [
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "usXXCPL4d5kST6IvfZa4S",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 1425,
			"versionNonce": 1928988842,
			"isDeleted": false,
			"id": "68sWx76iSq86ZCpKr-RWm",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11293.944702476412,
			"y": -2383.159311326187,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.821001919481205,
			"height": 802.3934342363773,
			"seed": 1663273664,
			"groupIds": [
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "1FVdfmjJ"
				}
			],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "qYqt4P1OEKdD9TsiQFEXF",
				"focus": -0.16059000261655232,
				"gap": 7.303820645718133
			},
			"endBinding": {
				"elementId": "eltjktgtrn8HkWh-wIUlz",
				"focus": -0.025632253374677928,
				"gap": 21.53538400679031
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-8.821001919481205,
					-802.3934342363773
				]
			]
		},
		{
			"type": "text",
			"version": 368,
			"versionNonce": 1476898550,
			"isDeleted": false,
			"id": "1FVdfmjJ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11276.311761424851,
			"y": -2748.117083819181,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 870593216,
			"groupIds": [
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "68sWx76iSq86ZCpKr-RWm",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 1089,
			"versionNonce": 1355244394,
			"isDeleted": false,
			"id": "5NKiWegBgXlFlmQNZMAML",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11023.865825426858,
			"y": -4277.089607990935,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 490.79027429685317,
			"height": 334.3630952380951,
			"seed": 1371935424,
			"groupIds": [
				"7eruL0onp9Al7MMIjzxuL",
				"jGROB8WmDD7SIkqi6O0xg",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1169,
			"versionNonce": 207773750,
			"isDeleted": false,
			"id": "x8IHKpp5",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11117.14598180856,
			"y": -4214.0630329326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 301.3190002441406,
			"height": 194.55630395433005,
			"seed": 1022737088,
			"groupIds": [
				"7eruL0onp9Al7MMIjzxuL",
				"jGROB8WmDD7SIkqi6O0xg",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864760,
			"link": null,
			"locked": false,
			"fontSize": 77.82252158173202,
			"fontFamily": 1,
			"text": "Storage\nService",
			"rawText": "Storage\nService",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Storage\nService",
			"lineHeight": 1.25,
			"baseline": 165
		},
		{
			"type": "rectangle",
			"version": 840,
			"versionNonce": 698050090,
			"isDeleted": false,
			"id": "16veHtkjtduo9FjnutlDl",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11949.629790460971,
			"y": -3548.6018852792695,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 490.79027429685317,
			"height": 334.3630952380951,
			"seed": 1945133760,
			"groupIds": [
				"PnA3JSmAhLdLEBysRcDgp",
				"tzwrZTNrA4teZks5W1apo",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "feDEPj9KatTs94R8dZmqA",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 968,
			"versionNonce": 1557457270,
			"isDeleted": false,
			"id": "ZsHaJFaB",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 12013.14565909275,
			"y": -3485.5753102209346,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 360.85125732421875,
			"height": 194.55630395433005,
			"seed": 1163266752,
			"groupIds": [
				"PnA3JSmAhLdLEBysRcDgp",
				"tzwrZTNrA4teZks5W1apo",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 77.82252158173202,
			"fontFamily": 1,
			"text": "Streaming\nService",
			"rawText": "Streaming\nService",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Streaming\nService",
			"lineHeight": 1.25,
			"baseline": 165
		},
		{
			"type": "arrow",
			"version": 987,
			"versionNonce": 912330986,
			"isDeleted": false,
			"id": "feDEPj9KatTs94R8dZmqA",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 12222.777469156348,
			"y": -2391.1408237713345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.707637534124824,
			"height": 818.7968749999995,
			"seed": 734442176,
			"groupIds": [
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "qYqt4P1OEKdD9TsiQFEXF",
				"focus": 0.5086110281060721,
				"gap": 15.285333090865606
			},
			"endBinding": {
				"elementId": "16veHtkjtduo9FjnutlDl",
				"focus": -0.005998622491304531,
				"gap": 4.301091269840299
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-21.707637534124824,
					-818.7968749999995
				]
			]
		},
		{
			"type": "line",
			"version": 3880,
			"versionNonce": 681855670,
			"isDeleted": false,
			"id": "Zh1EeDBZ4DtfYlL3KGYIn",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 4.70956944444772,
			"x": 11212.172375283819,
			"y": -4002.262310788993,
			"strokeColor": "#000000",
			"backgroundColor": "#eeeeee",
			"width": 113.09564138589296,
			"height": 492.92592225659297,
			"seed": 1306680000,
			"groupIds": [
				"oJd4TdKJa5QUElKwl9uES",
				"23huihzqGxh1jVwNnrbAb",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					113.09564138589296,
					-0.4350451061894613
				],
				[
					112.12606792336288,
					443.2714136519526
				],
				[
					54.38496906662732,
					492.4908771504035
				],
				[
					1.773298832785008,
					440.55567753452806
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1798,
			"versionNonce": 1520657322,
			"isDeleted": false,
			"id": "W7GQnqvGpPKMQXAb0vgoX",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11039.124952881819,
			"y": -3778.969626458938,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 92.00918879029342,
			"height": 61.155808118099465,
			"seed": 2118714048,
			"groupIds": [
				"WnFb1JlWhHJR3vxoqouB4",
				"oJd4TdKJa5QUElKwl9uES",
				"23huihzqGxh1jVwNnrbAb",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3122,
			"versionNonce": 511017974,
			"isDeleted": false,
			"id": "IR_ZC3Evl0KpJthBThgIA",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11087.562944729101,
			"y": -3748.9969120339465,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 89.56576748445045,
			"height": 28.890370479435358,
			"seed": 999992000,
			"groupIds": [
				"WnFb1JlWhHJR3vxoqouB4",
				"oJd4TdKJa5QUElKwl9uES",
				"23huihzqGxh1jVwNnrbAb",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					43.64176878137867,
					-28.890370479435358
				],
				[
					-45.92399870307177,
					-28.536623396265053
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 2064,
			"versionNonce": 1351442026,
			"isDeleted": false,
			"id": "jcheJwWoZ4CjHTQ1Iy0Kz",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dotted",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11234.0584271527,
			"y": -3743.747541530522,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 115.61120548241641,
			"height": 2.141748890171376,
			"seed": 813126336,
			"groupIds": [
				"oJd4TdKJa5QUElKwl9uES",
				"23huihzqGxh1jVwNnrbAb",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					115.61120548241641,
					-2.141748890171376
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1874,
			"versionNonce": 1347261750,
			"isDeleted": false,
			"id": "NF9mPK62GXnVQ6WmGdvDc",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11149.108881674661,
			"y": -3778.4400088243037,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 92.00918879029342,
			"height": 61.155808118099465,
			"seed": 863959744,
			"groupIds": [
				"m4z0YufEvi1nxiWLE7-Rd",
				"oJd4TdKJa5QUElKwl9uES",
				"23huihzqGxh1jVwNnrbAb",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3195,
			"versionNonce": 1424621866,
			"isDeleted": false,
			"id": "R-itEw219IOXxDM5LCwqV",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11197.620501345056,
			"y": -3750.607117365245,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 89.56576748445045,
			"height": 28.890370479435358,
			"seed": 1196532416,
			"groupIds": [
				"m4z0YufEvi1nxiWLE7-Rd",
				"oJd4TdKJa5QUElKwl9uES",
				"23huihzqGxh1jVwNnrbAb",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					43.64176878137867,
					-28.890370479435358
				],
				[
					-45.92399870307177,
					-28.536623396265053
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1923,
			"versionNonce": 1200717430,
			"isDeleted": false,
			"id": "mrjLR2LDu77hI4jaS-M6Z",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11346.479720182484,
			"y": -3780.558479362851,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 92.00918879029342,
			"height": 61.155808118099465,
			"seed": 445598400,
			"groupIds": [
				"fj0bsdeJHoHHr0ua1NYX3",
				"oJd4TdKJa5QUElKwl9uES",
				"23huihzqGxh1jVwNnrbAb",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3280,
			"versionNonce": 1394887658,
			"isDeleted": false,
			"id": "sNQsRRdR1zCjNJ2orO1iq",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11396.848950857971,
			"y": -3754.043306215615,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 89.56576748445045,
			"height": 28.890370479435358,
			"seed": 131592896,
			"groupIds": [
				"fj0bsdeJHoHHr0ua1NYX3",
				"oJd4TdKJa5QUElKwl9uES",
				"23huihzqGxh1jVwNnrbAb",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					43.64176878137867,
					-28.890370479435358
				],
				[
					-45.92399870307177,
					-28.536623396265053
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "text",
			"version": 1165,
			"versionNonce": 419839926,
			"isDeleted": false,
			"id": "PpTXSIFf",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11083.616012758648,
			"y": -3699.8198493169357,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 367.4896240234375,
			"height": 93.28273854239985,
			"seed": 365664960,
			"groupIds": [
				"23huihzqGxh1jVwNnrbAb",
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 69.09832484622203,
			"fontFamily": 1,
			"text": "Message Q",
			"rawText": "Message Q",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Message Q",
			"lineHeight": 1.3500000000000016,
			"baseline": 64
		},
		{
			"type": "rectangle",
			"version": 403,
			"versionNonce": 289881770,
			"isDeleted": false,
			"id": "QVqZv1DhDu158m5t1ZALj",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "dotted",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 10176.921760521838,
			"y": -3867.763910540236,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2407.8732638888887,
			"height": 310.03472222222234,
			"seed": 1296157376,
			"groupIds": [
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "68sWx76iSq86ZCpKr-RWm",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 237,
			"versionNonce": 2026952950,
			"isDeleted": false,
			"id": "ImDP4Fzz4bn0y_Pp2OpvU",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 9886.22892818056,
			"y": -4454.4116664663115,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3108.9409722222235,
			"height": 2513.333333333332,
			"seed": 493115712,
			"groupIds": [
				"Rp_1xpH1nbtdd4CFSF2aX"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 136,
			"versionNonce": 1543362922,
			"isDeleted": false,
			"id": "IkGxTPvR",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 11064.032277993389,
			"y": -4667.7449997996455,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 390.7460632324219,
			"height": 158.3333333333326,
			"seed": 1544233280,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 126.66666666666607,
			"fontFamily": 1,
			"text": "Node 1",
			"rawText": "Node 1",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Node 1",
			"lineHeight": 1.25,
			"baseline": 111
		},
		{
			"type": "rectangle",
			"version": 710,
			"versionNonce": 1316375094,
			"isDeleted": false,
			"id": "LEuM2LSp2_xBJ6O02rMmr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 13423.568003696548,
			"y": -3524.429151394752,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 456.20438248398773,
			"height": 310.8005952380951,
			"seed": 1786368320,
			"groupIds": [
				"gx1oCfPo-TSmxHqGLgPrS",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "o8RGpTJRqiUEtFbsOkAlA",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 744,
			"versionNonce": 848501802,
			"isDeleted": false,
			"id": "uOeeViPu",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 13530.803296790395,
			"y": -3491.7132992644256,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 244.18603515625,
			"height": 271.2689405806179,
			"seed": 900573504,
			"groupIds": [
				"gx1oCfPo-TSmxHqGLgPrS",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "o8RGpTJRqiUEtFbsOkAlA",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 72.33838415483143,
			"fontFamily": 1,
			"text": "User\nService\n(TS)",
			"rawText": "User\nService\n(TS)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "User\nService\n(TS)",
			"lineHeight": 1.25,
			"baseline": 244
		},
		{
			"type": "rectangle",
			"version": 836,
			"versionNonce": 1222349686,
			"isDeleted": false,
			"id": "VahSYKOXf-e5LqJk8bnIs",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14254.715342529746,
			"y": -3527.8887248074498,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 456.20438248398773,
			"height": 310.8005952380951,
			"seed": 480674112,
			"groupIds": [
				"JGsegF0qu9SYvw3ND2gk0",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "GGWj62x01Xqth13ygLgBE",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 948,
			"versionNonce": 1928464106,
			"isDeleted": false,
			"id": "jsUl1bA3",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14325.099762065924,
			"y": -3495.1728726771244,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 322.48382568359375,
			"height": 259.90926970203253,
			"seed": 1589926208,
			"groupIds": [
				"JGsegF0qu9SYvw3ND2gk0",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "GGWj62x01Xqth13ygLgBE",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 51.9818539404065,
			"fontFamily": 1,
			"text": "Messaging/\nNotifications\nService\n(Go)",
			"rawText": "Messaging/\nNotifications\nService\n(Go)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Messaging/\nNotifications\nService\n(Go)",
			"lineHeight": 1.25,
			"baseline": 240
		},
		{
			"type": "rectangle",
			"version": 605,
			"versionNonce": 1917170870,
			"isDeleted": false,
			"id": "Izho3X6EEdgVN6MGpWFED",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 13335.49733657736,
			"y": -2385.8554906804693,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2777.0089285714284,
			"height": 230.0148809523809,
			"seed": 1332162880,
			"groupIds": [
				"qw8_Q2vG4onUsw_RozjlI",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "GGWj62x01Xqth13ygLgBE",
					"type": "arrow"
				},
				{
					"id": "PotLYXn7F4UjIM57NzIzO",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 620,
			"versionNonce": 94738858,
			"isDeleted": false,
			"id": "E80V3AVB",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14243.794397243373,
			"y": -2321.806631553485,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 983.8018798828125,
			"height": 86.25558035714285,
			"seed": 1441728832,
			"groupIds": [
				"qw8_Q2vG4onUsw_RozjlI",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 69.00446428571428,
			"fontFamily": 1,
			"text": "Orchestrator Service (Proxy)",
			"rawText": "Orchestrator Service (Proxy)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Orchestrator Service (Proxy)",
			"lineHeight": 1.25,
			"baseline": 60
		},
		{
			"type": "text",
			"version": 671,
			"versionNonce": 1146727926,
			"isDeleted": false,
			"id": "LNtKujny",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14500.672473114826,
			"y": -2228.5466812083278,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 496.0892333984375,
			"height": 52.594866071428555,
			"seed": 1841029440,
			"groupIds": [
				"qw8_Q2vG4onUsw_RozjlI",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 42.07589285714285,
			"fontFamily": 1,
			"text": "(Go) (Service Discovery)",
			"rawText": "(Go) (Service Discovery)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "(Go) (Service Discovery)",
			"lineHeight": 1.25,
			"baseline": 36
		},
		{
			"type": "arrow",
			"version": 1268,
			"versionNonce": 165205098,
			"isDeleted": false,
			"id": "o8RGpTJRqiUEtFbsOkAlA",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 13682.614013450491,
			"y": -2385.199338735989,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.283020547089283,
			"height": 822.2096974206353,
			"seed": 640530752,
			"groupIds": [
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "OzMAE50J"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "uOeeViPu",
				"focus": -0.14187074224796173,
				"gap": 13.03532252718378
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-10.283020547089283,
					-822.2096974206353
				]
			]
		},
		{
			"type": "text",
			"version": 500,
			"versionNonce": 1008500534,
			"isDeleted": false,
			"id": "OzMAE50J",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 13649.752517215033,
			"y": -2808.8041874463065,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 581210432,
			"groupIds": [
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "o8RGpTJRqiUEtFbsOkAlA",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 1641,
			"versionNonce": 22460202,
			"isDeleted": false,
			"id": "GGWj62x01Xqth13ygLgBE",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14499.097461590383,
			"y": -2393.7246332365266,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.911769980542886,
			"height": 796.2726495723991,
			"seed": 444623168,
			"groupIds": [
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "AnDPj3lg"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Izho3X6EEdgVN6MGpWFED",
				"focus": -0.1604533026837273,
				"gap": 7.869142556057341
			},
			"endBinding": {
				"elementId": "VahSYKOXf-e5LqJk8bnIs",
				"focus": -0.00710940370070083,
				"gap": 27.090846760428803
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-11.911769980542886,
					-796.2726495723991
				]
			]
		},
		{
			"type": "text",
			"version": 501,
			"versionNonce": 1844652150,
			"isDeleted": false,
			"id": "AnDPj3lg",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14455.995911421962,
			"y": -2789.449276732019,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 1495351616,
			"groupIds": [
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "GGWj62x01Xqth13ygLgBE",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 1254,
			"versionNonce": 2089435626,
			"isDeleted": false,
			"id": "1YsrnPZO5wjXuBak4LZSs",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 15149.395339315748,
			"y": -4347.089607990936,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 490.79027429685317,
			"height": 334.3630952380951,
			"seed": 1038555456,
			"groupIds": [
				"G8VcH566WHZwJkRKVobv2",
				"x2JNg5KLaw6Ml211IqiDe",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1334,
			"versionNonce": 430090678,
			"isDeleted": false,
			"id": "VoUWSevZ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 15242.67549569745,
			"y": -4284.063032932601,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 301.3190002441406,
			"height": 194.55630395433005,
			"seed": 1009905984,
			"groupIds": [
				"G8VcH566WHZwJkRKVobv2",
				"x2JNg5KLaw6Ml211IqiDe",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 77.82252158173202,
			"fontFamily": 1,
			"text": "Storage\nService",
			"rawText": "Storage\nService",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Storage\nService",
			"lineHeight": 1.25,
			"baseline": 165
		},
		{
			"type": "rectangle",
			"version": 931,
			"versionNonce": 1182692522,
			"isDeleted": false,
			"id": "7GkYlZ6ig_jtvRiFt3Vhq",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 15155.15930434986,
			"y": -3558.6018852792695,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 490.79027429685317,
			"height": 334.3630952380951,
			"seed": 1533135168,
			"groupIds": [
				"u5YDiskz9wL2CxHku4jYM",
				"Hq9wuLKzoP4d-0DvGCC3s",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "PotLYXn7F4UjIM57NzIzO",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1059,
			"versionNonce": 1045431030,
			"isDeleted": false,
			"id": "io5qgSF9",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 15218.67517298164,
			"y": -3495.5753102209346,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 360.85125732421875,
			"height": 194.55630395433005,
			"seed": 920035648,
			"groupIds": [
				"u5YDiskz9wL2CxHku4jYM",
				"Hq9wuLKzoP4d-0DvGCC3s",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 77.82252158173202,
			"fontFamily": 1,
			"text": "Streaming\nService",
			"rawText": "Streaming\nService",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Streaming\nService",
			"lineHeight": 1.25,
			"baseline": 165
		},
		{
			"type": "arrow",
			"version": 1274,
			"versionNonce": 283004778,
			"isDeleted": false,
			"id": "PotLYXn7F4UjIM57NzIzO",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 15428.306983045239,
			"y": -2401.140823771335,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.707637534124824,
			"height": 818.7968749999995,
			"seed": 2112911680,
			"groupIds": [
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Izho3X6EEdgVN6MGpWFED",
				"focus": 0.5086110281060721,
				"gap": 15.285333090865606
			},
			"endBinding": {
				"elementId": "7GkYlZ6ig_jtvRiFt3Vhq",
				"focus": -0.00599862249130458,
				"gap": 4.301091269839844
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-21.707637534124824,
					-818.7968749999995
				]
			]
		},
		{
			"type": "line",
			"version": 3971,
			"versionNonce": 780153910,
			"isDeleted": false,
			"id": "XD5SJOwBeQvy9fuOnRw0d",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 4.70956944444772,
			"x": 14417.701889172708,
			"y": -4012.262310788994,
			"strokeColor": "#000000",
			"backgroundColor": "#eeeeee",
			"width": 113.09564138589296,
			"height": 492.92592225659297,
			"seed": 1947160896,
			"groupIds": [
				"kOjDmDHIn09Km-xYDi_Pc",
				"Dj8yNIv7qTdYtDXBWfmiR",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					113.09564138589296,
					-0.4350451061894613
				],
				[
					112.12606792336288,
					443.2714136519526
				],
				[
					54.38496906662732,
					492.4908771504035
				],
				[
					1.773298832785008,
					440.55567753452806
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1889,
			"versionNonce": 536138282,
			"isDeleted": false,
			"id": "DaGQOEBNVeVBJNlgvBLv6",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14244.654466770708,
			"y": -3788.9696264589384,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 92.00918879029342,
			"height": 61.155808118099465,
			"seed": 1888692544,
			"groupIds": [
				"ieou9vA5D92siUpVfzcqo",
				"kOjDmDHIn09Km-xYDi_Pc",
				"Dj8yNIv7qTdYtDXBWfmiR",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3213,
			"versionNonce": 605568374,
			"isDeleted": false,
			"id": "xVTuqSLUb75XeQyfLCz4m",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14293.092458617992,
			"y": -3758.9969120339465,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 89.56576748445045,
			"height": 28.890370479435358,
			"seed": 1591476544,
			"groupIds": [
				"ieou9vA5D92siUpVfzcqo",
				"kOjDmDHIn09Km-xYDi_Pc",
				"Dj8yNIv7qTdYtDXBWfmiR",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					43.64176878137867,
					-28.890370479435358
				],
				[
					-45.92399870307177,
					-28.536623396265053
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 2155,
			"versionNonce": 1991048426,
			"isDeleted": false,
			"id": "t7M67tflj7eOHJuHByR83",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dotted",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14439.58794104159,
			"y": -3753.7475415305225,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 115.61120548241641,
			"height": 2.141748890171376,
			"seed": 1045027136,
			"groupIds": [
				"kOjDmDHIn09Km-xYDi_Pc",
				"Dj8yNIv7qTdYtDXBWfmiR",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					115.61120548241641,
					-2.141748890171376
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1965,
			"versionNonce": 1415388854,
			"isDeleted": false,
			"id": "KGa8m7ZkhCK8CfuIqx8il",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14354.638395563552,
			"y": -3788.4400088243037,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 92.00918879029342,
			"height": 61.155808118099465,
			"seed": 574402880,
			"groupIds": [
				"gKHAe3jsTh8MFDDYIrCth",
				"kOjDmDHIn09Km-xYDi_Pc",
				"Dj8yNIv7qTdYtDXBWfmiR",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3286,
			"versionNonce": 43110314,
			"isDeleted": false,
			"id": "gkS8zhCyKuyRP1KgpnRI1",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14403.150015233945,
			"y": -3760.6071173652454,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 89.56576748445045,
			"height": 28.890370479435358,
			"seed": 840206656,
			"groupIds": [
				"gKHAe3jsTh8MFDDYIrCth",
				"kOjDmDHIn09Km-xYDi_Pc",
				"Dj8yNIv7qTdYtDXBWfmiR",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					43.64176878137867,
					-28.890370479435358
				],
				[
					-45.92399870307177,
					-28.536623396265053
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "rectangle",
			"version": 2014,
			"versionNonce": 66312182,
			"isDeleted": false,
			"id": "0dwT99Gu_dnrUPZEZw_8y",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14552.009234071376,
			"y": -3790.5584793628514,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 92.00918879029342,
			"height": 61.155808118099465,
			"seed": 691102016,
			"groupIds": [
				"2Baww-SzG2akKKgcaxsZx",
				"kOjDmDHIn09Km-xYDi_Pc",
				"Dj8yNIv7qTdYtDXBWfmiR",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3371,
			"versionNonce": 1204701802,
			"isDeleted": false,
			"id": "t0X7rgSZ8IGAm__KRi34-",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14602.378464746862,
			"y": -3764.0433062156153,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 89.56576748445045,
			"height": 28.890370479435358,
			"seed": 1458780480,
			"groupIds": [
				"2Baww-SzG2akKKgcaxsZx",
				"kOjDmDHIn09Km-xYDi_Pc",
				"Dj8yNIv7qTdYtDXBWfmiR",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					43.64176878137867,
					-28.890370479435358
				],
				[
					-45.92399870307177,
					-28.536623396265053
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "text",
			"version": 1256,
			"versionNonce": 450980150,
			"isDeleted": false,
			"id": "dKPCKvaT",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14289.14552664754,
			"y": -3709.8198493169366,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 367.4896240234375,
			"height": 93.28273854239985,
			"seed": 515510592,
			"groupIds": [
				"Dj8yNIv7qTdYtDXBWfmiR",
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 69.09832484622203,
			"fontFamily": 1,
			"text": "Message Q",
			"rawText": "Message Q",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Message Q",
			"lineHeight": 1.3500000000000016,
			"baseline": 64
		},
		{
			"type": "rectangle",
			"version": 460,
			"versionNonce": 221080874,
			"isDeleted": false,
			"id": "jBGFP-JpNhbTfbndXJu8n",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "dotted",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 13332.451274410729,
			"y": -3912.763910540236,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2507.8732638888882,
			"height": 340.0347222222222,
			"seed": 2011556160,
			"groupIds": [
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "GGWj62x01Xqth13ygLgBE",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 328,
			"versionNonce": 948621942,
			"isDeleted": false,
			"id": "dCiWY-Si1a8ddW0nRnFvs",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 13091.75844206945,
			"y": -4464.411666466312,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3108.9409722222235,
			"height": 2513.333333333332,
			"seed": 1842790720,
			"groupIds": [
				"lUbGfM28s9qRzgxT01VlN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 231,
			"versionNonce": 135935978,
			"isDeleted": false,
			"id": "5G7lVZ4M",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14241.643507783969,
			"y": -4677.744999799646,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 446.6031188964844,
			"height": 158.3333333333326,
			"seed": 535599424,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 126.66666666666607,
			"fontFamily": 1,
			"text": "Node 2",
			"rawText": "Node 2",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Node 2",
			"lineHeight": 1.25,
			"baseline": 111
		},
		{
			"type": "rectangle",
			"version": 676,
			"versionNonce": 1203049398,
			"isDeleted": false,
			"id": "S48s0wYSDlcRLCA_YPbnf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16643.56800369655,
			"y": -3542.762484728084,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 456.20438248398773,
			"height": 310.8005952380951,
			"seed": 313418048,
			"groupIds": [
				"QMMG8Y0pxsAPXZUa2vqO8",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "657IUcMDGIfZ36_RrEvYb",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 710,
			"versionNonce": 144681642,
			"isDeleted": false,
			"id": "IrJB5wfP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16750.803296790396,
			"y": -3510.0466325977577,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 244.18603515625,
			"height": 271.2689405806179,
			"seed": 147863872,
			"groupIds": [
				"QMMG8Y0pxsAPXZUa2vqO8",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "657IUcMDGIfZ36_RrEvYb",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 72.33838415483143,
			"fontFamily": 1,
			"text": "User\nService\n(TS)",
			"rawText": "User\nService\n(TS)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "User\nService\n(TS)",
			"lineHeight": 1.25,
			"baseline": 244
		},
		{
			"type": "rectangle",
			"version": 802,
			"versionNonce": 310717686,
			"isDeleted": false,
			"id": "hS9I81GG7e9fUzr8mu6b9",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17474.715342529747,
			"y": -3546.222058140782,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 456.20438248398773,
			"height": 310.8005952380951,
			"seed": 217518400,
			"groupIds": [
				"xu0VU1Qx3pQ71D-2s-g-e",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "tBz7DYHI65Xb8Sn8Rg9OO",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 913,
			"versionNonce": 627623274,
			"isDeleted": false,
			"id": "1ZItKg7e",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17545.099762065925,
			"y": -3513.5062060104574,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 322.48382568359375,
			"height": 259.90926970203253,
			"seed": 377678144,
			"groupIds": [
				"xu0VU1Qx3pQ71D-2s-g-e",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "tBz7DYHI65Xb8Sn8Rg9OO",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 51.9818539404065,
			"fontFamily": 1,
			"text": "Messaging/\nNotifications\nService\n(Go)",
			"rawText": "Messaging/\nNotifications\nService\n(Go)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Messaging/\nNotifications\nService\n(Go)",
			"lineHeight": 1.25,
			"baseline": 240
		},
		{
			"type": "rectangle",
			"version": 571,
			"versionNonce": 1451236918,
			"isDeleted": false,
			"id": "zcsv3_x_ANss8RSFynB4Q",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16555.497336577362,
			"y": -2404.1888240138014,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2777.0089285714284,
			"height": 230.0148809523809,
			"seed": 819183936,
			"groupIds": [
				"wM-_K949t2bzF3RDu3eVU",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "tBz7DYHI65Xb8Sn8Rg9OO",
					"type": "arrow"
				},
				{
					"id": "H8lOpKneVMCeYFMrQibir",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 586,
			"versionNonce": 1740671018,
			"isDeleted": false,
			"id": "ZnTHsicc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17463.794397243375,
			"y": -2340.1399648868182,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 983.8018798828125,
			"height": 86.25558035714285,
			"seed": 2068420928,
			"groupIds": [
				"wM-_K949t2bzF3RDu3eVU",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 69.00446428571428,
			"fontFamily": 1,
			"text": "Orchestrator Service (Proxy)",
			"rawText": "Orchestrator Service (Proxy)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Orchestrator Service (Proxy)",
			"lineHeight": 1.25,
			"baseline": 60
		},
		{
			"type": "text",
			"version": 637,
			"versionNonce": 1485498230,
			"isDeleted": false,
			"id": "KTLTTDaA",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17720.672473114828,
			"y": -2246.880014541661,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 496.0892333984375,
			"height": 52.594866071428555,
			"seed": 692351296,
			"groupIds": [
				"wM-_K949t2bzF3RDu3eVU",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 42.07589285714285,
			"fontFamily": 1,
			"text": "(Go) (Service Discovery)",
			"rawText": "(Go) (Service Discovery)",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "(Go) (Service Discovery)",
			"lineHeight": 1.25,
			"baseline": 36
		},
		{
			"type": "arrow",
			"version": 1195,
			"versionNonce": 2006053610,
			"isDeleted": false,
			"id": "657IUcMDGIfZ36_RrEvYb",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16902.614013450493,
			"y": -2403.532672069321,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.283020547089283,
			"height": 822.2096974206353,
			"seed": 35932480,
			"groupIds": [
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "4b8mh5jt"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "IrJB5wfP",
				"focus": -0.14182206894155122,
				"gap": 13.03532252718378
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-10.283020547089283,
					-822.2096974206353
				]
			]
		},
		{
			"type": "text",
			"version": 425,
			"versionNonce": 2028636342,
			"isDeleted": false,
			"id": "4b8mh5jt",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16869.752517215034,
			"y": -2827.1375207796386,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 1632182592,
			"groupIds": [
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "657IUcMDGIfZ36_RrEvYb",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 1535,
			"versionNonce": 1197999530,
			"isDeleted": false,
			"id": "tBz7DYHI65Xb8Sn8Rg9OO",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17720.34090232848,
			"y": -2421.084000919763,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.232442676857318,
			"height": 763.3779939949504,
			"seed": 907213120,
			"groupIds": [
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "8neGL49g"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "zcsv3_x_ANss8RSFynB4Q",
				"focus": -0.15835665767890375,
				"gap": 16.895176905961762
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-19.232442676857318,
					-763.3779939949504
				]
			]
		},
		{
			"type": "text",
			"version": 426,
			"versionNonce": 1195639286,
			"isDeleted": false,
			"id": "8neGL49g",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17675.995911421964,
			"y": -2807.7826100653524,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.439971923828125,
			"height": 25,
			"seed": 65130816,
			"groupIds": [
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "GRPC",
			"rawText": "GRPC",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "tBz7DYHI65Xb8Sn8Rg9OO",
			"originalText": "GRPC",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 1255,
			"versionNonce": 1080934506,
			"isDeleted": false,
			"id": "UYA6aDqlRr0nZDLarkyiM",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 18404.39533931575,
			"y": -4345.422941324268,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 490.79027429685317,
			"height": 334.3630952380951,
			"seed": 1645586752,
			"groupIds": [
				"7ZIUivfOEb8KjsF6Zy6-H",
				"lXQGQkLYEgNpxRmePTmRB",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1335,
			"versionNonce": 379343670,
			"isDeleted": false,
			"id": "VVbBHD6E",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 18497.67549569745,
			"y": -4282.3963662659335,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 301.3190002441406,
			"height": 194.55630395433005,
			"seed": 2081325376,
			"groupIds": [
				"7ZIUivfOEb8KjsF6Zy6-H",
				"lXQGQkLYEgNpxRmePTmRB",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 77.82252158173202,
			"fontFamily": 1,
			"text": "Storage\nService",
			"rawText": "Storage\nService",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Storage\nService",
			"lineHeight": 1.25,
			"baseline": 165
		},
		{
			"type": "rectangle",
			"version": 897,
			"versionNonce": 1852711722,
			"isDeleted": false,
			"id": "SiWacHolc3cjCKMC0GSuc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 18375.15930434986,
			"y": -3576.9352186126025,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 490.79027429685317,
			"height": 334.3630952380951,
			"seed": 288119104,
			"groupIds": [
				"7OCHlNhXgAy0X-aI-hrQH",
				"w6twpByNgY99Pc2YSeF9h",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "H8lOpKneVMCeYFMrQibir",
					"type": "arrow"
				}
			],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1025,
			"versionNonce": 291011702,
			"isDeleted": false,
			"id": "UdS9KHsW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 18438.675172981642,
			"y": -3513.9086435542677,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 360.85125732421875,
			"height": 194.55630395433005,
			"seed": 1959735616,
			"groupIds": [
				"7OCHlNhXgAy0X-aI-hrQH",
				"w6twpByNgY99Pc2YSeF9h",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 77.82252158173202,
			"fontFamily": 1,
			"text": "Streaming\nService",
			"rawText": "Streaming\nService",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Streaming\nService",
			"lineHeight": 1.25,
			"baseline": 165
		},
		{
			"type": "arrow",
			"version": 1162,
			"versionNonce": 735325674,
			"isDeleted": false,
			"id": "H8lOpKneVMCeYFMrQibir",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 18648.30698304524,
			"y": -2419.474157104667,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.707637534124824,
			"height": 818.7968749999995,
			"seed": 240585024,
			"groupIds": [
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "zcsv3_x_ANss8RSFynB4Q",
				"focus": 0.5086110281060734,
				"gap": 15.285333090865606
			},
			"endBinding": {
				"elementId": "SiWacHolc3cjCKMC0GSuc",
				"focus": -0.005998622491311765,
				"gap": 4.301091269840754
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-21.707637534124824,
					-818.7968749999995
				]
			]
		},
		{
			"type": "line",
			"version": 3937,
			"versionNonce": 1295875510,
			"isDeleted": false,
			"id": "OYKYEgQFII6jXGru9QSmy",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 4.70956944444772,
			"x": 17637.70188917271,
			"y": -4030.595644122326,
			"strokeColor": "#000000",
			"backgroundColor": "#eeeeee",
			"width": 113.09564138589296,
			"height": 492.92592225659297,
			"seed": 1495523648,
			"groupIds": [
				"MFnAE4vbecwYH7bCzgUk0",
				"HUiTzNTEp-VgzSFScDh6O",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					113.09564138589296,
					-0.4350451061894613
				],
				[
					112.12606792336288,
					443.2714136519526
				],
				[
					54.38496906662732,
					492.4908771504035
				],
				[
					1.773298832785008,
					440.55567753452806
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1855,
			"versionNonce": 1303044266,
			"isDeleted": false,
			"id": "mEeCVnao94CorXdDCb-bH",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17464.65446677071,
			"y": -3807.3029597922705,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 92.00918879029342,
			"height": 61.155808118099465,
			"seed": 1687533888,
			"groupIds": [
				"6ivs4qDTMgmRopjH79ZJG",
				"MFnAE4vbecwYH7bCzgUk0",
				"HUiTzNTEp-VgzSFScDh6O",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3179,
			"versionNonce": 1601197814,
			"isDeleted": false,
			"id": "egJYTAeqSsH6w3y8PJWyQ",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17513.092458617994,
			"y": -3777.3302453672795,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 89.56576748445045,
			"height": 28.890370479435358,
			"seed": 1410109760,
			"groupIds": [
				"6ivs4qDTMgmRopjH79ZJG",
				"MFnAE4vbecwYH7bCzgUk0",
				"HUiTzNTEp-VgzSFScDh6O",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					43.64176878137867,
					-28.890370479435358
				],
				[
					-45.92399870307177,
					-28.536623396265053
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 2121,
			"versionNonce": 1335704426,
			"isDeleted": false,
			"id": "hFJzH0alL5rv_vE6VAQPD",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dotted",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17659.58794104159,
			"y": -3772.0808748638556,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 115.61120548241641,
			"height": 2.141748890171376,
			"seed": 1592289600,
			"groupIds": [
				"MFnAE4vbecwYH7bCzgUk0",
				"HUiTzNTEp-VgzSFScDh6O",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					115.61120548241641,
					-2.141748890171376
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1931,
			"versionNonce": 1886783542,
			"isDeleted": false,
			"id": "gKMMinNEen_SU6aX2u22d",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17574.638395563554,
			"y": -3806.7733421576368,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 92.00918879029342,
			"height": 61.155808118099465,
			"seed": 1351172416,
			"groupIds": [
				"03bknV4kwvR_M5gdxNDMn",
				"MFnAE4vbecwYH7bCzgUk0",
				"HUiTzNTEp-VgzSFScDh6O",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3252,
			"versionNonce": 2146844202,
			"isDeleted": false,
			"id": "xTZzebInI-Fsoz7ZaQjG8",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17623.150015233947,
			"y": -3778.9404506985775,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 89.56576748445045,
			"height": 28.890370479435358,
			"seed": 139401536,
			"groupIds": [
				"03bknV4kwvR_M5gdxNDMn",
				"MFnAE4vbecwYH7bCzgUk0",
				"HUiTzNTEp-VgzSFScDh6O",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					43.64176878137867,
					-28.890370479435358
				],
				[
					-45.92399870307177,
					-28.536623396265053
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1980,
			"versionNonce": 1345556854,
			"isDeleted": false,
			"id": "xTCKGNG1EGgdjVPyo3-NB",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17772.009234071378,
			"y": -3808.8918126961835,
			"strokeColor": "#000000",
			"backgroundColor": "#868e96",
			"width": 92.00918879029342,
			"height": 61.155808118099465,
			"seed": 2040131904,
			"groupIds": [
				"mfprZ6l68AqLkm7P3NCAY",
				"MFnAE4vbecwYH7bCzgUk0",
				"HUiTzNTEp-VgzSFScDh6O",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3337,
			"versionNonce": 731965674,
			"isDeleted": false,
			"id": "AP3xYrBu9ATV_5vcPgtBR",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17822.378464746864,
			"y": -3782.3766395489474,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 89.56576748445045,
			"height": 28.890370479435358,
			"seed": 734644544,
			"groupIds": [
				"mfprZ6l68AqLkm7P3NCAY",
				"MFnAE4vbecwYH7bCzgUk0",
				"HUiTzNTEp-VgzSFScDh6O",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					43.64176878137867,
					-28.890370479435358
				],
				[
					-45.92399870307177,
					-28.536623396265053
				],
				[
					0,
					0
				]
			]
		},
		{
			"type": "text",
			"version": 1222,
			"versionNonce": 166589110,
			"isDeleted": false,
			"id": "YvDK2xIo",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17509.145526647542,
			"y": -3728.1531826502687,
			"strokeColor": "#000000",
			"backgroundColor": "#ced4da",
			"width": 367.4896240234375,
			"height": 93.28273854239985,
			"seed": 977183040,
			"groupIds": [
				"HUiTzNTEp-VgzSFScDh6O",
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864761,
			"link": null,
			"locked": false,
			"fontSize": 69.09832484622203,
			"fontFamily": 1,
			"text": "Message Q",
			"rawText": "Message Q",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Message Q",
			"lineHeight": 1.3500000000000016,
			"baseline": 64
		},
		{
			"type": "rectangle",
			"version": 474,
			"versionNonce": 1244150698,
			"isDeleted": false,
			"id": "AKNRRyXpdHJ_Vhwy8IkoX",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "dotted",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16492.45127441073,
			"y": -3896.097243873569,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2677.873263888892,
			"height": 280.03472222222223,
			"seed": 1415084352,
			"groupIds": [
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 294,
			"versionNonce": 2018126838,
			"isDeleted": false,
			"id": "vD9s7tCR1OuVO2_TPnRxM",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16311.758442069451,
			"y": -4482.744999799645,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3108.9409722222235,
			"height": 2513.333333333332,
			"seed": 1031229760,
			"groupIds": [
				"NAwv9qjLC37Zy5t4vZfgr"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 194,
			"versionNonce": 699872874,
			"isDeleted": false,
			"id": "xup9WkT2",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17463.596490368607,
			"y": -4691.0783331329785,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 442.6766662597656,
			"height": 158.3333333333326,
			"seed": 1291528512,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 126.66666666666607,
			"fontFamily": 1,
			"text": "Node 3",
			"rawText": "Node 3",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Node 3",
			"lineHeight": 1.25,
			"baseline": 111
		},
		{
			"type": "rectangle",
			"version": 149,
			"versionNonce": 1498234166,
			"isDeleted": false,
			"id": "x7hhmYOo-3X-ffZtdUFxA",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 9889.562261513878,
			"y": -1697.7449997996446,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9490,
			"height": 370,
			"seed": 1996689728,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "uPyQQiz3owVyj3Ib6FMiy",
					"type": "arrow"
				}
			],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 627,
			"versionNonce": 454613290,
			"isDeleted": false,
			"id": "TRIA9BSj",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14010.657131403237,
			"y": -1577.5394566448826,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 799.4454956054688,
			"height": 139.58891369047626,
			"seed": 1023691456,
			"groupIds": [
				"hCZJUY_7czPPwudVVOAPk",
				"4C-3RPDE3Rmlj48HbY3gI"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 111.671130952381,
			"fontFamily": 1,
			"text": "Load Balancer",
			"rawText": "Load Balancer",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Load Balancer",
			"lineHeight": 1.25,
			"baseline": 98
		},
		{
			"type": "rectangle",
			"version": 416,
			"versionNonce": 1650206326,
			"isDeleted": false,
			"id": "t1aGDK1r_lSxPEbiCgJgx",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14200.30676388349,
			"y": -397.66807498834305,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 717.1428571428571,
			"height": 488.57142857142844,
			"seed": 1418091200,
			"groupIds": [
				"3BZ7OvroRXq-qmI7UIvnl"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "uPyQQiz3owVyj3Ib6FMiy",
					"type": "arrow"
				}
			],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 471,
			"versionNonce": 498607082,
			"isDeleted": false,
			"id": "nBDHhpFh",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14393.98101852797,
			"y": -235.001408321677,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 307.58551025390625,
			"height": 142.14285714285697,
			"seed": 275579584,
			"groupIds": [
				"3BZ7OvroRXq-qmI7UIvnl"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 113.71428571428558,
			"fontFamily": 1,
			"text": "Client",
			"rawText": "Client",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Client",
			"lineHeight": 1.25,
			"baseline": 100
		},
		{
			"type": "arrow",
			"version": 752,
			"versionNonce": 1413212086,
			"isDeleted": false,
			"id": "uPyQQiz3owVyj3Ib6FMiy",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14514.970796661271,
			"y": -405.94462170887266,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 4.479367731057209,
			"height": 904.3333333333338,
			"seed": 804229440,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "t1aGDK1r_lSxPEbiCgJgx",
				"focus": -0.12551069618116759,
				"gap": 8.276546720529609
			},
			"endBinding": {
				"elementId": "x7hhmYOo-3X-ffZtdUFxA",
				"focus": 0.02404366694906816,
				"gap": 17.46704475743809
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					4.479367731057209,
					-904.3333333333338
				]
			]
		},
		{
			"type": "arrow",
			"version": 122,
			"versionNonce": 195040938,
			"isDeleted": false,
			"id": "5oHrhgJC9peDropuabaZt",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 14504.21152578825,
			"y": -5656.382360702624,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10,
			"height": 649.9999999999991,
			"seed": 494143808,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					10,
					649.9999999999991
				]
			]
		},
		{
			"type": "rectangle",
			"version": 195,
			"versionNonce": 252805366,
			"isDeleted": false,
			"id": "-QF24UIwbh_dJnGSUdCiS",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 9564.21152578825,
			"y": -6626.382360702624,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10099.999999999996,
			"height": 6969.999999999998,
			"seed": 719069888,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 213,
			"versionNonce": 1165734250,
			"isDeleted": false,
			"id": "cz06hPKv5RvSCvCAqjDli",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16264.80604238277,
			"y": -6497.118291438557,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 640.0000000000001,
			"height": 419.99999999999994,
			"seed": 1369049792,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 140,
			"versionNonce": 643953206,
			"isDeleted": false,
			"id": "MPU3Xob2",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16335.050076196247,
			"y": -6352.118291438557,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 465.52789306640625,
			"height": 105.0000000000004,
			"seed": 788232512,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 84.00000000000031,
			"fontFamily": 1,
			"text": "Prometheus",
			"rawText": "Prometheus",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Prometheus",
			"lineHeight": 1.25,
			"baseline": 74
		},
		{
			"type": "rectangle",
			"version": 256,
			"versionNonce": 1586885674,
			"isDeleted": false,
			"id": "4yU3spYCR3bX9zlQXufQl",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16994.80604238277,
			"y": -6487.118291438557,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 640.0000000000001,
			"height": 419.99999999999994,
			"seed": 1747763520,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 191,
			"versionNonce": 1964129142,
			"isDeleted": false,
			"id": "17YQdwAx",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 17122.5480060872,
			"y": -6342.118291438557,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 350.531982421875,
			"height": 105.0000000000004,
			"seed": 1602394432,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 84.00000000000031,
			"fontFamily": 1,
			"text": "Grafana",
			"rawText": "Grafana",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Grafana",
			"lineHeight": 1.25,
			"baseline": 74
		},
		{
			"type": "text",
			"version": 2036,
			"versionNonce": 1222237930,
			"isDeleted": false,
			"id": "wUi4m7JH",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 19919.62014177342,
			"y": -6527.730002211727,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6251.6201171875,
			"height": 1453.0585538658493,
			"seed": 1444057792,
			"groupIds": [
				"NxBENxYP6al99RN3QyAJx"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 232.48936861853588,
			"fontFamily": 1,
			"text": "Notes:\n- The monitoring may need its own node\n- Need to do stress testings\nlearning about generating fake users because we cant\nget real users",
			"rawText": "Notes:\n- The monitoring may need its own node\n- Need to do stress testings\nlearning about generating fake users because we cant\nget real users",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Notes:\n- The monitoring may need its own node\n- Need to do stress testings\nlearning about generating fake users because we cant\nget real users",
			"lineHeight": 1.25,
			"baseline": 1366
		},
		{
			"type": "arrow",
			"version": 181,
			"versionNonce": 828857526,
			"isDeleted": false,
			"id": "db92jeTka_Gq8rdxXr3oi",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "dashed",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 8027.990025066748,
			"y": -4024.2546550749253,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.8181818181819835,
			"height": 603.636363636364,
			"seed": 148625728,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "4LV1X0NuglGE98UHmXJ3W",
				"focus": -0.036440836721583394,
				"gap": 26.105892848082476
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": "arrow",
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					1.8181818181819835,
					603.636363636364
				]
			]
		},
		{
			"type": "image",
			"version": 151,
			"versionNonce": 13791658,
			"isDeleted": false,
			"id": "y_ENWygqSY0JrFCK204YW",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "dashed",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": -961.8351091687928,
			"y": -11507.899875089935,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"width": 10086,
			"height": 5892.076530612245,
			"seed": 582779155,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "11df65c7024920ac84ab4c2c6d08d0f77dbecc76",
			"scale": [
				1,
				1
			]
		},
		{
			"type": "rectangle",
			"version": 138,
			"versionNonce": 17192438,
			"isDeleted": false,
			"id": "rJETB-58611eVkAsMaWfy",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 439.9819481228742,
			"y": -2636.4623750899345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 610,
			"height": 225,
			"seed": 54777560,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "E8pbnPqDepWhBQG0caAB9",
					"type": "arrow"
				},
				{
					"id": "FFpDjztJ9szWe31O0tGQC",
					"type": "arrow"
				}
			],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 91,
			"versionNonce": 967486570,
			"isDeleted": false,
			"id": "eQLaOYMI",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 677.4819481228742,
			"y": -2538.9623750899345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 152.4599609375,
			"height": 45,
			"seed": 1436839592,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "PHP API",
			"rawText": "PHP API",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "PHP API",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 99,
			"versionNonce": 217327414,
			"isDeleted": false,
			"id": "E8pbnPqDepWhBQG0caAB9",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 884.9819481228741,
			"y": -2636.4623750899345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 330.0000000000001,
			"height": 155,
			"seed": 1739344088,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "rJETB-58611eVkAsMaWfy",
				"focus": -0.18276066350710932,
				"gap": 1
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": "arrow",
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					330.0000000000001,
					-155
				]
			]
		},
		{
			"type": "arrow",
			"version": 170,
			"versionNonce": 153980714,
			"isDeleted": false,
			"id": "FFpDjztJ9szWe31O0tGQC",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 742.491831721979,
			"y": -2396.4623750899345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.0179079231314745,
			"height": 227.5,
			"seed": 1252769704,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "rJETB-58611eVkAsMaWfy",
				"gap": 15,
				"focus": 0.017244460328806666
			},
			"endBinding": {
				"elementId": "NrdEyiABJNek_rzfwKNIA",
				"gap": 5,
				"focus": 0.07063562235975987
			},
			"lastCommittedPoint": null,
			"startArrowhead": "arrow",
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					5.0179079231314745,
					227.5
				]
			]
		},
		{
			"type": "rectangle",
			"version": 119,
			"versionNonce": 362139766,
			"isDeleted": false,
			"id": "NrdEyiABJNek_rzfwKNIA",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 451.9819481228742,
			"y": -2163.9623750899345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 556,
			"height": 195,
			"seed": 202931160,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "FFpDjztJ9szWe31O0tGQC",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "oi0DrioS"
				}
			],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 83,
			"versionNonce": 331749866,
			"isDeleted": false,
			"id": "oi0DrioS",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 681.0399544094953,
			"y": -2088.9623750899345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 97.88398742675781,
			"height": 45,
			"seed": 344517288,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "HTMX",
			"rawText": "HTMX",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "NrdEyiABJNek_rzfwKNIA",
			"originalText": "HTMX",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 85,
			"versionNonce": 112218550,
			"isDeleted": false,
			"id": "bpe6n3hqwHW9z9fFq2dXq",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": -1253.6847185437928,
			"y": 2891.5376249100646,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3370,
			"height": 530,
			"seed": 304177770,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 103,
			"versionNonce": 947866794,
			"isDeleted": false,
			"id": "i-aUEmhjSN9-g0_XN0YoX",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 1066.934329075255,
			"y": 2866.299529671969,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 1036,
			"height": 560,
			"seed": 1875616630,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 91,
			"versionNonce": 191408886,
			"isDeleted": false,
			"id": "1xqTt0a9",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 1234.934329075255,
			"y": 3050.299529671969,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 757.5,
			"height": 125.0000000000002,
			"seed": 1618269878,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 100.00000000000016,
			"fontFamily": 1,
			"text": "Sequence# Size",
			"rawText": "Sequence# Size",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Sequence# Size",
			"lineHeight": 1.25,
			"baseline": 88
		},
		{
			"type": "text",
			"version": 135,
			"versionNonce": 1023682410,
			"isDeleted": false,
			"id": "T7lvSFzv",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": -251.81551833685535,
			"y": 3111.799529671969,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 267.8999938964844,
			"height": 125.0000000000002,
			"seed": 2122352758,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 100.00000000000016,
			"fontFamily": 1,
			"text": "Data",
			"rawText": "Data",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Data",
			"lineHeight": 1.25,
			"baseline": 88
		},
		{
			"type": "freedraw",
			"version": 86,
			"versionNonce": 574872630,
			"isDeleted": false,
			"id": "wEexOPaDgI2MyTLarkb7b",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 2175.934329075256,
			"y": 3109.966196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 1275,
			"height": 885,
			"seed": 57840682,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					10,
					0
				],
				[
					35,
					0
				],
				[
					65,
					-5
				],
				[
					115,
					-10
				],
				[
					175,
					-15
				],
				[
					240,
					-15
				],
				[
					310,
					-15
				],
				[
					380,
					-15
				],
				[
					445,
					-15
				],
				[
					510,
					-5
				],
				[
					570,
					0
				],
				[
					630,
					15
				],
				[
					685,
					30
				],
				[
					740,
					45
				],
				[
					790,
					60
				],
				[
					840,
					75
				],
				[
					885,
					95
				],
				[
					925,
					115
				],
				[
					970,
					135
				],
				[
					1010,
					160
				],
				[
					1050,
					185
				],
				[
					1085,
					215
				],
				[
					1115,
					245
				],
				[
					1140,
					280
				],
				[
					1170,
					320
				],
				[
					1195,
					350
				],
				[
					1210,
					380
				],
				[
					1220,
					410
				],
				[
					1235,
					445
				],
				[
					1245,
					480
				],
				[
					1255,
					525
				],
				[
					1260,
					580
				],
				[
					1265,
					625
				],
				[
					1270,
					675
				],
				[
					1270,
					715
				],
				[
					1275,
					755
				],
				[
					1275,
					800
				],
				[
					1275,
					840
				],
				[
					1275,
					860
				],
				[
					1275,
					870
				],
				[
					1275,
					870
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 61,
			"versionNonce": 2040506922,
			"isDeleted": false,
			"id": "p73lxCjrmjSHL_eofQAqq",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 3300.934329075256,
			"y": 3964.966196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 220,
			"height": 185,
			"seed": 295470518,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					0
				],
				[
					10,
					0
				],
				[
					30,
					25
				],
				[
					50,
					55
				],
				[
					65,
					75
				],
				[
					70,
					85
				],
				[
					80,
					85
				],
				[
					90,
					90
				],
				[
					105,
					90
				],
				[
					130,
					85
				],
				[
					160,
					60
				],
				[
					190,
					20
				],
				[
					215,
					-20
				],
				[
					220,
					-70
				],
				[
					220,
					-95
				],
				[
					220,
					-95
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "rectangle",
			"version": 77,
			"versionNonce": 824632694,
			"isDeleted": false,
			"id": "v3EGQU6-1KLyGs7XWjAO_",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 3045.934329075256,
			"y": 4214.966196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 985,
			"height": 725,
			"seed": 1573357814,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 114,
			"versionNonce": 87872746,
			"isDeleted": false,
			"id": "H0GPAiPb",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 3235.934329075256,
			"y": 4434.966196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 567.6399536132812,
			"height": 230.0000000000003,
			"seed": 1345689462,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 184.00000000000026,
			"fontFamily": 1,
			"text": "Server",
			"rawText": "Server",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Server",
			"lineHeight": 1.25,
			"baseline": 162
		},
		{
			"type": "freedraw",
			"version": 160,
			"versionNonce": 425117366,
			"isDeleted": false,
			"id": "bdNCzcjmSTscRqXjSXCT1",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 3610.934329075256,
			"y": 5109.966196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1780,
			"height": 1020,
			"seed": 251415222,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					5
				],
				[
					0,
					20
				],
				[
					-5,
					35
				],
				[
					-10,
					55
				],
				[
					-15,
					70
				],
				[
					-20,
					85
				],
				[
					-20,
					95
				],
				[
					-25,
					110
				],
				[
					-25,
					125
				],
				[
					-30,
					140
				],
				[
					-35,
					160
				],
				[
					-40,
					175
				],
				[
					-40,
					185
				],
				[
					-45,
					200
				],
				[
					-55,
					220
				],
				[
					-60,
					240
				],
				[
					-65,
					255
				],
				[
					-70,
					265
				],
				[
					-80,
					275
				],
				[
					-80,
					285
				],
				[
					-85,
					295
				],
				[
					-90,
					305
				],
				[
					-95,
					315
				],
				[
					-100,
					325
				],
				[
					-105,
					335
				],
				[
					-110,
					340
				],
				[
					-115,
					350
				],
				[
					-120,
					360
				],
				[
					-125,
					375
				],
				[
					-135,
					385
				],
				[
					-140,
					395
				],
				[
					-150,
					405
				],
				[
					-160,
					420
				],
				[
					-165,
					430
				],
				[
					-180,
					445
				],
				[
					-190,
					460
				],
				[
					-205,
					470
				],
				[
					-220,
					490
				],
				[
					-235,
					505
				],
				[
					-255,
					515
				],
				[
					-275,
					530
				],
				[
					-295,
					545
				],
				[
					-315,
					555
				],
				[
					-335,
					570
				],
				[
					-365,
					575
				],
				[
					-390,
					590
				],
				[
					-415,
					595
				],
				[
					-435,
					605
				],
				[
					-460,
					610
				],
				[
					-490,
					615
				],
				[
					-520,
					615
				],
				[
					-555,
					625
				],
				[
					-590,
					625
				],
				[
					-625,
					630
				],
				[
					-655,
					630
				],
				[
					-685,
					630
				],
				[
					-710,
					635
				],
				[
					-745,
					635
				],
				[
					-770,
					635
				],
				[
					-800,
					635
				],
				[
					-830,
					635
				],
				[
					-855,
					635
				],
				[
					-880,
					635
				],
				[
					-910,
					630
				],
				[
					-940,
					625
				],
				[
					-975,
					615
				],
				[
					-1010,
					610
				],
				[
					-1035,
					600
				],
				[
					-1070,
					590
				],
				[
					-1095,
					580
				],
				[
					-1120,
					570
				],
				[
					-1145,
					560
				],
				[
					-1170,
					550
				],
				[
					-1190,
					535
				],
				[
					-1215,
					520
				],
				[
					-1240,
					500
				],
				[
					-1265,
					480
				],
				[
					-1300,
					450
				],
				[
					-1325,
					430
				],
				[
					-1350,
					405
				],
				[
					-1370,
					390
				],
				[
					-1390,
					375
				],
				[
					-1410,
					355
				],
				[
					-1430,
					335
				],
				[
					-1450,
					310
				],
				[
					-1475,
					285
				],
				[
					-1495,
					260
				],
				[
					-1510,
					240
				],
				[
					-1525,
					215
				],
				[
					-1540,
					190
				],
				[
					-1550,
					165
				],
				[
					-1565,
					135
				],
				[
					-1575,
					100
				],
				[
					-1590,
					60
				],
				[
					-1600,
					25
				],
				[
					-1610,
					-5
				],
				[
					-1625,
					-40
				],
				[
					-1630,
					-65
				],
				[
					-1645,
					-90
				],
				[
					-1655,
					-120
				],
				[
					-1670,
					-150
				],
				[
					-1680,
					-175
				],
				[
					-1695,
					-200
				],
				[
					-1705,
					-225
				],
				[
					-1715,
					-245
				],
				[
					-1730,
					-265
				],
				[
					-1740,
					-290
				],
				[
					-1750,
					-310
				],
				[
					-1760,
					-330
				],
				[
					-1770,
					-345
				],
				[
					-1775,
					-360
				],
				[
					-1775,
					-375
				],
				[
					-1780,
					-380
				],
				[
					-1780,
					-385
				],
				[
					-1780,
					-385
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 55,
			"versionNonce": 1634117546,
			"isDeleted": false,
			"id": "UBgLENRywUl8wmoCpF4ML",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 1760.9343290752558,
			"y": 4649.966196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 25,
			"height": 230,
			"seed": 180157226,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					5
				],
				[
					0,
					25
				],
				[
					0,
					55
				],
				[
					0,
					95
				],
				[
					-5,
					140
				],
				[
					-10,
					180
				],
				[
					-20,
					215
				],
				[
					-25,
					230
				],
				[
					-20,
					215
				],
				[
					-20,
					215
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 54,
			"versionNonce": 1266188278,
			"isDeleted": false,
			"id": "dkkiRedb9Fgwa-IKxRHFR",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 1770.9343290752558,
			"y": 4674.966196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 240,
			"height": 160,
			"seed": 58004394,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					10,
					0
				],
				[
					40,
					10
				],
				[
					75,
					40
				],
				[
					120,
					75
				],
				[
					165,
					115
				],
				[
					205,
					140
				],
				[
					230,
					155
				],
				[
					240,
					160
				],
				[
					240,
					160
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "rectangle",
			"version": 126,
			"versionNonce": 642261610,
			"isDeleted": false,
			"id": "BiI1lS0YWAvC4uFumzE5n",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 1153.4343290752558,
			"y": 3927.466196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 985,
			"height": 725,
			"seed": 938679594,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 170,
			"versionNonce": 1536233782,
			"isDeleted": false,
			"id": "p68I1q0u",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 1343.4343290752558,
			"y": 4147.466196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 497.7199401855469,
			"height": 230.0000000000003,
			"seed": 782886890,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 184.00000000000026,
			"fontFamily": 1,
			"text": "Client",
			"rawText": "Client",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Client",
			"lineHeight": 1.25,
			"baseline": 162
		},
		{
			"type": "rectangle",
			"version": 131,
			"versionNonce": 783041834,
			"isDeleted": false,
			"id": "gOEmeqTAJozPPRG5rLn_z",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 1425.9343290752558,
			"y": 6160.2042915767315,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3370,
			"height": 530,
			"seed": 2121237482,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 149,
			"versionNonce": 352680566,
			"isDeleted": false,
			"id": "ZHYS1TmDuNTvY3kqkF1EI",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 3746.5533766943036,
			"y": 6134.966196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 1036,
			"height": 560,
			"seed": 510359210,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 145,
			"versionNonce": 1140723690,
			"isDeleted": false,
			"id": "t1VTM3Xb",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 3914.5533766943036,
			"y": 6358.966196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 757.5,
			"height": 125.0000000000002,
			"seed": 668668266,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 100.00000000000016,
			"fontFamily": 1,
			"text": "Sequence# Size",
			"rawText": "Sequence# Size",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Sequence# Size",
			"lineHeight": 1.25,
			"baseline": 88
		},
		{
			"type": "text",
			"version": 186,
			"versionNonce": 245021622,
			"isDeleted": false,
			"id": "XfSMdPb1",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 2452.8035292821933,
			"y": 6375.466196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffc9c9",
			"width": 267.8999938964844,
			"height": 125.0000000000002,
			"seed": 2114540586,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 100.00000000000016,
			"fontFamily": 1,
			"text": "Data",
			"rawText": "Data",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Data",
			"lineHeight": 1.25,
			"baseline": 88
		},
		{
			"type": "text",
			"version": 199,
			"versionNonce": 1246266026,
			"isDeleted": false,
			"id": "F1g48v1F",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": -439.06567092474415,
			"y": 5442.466196338636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 844.3436889648438,
			"height": 180,
			"seed": 886291690,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "register => [seq#, size, size]\nget(servize_a) => [seq#, sizeSent, size, data]\ndelete => [seq#, sizeSent, size, data]\nupdate => [seq#, sizeSent, size]",
			"rawText": "register => [seq#, size, size]\nget(servize_a) => [seq#, sizeSent, size, data]\ndelete => [seq#, sizeSent, size, data]\nupdate => [seq#, sizeSent, size]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "register => [seq#, size, size]\nget(servize_a) => [seq#, sizeSent, size, data]\ndelete => [seq#, sizeSent, size, data]\nupdate => [seq#, sizeSent, size]",
			"lineHeight": 1.25,
			"baseline": 167
		},
		{
			"id": "UP4qepkknuw2L5OeLxTwr",
			"type": "freedraw",
			"x": 1492.981948122874,
			"y": -1647.0225279365459,
			"width": 4445,
			"height": 1310,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 554031658,
			"version": 222,
			"versionNonce": 239787562,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5,
					0
				],
				[
					-10,
					0
				],
				[
					-35,
					0
				],
				[
					-70,
					0
				],
				[
					-125,
					0
				],
				[
					-195,
					0
				],
				[
					-270,
					0
				],
				[
					-345,
					0
				],
				[
					-410,
					5
				],
				[
					-460,
					15
				],
				[
					-500,
					30
				],
				[
					-545,
					45
				],
				[
					-585,
					65
				],
				[
					-635,
					85
				],
				[
					-685,
					105
				],
				[
					-720,
					125
				],
				[
					-750,
					145
				],
				[
					-765,
					165
				],
				[
					-780,
					190
				],
				[
					-785,
					210
				],
				[
					-790,
					230
				],
				[
					-795,
					255
				],
				[
					-795,
					280
				],
				[
					-795,
					305
				],
				[
					-790,
					325
				],
				[
					-785,
					345
				],
				[
					-780,
					355
				],
				[
					-765,
					370
				],
				[
					-745,
					385
				],
				[
					-705,
					405
				],
				[
					-665,
					420
				],
				[
					-615,
					435
				],
				[
					-560,
					455
				],
				[
					-495,
					465
				],
				[
					-420,
					480
				],
				[
					-320,
					490
				],
				[
					-210,
					500
				],
				[
					-105,
					500
				],
				[
					5,
					510
				],
				[
					105,
					510
				],
				[
					210,
					510
				],
				[
					320,
					515
				],
				[
					440,
					520
				],
				[
					550,
					520
				],
				[
					670.0000000000002,
					520
				],
				[
					790.0000000000002,
					520
				],
				[
					895.0000000000002,
					520
				],
				[
					995.0000000000002,
					520
				],
				[
					1095.0000000000002,
					520
				],
				[
					1195.0000000000002,
					520
				],
				[
					1295.0000000000002,
					520
				],
				[
					1390.0000000000002,
					515
				],
				[
					1465.0000000000002,
					510
				],
				[
					1530.0000000000002,
					505
				],
				[
					1595.0000000000002,
					500
				],
				[
					1645.0000000000002,
					495
				],
				[
					1705.0000000000002,
					495
				],
				[
					1765.0000000000002,
					495
				],
				[
					1825.0000000000002,
					490
				],
				[
					1895.0000000000002,
					485
				],
				[
					1965.0000000000002,
					480
				],
				[
					2040.0000000000002,
					470
				],
				[
					2120,
					465
				],
				[
					2200,
					460
				],
				[
					2280,
					455
				],
				[
					2355,
					450
				],
				[
					2425,
					440
				],
				[
					2475,
					430
				],
				[
					2510,
					425
				],
				[
					2550,
					415
				],
				[
					2590,
					405
				],
				[
					2645,
					395
				],
				[
					2705,
					385
				],
				[
					2755,
					375
				],
				[
					2795,
					360
				],
				[
					2835,
					345
				],
				[
					2880,
					335
				],
				[
					2940,
					315
				],
				[
					3010,
					295
				],
				[
					3085,
					275
				],
				[
					3145,
					250
				],
				[
					3205,
					225
				],
				[
					3245,
					210
				],
				[
					3295,
					190
				],
				[
					3345,
					165
				],
				[
					3400,
					135
				],
				[
					3455,
					100
				],
				[
					3505,
					65
				],
				[
					3535,
					35
				],
				[
					3560,
					0
				],
				[
					3585,
					-40
				],
				[
					3605,
					-85
				],
				[
					3620,
					-130
				],
				[
					3635,
					-175
				],
				[
					3645,
					-220
				],
				[
					3650,
					-255
				],
				[
					3650,
					-290
				],
				[
					3650,
					-330
				],
				[
					3650,
					-370
				],
				[
					3650,
					-410
				],
				[
					3630,
					-455
				],
				[
					3605,
					-490
				],
				[
					3580,
					-520
				],
				[
					3555,
					-545
				],
				[
					3530,
					-570
				],
				[
					3495,
					-595
				],
				[
					3450,
					-630
				],
				[
					3400,
					-655
				],
				[
					3360,
					-680
				],
				[
					3325,
					-700
				],
				[
					3290,
					-720
				],
				[
					3250,
					-735
				],
				[
					3205,
					-755
				],
				[
					3160,
					-765
				],
				[
					3110,
					-775
				],
				[
					3055,
					-780
				],
				[
					2995,
					-785
				],
				[
					2940,
					-790
				],
				[
					2890,
					-790
				],
				[
					2845,
					-785
				],
				[
					2800,
					-775
				],
				[
					2745,
					-755
				],
				[
					2685,
					-735
				],
				[
					2620,
					-710
				],
				[
					2560,
					-675
				],
				[
					2505,
					-640
				],
				[
					2460,
					-605
				],
				[
					2400,
					-560
				],
				[
					2340,
					-515
				],
				[
					2290,
					-475
				],
				[
					2230,
					-425
				],
				[
					2170,
					-385
				],
				[
					2120,
					-340
				],
				[
					2070,
					-305
				],
				[
					2015.0000000000002,
					-270
				],
				[
					1960.0000000000002,
					-240
				],
				[
					1905.0000000000002,
					-215
				],
				[
					1850.0000000000002,
					-185
				],
				[
					1780.0000000000002,
					-160
				],
				[
					1710.0000000000002,
					-140
				],
				[
					1635.0000000000002,
					-120
				],
				[
					1570.0000000000002,
					-110
				],
				[
					1505.0000000000002,
					-95
				],
				[
					1425.0000000000002,
					-75
				],
				[
					1345.0000000000002,
					-70
				],
				[
					1265.0000000000002,
					-60
				],
				[
					1185.0000000000002,
					-50
				],
				[
					1115.0000000000002,
					-40
				],
				[
					1050.0000000000002,
					-35
				],
				[
					985.0000000000002,
					-30
				],
				[
					915.0000000000002,
					-20
				],
				[
					845.0000000000002,
					-20
				],
				[
					780.0000000000002,
					-20
				],
				[
					725.0000000000002,
					-20
				],
				[
					685.0000000000002,
					-20
				],
				[
					640.0000000000002,
					-20
				],
				[
					595.0000000000002,
					-20
				],
				[
					555,
					-15
				],
				[
					505,
					-15
				],
				[
					460,
					-15
				],
				[
					425,
					-15
				],
				[
					390,
					-15
				],
				[
					360,
					-15
				],
				[
					330,
					-10
				],
				[
					290,
					-5
				],
				[
					245,
					0
				],
				[
					205,
					5
				],
				[
					170,
					5
				],
				[
					145,
					5
				],
				[
					120,
					10
				],
				[
					105,
					10
				],
				[
					95,
					10
				],
				[
					85,
					10
				],
				[
					80,
					10
				],
				[
					70,
					10
				],
				[
					65,
					10
				],
				[
					50,
					10
				],
				[
					40,
					10
				],
				[
					25,
					10
				],
				[
					5,
					10
				],
				[
					-15,
					10
				],
				[
					-40,
					10
				],
				[
					-70,
					10
				],
				[
					-95,
					10
				],
				[
					-100,
					10
				],
				[
					-100,
					10
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-100,
				10
			]
		},
		{
			"type": "freedraw",
			"version": 46,
			"versionNonce": 1996026230,
			"isDeleted": true,
			"id": "_Fy-rmTLPrHQ3_xfFVl88",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 4407.981948122874,
			"y": -2742.022527936546,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 70,
			"height": 280,
			"seed": 104458230,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					0
				],
				[
					25,
					15
				],
				[
					45,
					55
				],
				[
					60,
					105
				],
				[
					70,
					150
				],
				[
					70,
					200
				],
				[
					70,
					245
				],
				[
					70,
					275
				],
				[
					70,
					280
				],
				[
					70,
					280
				]
			],
			"lastCommittedPoint": [
				70,
				280
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 49,
			"versionNonce": 1180797162,
			"isDeleted": true,
			"id": "c6p1Z5XGrPKFQtjBZgBMx",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 4367.981948122874,
			"y": -2547.022527936546,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 195,
			"height": 175,
			"seed": 319092598,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					0
				],
				[
					10,
					5
				],
				[
					50,
					40
				],
				[
					90,
					90
				],
				[
					130,
					135
				],
				[
					160,
					160
				],
				[
					165,
					160
				],
				[
					175,
					160
				],
				[
					180,
					130
				],
				[
					180,
					85
				],
				[
					185,
					30
				],
				[
					195,
					-10
				],
				[
					195,
					-15
				],
				[
					195,
					-15
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"id": "cLVuTn2hcBFiAFERPM99u",
			"type": "freedraw",
			"x": 3132.981948122874,
			"y": -1927.0225279365459,
			"width": 10,
			"height": 280,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 553459830,
			"version": 44,
			"versionNonce": 1896305334,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					35
				],
				[
					0,
					85
				],
				[
					0,
					140
				],
				[
					0,
					190
				],
				[
					0,
					225
				],
				[
					-5,
					255
				],
				[
					-5,
					270
				],
				[
					-10,
					280
				],
				[
					-10,
					280
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-10,
				280
			]
		},
		{
			"id": "d9j-Tya6Z9JN1sUB0ZZkl",
			"type": "freedraw",
			"x": 3067.981948122874,
			"y": -1932.0225279365459,
			"width": 235,
			"height": 165,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 256792490,
			"version": 51,
			"versionNonce": 64281514,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					5
				],
				[
					-5,
					20
				],
				[
					-15,
					45
				],
				[
					-20,
					65
				],
				[
					-20,
					75
				],
				[
					0,
					75
				],
				[
					45,
					55
				],
				[
					95,
					5
				],
				[
					125,
					-25
				],
				[
					140,
					-40
				],
				[
					155,
					-30
				],
				[
					175,
					10
				],
				[
					190,
					60
				],
				[
					205,
					100
				],
				[
					215,
					120
				],
				[
					215,
					125
				],
				[
					215,
					125
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				215,
				125
			]
		},
		{
			"id": "NrR3kTnARKJlJzULUDzNm",
			"type": "freedraw",
			"x": 1697.981948122874,
			"y": -1912.0225279365459,
			"width": 85,
			"height": 255,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 882199350,
			"version": 41,
			"versionNonce": 1966574582,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					0
				],
				[
					20,
					30
				],
				[
					40,
					90
				],
				[
					65,
					165
				],
				[
					80,
					215
				],
				[
					85,
					245
				],
				[
					85,
					255
				],
				[
					85,
					255
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				85,
				255
			]
		},
		{
			"id": "-rhtLDpVz9tS9bEvwQq18",
			"type": "freedraw",
			"x": 1582.981948122874,
			"y": -1932.0225279365459,
			"width": 260,
			"height": 175,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 999393654,
			"version": 53,
			"versionNonce": 1154471530,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					5
				],
				[
					0,
					15
				],
				[
					0,
					55
				],
				[
					-10,
					100
				],
				[
					-25,
					140
				],
				[
					-30,
					150
				],
				[
					-35,
					150
				],
				[
					-30,
					125
				],
				[
					-15,
					80
				],
				[
					5,
					25
				],
				[
					30,
					-10
				],
				[
					55,
					-25
				],
				[
					70,
					-25
				],
				[
					105,
					-15
				],
				[
					135,
					20
				],
				[
					165,
					45
				],
				[
					190,
					70
				],
				[
					210,
					80
				],
				[
					220,
					85
				],
				[
					225,
					90
				],
				[
					225,
					90
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				225,
				90
			]
		},
		{
			"id": "NM46rj91nVC8F0FpZwOii",
			"type": "freedraw",
			"x": 2952.981948122874,
			"y": -1657.0225279365459,
			"width": 4555,
			"height": 1560,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 351209398,
			"version": 192,
			"versionNonce": 294559030,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-10,
					0
				],
				[
					-55,
					-5
				],
				[
					-140,
					-15
				],
				[
					-290,
					-30
				],
				[
					-495,
					-45
				],
				[
					-725,
					-50
				],
				[
					-980.0000000000002,
					-60
				],
				[
					-1205.0000000000002,
					-60
				],
				[
					-1415.0000000000002,
					-60
				],
				[
					-1590.0000000000002,
					-50
				],
				[
					-1725.0000000000002,
					-40
				],
				[
					-1820.0000000000002,
					-25
				],
				[
					-1905.0000000000002,
					-15
				],
				[
					-1975.0000000000002,
					-5
				],
				[
					-2040.0000000000002,
					5
				],
				[
					-2095,
					15
				],
				[
					-2140,
					20
				],
				[
					-2180,
					30
				],
				[
					-2220,
					45
				],
				[
					-2250,
					55
				],
				[
					-2270,
					70
				],
				[
					-2300,
					85
				],
				[
					-2320,
					95
				],
				[
					-2335,
					110
				],
				[
					-2355,
					125
				],
				[
					-2365,
					140
				],
				[
					-2370,
					160
				],
				[
					-2370,
					180
				],
				[
					-2370,
					195
				],
				[
					-2375,
					215
				],
				[
					-2380,
					235
				],
				[
					-2385,
					270
				],
				[
					-2390,
					305
				],
				[
					-2385,
					340
				],
				[
					-2355,
					370
				],
				[
					-2315,
					400
				],
				[
					-2260,
					430
				],
				[
					-2170,
					470
				],
				[
					-2050,
					510
				],
				[
					-1905.0000000000002,
					540
				],
				[
					-1730.0000000000002,
					565
				],
				[
					-1540.0000000000002,
					585
				],
				[
					-1340.0000000000002,
					590
				],
				[
					-1095.0000000000002,
					595
				],
				[
					-840,
					600
				],
				[
					-590,
					600
				],
				[
					-340,
					600
				],
				[
					-115,
					600
				],
				[
					70,
					600
				],
				[
					245,
					600
				],
				[
					405,
					600
				],
				[
					555,
					600
				],
				[
					720,
					605
				],
				[
					885,
					605
				],
				[
					1040,
					605
				],
				[
					1200,
					595
				],
				[
					1340,
					585
				],
				[
					1455,
					575
				],
				[
					1565,
					560
				],
				[
					1655,
					550
				],
				[
					1730,
					540
				],
				[
					1805,
					520
				],
				[
					1870,
					490
				],
				[
					1925,
					455
				],
				[
					1965,
					410
				],
				[
					2000,
					355
				],
				[
					2035,
					285
				],
				[
					2080,
					185
				],
				[
					2120,
					65
				],
				[
					2140,
					-55
				],
				[
					2150,
					-170
				],
				[
					2155,
					-285
				],
				[
					2165,
					-385
				],
				[
					2165,
					-465
				],
				[
					2165,
					-535
				],
				[
					2165,
					-585
				],
				[
					2160,
					-635
				],
				[
					2150,
					-675
				],
				[
					2140,
					-710
				],
				[
					2130,
					-745
				],
				[
					2115,
					-785
				],
				[
					2100,
					-825
				],
				[
					2080,
					-860
				],
				[
					2055,
					-885
				],
				[
					2040,
					-905
				],
				[
					2035,
					-910
				],
				[
					2030,
					-910
				],
				[
					2015,
					-910
				],
				[
					1995,
					-915
				],
				[
					1970,
					-915
				],
				[
					1920,
					-925
				],
				[
					1855,
					-930
				],
				[
					1780,
					-940
				],
				[
					1700,
					-950
				],
				[
					1615,
					-955
				],
				[
					1555,
					-955
				],
				[
					1495,
					-955
				],
				[
					1445,
					-950
				],
				[
					1395,
					-935
				],
				[
					1350,
					-925
				],
				[
					1305,
					-905
				],
				[
					1265,
					-880
				],
				[
					1230,
					-850
				],
				[
					1205,
					-810
				],
				[
					1190,
					-755
				],
				[
					1175,
					-695
				],
				[
					1175,
					-635
				],
				[
					1170,
					-585
				],
				[
					1160,
					-530
				],
				[
					1160,
					-485
				],
				[
					1155,
					-435
				],
				[
					1150,
					-390
				],
				[
					1145,
					-355
				],
				[
					1135,
					-315
				],
				[
					1115,
					-285
				],
				[
					1095,
					-255
				],
				[
					1065,
					-225
				],
				[
					1025,
					-195
				],
				[
					985,
					-170
				],
				[
					935,
					-145
				],
				[
					885,
					-115
				],
				[
					835,
					-85
				],
				[
					780,
					-60
				],
				[
					720,
					-35
				],
				[
					660,
					-20
				],
				[
					595,
					-5
				],
				[
					525,
					5
				],
				[
					460,
					15
				],
				[
					390,
					25
				],
				[
					315,
					40
				],
				[
					250,
					50
				],
				[
					185,
					60
				],
				[
					120,
					65
				],
				[
					60,
					65
				],
				[
					10,
					65
				],
				[
					-25,
					65
				],
				[
					-50,
					65
				],
				[
					-60,
					65
				],
				[
					-75,
					65
				],
				[
					-80,
					65
				],
				[
					-85,
					65
				],
				[
					-90,
					65
				],
				[
					-90,
					60
				],
				[
					-85,
					50
				],
				[
					-85,
					40
				],
				[
					-80,
					30
				],
				[
					-80,
					25
				],
				[
					-80,
					15
				],
				[
					-80,
					5
				],
				[
					-80,
					-10
				],
				[
					-90,
					-25
				],
				[
					-100,
					-30
				],
				[
					-125,
					-40
				],
				[
					-155,
					-50
				],
				[
					-195,
					-50
				],
				[
					-250,
					-55
				],
				[
					-330,
					-60
				],
				[
					-410,
					-65
				],
				[
					-415,
					-65
				],
				[
					-415,
					-65
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-415,
				-65
			]
		},
		{
			"id": "aAajrG-98eua1yeQy1dGj",
			"type": "freedraw",
			"x": 4247.981948122874,
			"y": -2712.022527936546,
			"width": 65,
			"height": 370,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1192359402,
			"version": 42,
			"versionNonce": 169703722,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					25
				],
				[
					15,
					65
				],
				[
					25,
					115
				],
				[
					35,
					175
				],
				[
					45,
					240
				],
				[
					50,
					305
				],
				[
					60,
					340
				],
				[
					65,
					365
				],
				[
					65,
					370
				],
				[
					65,
					370
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				65,
				370
			]
		},
		{
			"id": "ETRnVz-JG1K2uGPzcguAP",
			"type": "freedraw",
			"x": 4207.981948122874,
			"y": -2392.022527936546,
			"width": 130,
			"height": 145,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 2113863274,
			"version": 45,
			"versionNonce": 1265731190,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					5
				],
				[
					25,
					30
				],
				[
					45,
					55
				],
				[
					70,
					80
				],
				[
					90,
					95
				],
				[
					100,
					100
				],
				[
					105,
					100
				],
				[
					105,
					95
				],
				[
					110,
					75
				],
				[
					120,
					40
				],
				[
					125,
					0
				],
				[
					130,
					-30
				],
				[
					130,
					-45
				],
				[
					130,
					-45
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				130,
				-45
			]
		},
		{
			"id": "QDnrYs-8MVgJwgvsi_644",
			"type": "freedraw",
			"x": 4907.981948122874,
			"y": -2242.022527936546,
			"width": 920,
			"height": 205,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1940550762,
			"version": 55,
			"versionNonce": 53003242,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-15,
					0
				],
				[
					-70,
					0
				],
				[
					-150,
					0
				],
				[
					-255,
					-5
				],
				[
					-385,
					-5
				],
				[
					-525,
					0
				],
				[
					-640,
					10
				],
				[
					-720,
					30
				],
				[
					-755,
					45
				],
				[
					-760,
					60
				],
				[
					-750,
					75
				],
				[
					-700,
					95
				],
				[
					-615,
					125
				],
				[
					-480,
					140
				],
				[
					-320,
					150
				],
				[
					-160,
					145
				],
				[
					-5,
					120
				],
				[
					105,
					90
				],
				[
					150,
					65
				],
				[
					160,
					45
				],
				[
					145,
					25
				],
				[
					70,
					0
				],
				[
					-70,
					-25
				],
				[
					-285,
					-50
				],
				[
					-340,
					-55
				],
				[
					-340,
					-55
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-340,
				-55
			]
		},
		{
			"id": "p_Idg-Ed4zCsVRmXViWB7",
			"type": "freedraw",
			"x": 1437.981948122874,
			"y": -1512.0225279365459,
			"width": 195,
			"height": 110,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 90254326,
			"version": 50,
			"versionNonce": 866469814,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-20,
					0
				],
				[
					-40,
					15
				],
				[
					-50,
					30
				],
				[
					-50,
					50
				],
				[
					-40,
					60
				],
				[
					-5,
					70
				],
				[
					30,
					75
				],
				[
					80,
					75
				],
				[
					120,
					75
				],
				[
					140,
					75
				],
				[
					145,
					65
				],
				[
					145,
					50
				],
				[
					130,
					25
				],
				[
					100,
					5
				],
				[
					65,
					-15
				],
				[
					35,
					-25
				],
				[
					5,
					-35
				],
				[
					-15,
					-35
				],
				[
					-25,
					-30
				],
				[
					0,
					0
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-25,
				-30
			]
		},
		{
			"id": "m7HyWQYzmv0h_rsE0QpWd",
			"type": "freedraw",
			"x": 3067.981948122874,
			"y": -1507.0225279365459,
			"width": 245,
			"height": 135,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 324872042,
			"version": 48,
			"versionNonce": 972863146,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-20,
					0
				],
				[
					-35,
					10
				],
				[
					-50,
					25
				],
				[
					-65,
					50
				],
				[
					-65,
					70
				],
				[
					-55,
					85
				],
				[
					-30,
					95
				],
				[
					5,
					100
				],
				[
					45,
					100
				],
				[
					85,
					100
				],
				[
					110,
					85
				],
				[
					120,
					70
				],
				[
					120,
					50
				],
				[
					95,
					20
				],
				[
					55,
					0
				],
				[
					0,
					-25
				],
				[
					-60,
					-35
				],
				[
					-105,
					-35
				],
				[
					-125,
					-35
				],
				[
					-125,
					-35
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-125,
				-35
			]
		},
		{
			"id": "6t7X9tA-otxjBM5LMhKFg",
			"type": "freedraw",
			"x": 3052.981948122874,
			"y": -1507.0225279365459,
			"width": 55,
			"height": 425,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1583913066,
			"version": 40,
			"versionNonce": 2051989750,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-5
				],
				[
					0,
					-15
				],
				[
					5,
					-40
				],
				[
					10,
					-75
				],
				[
					25,
					-125
				],
				[
					30,
					-185
				],
				[
					40,
					-255
				],
				[
					45,
					-315
				],
				[
					50,
					-365
				],
				[
					50,
					-395
				],
				[
					50,
					-415
				],
				[
					55,
					-425
				],
				[
					55,
					-425
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				55,
				-425
			]
		},
		{
			"id": "c12ezc0H7kZBMKhu-LtOd",
			"type": "freedraw",
			"x": 3107.981948122874,
			"y": -1967.0225279365459,
			"width": 150,
			"height": 125,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1050006518,
			"version": 44,
			"versionNonce": 1061441898,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5,
					0
				],
				[
					-10,
					10
				],
				[
					-30,
					40
				],
				[
					-55,
					65
				],
				[
					-85,
					90
				],
				[
					-95,
					100
				],
				[
					-80,
					85
				],
				[
					-60,
					60
				],
				[
					-40,
					30
				],
				[
					-20,
					10
				],
				[
					-10,
					5
				],
				[
					-5,
					0
				],
				[
					10,
					25
				],
				[
					30,
					65
				],
				[
					40,
					95
				],
				[
					50,
					115
				],
				[
					55,
					125
				],
				[
					55,
					125
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				55,
				125
			]
		},
		{
			"id": "MG74XTlTvpZlmZYaEw9i9",
			"type": "freedraw",
			"x": 1462.981948122874,
			"y": -1547.0225279365459,
			"width": 30,
			"height": 365,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1357871222,
			"version": 38,
			"versionNonce": 49500726,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					0
				],
				[
					5,
					-5
				],
				[
					5,
					-35
				],
				[
					5,
					-65
				],
				[
					5,
					-115
				],
				[
					5,
					-175
				],
				[
					-5,
					-230
				],
				[
					-15,
					-285
				],
				[
					-20,
					-330
				],
				[
					-20,
					-350
				],
				[
					-20,
					-360
				],
				[
					-25,
					-365
				],
				[
					-25,
					-365
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-25,
				-365
			]
		},
		{
			"id": "6djK6HAMkCe2pRIpQQZan",
			"type": "freedraw",
			"x": 1417.981948122874,
			"y": -1932.0225279365459,
			"width": 160,
			"height": 140,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1099177258,
			"version": 44,
			"versionNonce": 1447728170,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5,
					0
				],
				[
					-10,
					10
				],
				[
					-30,
					35
				],
				[
					-55,
					60
				],
				[
					-75,
					85
				],
				[
					-85,
					100
				],
				[
					-80,
					90
				],
				[
					-60,
					65
				],
				[
					-40,
					35
				],
				[
					-25,
					5
				],
				[
					-15,
					-15
				],
				[
					-10,
					-20
				],
				[
					-5,
					-25
				],
				[
					0,
					-25
				],
				[
					25,
					15
				],
				[
					45,
					55
				],
				[
					65,
					85
				],
				[
					70,
					105
				],
				[
					75,
					115
				],
				[
					75,
					115
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				75,
				115
			]
		},
		{
			"id": "_T7vS-tjlcdGULubX8XXG",
			"type": "freedraw",
			"x": 3212.981948122874,
			"y": -797.0225279365459,
			"width": 275,
			"height": 100,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1899920438,
			"version": 61,
			"versionNonce": 2021104502,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5,
					0
				],
				[
					-20,
					-5
				],
				[
					-45,
					-5
				],
				[
					-80,
					-5
				],
				[
					-120,
					-5
				],
				[
					-165,
					-5
				],
				[
					-205,
					-5
				],
				[
					-230,
					-5
				],
				[
					-240,
					-5
				],
				[
					-240,
					0
				],
				[
					-230,
					15
				],
				[
					-220,
					30
				],
				[
					-215,
					50
				],
				[
					-215,
					65
				],
				[
					-215,
					80
				],
				[
					-215,
					85
				],
				[
					-205,
					85
				],
				[
					-180,
					85
				],
				[
					-155,
					85
				],
				[
					-110,
					85
				],
				[
					-65,
					90
				],
				[
					-25,
					95
				],
				[
					10,
					95
				],
				[
					25,
					95
				],
				[
					30,
					95
				],
				[
					30,
					90
				],
				[
					30,
					85
				],
				[
					30,
					75
				],
				[
					30,
					65
				],
				[
					35,
					50
				],
				[
					35,
					30
				],
				[
					30,
					15
				],
				[
					25,
					5
				],
				[
					20,
					-5
				],
				[
					15,
					-5
				],
				[
					0,
					0
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				15,
				-5
			]
		},
		{
			"id": "hGb-YVQ_Zy4mWKnfZeu89",
			"type": "freedraw",
			"x": 3147.981948122874,
			"y": -772.0225279365459,
			"width": 45,
			"height": 1110,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1509715562,
			"version": 43,
			"versionNonce": 553287402,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-20
				],
				[
					0,
					-50
				],
				[
					-5,
					-95
				],
				[
					-10,
					-180
				],
				[
					-15,
					-290
				],
				[
					-30,
					-435
				],
				[
					-40,
					-570
				],
				[
					-45,
					-665
				],
				[
					-45,
					-750
				],
				[
					-45,
					-830
				],
				[
					-35,
					-910
				],
				[
					-35,
					-965
				],
				[
					-35,
					-1010
				],
				[
					-35,
					-1045
				],
				[
					-35,
					-1070
				],
				[
					-35,
					-1090
				],
				[
					-35,
					-1100
				],
				[
					-35,
					-1105
				],
				[
					-35,
					-1110
				],
				[
					-35,
					-1110
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-35,
				-1110
			]
		},
		{
			"id": "ezzzINzquwV1YDbVEQlWU",
			"type": "freedraw",
			"x": 3112.981948122874,
			"y": -747.0225279365459,
			"width": 1275.0000000000002,
			"height": 1285,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1433896106,
			"version": 45,
			"versionNonce": 1629535414,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5,
					-15
				],
				[
					-25,
					-55
				],
				[
					-55,
					-110
				],
				[
					-110,
					-185
				],
				[
					-185,
					-290
				],
				[
					-290,
					-420
				],
				[
					-410,
					-560
				],
				[
					-510,
					-670
				],
				[
					-640,
					-790
				],
				[
					-765,
					-895
				],
				[
					-875,
					-985
				],
				[
					-960,
					-1055
				],
				[
					-1030,
					-1115
				],
				[
					-1080.0000000000002,
					-1165
				],
				[
					-1130.0000000000002,
					-1205
				],
				[
					-1165.0000000000002,
					-1230
				],
				[
					-1195.0000000000002,
					-1250
				],
				[
					-1220.0000000000002,
					-1260
				],
				[
					-1245.0000000000002,
					-1270
				],
				[
					-1260.0000000000002,
					-1280
				],
				[
					-1270.0000000000002,
					-1280
				],
				[
					-1275.0000000000002,
					-1285
				],
				[
					-1275.0000000000002,
					-1285
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-1275.0000000000002,
				-1285
			]
		},
		{
			"id": "GtjgqRZxPErxWANxY-SS3",
			"type": "freedraw",
			"x": 1777.981948122874,
			"y": -2037.0225279365459,
			"width": 115,
			"height": 195,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 163312118,
			"version": 32,
			"versionNonce": 1272910250,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					0
				],
				[
					20,
					30
				],
				[
					40,
					75
				],
				[
					65,
					130
				],
				[
					95,
					170
				],
				[
					110,
					190
				],
				[
					115,
					195
				],
				[
					115,
					175
				],
				[
					110,
					155
				],
				[
					100,
					130
				],
				[
					100,
					130
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				100,
				130
			]
		},
		{
			"id": "IXMw0P_e-PvIEN5dF5S14",
			"type": "freedraw",
			"x": 1827.981948122874,
			"y": -2027.0225279365459,
			"width": 195,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1247017194,
			"version": 30,
			"versionNonce": 848541174,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-5
				],
				[
					15,
					-10
				],
				[
					45,
					-20
				],
				[
					80,
					-25
				],
				[
					120,
					-25
				],
				[
					160,
					-25
				],
				[
					190,
					-25
				],
				[
					195,
					-25
				],
				[
					195,
					-20
				],
				[
					195,
					-20
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				195,
				-20
			]
		},
		{
			"id": "RkXp8tlybHXYCu9dMu9ZP",
			"type": "freedraw",
			"x": 3092.981948122874,
			"y": -1922.0225279365459,
			"width": 55,
			"height": 110,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 648200554,
			"version": 25,
			"versionNonce": 975391850,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					5
				],
				[
					-5,
					20
				],
				[
					-15,
					55
				],
				[
					-35,
					85
				],
				[
					-55,
					110
				],
				[
					-55,
					110
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-55,
				110
			]
		},
		{
			"id": "vNI8fPf3ogrP2iTGOCPzc",
			"type": "freedraw",
			"x": 3092.981948122874,
			"y": -1947.0225279365459,
			"width": 130,
			"height": 135,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 113884266,
			"version": 25,
			"versionNonce": 1708492598,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					10,
					0
				],
				[
					40,
					35
				],
				[
					65,
					70
				],
				[
					100,
					100
				],
				[
					120,
					120
				],
				[
					130,
					135
				],
				[
					130,
					135
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				130,
				135
			]
		},
		{
			"id": "s5qpTVlEbBXCEpVIkZ7uW",
			"type": "freedraw",
			"x": 3097.981948122874,
			"y": -2552.022527936546,
			"width": 950,
			"height": 705,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 996415606,
			"version": 44,
			"versionNonce": 831663914,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-25,
					0
				],
				[
					-75,
					0
				],
				[
					-145,
					10
				],
				[
					-205,
					40
				],
				[
					-260,
					85
				],
				[
					-300,
					160
				],
				[
					-320,
					225
				],
				[
					-325,
					325
				],
				[
					-310,
					420
				],
				[
					-255,
					495
				],
				[
					-170,
					570
				],
				[
					-45,
					625
				],
				[
					90,
					645
				],
				[
					230,
					650
				],
				[
					375,
					625
				],
				[
					510,
					555
				],
				[
					575,
					495
				],
				[
					620,
					410
				],
				[
					625,
					330
				],
				[
					605,
					255
				],
				[
					545,
					170
				],
				[
					445,
					85
				],
				[
					315,
					20
				],
				[
					160,
					-40
				],
				[
					75,
					-55
				],
				[
					75,
					-55
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				75,
				-55
			]
		},
		{
			"id": "rCtJzS6f34iq8ExxCs0uE",
			"type": "freedraw",
			"x": 1797.981948122874,
			"y": -2482.022527936546,
			"width": 995.0000000000002,
			"height": 725,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1733358070,
			"version": 43,
			"versionNonce": 189476982,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-65,
					-15
				],
				[
					-145,
					-30
				],
				[
					-250,
					-35
				],
				[
					-360,
					-40
				],
				[
					-455,
					-40
				],
				[
					-545,
					-25
				],
				[
					-610,
					10
				],
				[
					-650,
					55
				],
				[
					-675,
					125
				],
				[
					-690,
					215
				],
				[
					-685,
					315
				],
				[
					-630,
					430
				],
				[
					-535,
					525
				],
				[
					-410,
					605
				],
				[
					-255,
					660
				],
				[
					-80,
					660
				],
				[
					50,
					615
				],
				[
					190,
					525
				],
				[
					275.0000000000002,
					420
				],
				[
					305.0000000000002,
					315
				],
				[
					290.0000000000002,
					215
				],
				[
					210,
					115
				],
				[
					85,
					20
				],
				[
					-80,
					-55
				],
				[
					-120,
					-65
				],
				[
					-120,
					-65
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-120,
				-65
			]
		},
		{
			"id": "SOBIDt6wSaH96RDyoEhng",
			"type": "freedraw",
			"x": 1772.981948122874,
			"y": -1772.0225279365459,
			"width": 30,
			"height": 310,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1723542390,
			"version": 27,
			"versionNonce": 110541290,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					15
				],
				[
					15,
					65
				],
				[
					25,
					115
				],
				[
					30,
					160
				],
				[
					30,
					205
				],
				[
					30,
					235
				],
				[
					25,
					255
				],
				[
					25,
					275
				],
				[
					25,
					300
				],
				[
					25,
					310
				],
				[
					25,
					310
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				25,
				310
			]
		},
		{
			"id": "SV7Dp7AHC8RGzbDPDFh7O",
			"type": "freedraw",
			"x": 1657.981948122874,
			"y": -1537.0225279365459,
			"width": 210,
			"height": 240,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 550909802,
			"version": 28,
			"versionNonce": 1589227958,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					30,
					25
				],
				[
					75,
					70
				],
				[
					115,
					110
				],
				[
					155,
					145
				],
				[
					185,
					180
				],
				[
					200,
					195
				],
				[
					200,
					190
				],
				[
					200,
					145
				],
				[
					205,
					85
				],
				[
					205,
					15
				],
				[
					210,
					-30
				],
				[
					210,
					-45
				],
				[
					210,
					-45
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				210,
				-45
			]
		},
		{
			"id": "XO4OrtMdNZqhWl-xE7YrX",
			"type": "freedraw",
			"x": 1587.981948122874,
			"y": -1457.0225279365459,
			"width": 400,
			"height": 30,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1085981942,
			"version": 21,
			"versionNonce": 1211886762,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					20,
					0
				],
				[
					75,
					0
				],
				[
					145,
					5
				],
				[
					250,
					15
				],
				[
					345,
					25
				],
				[
					400,
					30
				],
				[
					400,
					30
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				400,
				30
			]
		},
		{
			"id": "I0uamnbKU1sglDSQ9MDFP",
			"type": "freedraw",
			"x": 1627.981948122874,
			"y": -1312.0225279365459,
			"width": 210,
			"height": 10,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1355393130,
			"version": 20,
			"versionNonce": 1531316982,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					10,
					0
				],
				[
					40,
					-10
				],
				[
					80,
					-10
				],
				[
					140,
					-10
				],
				[
					200,
					-10
				],
				[
					210,
					-10
				],
				[
					210,
					-10
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				210,
				-10
			]
		},
		{
			"id": "aJChDgy3d0hLi8a0s_OmP",
			"type": "freedraw",
			"x": 1537.981948122874,
			"y": -1307.0225279365459,
			"width": 260,
			"height": 15,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 371236918,
			"version": 17,
			"versionNonce": 1814873962,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					35,
					0
				],
				[
					110,
					5
				],
				[
					190,
					10
				],
				[
					260,
					15
				],
				[
					260,
					15
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				260,
				15
			]
		},
		{
			"id": "uvjZkkRdrCpvkNBHFpdv6",
			"type": "freedraw",
			"x": 1597.981948122874,
			"y": -1202.0225279365459,
			"width": 355,
			"height": 30,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 833298026,
			"version": 18,
			"versionNonce": 1333083190,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					10,
					0
				],
				[
					45,
					0
				],
				[
					105,
					0
				],
				[
					200,
					10
				],
				[
					320,
					25
				],
				[
					355,
					30
				],
				[
					355,
					30
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				355,
				30
			]
		},
		{
			"id": "y-xblHq0_Yt7c-9bC7VxT",
			"type": "freedraw",
			"x": 1517.981948122874,
			"y": -1147.0225279365459,
			"width": 430,
			"height": 5,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 99912246,
			"version": 17,
			"versionNonce": 2058635818,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					15,
					0
				],
				[
					75,
					5
				],
				[
					165,
					5
				],
				[
					290,
					5
				],
				[
					410,
					5
				],
				[
					430,
					5
				],
				[
					430,
					5
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				430,
				5
			]
		},
		{
			"id": "dVlFS2X9BRaVSIGDDTMhF",
			"type": "freedraw",
			"x": 672.981948122874,
			"y": -1787.0225279365459,
			"width": 3125,
			"height": 1085,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 32637174,
			"version": 41,
			"versionNonce": 1898726774,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					25,
					0
				],
				[
					130,
					0
				],
				[
					305,
					0
				],
				[
					555,
					5
				],
				[
					930,
					5
				],
				[
					1210,
					10
				],
				[
					1590.0000000000002,
					10
				],
				[
					1960.0000000000002,
					-5
				],
				[
					2260,
					-15
				],
				[
					2520,
					-25
				],
				[
					2730,
					-30
				],
				[
					2875,
					-30
				],
				[
					2975,
					-25
				],
				[
					3035,
					-25
				],
				[
					3075,
					-20
				],
				[
					3095,
					-20
				],
				[
					3105,
					-20
				],
				[
					3115,
					-15
				],
				[
					3120,
					-15
				],
				[
					3125,
					-15
				],
				[
					3125,
					-30
				],
				[
					3125,
					-85
				],
				[
					3110,
					-180
				],
				[
					3075,
					-360
				],
				[
					3045,
					-510
				],
				[
					3020,
					-700
				],
				[
					2980,
					-895
				],
				[
					2950,
					-1025
				],
				[
					2940,
					-1065
				],
				[
					2940,
					-1075
				],
				[
					2940,
					-1075
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				2940,
				-1075
			]
		},
		{
			"id": "jBx07Fl7n7c9TWvJe3gCv",
			"type": "freedraw",
			"x": 4247.981948122874,
			"y": -2997.022527936546,
			"width": 95,
			"height": 540,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1217600310,
			"version": 20,
			"versionNonce": 985494762,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					5
				],
				[
					5,
					40
				],
				[
					20,
					80
				],
				[
					35,
					140
				],
				[
					55,
					220
				],
				[
					70,
					325
				],
				[
					85,
					460
				],
				[
					90,
					515
				],
				[
					95,
					540
				],
				[
					95,
					540
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				95,
				540
			]
		},
		{
			"id": "BZOh3G_cF1JjsbH64cPTs",
			"type": "freedraw",
			"x": 4842.981948122874,
			"y": -2402.022527936546,
			"width": 545,
			"height": 560,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 490155690,
			"version": 21,
			"versionNonce": 1047909622,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864762,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-10,
					15
				],
				[
					-40,
					35
				],
				[
					-90,
					80
				],
				[
					-160,
					155
				],
				[
					-255,
					255
				],
				[
					-350,
					355
				],
				[
					-435,
					450
				],
				[
					-505,
					520
				],
				[
					-535,
					545
				],
				[
					-545,
					560
				],
				[
					-545,
					560
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-545,
				560
			]
		},
		{
			"id": "53Ok8abJj_YLUdinScRRV",
			"type": "freedraw",
			"x": 4197.981948122874,
			"y": -2552.022527936546,
			"width": 670,
			"height": 895,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 279853174,
			"version": 22,
			"versionNonce": 1574127530,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					5
				],
				[
					10,
					40
				],
				[
					60,
					125
				],
				[
					125,
					230
				],
				[
					220,
					355
				],
				[
					300,
					450
				],
				[
					415,
					595
				],
				[
					520,
					725
				],
				[
					600,
					820
				],
				[
					645,
					870
				],
				[
					665,
					895
				],
				[
					670,
					895
				],
				[
					670,
					895
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				670,
				895
			]
		},
		{
			"id": "kZQzdTjyhlz0qfZXnU-_P",
			"type": "freedraw",
			"x": 3217.981948122874,
			"y": -1562.0225279365459,
			"width": 280,
			"height": 140,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1366908202,
			"version": 30,
			"versionNonce": 2078217014,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907864067,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-15,
					-5
				],
				[
					-35,
					-5
				],
				[
					-65,
					-5
				],
				[
					-105,
					5
				],
				[
					-140,
					25
				],
				[
					-165,
					60
				],
				[
					-170,
					85
				],
				[
					-165,
					100
				],
				[
					-140,
					110
				],
				[
					-85,
					115
				],
				[
					-45,
					110
				],
				[
					0,
					90
				],
				[
					35,
					70
				],
				[
					45,
					50
				],
				[
					50,
					35
				],
				[
					35,
					15
				],
				[
					0,
					0
				],
				[
					-60,
					-15
				],
				[
					-125,
					-25
				],
				[
					-200,
					-25
				],
				[
					-230,
					-20
				],
				[
					-230,
					-20
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-230,
				-20
			]
		},
		{
			"id": "m_7ynxSG_UoLhE3KJqNDJ",
			"type": "freedraw",
			"x": 1527.981948122874,
			"y": -1537.0225279365459,
			"width": 180,
			"height": 175,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 2145005098,
			"version": 27,
			"versionNonce": 1297194614,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907863923,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-30,
					0
				],
				[
					-65,
					10
				],
				[
					-95,
					35
				],
				[
					-115,
					60
				],
				[
					-115,
					85
				],
				[
					-110,
					100
				],
				[
					-80,
					115
				],
				[
					-35,
					115
				],
				[
					5,
					115
				],
				[
					30,
					115
				],
				[
					55,
					95
				],
				[
					65,
					75
				],
				[
					65,
					55
				],
				[
					55,
					25
				],
				[
					30,
					-10
				],
				[
					-5,
					-40
				],
				[
					-40,
					-50
				],
				[
					-70,
					-60
				],
				[
					-100,
					-60
				],
				[
					-100,
					-60
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-100,
				-60
			]
		},
		{
			"id": "OtZO9sqDV2Zd35hUAze3x",
			"type": "freedraw",
			"x": 1487.981948122874,
			"y": -1892.0225279365459,
			"width": 30,
			"height": 225,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 233086058,
			"version": 13,
			"versionNonce": 590408170,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907863791,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					10,
					30
				],
				[
					20,
					75
				],
				[
					25,
					135
				],
				[
					30,
					185
				],
				[
					30,
					210
				],
				[
					30,
					225
				],
				[
					30,
					225
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				30,
				225
			]
		},
		{
			"id": "1zYUjJ-LUDl95NSKoKd1k",
			"type": "freedraw",
			"x": 1457.981948122874,
			"y": -1932.0225279365459,
			"width": 175,
			"height": 125,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1004071990,
			"version": 24,
			"versionNonce": 2057676778,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907863666,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5,
					25
				],
				[
					-25,
					60
				],
				[
					-40,
					80
				],
				[
					-45,
					90
				],
				[
					-35,
					75
				],
				[
					-15,
					50
				],
				[
					0,
					25
				],
				[
					25,
					5
				],
				[
					35,
					-5
				],
				[
					40,
					-5
				],
				[
					55,
					0
				],
				[
					70,
					25
				],
				[
					85,
					55
				],
				[
					100,
					80
				],
				[
					110,
					100
				],
				[
					120,
					110
				],
				[
					125,
					115
				],
				[
					130,
					120
				],
				[
					130,
					120
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				130,
				120
			]
		},
		{
			"id": "vyigOiTP0jG7kFYoHK9Nn",
			"type": "freedraw",
			"x": 3107.981948122874,
			"y": -1922.0225279365459,
			"width": 0,
			"height": 275,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1287441834,
			"version": 13,
			"versionNonce": 23118966,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907863517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					5
				],
				[
					0,
					40
				],
				[
					0,
					95
				],
				[
					0,
					145
				],
				[
					0,
					200
				],
				[
					0,
					250
				],
				[
					0,
					265
				],
				[
					0,
					275
				],
				[
					0,
					275
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				0,
				275
			]
		},
		{
			"id": "8RGtyCwkHJMnYp0dkXIIP",
			"type": "freedraw",
			"x": 3077.981948122874,
			"y": -1957.0225279365459,
			"width": 255,
			"height": 135,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1499381814,
			"version": 23,
			"versionNonce": 56114486,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692907863343,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-15,
					20
				],
				[
					-40,
					45
				],
				[
					-70,
					75
				],
				[
					-85,
					90
				],
				[
					-85,
					85
				],
				[
					-75,
					60
				],
				[
					-55,
					30
				],
				[
					-35,
					5
				],
				[
					-20,
					-10
				],
				[
					-5,
					-20
				],
				[
					5,
					-20
				],
				[
					15,
					-20
				],
				[
					35,
					-5
				],
				[
					70,
					30
				],
				[
					100,
					60
				],
				[
					130,
					85
				],
				[
					150,
					100
				],
				[
					160,
					115
				],
				[
					170,
					115
				],
				[
					170,
					115
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				170,
				115
			]
		}
	],
	"appState": {
		"theme": "dark",
		"viewBackgroundColor": "#f5faff",
		"currentItemStrokeColor": "#1e1e1e",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "hachure",
		"currentItemStrokeWidth": 4,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 2,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 36,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 602.018051877126,
		"scrollY": 3730.381902936546,
		"zoom": {
			"value": 0.2
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"currentStrokeOptions": null,
		"previousGridSize": null
	},
	"files": {}
}
```
%%