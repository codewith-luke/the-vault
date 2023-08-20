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
			"version": 283,
			"versionNonce": 35401235,
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
			"updated": 1691605945351,
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
			"version": 479,
			"versionNonce": 1603514525,
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
			"updated": 1691605945351,
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
			"version": 285,
			"versionNonce": 1496511411,
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
			"updated": 1691605945351,
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
			"version": 504,
			"versionNonce": 1047368957,
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
			"updated": 1691605945351,
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
			"version": 339,
			"versionNonce": 1486882131,
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
			"updated": 1691605945351,
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
			"version": 600,
			"versionNonce": 88862045,
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
			"updated": 1691605945351,
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
			"version": 411,
			"versionNonce": 934929139,
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
			"updated": 1691605945351,
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
			"version": 724,
			"versionNonce": 595605949,
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
			"updated": 1691605945351,
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
			"version": 299,
			"versionNonce": 2131168403,
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
			"updated": 1691605945351,
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
			"version": 417,
			"versionNonce": 573307421,
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
			"updated": 1691605945351,
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
			"version": 418,
			"versionNonce": 1648230963,
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
			"updated": 1691605945351,
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
			"version": 480,
			"versionNonce": 1782623869,
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
			"updated": 1691605945351,
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
			"version": 149,
			"versionNonce": 1514488787,
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
			"updated": 1691605945351,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 181,
			"versionNonce": 1249892061,
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
			"updated": 1691605945351,
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
			"version": 181,
			"versionNonce": 2134069619,
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
			"updated": 1691605945351,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 208,
			"versionNonce": 1031467837,
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
			"updated": 1691605945351,
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
			"version": 253,
			"versionNonce": 575580947,
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
			"updated": 1691605945351,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 289,
			"versionNonce": 1871938461,
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
			"updated": 1691605945351,
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
			"version": 235,
			"versionNonce": 671994035,
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
			"updated": 1691605945351,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 353,
			"versionNonce": 83560445,
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
			"updated": 1691605945351,
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
			"version": 708,
			"versionNonce": 571949651,
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
			"updated": 1691605945351,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 826,
			"versionNonce": 531824733,
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
			"updated": 1691605945351,
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
			"version": 205,
			"versionNonce": 692158451,
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
			"updated": 1691605945351,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 227,
			"versionNonce": 629992637,
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
			"updated": 1691605945351,
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
			"version": 278,
			"versionNonce": 2006124947,
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
			"updated": 1691605945351,
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
			"version": 178,
			"versionNonce": 1177177373,
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
			"updated": 1691605945351,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 112,
			"versionNonce": 1111646003,
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
			"updated": 1691605945351,
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
			"version": 174,
			"versionNonce": 1090298237,
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
			"updated": 1691605945351,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 146,
			"versionNonce": 1404436691,
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
			"updated": 1691605945352,
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
			"version": 222,
			"versionNonce": 1799711197,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 209,
			"versionNonce": 1703177843,
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
			"updated": 1691605945352,
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
			"version": 209,
			"versionNonce": 1981163069,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 191,
			"versionNonce": 980690963,
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
			"updated": 1691605945352,
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
			"version": 82,
			"versionNonce": 1951422109,
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
			"updated": 1691605945352,
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
			"version": 153,
			"versionNonce": 2021371315,
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
			"updated": 1691605945352,
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
			"version": 270,
			"versionNonce": 547715837,
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
			"updated": 1691605945352,
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
			"version": 834,
			"versionNonce": 1119977299,
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
			"updated": 1691605945352,
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
			"version": 152,
			"versionNonce": 1670845277,
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
			"updated": 1691605945352,
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
			"version": 31,
			"versionNonce": 328998131,
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
			"updated": 1691605945352,
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
			"version": 60,
			"versionNonce": 427204541,
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
			"updated": 1691605945352,
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
			"version": 30,
			"versionNonce": 1452410515,
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
			"updated": 1691605945352,
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
			"version": 28,
			"versionNonce": 409313309,
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
			"updated": 1691605945352,
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
			"version": 214,
			"versionNonce": 1113177139,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 243,
			"versionNonce": 1985320061,
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
			"updated": 1691605945352,
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
			"version": 114,
			"versionNonce": 1926872531,
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
			"updated": 1691605945352,
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
			"version": 6464,
			"versionNonce": 252181725,
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
			"updated": 1691605945352,
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
			"version": 7185,
			"versionNonce": 1126730611,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 63,
			"versionNonce": 1242454333,
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
			"updated": 1691605945352,
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
			"version": 49,
			"versionNonce": 1737270547,
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
			"updated": 1691605945352,
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
			"version": 200,
			"versionNonce": 550119837,
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
			"updated": 1691605945352,
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
			"version": 72,
			"versionNonce": 1199344307,
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
			"updated": 1691605945352,
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
			"version": 72,
			"versionNonce": 1684860413,
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
			"updated": 1691605945352,
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
			"version": 6627,
			"versionNonce": 396278867,
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
			"updated": 1691605945352,
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
			"version": 7347,
			"versionNonce": 1140336221,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 242,
			"versionNonce": 868858355,
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
			"updated": 1691605945352,
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
			"version": 6724,
			"versionNonce": 306008765,
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
			"updated": 1691605945352,
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
			"version": 7444,
			"versionNonce": 956564371,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 368,
			"versionNonce": 1272836893,
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
			"updated": 1691605945352,
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
			"version": 154,
			"versionNonce": 1602492723,
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
			"updated": 1691605945352,
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
			"version": 192,
			"versionNonce": 1565230973,
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
			"updated": 1691605945352,
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
			"version": 82,
			"versionNonce": 347110099,
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
			"updated": 1691605945352,
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
			"version": 151,
			"versionNonce": 684167133,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 254,
			"versionNonce": 1428138099,
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
			"updated": 1691605945352,
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
			"version": 290,
			"versionNonce": 1281592381,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 346,
			"versionNonce": 1184375315,
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
			"updated": 1691605945352,
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
			"version": 437,
			"versionNonce": 671153309,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 471,
			"versionNonce": 303065011,
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
			"updated": 1691605945352,
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
			"version": 553,
			"versionNonce": 592535805,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 664,
			"versionNonce": 2108619091,
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
			"updated": 1691605945352,
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
			"version": 1166,
			"versionNonce": 869677405,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1282,
			"versionNonce": 1187665651,
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
			"updated": 1691605945352,
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
			"version": 321,
			"versionNonce": 585172413,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 337,
			"versionNonce": 1005125779,
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
			"updated": 1691605945352,
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
			"version": 388,
			"versionNonce": 328418845,
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
			"updated": 1691605945352,
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
			"version": 544,
			"versionNonce": 381777459,
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
			"updated": 1691605945352,
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
			"version": 771,
			"versionNonce": 1222539901,
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
			"updated": 1691605945352,
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
			"version": 154,
			"versionNonce": 372914131,
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
			"updated": 1691605945352,
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
			"version": 955,
			"versionNonce": 730079965,
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
			"updated": 1691605945352,
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
			"version": 156,
			"versionNonce": 1483326835,
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
			"updated": 1691605945352,
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
			"version": 7544,
			"versionNonce": 269860669,
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
			"updated": 1691605945352,
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
			"version": 8265,
			"versionNonce": 1956028179,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 6797,
			"versionNonce": 1022676893,
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
			"updated": 1691605945352,
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
			"version": 7517,
			"versionNonce": 1429685427,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 412,
			"versionNonce": 810734589,
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
			"updated": 1691605945352,
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
			"version": 6894,
			"versionNonce": 1374828115,
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
			"updated": 1691605945352,
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
			"version": 7614,
			"versionNonce": 640765021,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 538,
			"versionNonce": 161346547,
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
			"updated": 1691605945352,
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
			"version": 324,
			"versionNonce": 1583462589,
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
			"updated": 1691605945352,
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
			"version": 362,
			"versionNonce": 2084634003,
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
			"updated": 1691605945352,
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
			"version": 339,
			"versionNonce": 579180829,
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
			"updated": 1691605945352,
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
			"version": 921,
			"versionNonce": 1695666995,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1001,
			"versionNonce": 202272125,
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
			"updated": 1691605945352,
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
			"version": 648,
			"versionNonce": 1417082067,
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
			"updated": 1691605945352,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 776,
			"versionNonce": 171816413,
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
			"updated": 1691605945352,
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
			"version": 543,
			"versionNonce": 168223347,
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
			"updated": 1691605945353,
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
			"version": 3810,
			"versionNonce": 673509949,
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
			"updated": 1691605945353,
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
			"version": 1728,
			"versionNonce": 243801107,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3052,
			"versionNonce": 312844957,
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
			"updated": 1691605945353,
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
			"version": 1994,
			"versionNonce": 233906611,
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
			"updated": 1691605945353,
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
			"version": 1804,
			"versionNonce": 1584482045,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3125,
			"versionNonce": 1902670675,
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
			"updated": 1691605945353,
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
			"version": 1853,
			"versionNonce": 235495261,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3210,
			"versionNonce": 960794867,
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
			"updated": 1691605945353,
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
			"version": 1095,
			"versionNonce": 1472162749,
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
			"updated": 1691605945353,
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
			"version": 244,
			"versionNonce": 386661011,
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
			"updated": 1691605945353,
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
			"version": 1983,
			"versionNonce": 733277213,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1901,
			"versionNonce": 1198862387,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2308,
			"versionNonce": 2044420221,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2241,
			"versionNonce": 744927699,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2023,
			"versionNonce": 938756317,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1293,
			"versionNonce": 653721459,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 984,
			"versionNonce": 663823677,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1182,
			"versionNonce": 829200659,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1082,
			"versionNonce": 1544779165,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1037,
			"versionNonce": 960364211,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1287,
			"versionNonce": 11319805,
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
			"updated": 1691605945353,
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
			"version": 226,
			"versionNonce": 957460563,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 111,
			"versionNonce": 1583247965,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1595,
			"versionNonce": 314453491,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1730,
			"versionNonce": 570039997,
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
			"updated": 1691605945353,
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
			"version": 7924,
			"versionNonce": 692713363,
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
			"updated": 1691605945353,
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
			"version": 8645,
			"versionNonce": 1646346013,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 6883,
			"versionNonce": 988515635,
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
			"updated": 1691605945353,
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
			"version": 7603,
			"versionNonce": 1699042173,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 498,
			"versionNonce": 2064215763,
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
			"updated": 1691605945353,
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
			"version": 6980,
			"versionNonce": 665312221,
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
			"updated": 1691605945353,
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
			"version": 7700,
			"versionNonce": 1815747699,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 624,
			"versionNonce": 559568957,
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
			"updated": 1691605945353,
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
			"version": 410,
			"versionNonce": 2051282451,
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
			"updated": 1691605945353,
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
			"version": 448,
			"versionNonce": 1279150237,
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
			"updated": 1691605945353,
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
			"version": 381,
			"versionNonce": 1411242931,
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
			"updated": 1691605945353,
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
			"version": 2051,
			"versionNonce": 1778724093,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1972,
			"versionNonce": 99478867,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2379,
			"versionNonce": 170952029,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2312,
			"versionNonce": 1393216243,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 2094,
			"versionNonce": 1343345085,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1363,
			"versionNonce": 1341846675,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1055,
			"versionNonce": 2026541597,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1253,
			"versionNonce": 1014295091,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1153,
			"versionNonce": 558646909,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1106,
			"versionNonce": 492776403,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1358,
			"versionNonce": 1280863965,
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
			"updated": 1691605945353,
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
			"version": 545,
			"versionNonce": 382744947,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 579,
			"versionNonce": 679512893,
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
			"updated": 1691605945353,
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
			"version": 671,
			"versionNonce": 101618451,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 782,
			"versionNonce": 371596189,
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
			"updated": 1691605945353,
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
			"version": 440,
			"versionNonce": 1536211123,
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
			"updated": 1691605945353,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 455,
			"versionNonce": 1836752893,
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
			"updated": 1691605945354,
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
			"version": 506,
			"versionNonce": 889006675,
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
			"updated": 1691605945354,
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
			"version": 1005,
			"versionNonce": 75470941,
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
			"updated": 1691605945354,
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
			"version": 293,
			"versionNonce": 925526003,
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
			"updated": 1691605945354,
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
			"version": 1351,
			"versionNonce": 1963361469,
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
			"updated": 1691605945354,
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
			"version": 294,
			"versionNonce": 673116563,
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
			"updated": 1691605945354,
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
			"version": 1015,
			"versionNonce": 582018333,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1095,
			"versionNonce": 1225869107,
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
			"updated": 1691605945354,
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
			"version": 766,
			"versionNonce": 15743357,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 894,
			"versionNonce": 1885858003,
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
			"updated": 1691605945354,
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
			"version": 913,
			"versionNonce": 419824093,
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
			"updated": 1691605945354,
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
			"version": 3806,
			"versionNonce": 1673090675,
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
			"updated": 1691605945354,
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
			"version": 1724,
			"versionNonce": 1342422589,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3048,
			"versionNonce": 1909198867,
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
			"updated": 1691605945354,
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
			"version": 1990,
			"versionNonce": 1825238685,
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
			"updated": 1691605945354,
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
			"version": 1800,
			"versionNonce": 1284937139,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3121,
			"versionNonce": 1577915133,
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
			"updated": 1691605945354,
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
			"version": 1849,
			"versionNonce": 591357779,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3206,
			"versionNonce": 1078700893,
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
			"updated": 1691605945354,
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
			"version": 1091,
			"versionNonce": 2082276595,
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
			"updated": 1691605945354,
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
			"version": 329,
			"versionNonce": 601372605,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 163,
			"versionNonce": 1320545939,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 62,
			"versionNonce": 315897885,
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
			"updated": 1691605945354,
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
			"version": 636,
			"versionNonce": 1572906035,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 670,
			"versionNonce": 1462840445,
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
			"updated": 1691605945354,
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
			"version": 762,
			"versionNonce": 1361290707,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 874,
			"versionNonce": 11572445,
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
			"updated": 1691605945354,
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
			"version": 531,
			"versionNonce": 267744115,
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
			"updated": 1691605945354,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 546,
			"versionNonce": 719581501,
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
			"updated": 1691605945354,
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
			"version": 597,
			"versionNonce": 1518112019,
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
			"updated": 1691605945354,
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
			"version": 1194,
			"versionNonce": 53264797,
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
			"updated": 1691605945354,
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
			"version": 426,
			"versionNonce": 607089331,
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
			"updated": 1691605945354,
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
			"version": 1567,
			"versionNonce": 247236093,
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
			"updated": 1691605945355,
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
			"version": 427,
			"versionNonce": 766813267,
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
			"updated": 1691605945355,
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
			"version": 1180,
			"versionNonce": 815054429,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1260,
			"versionNonce": 1591910899,
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
			"updated": 1691605945355,
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
			"version": 857,
			"versionNonce": 1871112893,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 985,
			"versionNonce": 1623190419,
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
			"updated": 1691605945355,
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
			"version": 1200,
			"versionNonce": 2083818269,
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
			"updated": 1691605945355,
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
			"version": 3897,
			"versionNonce": 2005074227,
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
			"updated": 1691605945355,
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
			"version": 1815,
			"versionNonce": 1997479805,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3139,
			"versionNonce": 479355603,
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
			"updated": 1691605945355,
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
			"version": 2081,
			"versionNonce": 1985488861,
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
			"updated": 1691605945355,
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
			"version": 1891,
			"versionNonce": 1485082739,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3212,
			"versionNonce": 1277240381,
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
			"updated": 1691605945355,
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
			"version": 1940,
			"versionNonce": 1562380819,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3297,
			"versionNonce": 206279837,
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
			"updated": 1691605945355,
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
			"version": 1182,
			"versionNonce": 1599819699,
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
			"updated": 1691605945355,
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
			"version": 386,
			"versionNonce": 1384708349,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 254,
			"versionNonce": 828170579,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 157,
			"versionNonce": 1213911389,
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
			"updated": 1691605945355,
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
			"version": 602,
			"versionNonce": 477839091,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 636,
			"versionNonce": 1796382141,
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
			"updated": 1691605945355,
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
			"version": 728,
			"versionNonce": 2067589267,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 839,
			"versionNonce": 298966557,
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
			"updated": 1691605945355,
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
			"version": 497,
			"versionNonce": 324558387,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 512,
			"versionNonce": 864686717,
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
			"updated": 1691605945355,
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
			"version": 563,
			"versionNonce": 800333779,
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
			"updated": 1691605945355,
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
			"version": 1121,
			"versionNonce": 1828502237,
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
			"updated": 1691605945355,
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
			"version": 351,
			"versionNonce": 2053549427,
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
			"updated": 1691605945355,
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
			"version": 1461,
			"versionNonce": 1186682685,
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
			"updated": 1691605945355,
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
			"version": 352,
			"versionNonce": 381060883,
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
			"updated": 1691605945355,
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
			"version": 1181,
			"versionNonce": 992438173,
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
			"updated": 1691605945355,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1261,
			"versionNonce": 2065312947,
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
			"updated": 1691605945356,
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
			"version": 823,
			"versionNonce": 2087873533,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 951,
			"versionNonce": 188227155,
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
			"updated": 1691605945356,
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
			"version": 1088,
			"versionNonce": 2057167965,
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
			"updated": 1691605945356,
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
			"version": 3863,
			"versionNonce": 1910954995,
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
			"updated": 1691605945356,
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
			"version": 1781,
			"versionNonce": 695947453,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3105,
			"versionNonce": 992798099,
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
			"updated": 1691605945356,
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
			"version": 2047,
			"versionNonce": 111948061,
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
			"updated": 1691605945356,
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
			"version": 1857,
			"versionNonce": 775994163,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3178,
			"versionNonce": 1604453757,
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
			"updated": 1691605945356,
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
			"version": 1906,
			"versionNonce": 1737022675,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 3263,
			"versionNonce": 1469992413,
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
			"updated": 1691605945356,
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
			"version": 1148,
			"versionNonce": 849070707,
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
			"updated": 1691605945356,
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
			"version": 400,
			"versionNonce": 766675517,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 220,
			"versionNonce": 608175123,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 120,
			"versionNonce": 1119894173,
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
			"updated": 1691605945356,
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
			"version": 75,
			"versionNonce": 1953237427,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 553,
			"versionNonce": 1601756925,
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
			"updated": 1691605945356,
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
			"version": 342,
			"versionNonce": 407264083,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 397,
			"versionNonce": 979236701,
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
			"updated": 1691605945356,
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
			"version": 678,
			"versionNonce": 472217843,
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
			"updated": 1691605945356,
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
			"version": 48,
			"versionNonce": 1036059581,
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
			"updated": 1691605945356,
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
			"version": 121,
			"versionNonce": 1032839827,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 139,
			"versionNonce": 230917149,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 66,
			"versionNonce": 1161566259,
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
			"updated": 1691605945356,
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
			"version": 182,
			"versionNonce": 1314322557,
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
			"updated": 1691605945356,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 117,
			"versionNonce": 554736083,
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
			"updated": 1691605945356,
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
			"version": 1962,
			"versionNonce": 691855581,
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
			"updated": 1691605945356,
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
			"version": 107,
			"versionNonce": 1042540403,
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
			"updated": 1691605945356,
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
			"version": 77,
			"versionNonce": 589216829,
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
			"updated": 1691605949158,
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
			"version": 64,
			"versionNonce": 129046232,
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
			"updated": 1692540202010,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 17,
			"versionNonce": 1593257384,
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
			"updated": 1692540224982,
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
			"version": 25,
			"versionNonce": 967361752,
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
			"updated": 1692540198327,
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
			"version": 22,
			"versionNonce": 1107921624,
			"isDeleted": false,
			"id": "FFpDjztJ9szWe31O0tGQC",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 2,
			"opacity": 100,
			"angle": 0,
			"x": 742.481948122874,
			"y": -2396.4623750899345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.024866846510463,
			"height": 227.5,
			"seed": 1252769704,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692540392147,
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
					5.024866846510463,
					227.5
				]
			]
		},
		{
			"type": "rectangle",
			"version": 45,
			"versionNonce": 1290389464,
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
			"updated": 1692540214180,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 5,
			"versionNonce": 158686680,
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
			"updated": 1692540213244,
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
		"currentItemStartArrowhead": "arrow",
		"currentItemEndArrowhead": "triangle",
		"scrollX": 31.184718543792883,
		"scrollY": 3470.1420625899354,
		"zoom": {
			"value": 0.39999999999999997
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