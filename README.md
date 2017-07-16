# weibo-unsubscribe
batch unsubscribe 

1.网页端抓取批量取消关注的包

```
curl 'http://weibo.com/aj/f/unfollow?ajwvr=6&__rnd=1500178195301' -H 'Cookie: xxx' -H 'Origin: http://weibo.com' -H 'Accept-Encoding: gzip, deflate' -H 'Accept-Language: zh-CN,zh;q=0.8,en;q=0.6,zh-TW;q=0.4' -H 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.115 Safari/537.36' -H 'Content-Type: application/x-www-form-urlencoded' -H 'Accept: */*' -H 'Referer: http://weibo.com/6095056301/follow?rightmod=1&wvr=6' -H 'X-Requested-With: XMLHttpRequest' -H 'Connection: keep-alive' --data 'uid=2434102213%2c1744398934%2c2387878582%2c2456136577%2c5977030837%2c5206672203%2c2919523010%2c1440455352%2c1777780154%2c2920093012%2c5920619669%2c2920548362%2c6078699075&refer_flag=unfollow_all&_t=0' --compressed
```

2.手机端抓取关注列表
```
{
	"cardlistInfo": {
		"containerid": "231093_-_selffollowed",
		"title_top": "我的好友",
		"show_style": "1",
		"cardlist_head_cards": [{
			"head_type": 0,
			"head_type_name": "channel_list",
			"menu_scheme": "",
			"channel_list": [{
				"id": "231093_-_selfrecomm",
				"name": "推荐",
				"containerid": "231093_-_selfrecomm",
				"scheme": "",
				"must_show": 1,
				"default_add": 1
			}, {
				"id": "231093_-_selffollowed",
				"name": "全部关注",
				"containerid": "231093_-_selffollowed",
				"scheme": "",
				"must_show": 1,
				"default_add": 1
			}, {
				"id": "231093_-_lastmblog",
				"name": "最新发博",
				"containerid": "231093_-_lastmblog",
				"scheme": "",
				"must_show": 1,
				"default_add": 1
			}]
		}],
		"total": 20,
		"page_type": "03",
		"background": "",
		"cardlist_menus": [{
			"type": "button_menus_refresh",
			"name": "刷新"
		}, {
			"type": "gohome",
			"name": "返回首页",
			"params": {
				"scheme": "sinaweibo:\/\/gotohome"
			}
		}]
	},
	"cards": [{
		"card_style": 1,
		"card_type": 11,
		"card_group": [{
			"card_type": 31,
			"itemid": "2310930021_1_ _6095056301",
			"scheme": "sinaweibo:\/\/searchall?type=532&disable_search=1&disable_history=1",
			"desc": "搜全部关注",
			"openurl": ""
		}, {
			"card_type": 19,
			"col": 4,
			"group": [{
				"title_sub": "我的群",
				"pic": "https:\/\/h5.sinaimg.cn\/upload\/2017\/02\/07\/96\/wodequn.png",
				"scheme": "sinaweibo:\/\/grouplist"
			}, {
				"title_sub": "兴趣主页",
				"pic": "https:\/\/h5.sinaimg.cn\/upload\/2017\/02\/07\/96\/xingquzhuye.png",
				"scheme": "sinaweibo:\/\/cardlist?containerid=2305232"
			}, {
				"title_sub": "我的分组",
				"pic": "http:\/\/h5.sinaimg.cn\/upload\/2016\/05\/16\/13\/haoyouquan.png",
				"scheme": "sinaweibo:\/\/cardlist?containerid=231093_-_selfgroup"
			}, {
				"title_sub": "字母排序",
				"pic": "https:\/\/h5.sinaimg.cn\/upload\/2017\/02\/07\/96\/zimupaixu.png",
				"scheme": "sinaweibo:\/\/myallfollowerslist"
			}],
			"openurl": ""
		}],
		"openurl": ""
	}, {
		"card_type": 11,
		"title": "全部关注",
		"itemid": "2310930026_1_ _",
		"card_group": [{
			"card_type": 30,
			"itemid": "2310930026_1_ _2434102213",
			"scheme": "sinaweibo:\/\/userinfo?uid=2434102213",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "\/\/@感官君:哈哈哈哈天啦\/\/@warm_柒:我要看这个😂😂😂😂\/\/@蜜鱼mefish:不行了笑死了",
			"user": {
				"id": 2434102213,
				"screen_name": "我是豹纹君",
				"profile_image_url": "http:\/\/tvax4.sinaimg.cn\/crop.0.0.996.996.50\/911573c5ly8fdwx3gpkz4j20ro0rpq4i.jpg",
				"avatar_large": "http:\/\/tvax4.sinaimg.cn\/crop.0.0.996.996.180\/911573c5ly8fdwx3gpkz4j20ro0rpq4i.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 122,
				"mbtype": 0,
				"mbrank": 0,
				"remark": "",
				"friends_count": 399,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _2434102213",
				"oid": 2434102213,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=2434102213|uid:6095056301|follow:2434102213|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 2434102213,
					"need_follow": 1,
					"trend_ext": 2434102213,
					"trend_type": 42,
					"itemid": 2434102213
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _2434102213",
					"oid": 2434102213,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=2434102213|uid:6095056301|follow:2434102213"
				},
				"can_unfollow": 1,
				"relationship": 2
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _1744398934",
			"scheme": "sinaweibo:\/\/userinfo?uid=1744398934",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "所以我认识你就必须给你面子么？都是什么理论？我跟你之间的面子能值多少钱？",
			"user": {
				"id": 1744398934,
				"screen_name": "Hello耿小桃",
				"profile_image_url": "http:\/\/tvax1.sinaimg.cn\/crop.0.0.750.750.50\/67f96a56ly8fenmfx9wf3j20ku0kuwft.jpg",
				"avatar_large": "http:\/\/tvax1.sinaimg.cn\/crop.0.0.750.750.180\/67f96a56ly8fenmfx9wf3j20ku0kuwft.jpg",
				"verified": true,
				"verified_type": 0,
				"level": null,
				"followers_count": 745,
				"mbtype": 13,
				"mbrank": 2,
				"remark": "",
				"friends_count": 333,
				"icons": [{
					"url": "https:\/\/h5.sinaimg.cn\/upload\/2016\/09\/27\/494\/common_icon_membership_level2.png"
				}],
				"verified_type_ext": 0
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _1744398934",
				"oid": 1744398934,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=1744398934|uid:6095056301|follow:1744398934|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 1744398934,
					"need_follow": 1,
					"trend_ext": 1744398934,
					"trend_type": 42,
					"itemid": 1744398934
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _1744398934",
					"oid": 1744398934,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=1744398934|uid:6095056301|follow:1744398934"
				},
				"can_unfollow": 1,
				"relationship": 2
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _2387878582",
			"scheme": "sinaweibo:\/\/userinfo?uid=2387878582",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "\/\/@电影热搜令: \/\/@耗这口:\/\/@蒋ld:好运常在",
			"user": {
				"id": 2387878582,
				"screen_name": "全微博最忙的灯光师",
				"profile_image_url": "http:\/\/tvax2.sinaimg.cn\/crop.0.0.1002.1002.50\/8e5422b6ly8fhd6qe5maqj20ru0rudk0.jpg",
				"avatar_large": "http:\/\/tvax2.sinaimg.cn\/crop.0.0.1002.1002.180\/8e5422b6ly8fhd6qe5maqj20ru0rudk0.jpg",
				"verified": false,
				"verified_type": 200,
				"level": null,
				"followers_count": 1156,
				"mbtype": 0,
				"mbrank": 0,
				"remark": "",
				"friends_count": 159,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _2387878582",
				"oid": 2387878582,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=2387878582|uid:6095056301|follow:2387878582|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 2387878582,
					"need_follow": 1,
					"trend_ext": 2387878582,
					"trend_type": 42,
					"itemid": 2387878582
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _2387878582",
					"oid": 2387878582,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=2387878582|uid:6095056301|follow:2387878582"
				},
				"can_unfollow": 1,
				"relationship": 2
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _2456136577",
			"scheme": "sinaweibo:\/\/userinfo?uid=2456136577",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "\/\/@-夏明明:\/\/@舒淇:🙏🙏🙏請善待牠們求求您🙏🙏🙏",
			"user": {
				"id": 2456136577,
				"screen_name": "大大大大大大铭子",
				"profile_image_url": "http:\/\/tvax4.sinaimg.cn\/crop.0.0.512.512.50\/9265ab81ly8fhcg1e0lhkj20e80e8t97.jpg",
				"avatar_large": "http:\/\/tvax4.sinaimg.cn\/crop.0.0.512.512.180\/9265ab81ly8fhcg1e0lhkj20e80e8t97.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 1890,
				"mbtype": 11,
				"mbrank": 2,
				"remark": "",
				"friends_count": 172,
				"icons": [{
					"url": "https:\/\/h5.sinaimg.cn\/upload\/2016\/09\/27\/494\/common_icon_membership_level2.png"
				}],
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _2456136577",
				"oid": 2456136577,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=2456136577|uid:6095056301|follow:2456136577|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 2456136577,
					"need_follow": 1,
					"trend_ext": 2456136577,
					"trend_type": 42,
					"itemid": 2456136577
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _2456136577",
					"oid": 2456136577,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=2456136577|uid:6095056301|follow:2456136577"
				},
				"can_unfollow": 1,
				"relationship": 2
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _5977030837",
			"scheme": "sinaweibo:\/\/userinfo?uid=5977030837",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "当你还在犹豫的时候 有的人已经开始行动了\n当你刚刚行动的时候 有的人已经开始赚钱了\n你还在等什么？[思考]\n不要做追逐的人 要做让别人追逐的人❤️\n薇🎀【S121495】#信# 👈🏻👈🏻 ​​​",
			"user": {
				"id": 5977030837,
				"screen_name": "梓沐沐_H",
				"profile_image_url": "http:\/\/tva2.sinaimg.cn\/crop.4.0.1234.1234.50\/006wv0Lbjw8fck3oplp0ej30yi0yaadc.jpg",
				"avatar_large": "http:\/\/tva2.sinaimg.cn\/crop.4.0.1234.1234.180\/006wv0Lbjw8fck3oplp0ej30yi0yaadc.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 700,
				"mbtype": 0,
				"mbrank": 0,
				"remark": "",
				"friends_count": 1933,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _5977030837",
				"oid": 5977030837,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=5977030837|uid:6095056301|follow:5977030837|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 5977030837,
					"need_follow": 1,
					"trend_ext": 5977030837,
					"trend_type": 42,
					"itemid": 5977030837
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _5977030837",
					"oid": 5977030837,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=5977030837|uid:6095056301|follow:5977030837"
				},
				"can_unfollow": 1,
				"relationship": 2
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _5206672203",
			"scheme": "sinaweibo:\/\/userinfo?uid=5206672203",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "50kg 5x5开练[加油] http:\/\/t.cn\/z8AdrTF http:\/\/t.cn\/Ro4n4qG",
			"user": {
				"id": 5206672203,
				"screen_name": "翁英健啊",
				"profile_image_url": "http:\/\/tva4.sinaimg.cn\/crop.0.0.512.512.50\/005GmFhVjw8fd77u7xqa4j30e80e8wen.jpg",
				"avatar_large": "http:\/\/tva4.sinaimg.cn\/crop.0.0.512.512.180\/005GmFhVjw8fd77u7xqa4j30e80e8wen.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 82,
				"mbtype": 2,
				"mbrank": 1,
				"remark": "",
				"friends_count": 89,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _5206672203",
				"oid": 5206672203,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=5206672203|uid:6095056301|follow:5206672203|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 5206672203,
					"need_follow": 1,
					"trend_ext": 5206672203,
					"trend_type": 42,
					"itemid": 5206672203
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _5206672203",
					"oid": 5206672203,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=5206672203|uid:6095056301|follow:5206672203"
				},
				"can_unfollow": 1,
				"relationship": 3
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _2919523010",
			"scheme": "sinaweibo:\/\/userinfo?uid=2919523010",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "再得瑟！再得瑟就把你吃掉！~ http:\/\/t.cn\/RKOhdG6",
			"user": {
				"id": 2919523010,
				"screen_name": "1990年6月7日宏伯1980",
				"profile_image_url": "http:\/\/tva1.sinaimg.cn\/crop.0.0.180.180.50\/ae0462c2jw1e8qgp5bmzyj2050050aa8.jpg",
				"avatar_large": "http:\/\/tva1.sinaimg.cn\/crop.0.0.180.180.180\/ae0462c2jw1e8qgp5bmzyj2050050aa8.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 234,
				"mbtype": 0,
				"mbrank": 0,
				"remark": "",
				"friends_count": 1091,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _2919523010",
				"oid": 2919523010,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=2919523010|uid:6095056301|follow:2919523010|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 2919523010,
					"need_follow": 1,
					"trend_ext": 2919523010,
					"trend_type": 42,
					"itemid": 2919523010
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _2919523010",
					"oid": 2919523010,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=2919523010|uid:6095056301|follow:2919523010"
				},
				"can_unfollow": 1,
				"relationship": 3
			}],
			"desc2_struct": [{
				"name": "微博推荐",
				"scheme": "http:\/\/fansmore.biz.weibo.cn\/members\/order?FP=myfans"
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _1440455352",
			"scheme": "sinaweibo:\/\/userinfo?uid=1440455352",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "华安 今天(7月16日)天气：多云转小雨，24℃~36℃，东南风3-4级转≤3级，空气质量：轻度 (分享自@微心情)http:\/\/t.cn\/RJCeLtA华安",
			"user": {
				"id": 1440455352,
				"screen_name": "lady承允",
				"profile_image_url": "http:\/\/tva1.sinaimg.cn\/crop.0.0.180.180.50\/55db9ab8jw1e8qgp5bmzyj2050050aa8.jpg",
				"avatar_large": "http:\/\/tva1.sinaimg.cn\/crop.0.0.180.180.180\/55db9ab8jw1e8qgp5bmzyj2050050aa8.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 448,
				"mbtype": 0,
				"mbrank": 0,
				"remark": "",
				"friends_count": 1724,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _1440455352",
				"oid": 1440455352,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=1440455352|uid:6095056301|follow:1440455352|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 1440455352,
					"need_follow": 1,
					"trend_ext": 1440455352,
					"trend_type": 42,
					"itemid": 1440455352
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _1440455352",
					"oid": 1440455352,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=1440455352|uid:6095056301|follow:1440455352"
				},
				"can_unfollow": 1,
				"relationship": 3
			}],
			"desc2_struct": [{
				"name": "微博推荐",
				"scheme": "http:\/\/fansmore.biz.weibo.cn\/members\/order?FP=myfans"
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _1777780154",
			"scheme": "sinaweibo:\/\/userinfo?uid=1777780154",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "转发微博",
			"user": {
				"id": 1777780154,
				"screen_name": "18岁的俊誉Coco",
				"profile_image_url": "http:\/\/tva2.sinaimg.cn\/crop.0.0.180.180.50\/69f6c5bajw1e8qgp5bmzyj2050050aa8.jpg",
				"avatar_large": "http:\/\/tva2.sinaimg.cn\/crop.0.0.180.180.180\/69f6c5bajw1e8qgp5bmzyj2050050aa8.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 281,
				"mbtype": 0,
				"mbrank": 0,
				"remark": "",
				"friends_count": 323,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _1777780154",
				"oid": 1777780154,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=1777780154|uid:6095056301|follow:1777780154|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 1777780154,
					"need_follow": 1,
					"trend_ext": 1777780154,
					"trend_type": 42,
					"itemid": 1777780154
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _1777780154",
					"oid": 1777780154,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=1777780154|uid:6095056301|follow:1777780154"
				},
				"can_unfollow": 1,
				"relationship": 3
			}],
			"desc2_struct": [{
				"name": "微博推荐",
				"scheme": "http:\/\/fansmore.biz.weibo.cn\/members\/order?FP=myfans"
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _2920093012",
			"scheme": "sinaweibo:\/\/userinfo?uid=2920093012",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "孟津 今天(7月16日)天气：阵雨转阴，24℃~32℃，东风≤3级，空气质量：轻度 (分享自@微心情)http:\/\/t.cn\/RJCeLtA孟津",
			"user": {
				"id": 2920093012,
				"screen_name": "乐观的傲娇1991",
				"profile_image_url": "http:\/\/tva4.sinaimg.cn\/crop.0.0.180.180.50\/ae0d1554jw1e8qgp5bmzyj2050050aa8.jpg",
				"avatar_large": "http:\/\/tva4.sinaimg.cn\/crop.0.0.180.180.180\/ae0d1554jw1e8qgp5bmzyj2050050aa8.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 386,
				"mbtype": 0,
				"mbrank": 0,
				"remark": "",
				"friends_count": 2225,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _2920093012",
				"oid": 2920093012,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=2920093012|uid:6095056301|follow:2920093012|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 2920093012,
					"need_follow": 1,
					"trend_ext": 2920093012,
					"trend_type": 42,
					"itemid": 2920093012
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _2920093012",
					"oid": 2920093012,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=2920093012|uid:6095056301|follow:2920093012"
				},
				"can_unfollow": 1,
				"relationship": 3
			}],
			"desc2_struct": [{
				"name": "微博推荐",
				"scheme": "http:\/\/fansmore.biz.weibo.cn\/members\/order?FP=myfans"
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _5920619669",
			"scheme": "sinaweibo:\/\/userinfo?uid=5920619669",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "王思聪车展扫货 一年一次大旅行就够了 2美国·Waikiki Beach Hawaii",
			"user": {
				"id": 5920619669,
				"screen_name": "长发魔女希坨坨555",
				"profile_image_url": "http:\/\/tva2.sinaimg.cn\/crop.0.0.199.199.50\/006sGjDDjw1fa1y4czu15j305k05kweg.jpg",
				"avatar_large": "http:\/\/tva2.sinaimg.cn\/crop.0.0.199.199.180\/006sGjDDjw1fa1y4czu15j305k05kweg.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 347,
				"mbtype": 0,
				"mbrank": 0,
				"remark": "",
				"friends_count": 4227,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _5920619669",
				"oid": 5920619669,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=5920619669|uid:6095056301|follow:5920619669|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 5920619669,
					"need_follow": 1,
					"trend_ext": 5920619669,
					"trend_type": 42,
					"itemid": 5920619669
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _5920619669",
					"oid": 5920619669,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=5920619669|uid:6095056301|follow:5920619669"
				},
				"can_unfollow": 1,
				"relationship": 3
			}],
			"desc2_struct": [{
				"name": "微博推荐",
				"scheme": "http:\/\/fansmore.biz.weibo.cn\/members\/order?FP=myfans"
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _2920548362",
			"scheme": "sinaweibo:\/\/userinfo?uid=2920548362",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "转发微博",
			"user": {
				"id": 2920548362,
				"screen_name": "墨镜pm樱桃花1990",
				"profile_image_url": "http:\/\/tva2.sinaimg.cn\/crop.0.0.180.180.50\/ae14080ajw1e8qgp5bmzyj2050050aa8.jpg",
				"avatar_large": "http:\/\/tva2.sinaimg.cn\/crop.0.0.180.180.180\/ae14080ajw1e8qgp5bmzyj2050050aa8.jpg",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 363,
				"mbtype": 0,
				"mbrank": 0,
				"remark": "",
				"friends_count": 2712,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _2920548362",
				"oid": 2920548362,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=2920548362|uid:6095056301|follow:2920548362|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 2920548362,
					"need_follow": 1,
					"trend_ext": 2920548362,
					"trend_type": 42,
					"itemid": 2920548362
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _2920548362",
					"oid": 2920548362,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=2920548362|uid:6095056301|follow:2920548362"
				},
				"can_unfollow": 1,
				"relationship": 3
			}],
			"desc2_struct": [{
				"name": "微博推荐",
				"scheme": "http:\/\/fansmore.biz.weibo.cn\/members\/order?FP=myfans"
			}]
		}, {
			"card_type": 30,
			"itemid": "2310930026_1_ _6078699075",
			"scheme": "sinaweibo:\/\/userinfo?uid=6078699075",
			"background_color": 0,
			"openurl": "",
			"recom_remark": "",
			"desc1": "http:\/\/t.cn\/RJmHlwA",
			"user": {
				"id": 6078699075,
				"screen_name": "单于善榕胜松达",
				"profile_image_url": "http:\/\/tvax4.sinaimg.cn\/default\/images\/default_avatar_male_50.gif",
				"avatar_large": "http:\/\/tvax4.sinaimg.cn\/default\/images\/default_avatar_male_180.gif",
				"verified": false,
				"verified_type": -1,
				"level": null,
				"followers_count": 8,
				"mbtype": 2,
				"mbrank": 1,
				"remark": "",
				"friends_count": 212,
				"icons": null,
				"verified_type_ext": null
			},
			"actionlog": {
				"act_code": 695,
				"uicode": "10000011",
				"luicode": "10000011",
				"fid": "231093_-_selffollowed",
				"lfid": "1005056095056301",
				"lcardid": "",
				"cardid": "2310930026_1_ _6078699075",
				"oid": 6078699075,
				"featurecode": "",
				"mark": "",
				"ext": "act:skip|act_valu:sinaweibo:\/\/userinfo?uid=6078699075|uid:6095056301|follow:6078699075|skiptype:profile"
			},
			"buttons": [{
				"type": "follow",
				"sub_type": 1,
				"name": "关注",
				"skip_format": 1,
				"params": {
					"uid": 6078699075,
					"need_follow": 1,
					"trend_ext": 6078699075,
					"trend_type": 42,
					"itemid": 6078699075
				},
				"actionlog": {
					"act_code": 1338,
					"uicode": "10000011",
					"luicode": "10000011",
					"fid": "231093_-_selffollowed",
					"lfid": "1005056095056301",
					"lcardid": "",
					"cardid": "2310930026_1_ _6078699075",
					"oid": 6078699075,
					"featurecode": "",
					"mark": "",
					"ext": "act:follow|act_valu:sinaweibo:\/\/userinfo?uid=6078699075|uid:6095056301|follow:6078699075"
				},
				"can_unfollow": 1,
				"relationship": 3
			}]
		}],
		"openurl": ""
	}]
}
```
正则:```id: \d{10}```即能找到对应用户Id

