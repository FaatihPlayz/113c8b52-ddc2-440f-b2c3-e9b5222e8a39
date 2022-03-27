local Luminosity = loadstring(game:HttpGet("https://raw.githubusercontent.com/iHavoc101/Genesis-Studios/main/UserInterface/Luminosity.lua", true))()

local Window = Luminosity.new("Humanoid Hub", "v0.8.3a", 4370345701)

local Tab1 = Window.Tab("Main", 6026568198)
local Tab2 = Window.Tab("About", 6035181881)
local Folder = Tab1.Folder("Humanoid", "Basically your character settings.")
local Folder2 = Tab2.Folder("About Page", "you know what this means bro.")
Folder2.TextLabel("UI Lib = Luminosity V1")
Folder2.TextLabel("Current Repo Owner = Not telling discord, V3rmil = RenderQOnTop")
Folder2.TextLabel("UI Lib Maker (i think) = OminousVibes")
Folder2.TextLabel("Teleportation Section = ")
Folder.Switch("Test if your switches are working", function(Status)
print("Switch Triggered: " .. tostring(Status))
end)
Folder.Switch("Super Jump", function(SJump)
game.Players.LocalPlayer.Character.Humanoid.JumpPower = 150
end)
Folder.Switch("Super Speed", function(SSpeed)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 150
end)
Folder.Switch("Reset Speed", function(RSpeed)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 16
end)
Folder.Switch("Reset Jump", function(RJump)
game.Players.LocalPlayer.Character.Humanoid.JumpPower = 50
end)
Folder.Switch("Reset Speed but for PET SIM", function(RSpeedPetSim)
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 25
end)
