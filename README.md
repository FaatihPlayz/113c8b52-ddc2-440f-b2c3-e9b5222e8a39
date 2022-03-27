local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/AikaV3rm/UiLib/master/Lib.lua')))()

local t = library:CreateWindow("Main")

local b = t:CreateFolder("Humanoid")

local 
b:Label("Humanoid",{
    TextSize = 25; -- Self Explaining
    TextColor = Color3.fromRGB(255,255,255); -- Self Explaining
    BgColor = Color3.fromRGB(69,69,69); -- Self Explaining
    
}) 

b:Toggle("Abort All Functions",function(bool)
    shared.toggle = bool
    warn("Aborting.") then
        print(shared.toggle)
end)

b:Slider("WalkSpeed",{
    min = 16; -- min value of the slider
    max = 256; -- max value of the slider
    precise = true; -- max 2 decimals
},function(value1)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value1
end)

b:Slider("JumpPower",{
    min = 16; -- min value of the slider
    max = 256; -- max value of the slider
    precise = true; -- max 2 decimals
},function(value2)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = value2
end)

b:Bind("Bind",Enum.KeyCode.C,function() --Default bind
    print("wat")
end)

b:DestroyGui()