3.将id之间用```%2c```拼接起来，cmd执行即可
4.批量操作
```
  String ids = "";
        BufferedReader br = new BufferedReader(new FileReader("/Users/hzwengyingjian/Downloads/weibounsub"));
        String line = br.readLine();
        while (line != null) {
            if (line.contains("_")) {
                line = br.readLine();
                continue;
            }
            if (line.contains("\t\t\t\t\"id\": ")) {
                line = line.replace("\"id\": ", "");
                ids = ids + line.trim();
            }
            line = br.readLine();
        }
        ids = ids.replace(",", "%2c");
        ids = ids.substring(0, ids.length() - 3).trim();

        String cmd = "curl 'http://weibo.com/aj/f/unfollow?ajwvr=6&__rnd=1500178195301' -H 'Cookie: SINAGLOBAL=4800740298882.926.1493562846891; UM_distinctid=15bcde24cc263a-0fbd70d22cce9-143a655c-fa000-15bcde24cc375a; YF-Ugrow-G0=56862bac2f6bf97368b95873bc687eef; login_sid_t=7cdd452055220f11089f8120a97c7117; YF-V5-G0=16139189c1dbd74e7d073bc6ebfa4935; _s_tentry=-; Apache=3425240342423.732.1500174838345; ULV=1500174838395:8:1:1:3425240342423.732.1500174838345:1498619268184; YF-Page-G0=27b9c6f0942dad1bd65a7d61efdfa013; UOR=,www.weibo.com,login.sina.com.cn; SCF=Aspi_zgbx9SNcHagz2cQpbos5HTIygCIb8LjH0FrmMYy9dD8kQeMy5t0gaMwNLk4cBAUBsF-8j0VJkdo_Zkm9dg.; SUB=_2A250bpaYDeRhGeBO4lcR9SjPyz2IHXVXHY9QrDV8PUNbmtBeLRLTkW9g4hcR8gq_qMLdnwkV7-B0VFznyw..; SUBP=0033WrSXqPxfM725Ws9jqgMF55529P9D9W5GNsRHD20_MFfkyuV6Z4Sc5JpX5KzhUgL.Foq71K-7SKq0eh22dJLoIpLJIPxV9PS0i--Ni-zEi-i8i--4iKn7iKn4; SUHB=0wn1QUZO82JloS; ALF=1531714120; SSOLoginState=1500178120; wvr=6' -H 'Origin: http://weibo.com' -H 'Accept-Encoding: gzip, deflate' -H 'Accept-Language: zh-CN,zh;q=0.8,en;q=0.6,zh-TW;q=0.4' -H 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.115 Safari/537.36' -H 'Content-Type: application/x-www-form-urlencoded' -H 'Accept: */*' -H 'Referer: http://weibo.com/6095056301/follow?rightmod=1&wvr=6' -H 'X-Requested-With: XMLHttpRequest' -H 'Connection: keep-alive' --data 'uid=UID_REP&refer_flag=unfollow_all&_t=0' --compressed";
        System.out.println("ids=" + ids);
        System.out.println(cmd.replace("UID_REP", ids));
        //
        Runtime.getRuntime().exec(cmd.replace("UID_REP", ids));
```

