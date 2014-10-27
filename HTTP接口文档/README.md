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
		"banner":["http://...",...]
		"project":[ {"title":"...","image_url":"http://..."},...].],
		"inheritor":[ {"title":"...","image_url":"http://..."},...],
		"news":[ {"title":"...","image_url":"http://...","summary":"..."},...],
	}
}
```
## 项目名录列表
* 说明：根据分类返回项目列表
* 地址：http://....
* 入参：

| name | type | desc |
| - | - | - |
| genre | int | 音乐、舞蹈等分类 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"project":[ {"title":"...","image_url":"http://..."},...],
	}
}
```

## 传承人列表
* 说明：根据分类返回传承人列表
* 地址：http://....
* 入参：

| name | type | desc |
| - | - | - |
| genre | int | 音乐、舞蹈等分类 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"inheritor":[ {"title":"...","image_url":"http://..."},...],
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
		"news":[ {"title":"...","image_url":"http://...","summary":"..."},...],
	}
}
```

## 保护载体列表
* 说明：根据分类返回传承人列表
* 地址：http://....
* 入参：

| name | type | desc |
| - | - | - |
| genre | int | 传承基地、展示场馆等分类 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"carrier":[ {"title":"...","image_url":"http://..."},...],
	}
}