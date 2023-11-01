---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
BOOK info
 ^9oRbgy9v

title author genre >> string
ISBN  = ID for books >> string or int  
status bool ^fTi1ns0l

BOOK operation ^QjAcnulW

insert 
remove 
search
borrow
sort
statistics 
    total numbers of books
    available books
    borrowed books ^uDI4ZQsg

object
 ^Ya5KBgtH

Person who borrow the book ^DmuXSQBH

name >> string
id >> string or int
phone number >> int
school or collage >> string ^aCMp8Dth

object
 ^vaNcLQhv

May be finished ^Ep2udNf2

void set_tagi();
    void get_tagi();
    void set_status();
    void get_status();
    string return_title();
    string return_author();
    string return_genre();
    string return_ISBN();
    bool return_status(); ^EXEiKoAx

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.26",
	"elements": [
		{
			"type": "text",
			"version": 334,
			"versionNonce": 813223062,
			"isDeleted": false,
			"id": "9oRbgy9v",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -651.9631551854746,
			"y": 87.53045160630174,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 101.681048224954,
			"height": 50.657946491607284,
			"seed": 1315477,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 20.263178596642916,
			"fontFamily": 1,
			"text": "BOOK info\n",
			"rawText": "BOOK info\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BOOK info\n",
			"lineHeight": 1.25,
			"baseline": 41.99999999999999
		},
		{
			"type": "rectangle",
			"version": 628,
			"versionNonce": 538888662,
			"isDeleted": false,
			"id": "IF-Rs2P2MfFxXFS2e2cK2",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -787.1837434207688,
			"y": 122.72162807688997,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 420,
			"height": 359.8235294117646,
			"seed": 1019247061,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "7M7ukjC-wz5hYWrgZm0rm",
					"type": "arrow"
				}
			],
			"updated": 1698432219721,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 403,
			"versionNonce": 1016274710,
			"isDeleted": false,
			"id": "fTi1ns0l",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -760.4043316560629,
			"y": 146.01574572394884,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 400.2396240234375,
			"height": 75,
			"seed": 1074947989,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "title author genre >> string\nISBN  = ID for books >> string or int  \nstatus bool",
			"rawText": "title author genre >> string\nISBN  = ID for books >> string or int  \nstatus bool",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "title author genre >> string\nISBN  = ID for books >> string or int  \nstatus bool",
			"lineHeight": 1.25,
			"baseline": 68
		},
		{
			"type": "rectangle",
			"version": 375,
			"versionNonce": 172674134,
			"isDeleted": false,
			"id": "mAwhHHDHH4o42wGFHr8S5",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1378.4280630279986,
			"y": 256.92751042983116,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 464,
			"height": 298.5,
			"seed": 588581115,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "7M7ukjC-wz5hYWrgZm0rm",
					"type": "arrow"
				},
				{
					"id": "FncHSVlTDnU5fX9UlRWRi",
					"type": "arrow"
				}
			],
			"updated": 1698432219721,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 205,
			"versionNonce": 741860374,
			"isDeleted": false,
			"id": "QjAcnulW",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1251.4280630279986,
			"y": 199.17751042983116,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 218.06491088867188,
			"height": 35,
			"seed": 1705523675,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 28,
			"fontFamily": 1,
			"text": "BOOK operation",
			"rawText": "BOOK operation",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BOOK operation",
			"lineHeight": 1.25,
			"baseline": 25
		},
		{
			"type": "text",
			"version": 279,
			"versionNonce": 319746390,
			"isDeleted": false,
			"id": "uDI4ZQsg",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1349.4280630279986,
			"y": 304.17751042983116,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 269.919677734375,
			"height": 225,
			"seed": 1693768117,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "insert \nremove \nsearch\nborrow\nsort\nstatistics \n    total numbers of books\n    available books\n    borrowed books",
			"rawText": "insert \nremove \nsearch\nborrow\nsort\nstatistics \n    total numbers of books\n    available books\n    borrowed books",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "insert \nremove \nsearch\nborrow\nsort\nstatistics \n    total numbers of books\n    available books\n    borrowed books",
			"lineHeight": 1.25,
			"baseline": 218
		},
		{
			"type": "arrow",
			"version": 1848,
			"versionNonce": 750319626,
			"isDeleted": false,
			"id": "7M7ukjC-wz5hYWrgZm0rm",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -788.8254718219528,
			"y": 257.12456270869154,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 122.57352941176487,
			"height": 33.40556496088982,
			"seed": 1104494587,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698432219753,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "EXEiKoAx",
				"focus": 0.8639738963288136,
				"gap": 24.294531976475128
			},
			"endBinding": {
				"elementId": "mAwhHHDHH4o42wGFHr8S5",
				"focus": -0.24281919304049335,
				"gap": 3.029061794281006
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
					-122.57352941176487,
					33.40556496088982
				]
			]
		},
		{
			"type": "text",
			"version": 251,
			"versionNonce": 368514006,
			"isDeleted": false,
			"id": "Ya5KBgtH",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 6.097251897042594,
			"x": -880.3401777043059,
			"y": 241.3813881874085,
			"strokeColor": "#e03131",
			"backgroundColor": "transparent",
			"width": 60.07994079589844,
			"height": 50,
			"seed": 956100341,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "object\n",
			"rawText": "object\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "object\n",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "text",
			"version": 214,
			"versionNonce": 617752854,
			"isDeleted": false,
			"id": "DmuXSQBH",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -741.7533360649554,
			"y": 597.261398006888,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 382.28570556640625,
			"height": 35,
			"seed": 1155642043,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 28,
			"fontFamily": 1,
			"text": "Person who borrow the book",
			"rawText": "Person who borrow the book",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Person who borrow the book",
			"lineHeight": 1.25,
			"baseline": 25
		},
		{
			"type": "rectangle",
			"version": 368,
			"versionNonce": 1779996246,
			"isDeleted": false,
			"id": "XqheKMk_JsHZjF_C2GNOd",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -751.0033360649554,
			"y": 643.011398006888,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 310.75,
			"height": 211,
			"seed": 576616283,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 334,
			"versionNonce": 782195606,
			"isDeleted": false,
			"id": "aCMp8Dth",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -731.6951929260699,
			"y": 684.180831600638,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 257.7197265625,
			"height": 100,
			"seed": 490448187,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "name >> string\nid >> string or int\nphone number >> int\nschool or collage >> string",
			"rawText": "name >> string\nid >> string or int\nphone number >> int\nschool or collage >> string",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "name >> string\nid >> string or int\nphone number >> int\nschool or collage >> string",
			"lineHeight": 1.25,
			"baseline": 93
		},
		{
			"type": "arrow",
			"version": 926,
			"versionNonce": 129066698,
			"isDeleted": false,
			"id": "FncHSVlTDnU5fX9UlRWRi",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -747.068504759685,
			"y": 655.6638848325279,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 161.64454810214545,
			"height": 115.44906478032215,
			"seed": 1028531061,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1698432219753,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "mAwhHHDHH4o42wGFHr8S5",
				"focus": -0.11348687973453322,
				"gap": 5.715010166168213
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
					-161.64454810214545,
					-115.44906478032215
				]
			]
		},
		{
			"type": "text",
			"version": 298,
			"versionNonce": 1067576854,
			"isDeleted": false,
			"id": "vaNcLQhv",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.53885954192247,
			"x": -840.2530232597796,
			"y": 561.680831600638,
			"strokeColor": "#e03131",
			"backgroundColor": "transparent",
			"width": 60.07994079589844,
			"height": 50,
			"seed": 912892027,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "object\n",
			"rawText": "object\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "object\n",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "text",
			"version": 351,
			"versionNonce": 10992470,
			"isDeleted": false,
			"id": "Ep2udNf2",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -689.6831408809209,
			"y": 493.4315406154184,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 246.09375,
			"height": 33.6,
			"seed": 1256381269,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 28,
			"fontFamily": 3,
			"text": "May be finished",
			"rawText": "May be finished",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "May be finished",
			"lineHeight": 1.2,
			"baseline": 26
		},
		{
			"type": "text",
			"version": 191,
			"versionNonce": 1375854742,
			"isDeleted": false,
			"id": "EXEiKoAx",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -764.5309398454776,
			"y": 230.2525424536537,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 266.939697265625,
			"height": 225,
			"seed": 18265,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "7M7ukjC-wz5hYWrgZm0rm",
					"type": "arrow"
				}
			],
			"updated": 1698432219721,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "void set_tagi();\n    void get_tagi();\n    void set_status();\n    void get_status();\n    string return_title();\n    string return_author();\n    string return_genre();\n    string return_ISBN();\n    bool return_status();",
			"rawText": "void set_tagi();\n    void get_tagi();\n    void set_status();\n    void get_status();\n    string return_title();\n    string return_author();\n    string return_genre();\n    string return_ISBN();\n    bool return_status();",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "void set_tagi();\n    void get_tagi();\n    void set_status();\n    void get_status();\n    string return_title();\n    string return_author();\n    string return_genre();\n    string return_ISBN();\n    bool return_status();",
			"lineHeight": 1.25,
			"baseline": 218
		}
	],
	"appState": {
		"theme": "light",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#f08c00",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "solid",
		"currentItemStrokeWidth": 2,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 1811.5095022566184,
		"scrollY": 411.01657658464825,
		"zoom": {
			"value": 0.49999999999999983
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