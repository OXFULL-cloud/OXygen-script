
-- OX_FuII
-- mobile friendly custom hub

local Players = game:GetService("Players")
local player = Players.LocalPlayer

local gui = Instance.new("ScreenGui")
gui.Name = "OX_FuII"
gui.ResetOnSpawn = false
gui.Parent = player:WaitForChild("PlayerGui")

local toggle = Instance.new("TextButton")
toggle.Size = UDim2.fromOffset(55, 55)
toggle.Position = UDim2.new(0, 20, 0.5, -27)
toggle.BackgroundColor3 = Color3.fromRGB(25, 25, 30)
toggle.Text = "OX"
toggle.TextColor3 = Color3.new(1, 1, 1)
toggle.TextSize = 18
toggle.Parent = gui

local main = Instance.new("Frame")
main.Size = UDim2.new(0.85, 0, 0, 220)
main.Position = UDim2.new(0.075, 0, 0.35, 0)
main.BackgroundColor3 = Color3.fromRGB(25, 25, 30)
main.Visible = false
main.Parent = gui

local title = Instance.new("TextLabel")
title.Size = UDim2.new(1, 0, 0, 45)
title.BackgroundTransparency = 1
title.Text = "OX_FuII"
title.TextColor3 = Color3.new(1, 1, 1)
title.TextSize = 18
title.Parent = main

local info = Instance.new("TextButton")
info.Size = UDim2.new(1, -20, 0, 45)
info.Position = UDim2.fromOffset(10, 60)
info.Text = "player info"
info.Parent = main

info.Activated:Connect(function()
    title.Text = player.DisplayName
end)

toggle.Activated:Connect(function()
    main.Visible = not main.Visible
end)
