# QuickTween
Better Tweening

```luau
const ReplicatedStorage = game:GetService("ReplicatedStorage")
const QuickTween = require(ReplicatedStorage.Packages.QuickTween)



-- Play a tween, cleanup after
QuickTween.Spawn(objectToTween, duration, easingStyle, easingDirection, {objectValue = targetValue})

-- Create a tween object (Spawn but you can reuse it)
local tween = QuickTween.Object(objectToTween, duration, easingStyle, easingDirection, {objectValue = targetValue})

-- Create a tween group
local group = QuickTween.Group({tween})
group:Play()
group:Pause()
group:Cancel()
group:Destroy()

-- Tween model CFrame and Scale
QuickTween.TweenModelCFrame(modelToTween, duration, easingStyle, easingDirection, targetCFrame)
QuickTween.TweenModelScale(modelToTween, duration, easingStyle, easingDirection, targetScale)
```
