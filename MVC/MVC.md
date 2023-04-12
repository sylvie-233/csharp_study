# MVC基础

> Author: Sylvie233
>
> Date: 23/2/23
>
> Point:

[TOC]

## 基础介绍



### 项目结构

```
MVC:
	/Connected Services:
	/Properties:
	/wwwroot:
	/依赖项:
	/Contrrollers:
		HomeController.cs:
	/Models:
		ErrorViewModel.cs:
	/Views:
		/Home:
			Index.cshtml:
			Privacy.cshtml:
		/Shared:
			_Layout.cshtml:
			_ValidationScriptsPartial.cshtml:
		_ViewImports.cshtml:
		_ViewStart.cshtml:
	appsettings.json:
	Program.cs:
```



#### appsettings.json

```

```





#### Program.cs

```
var builder = WebApplication
	.CreateBuilder(args)
		WebApplicationOptions:
			WebRootPath:

builder
	.Services
		.AddControllersWithViews():
		.AddMvc():
			():
				options:
					EnableEndpointRouting:
					
		
var app = builder.Build();
if (!app.Environgment.IsDevelopment()) {
	app.UseExceptionHandler("/Home/Error")
}

app
	.UseStaticFiles():
	.UseDefaultFiles():
	.UseFileServer():
	.UseRouting():
	.UseAuthorization():
	.UseEndpoints():
		():
			endpoints:
				MapControllerRoute(): 自定义路由
				MapDefaultControllterRoute():
    .UseMvc():
    	route:
    		MapRoute():
	
	.MapControllerRoute():
	.MapGet():
	
	.Run():
```



#### libman.json

```
{
	"version":
	"defaultProvider": "cdnjs"
	"libraries": [
		{
			"library":
			"dstination":
			"provider":
		}
	]
}
```







## 核心内容

### 特性

```
:
	Route:
		
```



### razor模板

```
@model Xxx.Xxx
@using Xxx.Xxx
@addTagHelper *
@{
	Layout = "_Layout"
	ViewBag:
	ViewData[]:
}

@* 注释 *@

<html>
	@Model:
	@Html:
		ActionLink:
			
		
	@RenderBody():
	@RenderSectionAsync():
	
	@foreach () {}
</html>
```



#### 布局视图

```
定义布局:
	@RenderBody():

```





### TagHelper

```
:
	asp-action:
	asp-controller:
	asp-route-id:
```















## API

```
Mvc:
	Controller:
	IActionResult:
```



































