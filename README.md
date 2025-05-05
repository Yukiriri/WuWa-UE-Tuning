# WuWaUETuning
- 当前适配游戏版本：2.3.x

# RTX Off | 不开光追
```
[/Script/Engine.RendererOverrideSettings]
; Performance | 性能
a.ParallelAnimEvaluation=True
a.ParallelAnimInterpolation=True
a.ParallelAnimUpdate=True
a.ParallelBlendPhysics=True
rhi.MaximumFrameLatency=0
rhi.SyncSlackMS=0

; Tone | 后期色调 （解放UE该有的原色）
r.KuroTonemapping=1
r.Color.Mid=0.5
r.Color.Max=1.5
r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=True
r.Kuro.AutoExposure=True
r.Kuro.EyeAdaptation.CustomValueMode=True
r.Kuro.EyeAdaptation.ExposureBiasOverride=0.0

; Effects | 后期效果
r.Tonemapper.Quality=3
r.SceneColorFringeQuality=0
r.MotionBlur.TargetFPS=0

; AA | 抗锯齿
r.ScreenPercentage=100
; r.TemporalAA.Upsampling=True
; r.TemporalAA.Algorithm=1
; r.Tonemapper.Sharpen=0.5
; r.PostProcessAAQuality=4

; LOD | 细节层级
r.DetailMode=2
r.LODFadeTime=1.0

; Distance | 视距
; r.ViewDistanceScale=1.5
r.Kuro.Foliage.EnableFoliageCulling=False
r.Fog=True
r.FogDensity=0.5
r.FogStartDistance=10000

; AO | 环境遮蔽
; r.AmbientOcclusionRadiusScale=0

; Light | 光照
; r.SkylightIntensityMultiplier=1.25
r.Kuro.LightFadeTime=5.0

; Shadow | 阴影
r.ShadowQuality=3
r.Shadow.CSM.MaxCascades=8
r.Shadow.CacheMode3CacheUpdateIntervals=1,2,4,8,16,32,64,128
r.Shadow.PerObjShadowPCFQuality=3
r.Shadow.PerObjectResolutionMin=1024
r.Shadow.PerObjectResolutionMax=1024

[/Script/Engine.StreamingSettings]
r.Streaming.MipBias=0
r.Streaming.LimitPoolSizeToVRAM=True
r.Streaming.PoolSizeForMeshes=-1
r.Streaming.PoolSize.VRAMPercentageClamp=512
r.Streaming.FramesForFullUpdate=10
r.Streaming.AmortizeCPUToGPUCopy=True
r.Streaming.MaxNumTexturesToStreamPerFrame=5
s.ForceGCAfterLevelStreamedOut=False

[/Script/Engine.GarbageCollectionSettings]
gc.TimeBetweenPurgingPendingKillObjects=30

[Pak]
PakCheck=False
```

# RTX On | 开光追
