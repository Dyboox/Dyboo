# Example Dyboo Lib

```lua
local Dyboo = loadstring(game:HttpGet("https://raw.githubusercontent.com/Dyboox/Dyboo/refs/heads/main/DybooXXLib.lua"))()
local Window = Dyboo:AddWindow("Dyboo","Example",'original')

Window:AddTabLabel("Example")
local MainTab = Window:AddTab("Main","home")
local ExtraTab = Window:AddTab("Extra","star")
Window:AddTabLabel("System")
local VisualTab = Window:AddTab("Visual","earth")

local Main = MainTab:AddSection("MAIN","left")  
Main:AddToggle("Enable Feature",true,function(v)end)  
Main:AddToggle("Auto Action",false,function(v)end)  
Main:AddToggle("Background Run",true,function(v)end)  
Main:AddToggle("Safe Mode",true,function(v)end)  
Main:AddSlider("Power Level",1,100,50,function(v)end)  

local Settings = MainTab:AddSection("SETTINGS","left")  
Settings:AddDropdown("Mode",{"Normal","Fast","Extreme"},"Normal",function(v)end)  
Settings:AddDropdown("Priority",{"High","Medium","Low"},"Medium",function(v)end)  
Settings:AddDropdown("Profile",{"Default","Custom","Guest"},"Default",function(v)end)  
Settings:AddSlider("Speed",1,200,100,function(v)end)  
Settings:AddSlider("Delay",0,10,1,function(v)end)  
Settings:AddToggle("Protection",true,function(v)end)  
Settings:AddToggle("Auto Save",true,function(v)end)  

local Extra = MainTab:AddSection("EXTRA","right")  
Extra:AddDropdown("Theme",{"Dark","Light","Blue"},"Dark",function(v)end)  
Extra:AddToggle("Notification",true,function(v)end)  
Extra:AddToggle("Sound Effect",false,function(v)end)  
Extra:AddToggle("Mini Mode",false,function(v)end)  
Extra:AddDropdown("Animation",{"Off","Smooth","Fast"},"Smooth",function(v)end)  
Extra:AddDropdown("Refresh Rate",{"Low","Medium","High"},"High",function(v)end)  

local Control = MainTab:AddSection("CONTROL","right")  
Control:AddToggle("Enabled",false,function(v)end)  
Control:AddDropdown("State",{"Idle","Run","Pause"},"Idle",function(v)end)  
Control:AddDropdown("Direction",{"Forward","Backward","None"},"None",function(v)end)  
Control:AddDropdown("Variation",{"Disabled","Low","High"},"Disabled",function(v)end)  
Control:AddToggle("Slow Mode",false,function(v)end)  
Control:AddToggle("Assist",false,function(v)end)
