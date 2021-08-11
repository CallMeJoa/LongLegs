    spawn(function()
        local hum = game:GetService("Players").LocalPlayer.Character.Humanoid
        local anim = Instance.new("Animation")
        anim.AnimationId = "rbxassetid://5917459365"
        anim = hum:LoadAnimation(anim)
        anim.Priority = Enum.AnimationPriority.Action
        game:GetService("UserInputService").InputBegan:Connect(function(key, dont)
            if not(dont) and key.KeyCode == Enum.KeyCode.F then
                anim:Play(0, 9e9, 3)
            end
        end)
        game:GetService("UserInputService").InputEnded:Connect(function(key, dont)
            if not(dont) and key.KeyCode == Enum.KeyCode.F then
                anim:Stop(0, 9e9, 3)
            end
        end)
    end)
local lplr = game.Players.LocalPlayer
local chara = lplr.Character

function rm()
for i,v in pairs(chara:GetDescendants()) do
    if v:IsA("BasePart") then
        if v.Name == ("Handle") or v.Name == ("Head") then
            if chara.Head:FindFirstChild("OriginalSize") then
            chara.Head.OriginalSize:Destroy()
            end
            
            else
       
        for i,cav in pairs(v:GetDescendants()) do
        if cav:IsA("Attachment") then
        if cav:FindFirstChild("OriginalPosition") then
        cav.OriginalPosition:Destroy()  
        end
        end
        end
       
        v:FindFirstChild("OriginalSize"):Destroy()
        
end
end
end
end


rm()

wait(0.5)

  game.Players.LocalPlayer.Character.Humanoid.BodyProportionScale:Destroy()


wait(1)

rm()

wait(0.5)

  game.Players.LocalPlayer.Character.Humanoid.BodyHeightScale:Destroy()


wait(1)

rm()

wait(0.5)

  game.Players.LocalPlayer.Character.Humanoid.BodyWidthScale:Destroy()


wait(1)

rm()


wait(0.5)

  game.Players.LocalPlayer.Character.Humanoid.BodyDepthScale:Destroy()


wait(1)

rm()

wait()


wait(0.5)

  game.Players.LocalPlayer.Character.Humanoid.HeadScale:Destroy()


wait(1)
print('e')
rm()
wait(.5)
  game.Players.LocalPlayer.Character.Humanoid.HeadScale:Destroy()
