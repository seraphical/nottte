---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
前端->http     protocol
后端->server ^7rKWmAFP

请求
      请求头:携带很多信息, 比如浏览器信息,从哪来(从哪个 ip 发送的请求  ),期望后端能返回什么东西
      请求体: 携带给后端的东西:后端需要的东西  request
       
    

响应
    响应头: 对本次响应的简单描述,还有此次响应的状态码
    响应报文: 给你返回的   response ^CB8IZlK6

断开连接: 经过 4 次挥手 ^ZR7k1Mdi

进行连接: 经过三次握手 ^9szks48y

中间人 ^ATAUelMY

爬虫 ^G4vw9cmL

请求方式:  ^TmlaKKZ3

post,get,     put, DLETE patch  ^vocyhj9z

响应状态码: 100-199 之间表示连接继续
            200-299 之间表示各种成功
            300-399 之间表示重定向
            400-499 表示客户端错误
            500-599  表示服务端错误 ^UZfYGlrg

ajax ^3RNUuNRV

const xhr =  new  XMLHttpRequet() ^pmLpRxke

api 接口 ^ky13vtnb

后端给你的接口是一种通信的东西,你前端调用这个就可以实现各种目的 ^zUusnexL

后端接口
https://api.bilibili.com/x/v2/reply/add
要什么 请求体,你应该调用 api ^VPpbMZu1

一个东西给你抛出一些方法,可以实现一些功能,就叫接口 ^NzYaH8NG

function Car(){

    dirve(){}
} ^d3z6ZDWo

) ^kWsHQCKY

