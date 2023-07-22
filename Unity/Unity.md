# Unity

> Author: Sylvie233
>
> Date: 23/6/11
>
> Point: xlua P12

[TOC]

## 基础介绍

### AssetBundle

`.unity3d`



Files.txt资源列表





#### AssetBundleManifest

ab包依赖信息









### uGUI

用户界面



### 宏

```
:
	UNITY_IOS:
	UNITY_ANDROID:
```





### 编辑器扩展

```
:
	HeaderAttribute:
    MenuItemAttribute:
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

Animation Event 为特定帧绑定回调函数









#### Animator

```
Animator:
	Controller: 动画控制器
	Avatar:
	ApplyRootMotion:
	UpdateMode:
	CullingMode:
```



AnyState、Entry、Exit

`.anim`动画切片







##### AnimatorController

##### Animation







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



#### Toggle

```
Toggle:
	
```







### Script

#### ContentSizeFitter

```
ContentSizeFitter:
	
```



#### GraphicRaycaster

```
GraphicRaycaster:
	
```





#### GridLayoutGroup

```
GridLayoutGroup:
	
```



#### Mask

```
Mask:
	
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





#### ScrollRect

```
ScrollRect:
	
```









### 2D

#### Tilemap

##### RuleTile

##### AnimatedTile



#### PhysicsMaterial2D









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

#### CapsuleCollider2D

#### CircleCollider2D

#### Rigidbody2D

```

```











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



#### SpriteRenderer



#### TilemapRenderer



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

```
XLua:
	CSharpCallLuaAttribute:
	CustomLoader: 委托
	LuaEnv:
		Global:
			Get():
		AddLoader():
		Dispose():
		DoString():
	LuaFunction:
		Call():
	LuaTable:
		Length:
		Get():
		GetKeys():
		
```



Unity中可以用TextAsset格式加载lua文件

通过执行require来加载lua代码



自定义Loader：获取加载路径 

通过委托delegate	获取lua中的function（使用[CSharpCallLua]标注）







Lua调用C#代码

```
CS:
	UnityEngine:
		GameObject:
			Destory():
			Find():
		Time:
			deltaTime:
			timeScale:
```

CS命名空间









#### toLua

```
LuaInterface:
	LuaBinder:
		Bind():
	LuaFunction:
		Call():
	LuaResLoader:
	LuaState:
		DoFile():
		GetFunction():
		Start():
```





lua调用Unity

```
UnityEngine:
	AudioSource:
	Color:
	Gamobject:
		Find(): 
	Input:
		GetAxis():
	Rigidbody:
		AddForce():
	WWW():
	
coroutine:
	start():
	www():
```











## API

```
UnityEngine:
	Events:
		UnityAction:
	EventSystems:
		IBeginDragHandler:
		IDragHandler:
		IDropHandler:
		IEndDragHandler:
		IInitializePotentialDragHandler:
		IPointerClickHandler:
		IPointerDownHandler:
		IPointerEnterHandler:
		IPointerExitHandler:
		IPointerUpHandler:
		IScrollHandler:
		ISelectHandler:
		PointerEventData:
			position:
	Networking:
		ClientRpcAttribute:
		CommandAttribute:
		NetworkBehaviour:
			isLocalPlayer:
			OnStartLocalPlayer():
		SyncVarAttribute:
	SceneManagement:
		SceneManager:
			LoadScene():
	UI:
		ContentSizeFitter:
		GridLayoutGroup:
			
		Image:
			sprite:
			SetNativeSize():
		ScrollRect:
			horizontalNormalizedPosition:
		Text:
			text:
	Animator:
		GetCurrentAnimatorStateInfo():
		GetFloat():
		Play():
		SetFloat():
	Application:
		dataPath:
		persistentDataPath:
        streamingAssetsPath:
            persistentDataPath():
        temporaryCachePath:
	AssetBundle:
		LoadFromFile():
		LoadFromFileAsync():
		LoadFromMemory():
		LoadFromStream():
		UnloadAllAssetBundles():
		---
		LoadAllAssets():
		LoadAsset():
		Unload():
	AssetBundleManifest:
		GetAllDependencies():
    AssetDatabase:
    	Refresh():
    AudioClip:
	AudioSource:
		clip:
		loop:
		Play():
		PlayOneShot():
		Stop():
	AudioSourceManager:
	BuildPipeline:
		BuildAssetBundles():
	Camera:
		main:
			ScreenToWorldPoint():
	Collider2D:
		tag:
		OnTriggerEnter2D():
		OnTriggerExit2D():
		OnTriggerStay2D():
	CreateAssetMenuAttribute:
		TextAreaAttribute:
	Debug:
		Log():
	GameObject:
		activeSelf:
		transform:
			GetComponent():
		Destroy():
		FindGameObjectsWithTag():
		SetActive():
	Gizmos:
		DrawWireSphere():
	Input:
		mousePosition:
		GetAxis():
		GetKeyDown():
	JsonUtility:
		FromJson():
		ToJson():
	KeyCode:
		Space:
	LayerMask:
	Mathf:
		Abs():
		Clamp():
		Lerp():
	MonoBehaviour:
		Awake(): 
		Start():
		Update():
		OnDrawGizmos():
		OnDrawGizmosSelected():
		OnDrag():
		OnBeginDrag():
		OnEndDrag():
		OnPointerEnter():
		onPointerExit():
		IsRaycastLocationValid():
		---
		transform:
		CancelInvoke():
		GetComponent():
		Instantiate():
		Invoke():
		InvokeRepeating():
		StartCoroutine():
		StopAllCoroutines():
	Physics2D:
		OverlapCircle():
		OverlapPointAll():
	Quaternion:
		Euler():
	RectTransform:
		anchoredPosition:
		GetWorldCorners():
	Resources:
		Load():
	Rigidbody2D:
		velocity:
			x:
			y:
	ScriptableObject:
	Sprite:
	TextAsset:
	Transform:
		eulerAngles:
		localPosition:
		getChild():
		LookAt():
		SetParent():
		Translate():
	Vector3:
		normalized:
    	zero:
    	Distance():
    	
    WWW:
    	LoadFromCacheOrDownload():
    	---
    	asssetBundle:
```



