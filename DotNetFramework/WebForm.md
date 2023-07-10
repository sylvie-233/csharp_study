# WebForm

> Author: Sylvie233
>
> Date: 23/7/10
>
> Point: ASP.NET开发 P10

[TOC]

## 基础介绍

ASP.NET





`.aspx`、`.aspx.cs`



### 目录结构

```
:
	/Account:
	/App_Code:
		AuthConfig.cs:
		RouteCOnfig.cs:	
	/App_Data:
	/bin:
	/Content:
	/Images:
	/Scripts:
	About.aspx:
	Contact.aspx:
	Default.aspx:
	favicon.icon:
	Global.asax:
	packages.config:
	Web.config:
```























## 核心内容

### ASP页面

```
<%@ Page Title Language MasterPageFile %>

html代码



---
Page:
	Page_Load():
```



Page：asp页面关联的C#类





#### 模板页面

Master：`.master`文件

ContentPlaceHolder与Content





### 内置组件

```
asp:
	Button:
	Content:
		ID:
		ContentPlaceHolderID:
		Runat:
	CompareValidator:
		ControlToValidate:
		ControlToCompare:
	ContentPlaceHolder: 插槽
	CustomValidator: 自定义验证
		ErrorMessage:
		ServerValidateEvent: 自定义事件处理
	Image:
	Label:
	RangeValidate:
		ControlToValidate:
		MaximumValue:
		MinimumValue:
	RegularExpressionValidate: 正则表达式验证
		ValidationExpression:
	RequiredFieldValidator:
		ID:
		runat:
		ControlToValidate:
		ErrorMessage:
		ForeColor:
	TextBox:
		TextMode:
	ValidationSummary:
		ShowMessageBox:
```











## API

```
System.Web:
    UI:
        Page:
```





























