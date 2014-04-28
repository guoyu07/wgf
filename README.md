[[English Documentation](<README-en.md>)]

# Wgf 文档

> * 源码: http://github.com/walu/wgf
> * 微博: http://weibo.com/walu

## 是什么？

[wgf](<http://github.com/walu/wgf>)是基于[Golang](<golang.org>)的web框架，目前做wgf的目标只有一点：

* 一款支持Http、Websocket、Cli的编程框架。

> **强烈建议大家先浏览一下app目录源码（一个index＋login事例），即可对wgf有个大体的了解。**

## 扩展机制

灵活的扩展机制是Wgf的一大特点，借鉴了php的设计理念，简化新功能的增添，保持核心结构与整体理念的稳定。

## Package的依赖关系

Package dependencies(自上至下):

* app
	* action
	* model
* wgf
	* plugin
	* sapi
	* lib

上层依赖下层，下层不依赖上层。

## 支持的功能

* mvc
	* 可以查看源码中的app目录，查看基本的mvc使用。
* plugin
	* httpparam, 获取http请求中的参数，GET、POST、文件上传等。
	* session (完善中), 处理Session问题。
	* cookie, 获取、设置Cookie。
	* header, 获取、设置Header信息、重定向请求等。
	* router, 根据路由规则分发请求、生成URL等。
	* view, 管理模版文件，无重启更新模版。

## 使用介绍(整理中)

> 类库文档，大家可以使用godoc。
> 这里的介绍是为了说一些godoc表达不了的。

* 介绍
	* [入门Demo](<docs/1-1-the-first-demo.md>)
* 核心扩展介绍
	* httpparam
		* 获取Get\Post参数。
		* 处理文件上传。
	* session
		* 处理session。
		* 更换session的保存方式。
	* cookie
		* 处理Cookie。
	* header
	* router
		* 设置路由规则。
		* URL生成。
		* 路由性能
	* view
		* 基本使用。
		* view配置参数说明。

* 进阶介绍
	* wgf架构介绍
	* wgf扩展开发
