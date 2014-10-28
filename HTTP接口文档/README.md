# FY接口：
## 主页数据接口：
* 说明：获取主页所需信息，包含Banner图片列表，穿透项目名录列表，穿透传承人列表，穿透新闻动态列表。
* 地址：http://....
* 入参：无
* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"banner":[ {"id":1,"image_url":"http://...","link_url":"http://..."},...],
		"project":[ {"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://..."},...],
		"inheritor":[ {"id":1,"title":"...","sex":"...","age":"...","project":{"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://..."},"content":"...","type":{"id":1,"type":"..."},"image_url":"http://..."},...],
		"news":[ {"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://...","from":"...","datetime":"..."},...],
		"carrier":null
	}
}
```
## 项目名录列表
* 说明：根据分类返回项目列表
* 地址：http://....
* 入参：

| name | type | desc |
| ------------ | ------------- | ------------ |
| typeid | int | 音乐、舞蹈等分类 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"banner":null,
		"project":[ {"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://..."},...],
		"inheritor":null,
		"news":null,
		"carrier":null
	}
}
```
## 项目名录详情
* 说明：根据项目名录ID返回项目详情
* 地址：http://....
* 入参：

| name | type | desc |
| ------------ | ------------- | ------------ |
| id | int | 项目名录 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://..."
	}
}
```

## 传承人列表
* 说明：根据分类返回传承人列表
* 地址：http://....
* 入参：

| name | type | desc |
| ------------ | ------------- | ------------ |
| typeid | int | 音乐、舞蹈等分类 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"banner":null,
		"project":null,
		"inheritor":[ {"id":1,"title":"...","sex":"...","age":"...","project":{"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://..."},"content":"...","type":{"id":1,"type":"..."},"image_url":"http://..."},...],
		"news":null,
		"carrier":null
	}
}
```
## 传承人详情
* 说明：根据传承人ID返回传承人详情
* 地址：http://....
* 入参：

| name | type | desc |
| ------------ | ------------- | ------------ |
| id | int | 传承人 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"id":1,"title":"...","sex":"...","age":"...","project":{"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://..."},"content":"...","type":{"id":1,"type":"..."},"image_url":"http://..."
	}
}
```
## 新闻动态列表
* 说明：根据分类返回新闻动态列表
* 地址：http://....
* 入参：无
* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"banner":null,
		"project":null,
		"inheritor":null,
		"news":[ {"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://...","from":"...","datetime":"..."},...],
		"carrier":null
	
	}
}
```
## 新闻详情
* 说明：根据新闻ID返回新闻动态详情
* 地址：http://....
* 入参：无
* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://...","from":"...","datetime":"..."
	
	}
}
```
## 保护载体列表
* 说明：根据分类返回传承人列表
* 地址：http://....
* 入参：

| name | type | desc |
| ------------ | ------------- | ------------ |
| typeid | int | 传承基地、展示场馆等分类 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"banner":null,
		"project":null,
		"inheritor":null,
		"news":null,
		"carrier":[ {"id":1,"title":"...","content","...","type":{"id":1,"type":"..."},"image_url":"http://..."},...]
	}
}
```
## 保护载体详情
* 说明：根据保护载体ID返回保护载体详情
* 地址：http://....
* 入参：

| name | type | desc |
| ------------ | ------------- | ------------ |
| id | int | 保护载体 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"id":1,"title":"...","content","...","type":{"id":1,"type":"..."},"image_url":"http://..."
	}
}
```