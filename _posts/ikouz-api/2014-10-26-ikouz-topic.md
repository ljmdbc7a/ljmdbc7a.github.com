---
layout: post
category : ikouz-api
tagline: "ikouz.com"
tags : [private, ikouz-api]
---
{% include JB/setup %}

## Introduction

This is first project api doc of ikouz studio. For more infomation, welcome to [www.ikouz.com](http://www.ikouz.com)

### 请求地址
测试环境	http://121.199.8.141:9002/
线上环境	http://121.199.8.141:9002/

### 公共参数说明
参数名	   参数说明	参数格式	是否可空	默认值	可选值
userId	   用户id	string		TRUE		
clientCode 平台id	int			TRUE				0：android 1：iPhone 2：iPad

### 公共参数说明

## 接口定义

### 1. 获取话题 — getTopic.do

### 请求示例：
http://121.199.8.141:9002/getTopic.do?limit=7

### 入参说明：
参数名	参数说明		参数格式	是否可空	默认值	可选值
limit	限制返回条数	int			TRUE		7	

### 出参说明：
编号 	字段名			数据类型 	说明 
1		title			String		话题标题 
2		summary			String		话题纲要
3		linkUrl			String		话题详情链接
4		imgUrl			String		话题图片
5		agreeCount		int			赞同个数
6		showTimestamp	long		展示时间戳
7		date			String		展示时间

### 返回示例
{
head: {
		  code: "200",
		  message: "success"
	  },
body: {
		  topicInfoList: [
			   {
					topicId: 4,
					title: "this is title",
					summary: "this is summary...",
					imgUrl: "http://images.wandafilm.com/uploadServer/resource/images/2014/07/20140711101321993513.jpg",
					linkUrl: "http://mp.weixin.qq.com/s?__biz=MzAxMzA3ODY4NA==&mid=204068282&idx=1&sn=2edb8a42c326d306de75c318edf8e5d0",
					showTimestamp: 1414297286000,
					date: "10月26日"
			   }
			   ]
	  }
}


### 2. 获取评论接口





