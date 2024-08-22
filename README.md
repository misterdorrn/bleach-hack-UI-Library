# Example
```lua
local Lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/devdoroz/bleachhack-ui-lib/main/zmacsploitsynchrousfix.lua"))()
local UI = Lib:Create()

local configSavingUI = game:GetObjects("rbxassetid://18187656247")[1]:Clone()
configSavingUI.Parent = (gethui and gethui()) or game:GetService("CoreGui")
configSavingUI.Enabled = false

local w1 = UI:CreateCategory("Main", "")

local ws = w1:CreateToggle({
	Title = "Walkspeed"
})

local wsadjust = w1:CreateSlider({
	Title = "Custom Walkspeed",
	Range = {20, 23}
})

local wa1 = Physics:CreateModule("Walkspeed")
local walk = w1:CreateSwitch({
	Title = "Type",
	Range = {"CFrame", "Humanoid"}
})

local TP = quickTP:CreateKeybind({
	Title = "Keybind",
	Value = Enum.KeyCode.F
})


```
