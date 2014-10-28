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
		"news":[ {"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://...","from":"...","datetime":"..."},...]
	}
}
```
## 项目名录列表
* 说明：根据分类返回项目列表
* 地址：http://....
* 入参：

| name | type | desc |
| - | - | - |
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
		"news":null
	}
}
```

## 传承人列表
* 说明：根据分类返回传承人列表
* 地址：http://....
* 入参：

| name | type | desc |
| - | - | - |
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
		"news":null
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
		"news":[ {"id":1,"title":"...","content":"...","type":{"id":1,"type":"..."},"image_url":"http://...","from":"...","datetime":"..."},...]
	
	}
}
```

## 保护载体列表
* 说明：根据分类返回传承人列表
* 地址：http://....
* 入参：

| name | type | desc |
| - | - | - |
| typeid | int | 传承基地、展示场馆等分类 |

* 返回：

```
{
	"code":200,	// 成功
	"msg":"成功",
	"data": 
	{
		"carrier":[ {"id":1,"title":"...","content","...","type":{"id":1,"type":"..."},"image_url":"http://..."},...],
	}
}
```