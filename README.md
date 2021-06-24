local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local Sell = Instance.new("TextButton")
local Rank = Instance.new("TextButton")
local LVL = Instance.new("TextButton")
local LVL_2 = Instance.new("TextButton")
local Frame_2 = Instance.new("Frame")
local Frame_3 = Instance.new("Frame")
local TextLabel_2 = Instance.new("TextLabel")
local TextLabel_3 = Instance.new("TextLabel")
local Jump = Instance.new("TextButton")
local Jump_2 = Instance.new("TextButton")
local Frame_4 = Instance.new("Frame")
local Coins = Instance.new("TextButton")
local TextButton = Instance.new("TextButton")
 
 
ScreenGui.Parent = game.CoreGui
 
Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(61, 61, 61)
Frame.Position = UDim2.new(0.244379282, 0, 0.0110410145, 0)
Frame.Size = UDim2.new(0, 214, 0, 127)
Frame.Visible = true
Frame.Active = true
Frame.Draggable = true
 
TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.Size = UDim2.new(0, 214, 0, 16)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "SR destruction simulator"
TextLabel.TextColor3 = Color3.fromRGB(255, 17, 17)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true
 
Sell.Name = "Sell"
Sell.Parent = Frame
Sell.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Sell.BorderColor3 = Color3.fromRGB(0, 0, 0)
Sell.Position = UDim2.new(0.0747663528, 0, 0.203389823, 0)
Sell.Size = UDim2.new(0, 84, 0, 26)
Sell.Font = Enum.Font.SourceSans
Sell.Text = "Sell Brick"
Sell.TextColor3 = Color3.fromRGB(102, 255, 75)
Sell.TextSize = 16.000
Sell.TextWrapped = true
Sell.MouseButton1Down:connect(function()
	local Event = game:GetService("ReplicatedStorage").Remotes.sellBricks
	Event:FireServer()
end)
 
Rank.Name = "Rank"
Rank.Parent = Frame
Rank.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Rank.BorderColor3 = Color3.fromRGB(0, 0, 0)
Rank.Position = UDim2.new(0.556074798, 0, 0.203389823, 0)
Rank.Size = UDim2.new(0, 84, 0, 26)
Rank.Font = Enum.Font.SourceSans
Rank.Text = "Rank UP"
Rank.TextColor3 = Color3.fromRGB(58, 255, 173)
Rank.TextSize = 16.000
Rank.MouseButton1Down:connect(function()
	local Event = game:GetService("ReplicatedStorage").Remotes.rankUp
	Event:FireServer()
end)
 
LVL.Name = "LVL+"
LVL.Parent = Frame
LVL.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
LVL.BorderColor3 = Color3.fromRGB(0, 0, 0)
LVL.Position = UDim2.new(0.0747663528, 0, 0.477579087, 0)
LVL.Size = UDim2.new(0, 84, 0, 26)
LVL.Font = Enum.Font.SourceSans
LVL.Text = "LVL +10"
LVL.TextColor3 = Color3.fromRGB(76, 79, 255)
LVL.TextSize = 16.000
LVL.MouseButton1Down:connect(function()
	local A_1 = "Levels"
	local A_2 = 180
	local A_3 = 10
	local Event = game:GetService("ReplicatedStorage").Remotes.generateBoost
	Event:FireServer(A_1, A_2, A_3)
end)
LVL_2.Name = "-LVL"
LVL_2.Parent = Frame
LVL_2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
LVL_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
LVL_2.Position = UDim2.new(0.556074679, 0, 0.477579117, 0)
LVL_2.Size = UDim2.new(0, 84, 0, 26)
LVL_2.Font = Enum.Font.SourceSans
LVL_2.Text = "LVL -10"
LVL_2.TextColor3 = Color3.fromRGB(190, 99, 255)
LVL_2.TextSize = 16.000
LVL_2.MouseButton1Down:connect(function()
	local A_1 = "Levels"
	local A_2 = 180
	local A_3 = -10
	local Event = game:GetService("ReplicatedStorage").Remotes.generateBoost
	Event:FireServer(A_1, A_2, A_3)
end)
Frame_2.Parent = Frame
Frame_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame_2.Position = UDim2.new(0, 0, 0.125984192, 0)
Frame_2.Size = UDim2.new(0, 214, 0, 4)
 
Frame_3.Parent = Frame
Frame_3.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
Frame_3.Position = UDim2.new(1.08878505, 0, 0, 0)
Frame_3.Size = UDim2.new(0, 193, 0, 127)
 
