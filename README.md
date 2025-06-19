# WuWaUETuning
- 当前适配游戏版本：2.4.x

```
[/Script/Engine.RendererOverrideSettings]

; Tone | 后期色调 （解放UE该有的原色）
r.KuroTonemapping=1
r.Color.Mid=0.5
r.Color.Max=1.25
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=True
r.Kuro.AutoExposure=True
r.Kuro.EyeAdaptation.CustomValueMode=True
r.Kuro.EyeAdaptation.ExposureBiasOverride=0.0

; Effects | 后期效果
r.Tonemapper.Quality=3
r.SceneColorFringeQuality=0
r.MotionBlur.TargetFPS=0

; AA | 抗锯齿
r.Upscale.Quality=4
; r.ScreenPercentage=100
; r.TemporalAA.Upsampling=True
; r.TemporalAA.Algorithm=1
; r.Tonemapper.Sharpen=0.5
; r.PostProcessAAQuality=4

; LOD | 细节层级
r.DetailMode=2
r.MaterialQualityLevel=1
r.KuroMaterialQualityLevel=1
r.StaticMeshLODDistanceScale=0.5

; Distance | 视距
; r.ViewDistanceScale=1.5
foliage.DensityType=2
r.Fog=True
r.FogDensity=0.5
r.FogStartDistance=10000

; Light | 光照
r.Kuro.LightFadeTime=5.0
; r.SkylightIntensityMultiplier=1.25

; Shadow | 阴影
r.ShadowQuality=3
r.Shadow.CSM0ShadowPCFQuality=3
r.Shadow.CSM1ShadowPCFQuality=3
r.Shadow.CSM2ShadowPCFQuality=3
r.Shadow.PerObjShadowPCFQuality=3
r.Shadow.PerObjectResolutionMin=1024
r.Shadow.PerObjectResolutionMax=1024
r.Shadow.RadiusThreshold=0.01
r.Shadow.RadiusThresholdCSM0=0.022
r.Shadow.RadiusThresholdCSM1=0.022
r.Shadow.RadiusThresholdCSM2=0.022
r.Shadow.RadiusThresholdCSM3=0.022
r.Shadow.RadiusThresholdCSM4=0.04
r.Shadow.RadiusThresholdCSM5=0.07
r.Shadow.ForbidHISMShadowStartIndex=3
r.Shadow.CacheMode3CacheUpdateIntervals=1,2,4,8,16,32,64,128

; AO | 环境遮蔽
r.AmbientOcclusionMaxQuality=100

; Reflection | 反射
r.SSR.Quality=4

; Misc | 杂项性能优化
wp.Runtime.OverrideMultipleRuntimeGridLoadingRangeValues=150&400&450&600&1500&5000&500&600&1000&500&650&800&1000&1500&120&150&200&350&80&160&200&200&1500&5000&100&160&200&1000&1500

[Pak]
PakCheck=False
```

# Credits
- [WuWa-Configs](https://github.com/AlteriaX/WuWa-Configs)
