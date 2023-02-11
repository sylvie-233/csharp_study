# Blazor基础

> Author: Sylvie233
>
> Date: 23/2/11
>
> Point:

[TOC]

## 基础介绍

C#代替JavaScript



Blazor Server、Blazor WebAssembly



### 项目结构

```
Blazor:
	/Connected Services:
	/Properties:
	/wwwroot:
	/依赖项:
	/Pages:
		_Host.cshtml:
		Index.razor:
	_Imports.razor:
	App.razor:
	appsettings.json
	MainLayout.razor:
	Program.cs:
```



#### App.razor

路由

```
<Router 
	AppAssembly="@typeof(Program).Assmbly"
	AdditionalAssemblies
>
	<Found 
		Context="routeData"
	>
		<RouteView 
			routeData="@routeData" 
			DefaultLayout="@typeof(MainLayout)"/>
	</Found>
	<NotFound>
		<p> </p>
	</NotFound>
</Router>
```



#### MainLayout.razor

```
@inherits LayoutComponentBase

<main>
	@Body
</main>
```



#### Index.razor

```
@page "/"

<h1> Hello Sylvie~~~ </h1>
```



#### appsettings.json

```
{
	"DetailedErrors":
	"Logging":
		"LogLevel":
			"Default": "Infomation"
			"Microsoft.xxx":
}
```





## 核心内容

### razor组件

```
@page "/xxx"

@layout 布局组件

@using 引入类;

@inject 注入类;
	NavigationManager

<html代码>
	@bind
	@bind-Xxx
	@onxxx: 事件绑定code代码
	@xxx: 引用c#变量
	
	@foreach () {}

@code {
	[Parameter]
	[CascadingParameter]
	
	SetParametersAsync()
	OnInitialized()
	OnInitializedAsync()
	ShouldRender()
	OnAfterRender(bool firstRender)
	Dispose()
		StateHasChanged()
		InvokeAsync()
}
```



#### 内置组件

```
内置组件:
	CascadingValue:
		Value:
```



#### 模板组件

RenderFragment：页面html片段



数据绑定



生命周期



父子组件通信











### 路由



### 配置



### 依赖注入

内置对象

```
内置对象:
	NavigationManager:
		
```





### 异常处理





## API

### WebApplication

```
WebApplication:
	CreateBuilder():
		Services:
			
```



































