-- MM2 Auto Farm - Delta Fix
local Players = game:GetService("Players")
local player = Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

_G.Farm = true -- Durdurmak istersen false yap

spawn(function()
    while _G.Farm do
        wait(0.1)
        local coins = workspace:FindFirstChild("CoinContainer", true)
        if coins then
            for _, coin in pairs(coins:GetChildren()) do
                if coin:IsA("BasePart") and _G.Farm then
                    -- Altına ışınlanmak yerine altını karakterine çeken "Magnet" mantığı
                    coin.CFrame = character.HumanoidRootPart.CFrame
                    wait(0.05) 
                end
            end
        end
    end
end)
