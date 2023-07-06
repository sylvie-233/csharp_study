# Unity

> Author: Sylvie233
>
> Date: 23/6/11
>
> Point: Unity Galgame教程P51

[TOC]

## 基础介绍





### uGUI





## 核心内容

### Scene











### Camera

```
Camera:
	ClearFlags:
	CullingMask:
	Projection:
	FOVAxis:
	FieldOfView:
	PhysicalCamera:
	ClippingPlanes:
	ViewportRect:
	Depth:
	RenderingPath:
	TargetTexture:
	HDR:
	MSAA:
	AllowDynamicResoll:
	TargetDisplay:
```





### EventSystem

#### Event Trigger









### Light









### UI

#### Button





#### Canvas

```
Canvas:
	RenderMode:
		ScreenSpace-Overlay:
		ScreenSpace-Camera:
		WorldSpace:
```



Canvas



Canvas Scaler



Graphic Raycaster





#### Image

```
Image:
	SourceImage:
	Color:
	Material:
	RaycastTarget:
```



#### ScrollView

```
ScrollView:
	
```

ViewPort

Content

ScrollbarHorizontal

ScrollbarVertical





#### Text

```
Text:
	Text:
	Character:
		Font:
		FontSize:
	Paragraph:
	Color:
	Material:
	RaycastTarget:
	
```







### Script

#### ContentSizeFitter

```
ContentSizeFitter:
	
```





#### GridLayoutGroup

```
GridLayoutGroup:
	
```





### Component

#### AudioSource

#### AudioListener



#### RawImage



#### ReactTransform

```
RectTransform:
	PosX:
	Anchors:
	Pivot:
	Rotation:
	Scale:
```





#### Transform





#### VideoPlayer







## API

```
UnityEngine:
	EventSystems:
		IBeginDragHandler:
		IPointerClickHandler:
		IPointerUpHandler:
		PointerEventData:
	UI:
		Image:
			sprite:
			SetNativeSize():
		Text:
			text:
	AudioSource:
		clip:
		loop:
		Play():
		PlayOneShot():
		Stop():
	AudioSourceManager:
	Camera:
		
	Debug:
		Log():
	GameObject:
		SetActive():
	MonoBehaviour:
		Awake(): 
		Start():
		Update():
		---
	Resources:
		Load():
	Transform:
		eulerAngles:
		localPosition:
	Vector3:
    	zero:
```



