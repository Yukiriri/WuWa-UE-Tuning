# WuWaUETuning
- 当前适配游戏版本：2.1.x

# 不开光追
```
[/Script/Engine.RendererOverrideSettings]
; Framerate | 帧率
a.ParallelAnimEvaluation=True
a.ParallelAnimInterpolation=True
a.ParallelAnimUpdate=True
a.ParallelBlendPhysics=True
rhi.MaximumFrameLatency=0
rhi.SyncSlackMS=0

; AA | 抗锯齿
r.ScreenPercentage=100
r.TemporalAACurrentFrameWeight=0.2
r.PostProcessAAQuality=4

; Tone | 后期色调
r.KuroTonemapping=1
r.Color.Mid=0.37
r.Color.Max=1.12
r.Tonemapper.Quality=1
r.Tonemapper.GrainQuantization=0
r.SceneColorFringeQuality=0

; Effects | 后期效果
r.Tonemapper.Sharpen=0.8
r.MotionBlur.TargetFPS=0
r.EyeAdaptationQuality=0
r.Kuro.AutoExposure=False
; r.Kuro.EyeAdaptation.CustomValueMode=True
; r.Kuro.EyeAdaptation.ExposureBiasOverride=-1.25
; r.DefaultFeature.AutoExposure.ExtendDefaultLuminanceRange=True

; Texture | 材质
; r.MaterialQualityLevel=3
; r.AnisotropicMaterials=True

; LOD | 细节层级
; r.DetailMode=2
r.LODFadeTime=1.0

; Distance | 视距
r.ViewDistanceScale=1.5
r.Kuro.Foliage.EnableFoliageCulling=False
r.Fog=True
r.FogDensity=0.5
r.FogStartDistance=10000

; Light | 光照
r.SkylightIntensityMultiplier=0.75
r.Kuro.LightFadeTime=5.0

; AO | 环境遮蔽
r.AmbientOcclusionRadiusScale=0

; Shadow | 阴影
r.Shadow.AkiSoftShadowCascadeNum=0
r.Shadow.CacheMode3CacheUpdateIntervals=5,7,9,12,18,38,78,158
r.Shadow.CSM.MaxCascades=8
r.Shadow.MaxCSMResolution=2048
r.Shadow.PerObjShadowPCFQuality=3
r.Shadow.PerObjectResolutionMin=1024
r.Shadow.PerObjectResolutionMax=1024

[/Script/Engine.StreamingSettings]
r.Streaming.LimitPoolSizeToVRAM=True
r.Streaming.PoolSizeForMeshes=-1
r.Streaming.PoolSize.VRAMPercentageClamp=512
r.Streaming.FramesForFullUpdate=15
r.Streaming.AmortizeCPUToGPUCopy=True
r.Streaming.MaxNumTexturesToStreamPerFrame=5
s.ForceGCAfterLevelStreamedOut=False

[/Script/Engine.GarbageCollectionSettings]
gc.TimeBetweenPurgingPendingKillObjects=20

[Pak]
PakCheck=False
```

# 开光追