xhr.open(https://api.bilibili.com/x/v2/reply/add,'post') ^5zEUwACg

xhr.send() ^c1gkVrOx

xhr.onload = ()=>{
    请求完成后进行触发的操作
} ^BTSpwZ6x

浏览器的一个策略: 同源策略,只要上面有一个不一样,浏览器就不接收响应, 跨域 ^7LHa5WPE

url:   https  协议    ip=>域名      端口   ^pcEgewk1

cors 跨域 :  前端: webpack: dev server


             cors: 后端的中间件 ^TfSkX91e

b ^Cj5ENzjX

client ^eX5K4aaj

server ^olJF420h

nginx 进行转发: server

        ^GxzLrTiS

axios
 ^2IxfukHo

a ^TVYi32gE

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.24",
	"elements": [
		{
			"id": "7rKWmAFP",
			"type": "text",
			"x": 1.25,
			"y": -296.75,
			"width": 228.55984497070312,
			"height": 50,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1251447366,
			"version": 64,
			"versionNonce": 140481690,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697786675824,
			"link": null,
			"locked": false,
			"text": "前端->http     protocol\n后端->server",
			"rawText": "前端->http     protocol\n后端->server",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 43,
			"containerId": null,
			"originalText": "前端->http     protocol\n后端->server",
			"lineHeight": 1.25
		},
		{
			"id": "CB8IZlK6",
			"type": "text",
			"x": 42.98828125,
			"y": -65.04296875,
			"width": 919.5599365234375,
			"height": 225,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 554817818,
			"version": 565,
			"versionNonce": 1211490438,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697788442110,
			"link": null,
			"locked": false,
			"text": "请求\n      请求头:携带很多信息, 比如浏览器信息,从哪来(从哪个 ip 发送的请求  ),期望后端能返回什么东西\n      请求体: 携带给后端的东西:后端需要的东西  request\n       \n    \n\n响应\n    响应头: 对本次响应的简单描述,还有此次响应的状态码\n    响应报文: 给你返回的   response",
			"rawText": "请求\n      请求头:携带很多信息, 比如浏览器信息,从哪来(从哪个 ip 发送的请求  ),期望后端能返回什么东西\n      请求体: 携带给后端的东西:后端需要的东西  request\n       \n    \n\n响应\n    响应头: 对本次响应的简单描述,还有此次响应的状态码\n    响应报文: 给你返回的   response",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 218,
			"containerId": null,
			"originalText": "请求\n      请求头:携带很多信息, 比如浏览器信息,从哪来(从哪个 ip 发送的请求  ),期望后端能返回什么东西\n      请求体: 携带给后端的东西:后端需要的东西  request\n       \n    \n\n响应\n    响应头: 对本次响应的简单描述,还有此次响应的状态码\n    响应报文: 给你返回的   response",
			"lineHeight": 1.25
		},
		{
			"id": "ZR7k1Mdi",
			"type": "text",
			"x": 205.4921875,
			"y": 217.46875,
			"width": 227.63998413085938,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 984839558,
			"version": 83,
			"versionNonce": 1766045402,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697787541582,
			"link": null,
			"locked": false,
			"text": "断开连接: 经过 4 次挥手",
			"rawText": "断开连接: 经过 4 次挥手",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "断开连接: 经过 4 次挥手",
			"lineHeight": 1.25
		},
		{
			"id": "9szks48y",
			"type": "text",
			"x": 187.32421875,
			"y": -131.77734375,
			"width": 214.83999633789062,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1798564102,
			"version": 45,
			"versionNonce": 1356477274,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697787402578,
			"link": null,
			"locked": false,
			"text": "进行连接: 经过三次握手",
			"rawText": "进行连接: 经过三次握手",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "进行连接: 经过三次握手",
			"lineHeight": 1.25
		},
		{
			"id": "ATAUelMY",
			"type": "text",
			"x": 676.21484375,
			"y": 96.859375,
			"width": 60,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1955038042,
			"version": 381,
			"versionNonce": 110659226,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697787513825,
			"link": null,
			"locked": false,
			"text": "中间人",
			"rawText": "中间人",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "中间人",
			"lineHeight": 1.25
		},
		{
			"id": "G4vw9cmL",
			"type": "text",
			"x": 694.69921875,
			"y": 145.42578125,
			"width": 40,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 2004425434,
			"version": 239,
			"versionNonce": 1105374746,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697787543676,
			"link": null,
			"locked": false,
			"text": "爬虫",
			"rawText": "爬虫",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "爬虫",
			"lineHeight": 1.25
		},
		{
			"id": "TmlaKKZ3",
			"type": "text",
			"x": 55.32421875,
			"y": 352.22265625,
			"width": 94.83999633789062,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 420339930,
			"version": 20,
			"versionNonce": 1045017478,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697787564058,
			"link": null,
			"locked": false,
			"text": "请求方式: ",
			"rawText": "请求方式: ",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "请求方式: ",
			"lineHeight": 1.25
		},
		{
			"id": "vocyhj9z",
			"type": "text",
			"x": 162.90234375,
			"y": 353.984375,
			"width": 328.33978271484375,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 789043526,
			"version": 64,
			"versionNonce": 219199814,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697787887790,
			"link": null,
			"locked": false,
			"text": "post,get,     put, DLETE patch ",
			"rawText": "post,get,     put, DLETE patch ",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "post,get,     put, DLETE patch ",
			"lineHeight": 1.25
		},
		{
			"id": "UZfYGlrg",
			"type": "text",
			"x": 61.32421875,
			"y": 440.70703125,
			"width": 378.5799560546875,
			"height": 125,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1633525190,
			"version": 263,
			"versionNonce": 1045468550,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697787976662,
			"link": null,
			"locked": false,
			"text": "响应状态码: 100-199 之间表示连接继续\n            200-299 之间表示各种成功\n            300-399 之间表示重定向\n            400-499 表示客户端错误\n            500-599  表示服务端错误",
			"rawText": "响应状态码: 100-199 之间表示连接继续\n            200-299 之间表示各种成功\n            300-399 之间表示重定向\n            400-499 表示客户端错误\n            500-599  表示服务端错误",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 118,
			"containerId": null,
			"originalText": "响应状态码: 100-199 之间表示连接继续\n            200-299 之间表示各种成功\n            300-399 之间表示重定向\n            400-499 表示客户端错误\n            500-599  表示服务端错误",
			"lineHeight": 1.25
		},
		{
			"id": "3RNUuNRV",
			"type": "text",
			"x": 217.69140625,
			"y": 2052.45703125,
			"width": 44.47998046875,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1926105754,
			"version": 117,
			"versionNonce": 238306822,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "haxv0P9187RDlFQNfmKiT",
					"type": "arrow"
				}
			],
			"updated": 1697789566636,
			"link": null,
			"locked": false,
			"text": "ajax",
			"rawText": "ajax",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "ajax",
			"lineHeight": 1.25
		},
		{
			"id": "pmLpRxke",
			"type": "text",
			"x": 392.63671875,
			"y": 2007.640625,
			"width": 353.9597473144531,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 2127137306,
			"version": 111,
			"versionNonce": 1588739910,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789602907,
			"link": null,
			"locked": false,
			"text": "const xhr =  new  XMLHttpRequet()",
			"rawText": "const xhr =  new  XMLHttpRequet()",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "const xhr =  new  XMLHttpRequet()",
			"lineHeight": 1.25
		},
		{
			"id": "ky13vtnb",
			"type": "text",
			"x": 48.6875,
			"y": 1459.40625,
			"width": 77.57997131347656,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 2093542918,
			"version": 87,
			"versionNonce": 1365418310,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697788161240,
			"link": null,
			"locked": false,
			"text": "api 接口",
			"rawText": "api 接口",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "api 接口",
			"lineHeight": 1.25
		},
		{
			"id": "zUusnexL",
			"type": "text",
			"x": 304.45703125,
			"y": 1605.76171875,
			"width": 625.1400146484375,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1319948870,
			"version": 115,
			"versionNonce": 953791130,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697788067977,
			"link": null,
			"locked": false,
			"text": "后端给你的接口是一种通信的东西,你前端调用这个就可以实现各种目的",
			"rawText": "后端给你的接口是一种通信的东西,你前端调用这个就可以实现各种目的",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "后端给你的接口是一种通信的东西,你前端调用这个就可以实现各种目的",
			"lineHeight": 1.25
		},
		{
			"id": "VPpbMZu1",
			"type": "text",
			"x": 509.48828125,
			"y": 1427.03515625,
			"width": 354.79974365234375,
			"height": 75,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1497515334,
			"version": 113,
			"versionNonce": 127521350,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697788327393,
			"link": null,
			"locked": false,
			"text": "后端接口\nhttps://api.bilibili.com/x/v2/reply/add\n要什么 请求体,你应该调用 api",
			"rawText": "后端接口\nhttps://api.bilibili.com/x/v2/reply/add\n要什么 请求体,你应该调用 api",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 68,
			"containerId": null,
			"originalText": "后端接口\nhttps://api.bilibili.com/x/v2/reply/add\n要什么 请求体,你应该调用 api",
			"lineHeight": 1.25
		},
		{
			"id": "NzYaH8NG",
			"type": "text",
			"x": -3.54296875,
			"y": 1518.76171875,
			"width": 490.280029296875,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 549660102,
			"version": 112,
			"versionNonce": 41976026,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697788157965,
			"link": null,
			"locked": false,
			"text": "一个东西给你抛出一些方法,可以实现一些功能,就叫接口",
			"rawText": "一个东西给你抛出一些方法,可以实现一些功能,就叫接口",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "一个东西给你抛出一些方法,可以实现一些功能,就叫接口",
			"lineHeight": 1.25
		},
		{
			"id": "d3z6ZDWo",
			"type": "text",
			"x": -85.6796875,
			"y": 1634.76171875,
			"width": 147.89987182617188,
			"height": 100,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 687281542,
			"version": 51,
			"versionNonce": 558323846,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697788223100,
			"link": null,
			"locked": false,
			"text": "function Car(){\n\n    dirve(){}\n}",
			"rawText": "function Car(){\n\n    dirve(){}\n}",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 93,
			"containerId": null,
			"originalText": "function Car(){\n\n    dirve(){}\n}",
			"lineHeight": 1.25
		},
		{
			"text": ")",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"id": "kWsHQCKY",
			"type": "text",
			"x": 54.45703125,
			"y": 1792.76171875,
			"width": 6.7599945068359375,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"roundness": null,
			"seed": 51822,
			"version": 1,
			"versionNonce": 887227828,
			"updated": 1697788241544,
			"isDeleted": false,
			"groupIds": [],
			"boundElements": [],
			"link": null,
			"locked": false,
			"containerId": null,
			"originalText": ")",
			"rawText": ")",
			"lineHeight": 1.25
		},
		{
			"id": "Jig-R5ufvqE1Hy80iR8Cp",
			"type": "freedraw",
			"x": 326.58203125,
			"y": 1985.7734375,
			"width": 47.26953125,
			"height": 248.7734375,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1707520794,
			"version": 280,
			"versionNonce": 216251142,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697788301309,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.171875,
					0
				],
				[
					-0.14453125,
					0.03125
				],
				[
					-0.546875,
					0.26171875
				],
				[
					-1.0625,
					0.8515625
				],
				[
					-1.98046875,
					2.2890625
				],
				[
					-2.99609375,
					4.13671875
				],
				[
					-3.890625,
					5.49609375
				],
				[
					-4.8671875,
					7.10546875
				],
				[
					-5.90234375,
					9.1953125
				],
				[
					-6.796875,
					11.29296875
				],
				[
					-7.69140625,
					13.40234375
				],
				[
					-9.55859375,
					17.546875
				],
				[
					-10.21484375,
					19.32421875
				],
				[
					-11.0390625,
					20.875
				],
				[
					-12.046875,
					22.8046875
				],
				[
					-12.80859375,
					24.5390625
				],
				[
					-13.41015625,
					26.07421875
				],
				[
					-13.81640625,
					27.56640625
				],
				[
					-14.6171875,
					29.9296875
				],
				[
					-14.96484375,
					31.12890625
				],
				[
					-15.16015625,
					31.90234375
				],
				[
					-15.37890625,
					32.68359375
				],
				[
					-15.64453125,
					33.7734375
				],
				[
					-15.8671875,
					34.7890625
				],
				[
					-15.9453125,
					35.5625
				],
				[
					-16.3984375,
					37.0546875
				],
				[
					-16.3984375,
					37.78515625
				],
				[
					-16.3984375,
					38.390625
				],
				[
					-16.3984375,
					38.7890625
				],
				[
					-16.3984375,
					39.1875
				],
				[
					-16.3984375,
					39.5859375
				],
				[
					-16.3984375,
					39.984375
				],
				[
					-16.3984375,
					40.76953125
				],
				[
					-16.3984375,
					41.01171875
				],
				[
					-16.3984375,
					41.18359375
				],
				[
					-16.3984375,
					41.484375
				],
				[
					-16.3984375,
					41.7109375
				],
				[
					-16.3984375,
					41.87890625
				],
				[
					-16.3984375,
					42.2265625
				],
				[
					-16.3984375,
					42.625
				],
				[
					-16.3984375,
					43
				],
				[
					-16.3984375,
					43.39453125
				],
				[
					-16.3984375,
					43.79296875
				],
				[
					-16.3984375,
					44.19140625
				],
				[
					-16.3125,
					44.703125
				],
				[
					-16.05078125,
					45.43359375
				],
				[
					-15.87890625,
					48.18359375
				],
				[
					-15.87890625,
					49.09765625
				],
				[
					-15.87890625,
					49.85546875
				],
				[
					-15.87890625,
					50.8046875
				],
				[
					-15.87890625,
					51.90234375
				],
				[
					-15.87890625,
					52.9296875
				],
				[
					-15.87890625,
					54.87109375
				],
				[
					-15.87890625,
					55.671875
				],
				[
					-15.87890625,
					56.375
				],
				[
					-15.87890625,
					57.05859375
				],
				[
					-15.87890625,
					57.83203125
				],
				[
					-15.87890625,
					58.66015625
				],
				[
					-15.87890625,
					59.3828125
				],
				[
					-15.87890625,
					61.2421875
				],
				[
					-15.87890625,
					61.71484375
				],
				[
					-15.87890625,
					62.44921875
				],
				[
					-15.87890625,
					63.10546875
				],
				[
					-15.87890625,
					63.65234375
				],
				[
					-15.87890625,
					65.13671875
				],
				[
					-15.87890625,
					66.4375
				],
				[
					-15.87890625,
					66.8359375
				],
				[
					-15.87890625,
					67.41796875
				],
				[
					-15.87890625,
					68.12890625
				],
				[
					-15.87890625,
					68.65234375
				],
				[
					-15.87890625,
					69.04296875
				],
				[
					-15.87890625,
					70.22265625
				],
				[
					-15.87890625,
					70.67578125
				],
				[
					-15.87890625,
					71.08203125
				],
				[
					-15.87890625,
					71.4765625
				],
				[
					-15.87890625,
					71.87109375
				],
				[
					-15.87890625,
					72.2734375
				],
				[
					-15.87890625,
					72.671875
				],
				[
					-15.87890625,
					73.01171875
				],
				[
					-15.87890625,
					73.30859375
				],
				[
					-15.87890625,
					73.56640625
				],
				[
					-15.87890625,
					73.72265625
				],
				[
					-15.87890625,
					73.8828125
				],
				[
					-15.98828125,
					74.14453125
				],
				[
					-16.29296875,
					74.3828125
				],
				[
					-17.08984375,
					74.59375
				],
				[
					-17.5,
					74.92578125
				],
				[
					-17.87890625,
					75.30078125
				],
				[
					-18.546875,
					75.5390625
				],
				[
					-19.28515625,
					75.74609375
				],
				[
					-19.953125,
					76.125
				],
				[
					-20.9140625,
					76.625
				],
				[
					-22.671875,
					77.3046875
				],
				[
					-23.77734375,
					77.82421875
				],
				[
					-24.87890625,
					78.109375
				],
				[
					-25.97265625,
					78.37109375
				],
				[
					-26.984375,
					78.63671875
				],
				[
					-27.75,
					78.82421875
				],
				[
					-28.59375,
					79.0546875
				],
				[
					-30.3359375,
					79.6015625
				],
				[
					-31.06640625,
					79.86328125
				],
				[
					-31.828125,
					80.14453125
				],
				[
					-32.5703125,
					80.51171875
				],
				[
					-33.140625,
					80.83203125
				],
				[
					-34.4921875,
					81.04296875
				],
				[
					-35.00390625,
					81.23046875
				],
				[
					-35.40234375,
					81.43359375
				],
				[
					-35.8125,
					81.62109375
				],
				[
					-36.23828125,
					81.8515625
				],
				[
					-36.62109375,
					82.0390625
				],
				[
					-36.78125,
					82.0390625
				],
				[
					-36.78515625,
					82.18359375
				],
				[
					-36.78515625,
					82.44921875
				],
				[
					-36.78515625,
					82.57421875
				],
				[
					-36.609375,
					82.8359375
				],
				[
					-35.82421875,
					82.83984375
				],
				[
					-35.09375,
					83.1015625
				],
				[
					-34.328125,
					83.35546875
				],
				[
					-33.546875,
					83.35546875
				],
				[
					-31.75,
					83.35546875
				],
				[
					-30.25390625,
					83.35546875
				],
				[
					-29.5234375,
					83.35546875
				],
				[
					-28.77734375,
					83.35546875
				],
				[
					-28.04296875,
					83.35546875
				],
				[
					-27.265625,
					83.4921875
				],
				[
					-25.45703125,
					83.9921875
				],
				[
					-24.70703125,
					84.34765625
				],
				[
					-23.73828125,
					84.68359375
				],
				[
					-22.625,
					84.9765625
				],
				[
					-21.81640625,
					85.3671875
				],
				[
					-21.375,
					85.7421875
				],
				[
					-20.671875,
					85.9921875
				],
				[
					-19.9453125,
					86.19140625
				],
				[
					-19.0546875,
					86.625
				],
				[
					-18.65625,
					86.828125
				],
				[
					-18.28125,
					87.015625
				],
				[
					-17.9609375,
					87.3359375
				],
				[
					-17.81640625,
					87.59765625
				],
				[
					-17.81640625,
					87.7265625
				],
				[
					-17.81640625,
					87.86328125
				],
				[
					-17.81640625,
					87.99609375
				],
				[
					-17.81640625,
					88.13671875
				],
				[
					-17.81640625,
					88.29296875
				],
				[
					-17.81640625,
					88.4375
				],
				[
					-17.81640625,
					88.75
				],
				[
					-17.81640625,
					89.15625
				],
				[
					-17.81640625,
					89.578125
				],
				[
					-17.81640625,
					90.37109375
				],
				[
					-17.81640625,
					91.171875
				],
				[
					-17.81640625,
					91.5703125
				],
				[
					-17.81640625,
					92.0625
				],
				[
					-17.81640625,
					92.7890625
				],
				[
					-17.81640625,
					93.546875
				],
				[
					-17.81640625,
					95.3671875
				],
				[
					-17.953125,
					96.12890625
				],
				[
					-18.21875,
					97.0546875
				],
				[
					-18.34765625,
					97.94921875
				],
				[
					-18.34765625,
					98.71484375
				],
				[
					-18.53125,
					99.6796875
				],
				[
					-18.796875,
					100.765625
				],
				[
					-18.87890625,
					102.66796875
				],
				[
					-18.87890625,
					103.40625
				],
				[
					-18.87890625,
					104.34765625
				],
				[
					-18.87890625,
					105.46875
				],
				[
					-18.87890625,
					106.32421875
				],
				[
					-18.87890625,
					107.109375
				],
				[
					-18.87890625,
					108.21875
				],
				[
					-18.87890625,
					110.3984375
				],
				[
					-18.87890625,
					111.4921875
				],
				[
					-18.87890625,
					112.59375
				],
				[
					-18.87890625,
					113.86328125
				],
				[
					-18.87890625,
					115.43359375
				],
				[
					-18.87890625,
					116.8359375
				],
				[
					-18.87890625,
					117.93359375
				],
				[
					-18.87890625,
					120.86328125
				],
				[
					-18.87890625,
					122.45703125
				],
				[
					-18.87890625,
					124.33203125
				],
				[
					-18.87890625,
					126.4453125
				],
				[
					-18.87890625,
					128.140625
				],
				[
					-18.87890625,
					129.69921875
				],
				[
					-18.87890625,
					131.6015625
				],
				[
					-18.87890625,
					135.77734375
				],
				[
					-18.87890625,
					137.76953125
				],
				[
					-18.87890625,
					139.8671875
				],
				[
					-18.87890625,
					141.7890625
				],
				[
					-18.87890625,
					143.4140625
				],
				[
					-18.82421875,
					145.515625
				],
				[
					-18.4921875,
					147.62109375
				],
				[
					-17.70703125,
					151.7890625
				],
				[
					-17.125,
					153.8671875
				],
				[
					-16.23828125,
					158.39453125
				],
				[
					-15.6328125,
					161.10546875
				],
				[
					-15.234375,
					163.53125
				],
				[
					-14.71484375,
					165.609375
				],
				[
					-13.3203125,
					171.8125
				],
				[
					-12.8515625,
					173.96875
				],
				[
					-12.5390625,
					175.70703125
				],
				[
					-12,
					177.32421875
				],
				[
					-11.375,
					179.14453125
				],
				[
					-10.98828125,
					180.68359375
				],
				[
					-9.6796875,
					185.79296875
				],
				[
					-9.390625,
					187.3515625
				],
				[
					-8.88671875,
					188.44921875
				],
				[
					-8.60546875,
					189.53515625
				],
				[
					-8.34375,
					190.625
				],
				[
					-8.05078125,
					191.734375
				],
				[
					-6.95703125,
					196.12109375
				],
				[
					-6.6953125,
					197.2109375
				],
				[
					-6.453125,
					198.1171875
				],
				[
					-6.265625,
					198.88671875
				],
				[
					-6.01171875,
					199.83984375
				],
				[
					-5.75,
					200.9375
				],
				[
					-5.453125,
					202.54296875
				],
				[
					-5.19140625,
					203.55078125
				],
				[
					-4.953125,
					204.5546875
				],
				[
					-4.69140625,
					205.3359375
				],
				[
					-4.6171875,
					206.08984375
				],
				[
					-4.35546875,
					207.1796875
				],
				[
					-4.07421875,
					208.41015625
				],
				[
					-3.390625,
					211.53515625
				],
				[
					-3.12890625,
					212.63671875
				],
				[
					-2.91015625,
					213.734375
				],
				[
					-2.8359375,
					214.82421875
				],
				[
					-2.57421875,
					215.921875
				],
				[
					-2.390625,
					217.0234375
				],
				[
					-2.24609375,
					218.32421875
				],
				[
					-1.7265625,
					221.26953125
				],
				[
					-1.58203125,
					222.3515625
				],
				[
					-1.3203125,
					223.44921875
				],
				[
					-1.203125,
					224.33203125
				],
				[
					-1.203125,
					225.0859375
				],
				[
					-1.0390625,
					226.01171875
				],
				[
					-0.77734375,
					227.0625
				],
				[
					-0.453125,
					229.3046875
				],
				[
					-0.19140625,
					230.44140625
				],
				[
					0.28515625,
					232.50390625
				],
				[
					0.5546875,
					233.4140625
				],
				[
					0.73828125,
					234.16796875
				],
				[
					0.76953125,
					235.2109375
				],
				[
					1.1640625,
					236.71875
				],
				[
					1.3515625,
					237.48046875
				],
				[
					1.55859375,
					238.2109375
				],
				[
					1.74609375,
					238.9765625
				],
				[
					1.8671875,
					239.70703125
				],
				[
					1.8671875,
					240.3046875
				],
				[
					1.96484375,
					240.703125
				],
				[
					2.3515625,
					242.01953125
				],
				[
					2.7109375,
					242.76953125
				],
				[
					3.05078125,
					243.5078125
				],
				[
					3.14453125,
					244.03125
				],
				[
					3.28125,
					244.4140625
				],
				[
					3.46875,
					244.7890625
				],
				[
					3.640625,
					245.15234375
				],
				[
					3.828125,
					245.5234375
				],
				[
					4.21875,
					246.36328125
				],
				[
					4.28125,
					246.80859375
				],
				[
					4.46875,
					247.20703125
				],
				[
					4.6796875,
					247.609375
				],
				[
					4.8671875,
					247.96875
				],
				[
					5.1171875,
					248.21875
				],
				[
					5.2734375,
					248.375
				],
				[
					5.6640625,
					248.4375
				],
				[
					5.9140625,
					248.4375
				],
				[
					6.1328125,
					248.4375
				],
				[
					6.390625,
					248.4375
				],
				[
					6.7421875,
					248.4375
				],
				[
					7.140625,
					248.4375
				],
				[
					7.5390625,
					248.4375
				],
				[
					8.33203125,
					248.4375
				],
				[
					8.71875,
					248.4375
				],
				[
					9.10546875,
					248.4375
				],
				[
					9.4453125,
					248.5390625
				],
				[
					9.7734375,
					248.70703125
				],
				[
					10.171875,
					248.7734375
				],
				[
					10.4375,
					248.7734375
				],
				[
					10.484375,
					248.51953125
				],
				[
					10.484375,
					248.07421875
				],
				[
					10.484375,
					248.07421875
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				10.484375,
				248.07421875
			]
		},
		{
			"id": "kc-7islf0vT_PEzzXjPEL",
			"type": "freedraw",
			"x": 693.49609375,
			"y": 1985.5234375,
			"width": 0.0001,
			"height": 0.0001,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 929350938,
			"version": 3,
			"versionNonce": 1312100550,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697788302292,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				0.0001,
				0.0001
			]
		},
		{
			"id": "5zEUwACg",
			"type": "text",
			"x": 380.90625,
			"y": 2069.4609375,
			"width": 505.15960693359375,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1362234522,
			"version": 36,
			"versionNonce": 1500343366,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789603641,
			"link": null,
			"locked": false,
			"text": "xhr.open(https://api.bilibili.com/x/v2/reply/add,'post')",
			"rawText": "xhr.open(https://api.bilibili.com/x/v2/reply/add,'post')",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "xhr.open(https://api.bilibili.com/x/v2/reply/add,'post')",
			"lineHeight": 1.25
		},
		{
			"id": "c1gkVrOx",
			"type": "text",
			"x": 396.35546875,
			"y": 2111.44140625,
			"width": 92.7799072265625,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1512401562,
			"version": 59,
			"versionNonce": 1422678470,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789604398,
			"link": null,
			"locked": false,
			"text": "xhr.send()",
			"rawText": "xhr.send()",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "xhr.send()",
			"lineHeight": 1.25
		},
		{
			"id": "BTSpwZ6x",
			"type": "text",
			"x": 409.12109375,
			"y": 2162.140625,
			"width": 280,
			"height": 75,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 609214662,
			"version": 178,
			"versionNonce": 2016356742,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789605547,
			"link": null,
			"locked": false,
			"text": "xhr.onload = ()=>{\n    请求完成后进行触发的操作\n}",
			"rawText": "xhr.onload = ()=>{\n    请求完成后进行触发的操作\n}",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 68,
			"containerId": null,
			"originalText": "xhr.onload = ()=>{\n    请求完成后进行触发的操作\n}",
			"lineHeight": 1.25
		},
		{
			"id": "7LHa5WPE",
			"type": "text",
			"x": 149.4921875,
			"y": 2387.79296875,
			"width": 700.260009765625,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1417750234,
			"version": 172,
			"versionNonce": 253152730,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789142166,
			"link": null,
			"locked": false,
			"text": "浏览器的一个策略: 同源策略,只要上面有一个不一样,浏览器就不接收响应, 跨域",
			"rawText": "浏览器的一个策略: 同源策略,只要上面有一个不一样,浏览器就不接收响应, 跨域",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "浏览器的一个策略: 同源策略,只要上面有一个不一样,浏览器就不接收响应, 跨域",
			"lineHeight": 1.25
		},
		{
			"id": "pcEgewk1",
			"type": "text",
			"x": 164.16796875,
			"y": 2307.140625,
			"width": 409.53985595703125,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1013530906,
			"version": 58,
			"versionNonce": 1874304454,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789173319,
			"link": null,
			"locked": false,
			"text": "url:   https  协议    ip=>域名      端口  ",
			"rawText": "url:   https  协议    ip=>域名      端口  ",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "url:   https  协议    ip=>域名      端口  ",
			"lineHeight": 1.25
		},
		{
			"id": "TfSkX91e",
			"type": "text",
			"x": 355.0546875,
			"y": 2493.94140625,
			"width": 374.5397644042969,
			"height": 100,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1452188422,
			"version": 116,
			"versionNonce": 964564378,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789500719,
			"link": null,
			"locked": false,
			"text": "cors 跨域 :  前端: webpack: dev server\n\n\n             cors: 后端的中间件",
			"rawText": "cors 跨域 :  前端: webpack: dev server\n\n\n             cors: 后端的中间件",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 93,
			"containerId": null,
			"originalText": "cors 跨域 :  前端: webpack: dev server\n\n\n             cors: 后端的中间件",
			"lineHeight": 1.25
		},
		{
			"id": "VZ_G27RO4fgF9iVKNXigd",
			"type": "rectangle",
			"x": 475.33203125,
			"y": 1767.81640625,
			"width": 57.30078125,
			"height": 136.05078125,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 1859140314,
			"version": 77,
			"versionNonce": 516232794,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "eX5K4aaj"
				},
				{
					"id": "UPK4_uWGswqZvI3PePj4-",
					"type": "arrow"
				},
				{
					"id": "Ky3VrgqJDfszZ5p6PWaqz",
					"type": "arrow"
				}
			],
			"updated": 1697789381744,
			"link": null,
			"locked": false
		},
		{
			"id": "eX5K4aaj",
			"type": "text",
			"x": 484.00244140625,
			"y": 1810.841796875,
			"width": 39.9599609375,
			"height": 50,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 766272538,
			"version": 10,
			"versionNonce": 521843462,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789218827,
			"link": null,
			"locked": false,
			"text": "clien\nt",
			"rawText": "client",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 43,
			"containerId": "VZ_G27RO4fgF9iVKNXigd",
			"originalText": "client",
			"lineHeight": 1.25
		},
		{
			"id": "SwSpqv-RsJ8VVgsAH_EUX",
			"type": "rectangle",
			"x": 652.26171875,
			"y": 1760.84375,
			"width": 109.6484375,
			"height": 143.06640625,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 1968538202,
			"version": 73,
			"versionNonce": 1861641306,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "UPK4_uWGswqZvI3PePj4-",
					"type": "arrow"
				},
				{
					"id": "OhiJvXPtDWTdyMLOYMqT_",
					"type": "arrow"
				}
			],
			"updated": 1697789254008,
			"link": null,
			"locked": false
		},
		{
			"id": "DJ4GZAoRp6f5sPw5xMECc",
			"type": "rectangle",
			"x": 317.48046875,
			"y": 1699.33203125,
			"width": 126.01953125,
			"height": 137.74609375,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 225159514,
			"version": 135,
			"versionNonce": 885623962,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "Cj5ENzjX"
				},
				{
					"id": "OhiJvXPtDWTdyMLOYMqT_",
					"type": "arrow"
				},
				{
					"id": "Ky3VrgqJDfszZ5p6PWaqz",
					"type": "arrow"
				},
				{
					"id": "HN-hK9Iw7YjWTUEhVkWWN",
					"type": "arrow"
				}
			],
			"updated": 1697789879574,
			"link": null,
			"locked": false
		},
		{
			"id": "Cj5ENzjX",
			"type": "text",
			"x": 375.41024017333984,
			"y": 1755.705078125,
			"width": 10.159988403320312,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 401603270,
			"version": 78,
			"versionNonce": 1193691974,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789881929,
			"link": null,
			"locked": false,
			"text": "b",
			"rawText": "b",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "DJ4GZAoRp6f5sPw5xMECc",
			"originalText": "b",
			"lineHeight": 1.25
		},
		{
			"id": "olJF420h",
			"type": "text",
			"x": 668.48828125,
			"y": 1826.96875,
			"width": 60.399932861328125,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 858720454,
			"version": 7,
			"versionNonce": 1205211930,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789223663,
			"link": null,
			"locked": false,
			"text": "server",
			"rawText": "server",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "server",
			"lineHeight": 1.25
		},
		{
			"id": "UPK4_uWGswqZvI3PePj4-",
			"type": "arrow",
			"x": 533.9609375,
			"y": 1793.0261816508414,
			"width": 115.203125,
			"height": 13.900575441131423,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1256952986,
			"version": 173,
			"versionNonce": 1492400006,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789247782,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					115.203125,
					13.900575441131423
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "VZ_G27RO4fgF9iVKNXigd",
				"focus": -0.6497753208097322,
				"gap": 1.328125
			},
			"endBinding": {
				"elementId": "SwSpqv-RsJ8VVgsAH_EUX",
				"focus": 0.2362334408784866,
				"gap": 3.09765625
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "OhiJvXPtDWTdyMLOYMqT_",
			"type": "arrow",
			"x": 645.2421875,
			"y": 1813.4508735193026,
			"width": 183.21875,
			"height": 26.687492364487525,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1350864390,
			"version": 196,
			"versionNonce": 577172058,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789892514,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-183.21875,
					-26.687492364487525
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "SwSpqv-RsJ8VVgsAH_EUX",
				"gap": 7.01953125,
				"focus": 0.12480546075085325
			},
			"endBinding": {
				"elementId": "DJ4GZAoRp6f5sPw5xMECc",
				"gap": 18.5234375,
				"focus": 0.08561381618126648
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "pxCxqJ9uhbfFr6X6ys48H",
			"type": "arrow",
			"x": 495.640625,
			"y": 2086.75390625,
			"width": 48.44921875,
			"height": 17.0703125,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1645230534,
			"version": 237,
			"versionNonce": 869616090,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789290611,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					48.44921875,
					-17.0703125
				],
				[
					5.45703125,
					-13.4453125
				]
			],
			"lastCommittedPoint": [
				5.45703125,
				-13.4453125
			],
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "Ky3VrgqJDfszZ5p6PWaqz",
			"type": "arrow",
			"x": 495.56296245021184,
			"y": 1759.84375,
			"width": 41.84811870021184,
			"height": 29.72264544094287,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1487817158,
			"version": 225,
			"versionNonce": 196977626,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789892514,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-41.84811870021184,
					-29.72264544094287
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "VZ_G27RO4fgF9iVKNXigd",
				"gap": 7.97265625,
				"focus": 0.7925706641401195
			},
			"endBinding": {
				"elementId": "DJ4GZAoRp6f5sPw5xMECc",
				"gap": 10.21484375,
				"focus": -0.792881688898061
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "GxzLrTiS",
			"type": "text",
			"x": 481.48828125,
			"y": 2635.79296875,
			"width": 209.5598907470703,
			"height": 75,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1935808858,
			"version": 55,
			"versionNonce": 736942938,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789551136,
			"link": null,
			"locked": false,
			"text": "nginx 进行转发: server\n\n       ",
			"rawText": "nginx 进行转发: server\n\n       ",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 68,
			"containerId": null,
			"originalText": "nginx 进行转发: server\n\n       ",
			"lineHeight": 1.25
		},
		{
			"id": "2IxfukHo",
			"type": "text",
			"x": -219.3046875,
			"y": 1902.73046875,
			"width": 50.89994812011719,
			"height": 50,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 886219162,
			"version": 63,
			"versionNonce": 595924486,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789601236,
			"link": null,
			"locked": false,
			"text": "axios\n",
			"rawText": "axios\n",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 43,
			"containerId": null,
			"originalText": "axios\n",
			"lineHeight": 1.25
		},
		{
			"id": "haxv0P9187RDlFQNfmKiT",
			"type": "arrow",
			"x": -93.44921875,
			"y": 1960.68359375,
			"width": 315.55859375,
			"height": 118.44140625,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1213719642,
			"version": 44,
			"versionNonce": 1427508934,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789566636,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					315.55859375,
					118.44140625
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": {
				"elementId": "3RNUuNRV",
				"focus": -1.0004668824949137,
				"gap": 1.66796875
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "YfcCV6Xl7kJpwZXGwDVjo",
			"type": "rectangle",
			"x": 135.25,
			"y": 1766.55078125,
			"width": 93.52734375,
			"height": 84.140625,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 304032198,
			"version": 99,
			"versionNonce": 1742729670,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "TVYi32gE"
				},
				{
					"id": "Z771Nz5jbUSkbowrPp82W",
					"type": "arrow"
				},
				{
					"id": "gkL723QjYOsYqLzYFMMEA",
					"type": "arrow"
				},
				{
					"id": "HN-hK9Iw7YjWTUEhVkWWN",
					"type": "arrow"
				}
			],
			"updated": 1697789895445,
			"link": null,
			"locked": false
		},
		{
			"id": "TVYi32gE",
			"type": "text",
			"x": 175.3436737060547,
			"y": 1796.12109375,
			"width": 13.339996337890625,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 422471942,
			"version": 65,
			"versionNonce": 784162266,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789895434,
			"link": null,
			"locked": false,
			"text": "a",
			"rawText": "a",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "YfcCV6Xl7kJpwZXGwDVjo",
			"originalText": "a",
			"lineHeight": 1.25
		},
		{
			"id": "Z771Nz5jbUSkbowrPp82W",
			"type": "arrow",
			"x": 233.1328125,
			"y": 1787.283772075344,
			"width": 92.98046875,
			"height": 26.209553325343904,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1729437894,
			"version": 89,
			"versionNonce": 1304990362,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789895434,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					92.98046875,
					-26.209553325343904
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "YfcCV6Xl7kJpwZXGwDVjo",
				"gap": 4.35546875,
				"focus": -0.12538400720164988
			},
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "HN-hK9Iw7YjWTUEhVkWWN",
			"type": "arrow",
			"x": 315.8671875,
			"y": 1813.6904407570078,
			"width": 82.0859375,
			"height": 27.270496742992236,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1611228506,
			"version": 22,
			"versionNonce": 1471951494,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789895445,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-82.0859375,
					27.270496742992236
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "DJ4GZAoRp6f5sPw5xMECc",
				"gap": 1.61328125,
				"focus": -0.2674247408621128
			},
			"endBinding": {
				"elementId": "YfcCV6Xl7kJpwZXGwDVjo",
				"focus": 0.8599440229193993,
				"gap": 5.00390625
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "gkL723QjYOsYqLzYFMMEA",
			"type": "arrow",
			"x": 187.48900840954883,
			"y": 1756.95703125,
			"width": 137.00708534045117,
			"height": 40.8671875,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 552335258,
			"version": 201,
			"versionNonce": 1997483866,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1697789895434,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					137.00708534045117,
					-40.8671875
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "YfcCV6Xl7kJpwZXGwDVjo",
				"gap": 9.59375,
				"focus": -0.8931014526449658
			},
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "L3pfIPRu",
			"type": "text",
			"x": 6.45703125,
			"y": 1780.76171875,
			"width": 98.2799072265625,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1752748314,
			"version": 19,
			"versionNonce": 227435974,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1697788245630,
			"link": null,
			"locked": false,
			"text": "car.drive()",
			"rawText": "car.drive()",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "car.drive()",
			"lineHeight": 1.25
		},
		{
			"id": "617C63us",
			"type": "text",
			"x": 488.45703125,
			"y": 1833.76171875,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 894754778,
			"version": 2,
			"versionNonce": 938007046,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1697788260491,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "5MjsUtcH",
			"type": "text",
			"x": 604.48828125,
			"y": 1745.96875,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 378674886,
			"version": 3,
			"versionNonce": 2005580314,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1697788326960,
			"link": null,
			"locked": false,
			"text": " ",
			"rawText": " ",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": " ",
			"lineHeight": 1.25
		},
		{
			"id": "Iw2ks78l",
			"type": "text",
			"x": 230.48828125,
			"y": 2383.96875,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1732302362,
			"version": 2,
			"versionNonce": 2065084358,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1697788645541,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "phmKZ6bO",
			"type": "text",
			"x": 450.48828125,
			"y": 2398.96875,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 938771462,
			"version": 2,
			"versionNonce": 1077947418,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1697789089341,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "Z2Xrgo4e",
			"type": "text",
			"x": 444.48828125,
			"y": 2485.96875,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1377697498,
			"version": 2,
			"versionNonce": 1498614534,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1697789138536,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "6sohZrwj",
			"type": "text",
			"x": 433.48828125,
			"y": 2490.96875,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1189380486,
			"version": 2,
			"versionNonce": 1770092186,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1697789139366,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "tYGh90xQilT5k8kO-fQmg",
			"type": "rectangle",
			"x": 756.390625,
			"y": 1813.3125,
			"width": 53.16796875,
			"height": 13.1953125,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 962319366,
			"version": 76,
			"versionNonce": 184456090,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1697789241861,
			"link": null,
			"locked": false
		},
		{
			"id": "wo9gh4KK",
			"type": "text",
			"x": -122.75,
			"y": 1966.12109375,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 2062744710,
			"version": 2,
			"versionNonce": 1254984602,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1697789569106,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		}
	],
	"appState": {
		"theme": "dark",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#1e1e1e",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "hachure",
		"currentItemStrokeWidth": 1,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 288.75,
		"scrollY": -1595.62109375,
		"zoom": {
			"value": 1
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"gridColor": {
			"Bold": "#C9C9C9FF",
			"Regular": "#EDEDEDFF"
		},
		"currentStrokeOptions": null,
		"previousGridSize": null,
		"frameRendering": {
			"enabled": true,
			"clip": true,
			"name": true,
			"outline": true
		}
	},
	"files": {}
}
```
%%