TextLabel_2.Parent = Frame_3
TextLabel_2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_2.Size = UDim2.new(0, 193, 0, 16)
TextLabel_2.Font = Enum.Font.SourceSans
TextLabel_2.Text = "Fun Options"
TextLabel_2.TextColor3 = Color3.fromRGB(255, 17, 17)
TextLabel_2.TextScaled = true
TextLabel_2.TextSize = 14.000
TextLabel_2.TextWrapped = true
 
TextLabel_3.Parent = TextLabel_2
TextLabel_3.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_3.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_3.Position = UDim2.new(0.150259063, 0, 4.5625, 0)
TextLabel_3.Size = UDim2.new(0, 135, 0, 31)
TextLabel_3.Font = Enum.Font.SourceSans
TextLabel_3.Text = "well im bord."
TextLabel_3.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_3.TextSize = 14.000
 
Jump.Name = "Jump"
Jump.Parent = Frame_3
Jump.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Jump.BorderColor3 = Color3.fromRGB(0, 0, 0)
Jump.Position = UDim2.new(0.0369714312, 0, 0.196983844, 0)
Jump.Size = UDim2.new(0, 84, 0, 26)
Jump.Font = Enum.Font.SourceSans
Jump.Text = "Jump x2"
Jump.TextColor3 = Color3.fromRGB(255, 255, 47)
Jump.TextSize = 16.000
Jump.MouseButton1Down:connect(function()
	local A_1 = "SuperJump"
	local A_2 = 1200
	local A_3 = 3
	local Event = game:GetService("ReplicatedStorage").Remotes.generateBoost
	Event:FireServer(A_1, A_2, A_3)
end)
 
Jump_2.Name = "Jump"
Jump_2.Parent = Frame_3
Jump_2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Jump_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
Jump_2.Position = UDim2.new(0.529199421, 0, 0.196983844, 0)
Jump_2.Size = UDim2.new(0, 84, 0, 26)
Jump_2.Font = Enum.Font.SourceSans
Jump_2.Text = "- Jump x2"
Jump_2.TextColor3 = Color3.fromRGB(255, 129, 19)
Jump_2.TextSize = 16.000
Jump_2.MouseButton1Down:connect(function()
	local A_1 = "SuperJump"
	local A_2 = -1200
	local A_3 = 3
	local Event = game:GetService("ReplicatedStorage").Remotes.generateBoost
	Event:FireServer(A_1, A_2, A_3)
end)
 
Frame_4.Parent = Frame_3
Frame_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame_4.Position = UDim2.new(0, 0, 0.125984192, 0)
Frame_4.Size = UDim2.new(0, 193, 0, 4)
 
Coins.Name = "Coins"
Coins.Parent = Frame
Coins.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Coins.BorderColor3 = Color3.fromRGB(0, 0, 0)
Coins.Position = UDim2.new(0.0746210814, 0, 0.74029094, 0)
Coins.Size = UDim2.new(0, 84, 0, 26)
Coins.Font = Enum.Font.SourceSans
Coins.Text = "1M Coins"
Coins.TextColor3 = Color3.fromRGB(238, 49, 255)
Coins.TextSize = 16.000
Coins.MouseButton1Down:connect(function()
	game:GetService("ReplicatedStorage").Remotes.generateBoost:FireServer("Coins", 480, 1000000)
end)
 
TextButton.Name = ""
TextButton.Parent = Frame
TextButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
TextButton.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextButton.Position = UDim2.new(0.552563906, 0, 0.74029088, 0)
TextButton.Size = UDim2.new(0, 84, 0, 26)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = "- 1M Coins"
TextButton.TextColor3 = Color3.fromRGB(111, 8, 255)
TextButton.TextSize = 16.000
TextButton.MouseButton1Down:connect(function()
	game:GetService("ReplicatedStorage").Remotes.generateBoost:FireServer("Coins", 480, -1000000)
end)
 
-- Scripts:
 
local function MWUUDFA_fake_script() -- Frame_2.LocalScript 
	local script = Instance.new('LocalScript', Frame_2)
 
	function zigzag(X) return math.acos(math.cos(X*math.pi))/math.pi end
 
	counter = 0
 
	while wait(0.2)do
	 script.Parent.BackgroundColor3 = Color3.fromHSV(zigzag(counter),1,1)
 
	 counter = counter + 0.01
	end
end
coroutine.wrap(MWUUDFA_fake_script)()
local function NXPK_fake_script() -- Frame_4.LocalScript 
	local script = Instance.new('LocalScript', Frame_4)
 
	function zigzag(X) return math.acos(math.cos(X*math.pi))/math.pi end
 
	counter = 0
 
	while wait(0.1)do
	 script.Parent.BackgroundColor3 = Color3.fromHSV(zigzag(counter),1,1)
 
	 counter = counter + 0.01
	end
end
coroutine.wrap(NXPK_fake_script)()
