# WuWaUETuning
- 当前适配游戏版本：2.0.x

# Engine.ini
## [/Script/Engine.StreamingSettings]
```
r.Streaming.LimitPoolSizeToVRAM=True
r.Streaming.PoolSizeForMeshes=-1
r.Streaming.HLODStrategy=2
r.Streaming.FullyLoadUsedTextures=True
r.Streaming.FramesForFullUpdate=30
; r.Streaming.AmortizeCPUToGPUCopy=True
; r.Streaming.MaxNumTexturesToStreamPerFrame=5
s.ForceGCAfterLevelStreamedOut=False
s.IoDispatcherCacheSizeMB=2048
```
- r.Streaming.HLODStrategy  
  内存<16G，填0  
  内存>=16G，填2  
- s.IoDispatcherCacheSizeMB  
  内存<8G，填256  
  内存>=8G，填512  
  内存>=12G，填1024  
  内存>=16G，填2048  

## [/Script/Engine.RendererOverrideSettings]
### Framerate | 帧率
```
r.Shaders.AllowCompilingThroughWorkers=False
FX.BatchAsync=True
FX.EarlyScheduleAsync=True
r.GTSyncType=1
RHI.MaximumFrameLatency=3
RHI.SyncSlackMS=0
RHI.SyncInterval=0
a.URO.ForceAnimRate=1
```
### AA | 抗锯齿
```
r.ScreenPercentage=100
r.TemporalAACurrentFrameWeight=0.2
r.TemporalAASamples=4
r.Tonemapper.Sharpen=0.8
r.NGX.DLSS.Sharpness=0.8
```
### Tone | 后期色调
```
; r.KuroTonemapping=1
r.Color.Mid=0.37
r.Color.Max=1.12
r.TonemapperFilm=True
r.Tonemapper.Quality=1
r.Tonemapper.GrainQuantization=0
r.SceneColorFringeQuality=0
```
### Effects | 后期视觉
```
r.MotionBlur.TargetFPS=0
r.MotionBlur.Amount=0.5
r.MotionBlur.Scale=5.0
r.Kuro.AutoExposure=True
r.Kuro.EyeAdaptation.CustomValueMode=True
r.Kuro.EyeAdaptation.ExposureBiasOverride=-1.25
```
### Texture | 材质
```
; r.DetailMode=2
; r.MaterialQualityLevel=3
r.MaxAnisotropy=16
; r.AnisotropicMaterials=True
r.MipMapLODBias=0
r.LandscapeLODBias=0
r.SkeletalMeshLODBias=0
r.ClearCoatNormal=True
```
### Distance | 视距
```
r.ViewDistanceScale=1.5
foliage.LODDistanceScale=1.5
r.LandscapeLODDistributionScale=1.5
r.LandscapeLOD0DistributionScale=1.5
r.LODFadeTime=1.0
```
### GI | 全局光照
```
r.SkyLightingQuality=1
r.SkylightIntensityMultiplier=0.75
; r.Kuro.GlobalLightQuality=4
; r.Kuro.LightFadeTime=1.0
```
### AO | 环境遮蔽
```
r.DistanceFieldAO=True
r.AOObjectDistanceField=True
r.DistanceFieldShadowing=True
r.AmbientOcclusionMaxQuality=100
r.AmbientOcclusion.Method=1
```
### Shadow | 阴影
```
r.AllowLandscapeShadows=True
r.AllowPointLightCubemapShadows=True
r.Shadow.MinResolution=2048
r.Shadow.MaxResolution=2048
r.Shadow.MaxCSMResolution=2048
r.Shadow.PerObjectResolutionMin=2048
r.Shadow.PerObjectResolutionMax=2048
r.Shadow.PerObjectShadowMapResolution=2048
```
显存<8G，分辨率全部填512  
显存>=8G，分辨率全部填1024  
显存>=12G，分辨率全部填2048  
显存>=16G，分辨率全部填4096  

### Reflection | 反射
```
r.SSR.Quality=4
r.SSR.HalfResSceneColor=False
r.SSR.Temporal=False
```

## [Pak]
```
PakCheck=False
```
