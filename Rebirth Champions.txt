
-- Script by QuiKz aka Exsicy
-- i am not good at making scripts i made this just cuz i was bored





local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Roblox", "Synapse")

local Tab = Window:NewTab("Scripts")
local Section = Tab:NewSection("Autofarm")

Section:NewButton("Collect Easter Eggs", "ButtonInfo", function()
    Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Forest.Forest.Leaves.CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Snowman.Snowman.Main.CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Fire.Fire["Meshes/vulcaonegg1_Cylinder"].CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Atlantis.Atlantis.part.CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Toxic.Toxic["Meshes/toxicegg_egg.002"].CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Cave.Cave["Meshes/easteregg1_egg.001"].CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Alien.Note.CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Alien.Note2.CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Alien.Note3.CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=game:GetService("Workspace").Scripts.EggHunt.Cave.Cave["Meshes/easteregg1_egg.001"].CFrame;wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=CFrame.new(390,4,695)wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=CFrame.new(384,4,691)wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=CFrame.new(371,4,676)wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)Game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame=CFrame.new(387,5,675)wait(0.3)local a=game:GetService('VirtualUser')a:CaptureController()a:SetKeyDown('0x65')wait(0.1)a:SetKeyUp('0x65')wait(1)game:GetService("ReplicatedStorage").Events.Codes:FireServer("834519-385-3092")game:GetService("ReplicatedStorage").Events.EggHunt:FireServer()
end)

Section:NewToggle("1500x Boost Loop", "ToggleInfo", function(state)
    _G.ClickLoop = state
 while _G.ClickLoop == true do 
    game:GetService("ReplicatedStorage").Events.WorldBoost:FireServer("Cave")
 wait() end end)



Section:NewToggle("Click", "ToggleInfo", function(state)
   _G.Toggle = state
while _G.Toggle == true do 
game:GetService("ReplicatedStorage").Events.Click3:FireServer()
wait() end end)

local list = {
    "100 Egg";
    "25k Egg";
    "Forest Egg";
    "Beach Egg";
    "Atlantis Egg";
    "Desert Egg";
    "Winter Egg";
    "Volcano Egg";
    "Spooky Egg";
    "Cave Egg"; 
    "Easter Egg";  
}

Section:NewDropdown("Select Egg", "DropdownInf", list, function(currentOption)
    _G.SelectedEgg = currentOption
end)

Section:NewToggle("Auto Hatch", "ToggleInfo", function(state)
    _G.Hatch = state
    while _G.Hatch == true do
        if _G.SelectedEgg == "100 Egg" then
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Basic",_G.TripleEgg)
            wait() else 
        if _G.SelectedEgg == "25k Egg" then
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Mythic",_G.TripleEgg)
            wait() else 
        if _G.SelectedEgg == "Forest Egg" then
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Forest",_G.TripleEgg)
            wait() else
        if _G.SelectedEgg == "Beach Egg" then
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Beach", _G.TripleEgg)
            wait() else 
        if _G.SelectedEgg == "Atlantis Egg" then
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Atlantis", _G.TripleEgg)
            wait() else
        if _G.SelectedEgg == "Desert Egg" then
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Desert", _G.TripleEgg)
            wait() else
        if _G.SelectedEgg == "Winter Egg" then
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Winter", _G.TripleEgg)
            wait() else
        if _G.SelectedEgg == "Volcano Egg" then
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Volcano", _G.TripleEgg)
            wait() else 
        if _G.SelectedEgg == "Spooky Egg" then 
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Spooky", _G.TripleEgg)
            wait() else
        if _G.SelectedEgg == "Cave Egg" then 
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Cave", _G.TripleEgg)
            wait() else
        if _G.SelectedEgg == "Easter Egg" then 
            game:GetService("ReplicatedStorage").Functions.Unbox:InvokeServer("Easter Part 2", _G.TripleEgg)
            wait() else
            
        end end end end end end end end end end end end end)

        Section:NewToggle("Triple Egg", "ToggleInfo", function(state)
            if state == true then
                _G.TripleEgg = "Triple" else if state == false then _G.TripleEgg = "Single"
            
       end end end)



local teleports = Window:NewTab("Teleports")
local worlds = teleports:NewSection("Worlds")

local teleports = {
    "Spawn";
    "Forest";
    "Beach";
    "Atlantis";
    "Desert";
    "Winter";
    "Volcano";
    "Moon";
    "Cyber";
    "Magic";
    "Heaven";
    "Nuclear";
    "Void";
    "Spooky";
    "Cave"
}
worlds:NewDropdown("Teleport", "DropdownInf", teleports, function(currentOption)
    _G.Location = currentOption
    if _G.Location == "Spawn" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(225, 29, 66) else
    if _G.Location == "Forest" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-380, 30, 176) else
    if _G.Location == "Beach" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-517, 35, 458) else
    if _G.Location == "Atlantis" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(40, 8, 676) else
    if _G.Location == "Desert" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(469, 5, 705) else
    if _G.Location == "Winter" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1035, -49, 165) else
    if _G.Location == "Volcano" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1044, -39, 596) else
    if _G.Location == "Moon" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-373, 34, -184) else
    if _G.Location == "Cyber" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-373, 36, -477) else        
    if _G.Location == "Magic" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-27, 36, -479) else
    if _G.Location == "Heaven" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-392, 34, -760) else
    if _G.Location == "Nuclear" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(251, 48, -505) else
    if _G.Location == "Void" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(246, 48, -779) else
    if _G.Location == "Spooky" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-82, 31, -760) else
     if _G.Location == "Cave" then 
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(416, 9, -334) else
end end end end end end end end end end end end end end end end)



local menu = Window:NewTab("Settings")
local settings = menu:NewSection("Misc")

settings:NewKeybind("Toggle Menu", "KeybindInfo", Enum.KeyCode.RightShift, function()
	Library:ToggleUI()
end)