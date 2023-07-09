# Unity

> Author: Sylvie233
>
> Date: 23/6/11
>
> Point:

[TOC]

## 基础介绍

### AssetBundle

#### AssetBundleManifest

ab包依赖信息









### uGUI



### 宏

```
:
	UNITY_IOS:
	UNITY_ANDROID:
```







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







### Animation

#### Animator

```
Animator:
	Controller:
	Avatar:
	ApplyRootMotion:
	UpdateMode:
	CullingMode:
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



#### InputField

```
InputField:
	text:
```



#### Panel

```
Panel:
	
```





#### ScrollView

```
ScrollView:
	
```

ViewPort

Content

ScrollbarHorizontal

ScrollbarVertical



#### Slider

```
Slider:
	
```



#### Sprite

```
Sprite:
	
```





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





#### NetworkManager

```
NetworkManager:
	
```



##### NetworkAnimator

```
NetworkAnimator:
	
```



##### NetworkIdentity

```
NetworkIdentity:
	
```





##### NetworkManagerHUD

```
NetworkManagerHUD:
	
```



##### NetworkTransform

```
NetworkTransform:
	
```



### 3D

#### Cube

```
Cube:
	
```



#### Capsule



#### Cylinder

#### Sphere

#### Plane

#### Terrain

#### Tree

#### WindZone

#### 3DText







### physics

#### BoxCollider2D









### Component

#### AudioSource

#### AudioListener



#### MeshRenderer

```
MeshRenderer:
	Materials:
	Lighting:
	Probes:
```





#### RawImage



#### RectTransform

```
RectTransform:
	PosX:
	Anchors:
	Pivot:
	Rotation:
	Scale:
```



#### Renderer

```
Renderer:
	material:	
	
```





#### Transform





#### VideoPlayer







## 插件

### Photon

```
Photon
	Pun:
		MonoBehaviourPun:
			photonView:
				IsMine:
        MonoBehaviourPunCallbacks:
            OnConnectedToMaster():
            OnJoinedRoom():
            OnRoomListUpdate():
        PhotonNetwork:
        	InLobby:
        	IsConnected:
            ConnectUsingSettings():
            Instantiate():
            JoinLobby():
            JoinOrCreateRoom():
            LoadLevel():
    Realtime:
    	RoomInfo:
    	RoomOptions:
```



Photon Pun2

```
Photon:
	/PhotonChat:
	/PhotonLibs:
	/PhotonRealtime:
	/PhotonUnityNetworking:
		/Code:
		/Demos:
		/Icons:
		/Resources:
		/UtilityScripts:
```







#### 组件

##### PhotonServerSettings

```
PhotonServerSettings:
	Settings:
		AppVersion:
	PUNLogging:
```



##### PhotonView

```
PhotonView:
	Owner:
	ViewId:
	ObservedComponents:
```



##### PhotonAnimatorView

```
PhotonAnimatorView:
	
```





##### PhotonTransformView

```
PhotonTransformView:
	
```





### Lua

#### xLua





#### toLua













## API

```
UnityEngine:
	Events:
		UnityAction:
	EventSystems:
		IBeginDragHandler:
		IPointerClickHandler:
		IPointerUpHandler:
		PointerEventData:
	Networking:
		ClientRpcAttribute:
		CommandAttribute:
		NetworkBehaviour:
			isLocalPlayer:
			OnStartLocalPlayer():
		SyncVarAttribute:
	UI:
		Image:
			sprite:
			SetNativeSize():
		Text:
			text:
	Animator:
		
	Application:
	streamingAssetsPath:
		persistentDataPath():
	AssetBundle:
		LoadFromFile():
		LoadFromFileAsync():
		LoadFromMemory():
		LoadFromStream():
		UnloadAllAssetBundles():
		---
		LoadAsset():
		Unload():
	AudioSource:
		clip:
		loop:
		Play():
		PlayOneShot():
		Stop():
	AudioSourceManager:
	Camera:
	CreateAssetMenuAttribute:
		TextAreaAttribute:
	Debug:
		Log():
	GameObject:
		FindGameObjectsWithTag():
		SetActive():
	Input:
		GetAxis():
		GetKeyDown():
	JsonUtility:
		FromJson():
		ToJson():
	KeyCode:
		Space:
	MonoBehaviour:
		Awake(): 
		Start():
		Update():
		---
		transform:
		GetComponent():
		Instantiate():
		StartCoroutine():
	Resources:
		Load():
	ScriptableObject:
	Sprite:
	Transform:
		eulerAngles:
		localPosition:
		getChild():
		LookAt():
		Translate():
	Vector3:
    	zero:
```



