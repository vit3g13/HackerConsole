local CoreGui = game:GetService("StarterGui")
CoreGui:SetCore("SendNotification", {
    Title = "vit3g Script",
    Text = "from https://robloxscripts15.webnode.cz",
    Icon = "",
    Duration = 10,
    Callback = AllowRunServiceBind,
})

print("executed hacker console")


local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Name = "LoadstringGui"
ScreenGui.ResetOnSpawn = false
ScreenGui.Parent = game.CoreGui

local Frame = Instance.new("Frame")
Frame.Size = UDim2.new(0, 800, 0, 480)
Frame.Position = UDim2.new(0.25, 0, 0.25, 0)
Frame.BackgroundColor3 = Color3.fromRGB(0, 245, 0)
Frame.Active = true
Frame.Draggable = true
Frame.Parent = ScreenGui

local UICorner = Instance.new("UICorner", Frame)
UICorner.CornerRadius = UDim.new(0, 10)

local Title = Instance.new("TextLabel")
Title.Text = "Admin"
Title.Font = Enum.Font.GothamBold
Title.TextSize = 24
Title.TextColor3 = Color3.new(0, 0, 0)
Title.BackgroundTransparency = 1
Title.Size = UDim2.new(1, -50, 0, 40)
Title.Position = UDim2.new(0, 610, 0, 155)
Title.TextXAlignment = Enum.TextXAlignment.Left
Title.Parent = Frame


local Title = Instance.new("TextLabel")
Title.Text = "Speed"
Title.Font = Enum.Font.GothamBold
Title.TextSize = 24
Title.TextColor3 = Color3.new(0, 0, 0)
Title.BackgroundTransparency = 1
Title.Size = UDim2.new(1, -1, 0, 40)
Title.Position = UDim2.new(0, 630, 0, 10)
Title.TextXAlignment = Enum.TextXAlignment.Left
Title.Parent = Frame

local Title = Instance.new("TextLabel")
Title.Text = "idk"
Title.Font = Enum.Font.GothamBold
Title.TextSize = 24
Title.TextColor3 = Color3.new(0, 0, 0)
Title.BackgroundTransparency = 1
Title.Size = UDim2.new(1, -50, 0, 40)
Title.Position = UDim2.new(0, 630, 0, 240)
Title.TextXAlignment = Enum.TextXAlignment.Left
Title.Parent = Frame

local Title = Instance.new("TextLabel")
Title.Text = "Terminal/developer console"
Title.Font = Enum.Font.GothamBold
Title.TextSize = 24
Title.TextColor3 = Color3.new(0, 0, 0)
Title.BackgroundTransparency = 1
Title.Size = UDim2.new(1, -50, 0, 40)
Title.Position = UDim2.new(0, 10, 0, 5)
Title.TextXAlignment = Enum.TextXAlignment.Left
Title.Parent = Frame

local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 280, 0, 50)
CloseButton.Position = UDim2.new(1, -295, 0, 110)
CloseButton.Text = " Reset walk speed"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()
  game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 16
end)



local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 150, 0, 20)
CloseButton.Position = UDim2.new(1, -325, 0, 15)
CloseButton.Text = "Stop Music"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()
-- Počkej chvilku na načtení hry
task.wait(1)

-- Projdi všechny objekty ve hře
for _, obj in ipairs(game:GetDescendants()) do
	-- Pokud je to Sound a právě hraje, zastav ho
	if obj:IsA("Sound") and obj.IsPlaying then
		obj:Stop()
	end
end

end)


local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 150, 0, 20)
CloseButton.Position = UDim2.new(1, -480, 0, 15)
CloseButton.Text = "Play Music"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()
  local Sound = Instance.new("Sound")
Sound.SoundId = "rbxassetid://142376088"
Sound.Volume = 1
Sound.Looped = true
Sound.Parent = workspace
Sound:Play()

end)







local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 280, 0, 50)
CloseButton.Position = UDim2.new(1, -295, 0, 400)
CloseButton.Text = "1x1x1x1 Visual"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()
loadstring(game:HttpGet("https://pastebin.com/raw/gd4qQJGu"))()
end)



local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 280, 0, 20)
CloseButton.Position = UDim2.new(1, -295, 0, 460)
CloseButton.Text = "Dont click me!!!"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()

end)




local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 280, 0, 50)
CloseButton.Position = UDim2.new(1, -295, 0, 340)
CloseButton.Text = "Universal aimbot,esp"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()
  loadstring(game:HttpGet("https://raw.githubusercontent.com/ttwizz/Open-Aimbot/master/source.lua"))()
end)




local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 280, 0, 50)
CloseButton.Position = UDim2.new(1, -295, 0, 280)
CloseButton.Text = "Sus Emote"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()
  loadstring(game:HttpGet("https://pastefy.app/wa3v2Vgm/raw"))()
loadstring(game:HttpGet("https://pastefy.app/YZoglOyJ/raw"))()
end)



local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 280, 0, 50)
CloseButton.Position = UDim2.new(1, -295, 0, 190)
CloseButton.Text = "Infinite Yield"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()
 loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
end)







local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 280, 0, 50)
CloseButton.Position = UDim2.new(1, -295, 0, 50)
CloseButton.Text = "Walk speed 100"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()
  game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 100
end)





local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 40, 0, 30)
CloseButton.Position = UDim2.new(1, -45, 0, 5)
CloseButton.Text = "X"
CloseButton.Font = Enum.Font.GothamBold
CloseButton.TextSize = 20
CloseButton.TextColor3 = Color3.new(0, 255, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
CloseButton.Parent = Frame

local CloseCorner = Instance.new("UICorner", CloseButton)
CloseCorner.CornerRadius = UDim.new(0, 6)

CloseButton.MouseButton1Click:Connect(function()
	ScreenGui:Destroy()
end)


local TextBox = Instance.new("TextBox")
TextBox.Size = UDim2.new(0, 480, 0, 360)
TextBox.Position = UDim2.new(0, 10, 0, 50)
TextBox.PlaceholderText = ""
TextBox.Text = ""
TextBox.TextSize = 16
TextBox.ClearTextOnFocus = false
TextBox.TextWrapped = true
TextBox.TextXAlignment = Enum.TextXAlignment.Left
TextBox.TextYAlignment = Enum.TextYAlignment.Top
TextBox.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
TextBox.TextColor3 = Color3.new(0, 255, 0)
TextBox.Parent = Frame

local UICorner2 = Instance.new("UICorner", TextBox)
UICorner2.CornerRadius = UDim.new(0, 6)


local LoadButton = Instance.new("TextButton")
LoadButton.Size = UDim2.new(0, 480, 0, 50)
LoadButton.Position = UDim2.new(0, 10, 0, 420)
LoadButton.Text = "Hack"
LoadButton.Font = Enum.Font.GothamBold
LoadButton.TextSize = 18
LoadButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
LoadButton.TextColor3 = Color3.new(0, 255, 0)
LoadButton.Parent = Frame

local UICorner3 = Instance.new("UICorner", LoadButton)
UICorner3.CornerRadius = UDim.new(0, 6)


LoadButton.MouseButton1Click:Connect(function()
    local success, err = pcall(function()
        loadstring(TextBox.Text)()
    end)
    if not success then
        warn("Error (Reson script): " .. err)
    end
end)
