-- ⚡ LIT ENERGY • TOP 1 SCRIPT ⚡
local Players = game:GetService("Players")
local UserInputService = game:GetService("UserInputService")
local RunService = game:GetService("RunService")
local TweenService = game:GetService("TweenService")
local Workspace = game:GetService("Workspace")
local Lighting = game:GetService("Lighting")
local StarterGui = game:GetService("StarterGui")

local player = Players.LocalPlayer
local camera = Workspace.CurrentCamera

------------------------------------------------------------
-- НАСТРОЙКИ
------------------------------------------------------------
local Settings = {
	AntiRagdoll  = true,
	InfiniteJump = false,
	Aimbot       = false,
	AntiLag      = false,
	AntiDie      = false,
	AutoGrab     = false,
	WalkSpeed    = 16,
	ToggleKey    = Enum.KeyCode.RightShift,
}

local InfJumpMode = 1
local InfJumpModes = { "Hold", "Tap" }

------------------------------------------------------------
-- ИНТРО
------------------------------------------------------------
local intro = Instance.new("ScreenGui")
intro.Name = "LitEnergyIntro"
intro.ResetOnSpawn = false
intro.IgnoreGuiInset = true
intro.DisplayOrder = 10
intro.Parent = player:WaitForChild("PlayerGui")

local function makeIntroLabel(text, color, fromX)
	local lbl = Instance.new("TextLabel")
	lbl.AnchorPoint = Vector2.new(0.5, 0.5)
	lbl.Size = UDim2.new(0, 600, 0, 80)
	lbl.Position = UDim2.new(fromX, 0, 0.4, 0)
	lbl.BackgroundTransparency = 1
	lbl.Text = text
	lbl.TextColor3 = color
	lbl.Font = Enum.Font.GothamBlack
	lbl.TextSize = 60
	lbl.TextStrokeTransparency = 0
	lbl.TextStrokeColor3 = Color3.fromRGB(0, 0, 0)
	lbl.Parent = intro
	return lbl
end

local leftPart  = makeIntroLabel("TOP 1 SCRIPT", Color3.fromRGB(255, 220, 60), -0.5)
local rightPart = makeIntroLabel("LIT ENERGY",   Color3.fromRGB(80, 220, 255), 1.5)

local linkPart = Instance.new("TextLabel")
linkPart.AnchorPoint = Vector2.new(0.5, 0.5)
linkPart.Size = UDim2.new(0, 900, 0, 40)
linkPart.Position = UDim2.new(0.5, 0, 0.55, 0)
linkPart.BackgroundTransparency = 1
linkPart.Text = "TOP 1 PURCHASE SCRIPT LINK IS discord.gg/q3BKJ2hvY"
linkPart.TextColor3 = Color3.fromRGB(255, 255, 255)
linkPart.Font = Enum.Font.GothamBold
linkPart.TextSize = 22
linkPart.TextStrokeTransparency = 1
linkPart.TextTransparency = 1
linkPart.Parent = intro

task.spawn(function()
	task.wait(0.3)
	TweenService:Create(leftPart, TweenInfo.new(0.9, Enum.EasingStyle.Quart, Enum.EasingDirection.Out),
		{Position = UDim2.new(0.5, -230, 0.4, 0)}):Play()
	TweenService:Create(rightPart, TweenInfo.new(0.9, Enum.EasingStyle.Quart, Enum.EasingDirection.Out),
		{Position = UDim2.new(0.5, 230, 0.4, 0)}):Play()
	task.wait(1.0)
	TweenService:Create(linkPart, TweenInfo.new(0.5), {TextTransparency = 0, TextStrokeTransparency = 0}):Play()
	task.wait(0.6)
	for _ = 1, 2 do
		TweenService:Create(leftPart, TweenInfo.new(0.15), {TextSize = 66}):Play()
		TweenService:Create(rightPart, TweenInfo.new(0.15), {TextSize = 66}):Play()
		task.wait(0.15)
		TweenService:Create(leftPart, TweenInfo.new(0.15), {TextSize = 60}):Play()
		TweenService:Create(rightPart, TweenInfo.new(0.15), {TextSize = 60}):Play()
		task.wait(0.15)
	end
	task.wait(0.5)
	TweenService:Create(leftPart, TweenInfo.new(0.7, Enum.EasingStyle.Quart, Enum.EasingDirection.In),
		{Position = UDim2.new(-0.6, 0, 0.4, 0), TextTransparency = 1, TextStrokeTransparency = 1}):Play()
	TweenService:Create(rightPart, TweenInfo.new(0.7, Enum.EasingStyle.Quart, Enum.EasingDirection.In),
		{Position = UDim2.new(1.6, 0, 0.4, 0), TextTransparency = 1, TextStrokeTransparency = 1}):Play()
	TweenService:Create(linkPart, TweenInfo.new(0.7, Enum.EasingStyle.Quart, Enum.EasingDirection.In),
		{Position = UDim2.new(0.5, 0, 0.7, 0), TextTransparency = 1, TextStrokeTransparency = 1}):Play()
	task.wait(1)
	intro:Destroy()
end)

------------------------------------------------------------
-- ПОСТОЯННЫЙ ТЕКСТ ССЫЛКИ
------------------------------------------------------------
local linkGui = Instance.new("ScreenGui")
linkGui.Name = "LitEnergyLink"
linkGui.ResetOnSpawn = false
linkGui.IgnoreGuiInset = true
linkGui.DisplayOrder = 50
linkGui.Parent = player:WaitForChild("PlayerGui")

local linkLabel = Instance.new("TextLabel")
linkLabel.AnchorPoint = Vector2.new(0.5, 1)
linkLabel.Size = UDim2.new(1, 0, 0, 22)
linkLabel.Position = UDim2.new(0.5, 0, 1, -6)
linkLabel.BackgroundTransparency = 1
linkLabel.Text = "TOP 1 PURCHASE SCRIPT LINK IS discord.gg/q3BKJ2hvY"
linkLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
linkLabel.Font = Enum.Font.GothamBold
linkLabel.TextSize = 16
linkLabel.TextStrokeTransparency = 0
linkLabel.TextStrokeColor3 = Color3.fromRGB(0, 0, 0)
linkLabel.Parent = linkGui

task.spawn(function()
	while linkGui.Parent do
		TweenService:Create(linkLabel, TweenInfo.new(1.2, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut),
			{TextTransparency = 0.35}):Play()
		task.wait(1.2)
		TweenService:Create(linkLabel, TweenInfo.new(1.2, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut),
			{TextTransparency = 0}):Play()
		task.wait(1.2)
	end
end)

------------------------------------------------------------
-- GUI КОРЕНЬ
------------------------------------------------------------
local gui = Instance.new("ScreenGui")
gui.Name = "LitEnergyUI"
gui.ResetOnSpawn = false
gui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
gui.DisplayOrder = 100
gui.IgnoreGuiInset = true
gui.Parent = player:WaitForChild("PlayerGui")

local openBtn = Instance.new("TextButton")
openBtn.Size = UDim2.new(0, 50, 0, 50)
openBtn.Position = UDim2.new(1, -65, 0, 15)
openBtn.BackgroundColor3 = Color3.fromRGB(25, 25, 32)
openBtn.Text = "⚙"
openBtn.TextColor3 = Color3.fromRGB(80, 220, 130)
openBtn.Font = Enum.Font.GothamBlack
openBtn.TextSize = 26
openBtn.BorderSizePixel = 0
openBtn.Parent = gui

local obc = Instance.new("UICorner")
obc.CornerRadius = UDim.new(0, 12)
obc.Parent = openBtn

local obstroke = Instance.new("UIStroke")
obstroke.Color = Color3.fromRGB(80, 220, 130)
obstroke.Thickness = 1.5
obstroke.Transparency = 0.4
obstroke.Parent = openBtn

local aimBtn = Instance.new("TextButton")
aimBtn.Size = UDim2.new(0, 55, 0, 55)
aimBtn.Position = UDim2.new(1, -68, 0, 75)
aimBtn.BackgroundColor3 = Color3.fromRGB(25, 25, 32)
aimBtn.Text = "🎯"
aimBtn.TextColor3 = Color3.fromRGB(255, 255, 255)
aimBtn.Font = Enum.Font.GothamBlack
aimBtn.TextSize = 22
aimBtn.BorderSizePixel = 0
aimBtn.Parent = gui

local abc = Instance.new("UICorner")
abc.CornerRadius = UDim.new(1, 0)
abc.Parent = aimBtn

local abstroke = Instance.new("UIStroke")
abstroke.Color = Color3.fromRGB(90, 90, 110)
abstroke.Thickness = 2
abstroke.Parent = aimBtn

local aimLabel = Instance.new("TextLabel")
aimLabel.Size = UDim2.new(0, 80, 0, 14)
aimLabel.Position = UDim2.new(1, -80, 0, 133)
aimLabel.BackgroundTransparency = 1
aimLabel.Text = "AIM BOT"
aimLabel.TextColor3 = Color3.fromRGB(180, 180, 200)
aimLabel.Font = Enum.Font.GothamBold
aimLabel.TextSize = 11
aimLabel.Parent = gui

local function updateAimBtn()
	if Settings.Aimbot then
		aimBtn.BackgroundColor3 = Color3.fromRGB(40, 160, 90)
		abstroke.Color = Color3.fromRGB(80, 255, 140)
		aimLabel.TextColor3 = Color3.fromRGB(120, 255, 160)
	else
		aimBtn.BackgroundColor3 = Color3.fromRGB(25, 25, 32)
		abstroke.Color = Color3.fromRGB(90, 90, 110)
		aimLabel.TextColor3 = Color3.fromRGB(180, 180, 200)
	end
end

aimBtn.MouseButton1Click:Connect(function()
	Settings.Aimbot = not Settings.Aimbot
	updateAimBtn()
end)

------------------------------------------------------------
-- МЕНЮ
------------------------------------------------------------
local main = Instance.new("Frame")
main.Size = UDim2.new(0, 500, 0, 340)
main.Position = UDim2.new(0.5, -250, 0.5, -170)
main.BackgroundColor3 = Color3.fromRGB(18, 18, 24)
main.BorderSizePixel = 0
main.Visible = false
main.Parent = gui

local mc = Instance.new("UICorner")
mc.CornerRadius = UDim.new(0, 14)
mc.Parent = main

local mstroke = Instance.new("UIStroke")
mstroke.Color = Color3.fromRGB(45, 45, 55)
mstroke.Thickness = 1
mstroke.Parent = main

local header = Instance.new("Frame")
header.Size = UDim2.new(1, 0, 0, 60)
header.BackgroundColor3 = Color3.fromRGB(22, 22, 30)
header.BorderSizePixel = 0
header.Parent = main

local hc = Instance.new("UICorner")
hc.CornerRadius = UDim.new(0, 14)
hc.Parent = header

local logo = Instance.new("TextLabel")
logo.Size = UDim2.new(0, 160, 0, 30)
logo.Position = UDim2.new(0, 14, 0, 8)
logo.BackgroundTransparency = 1
logo.Text = "LIT ENERGY"
logo.TextColor3 = Color3.fromRGB(80, 220, 130)
logo.Font = Enum.Font.GothamBlack
logo.TextSize = 20
logo.TextXAlignment = Enum.TextXAlignment.Left
logo.Parent = header

local madeBy = Instance.new("TextLabel")
madeBy.Size = UDim2.new(0, 260, 0, 16)
madeBy.Position = UDim2.new(0, 14, 0, 36)
madeBy.BackgroundTransparency = 1
madeBy.Text = "Made by LIT • discord.gg/q3BKJ2hvY"
madeBy.TextColor3 = Color3.fromRGB(140, 140, 160)
madeBy.Font = Enum.Font.Gotham
madeBy.TextSize = 11
madeBy.TextXAlignment = Enum.TextXAlignment.Left
madeBy.Parent = header

local closeBtn = Instance.new("TextButton")
closeBtn.Size = UDim2.new(0, 28, 0, 28)
closeBtn.Position = UDim2.new(1, -38, 0, 16)
closeBtn.BackgroundColor3 = Color3.fromRGB(40, 40, 50)
closeBtn.Text = "✕"
closeBtn.TextColor3 = Color3.fromRGB(220, 220, 230)
closeBtn.Font = Enum.Font.GothamBold
closeBtn.TextSize = 14
closeBtn.BorderSizePixel = 0
closeBtn.Parent = header

local cbc = Instance.new("UICorner")
cbc.CornerRadius = UDim.new(0, 6)
cbc.Parent = closeBtn

closeBtn.MouseButton1Click:Connect(function()
	main.Visible = false
end)

local sidebar = Instance.new("Frame")
sidebar.Size = UDim2.new(0, 110, 1, -70)
sidebar.Position = UDim2.new(0, 10, 0, 60)
sidebar.BackgroundColor3 = Color3.fromRGB(22, 22, 30)
sidebar.BorderSizePixel = 0
sidebar.Parent = main

local sbc = Instance.new("UICorner")
sbc.CornerRadius = UDim.new(0, 10)
sbc.Parent = sidebar

local contentHolder = Instance.new("Frame")
contentHolder.Size = UDim2.new(1, -135, 1, -70)
contentHolder.Position = UDim2.new(0, 125, 0, 60)
contentHolder.BackgroundTransparency = 1
contentHolder.Parent = main

local pages = {}

local function makePage(name, title, desc)
	local page = Instance.new("Frame")
	page.Name = name
	page.Size = UDim2.new(1, 0, 1, 0)
	page.BackgroundTransparency = 1
	page.Visible = false
	page.Parent = contentHolder

	local t = Instance.new("TextLabel")
	t.Size = UDim2.new(1, -10, 0, 22)
	t.Position = UDim2.new(0, 5, 0, 0)
	t.BackgroundTransparency = 1
	t.Text = title
	t.TextColor3 = Color3.fromRGB(240, 240, 250)
	t.Font = Enum.Font.GothamBold
	t.TextSize = 18
	t.TextXAlignment = Enum.TextXAlignment.Left
	t.Parent = page

	local d = Instance.new("TextLabel")
	d.Size = UDim2.new(1, -10, 0, 16)
	d.Position = UDim2.new(0, 5, 0, 22)
	d.BackgroundTransparency = 1
	d.Text = desc
	d.TextColor3 = Color3.fromRGB(130, 130, 150)
	d.Font = Enum.Font.Gotham
	d.TextSize = 11
	d.TextXAlignment = Enum.TextXAlignment.Left
	d.Parent = page

	pages[name] = page
	return page
end

local movementPage = makePage("Movement", "Movement", "Speed, movement and jump control")
local stealPage    = makePage("Steal", "Steal", "Auto grab and item collection")
local miscPage     = makePage("Misc", "Misc", "Extra features")
local settingsPage = makePage("Settings", "Settings", "Script information")

local activeTab = "Movement"

local function switchTab(name)
	activeTab = name
	for tabName, page in pairs(pages) do
		page.Visible = (tabName == name)
	end
	for _, c in ipairs(sidebar:GetChildren()) do
		if c:IsA("TextButton") then
			local bar = c:FindFirstChild("Indicator")
			if bar then bar.Visible = (c.Name == name) end
			c.TextColor3 = (c.Name == name)
				and Color3.fromRGB(230, 230, 240)
				or Color3.fromRGB(160, 160, 180)
		end
	end
end

local function makeTab(name, text, y)
	local btn = Instance.new("TextButton")
	btn.Name = name
	btn.Size = UDim2.new(1, -12, 0, 34)
	btn.Position = UDim2.new(0, 6, 0, y)
	btn.BackgroundColor3 = Color3.fromRGB(22, 22, 30)
	btn.Text = "  " .. text
	btn.TextColor3 = Color3.fromRGB(160, 160, 180)
	btn.Font = Enum.Font.GothamMedium
	btn.TextSize = 13
	btn.TextXAlignment = Enum.TextXAlignment.Left
	btn.BorderSizePixel = 0
	btn.AutoButtonColor = false
	btn.Parent = sidebar

	local bc = Instance.new("UICorner")
	bc.CornerRadius = UDim.new(0, 6)
	bc.Parent = btn

	local bar = Instance.new("Frame")
	bar.Name = "Indicator"
	bar.Size = UDim2.new(0, 3, 0.6, 0)
	bar.Position = UDim2.new(0, 0, 0.2, 0)
	bar.BackgroundColor3 = Color3.fromRGB(80, 220, 130)
	bar.BorderSizePixel = 0
	bar.Visible = (name == activeTab)
	bar.Parent = btn

	local brc = Instance.new("UICorner")
	brc.CornerRadius = UDim.new(1, 0)
	brc.Parent = bar

	btn.MouseButton1Click:Connect(function()
		switchTab(name)
	end)
end

makeTab("Movement", "Movement", 8)
makeTab("Steal",    "Steal",    46)
makeTab("Misc",     "Misc",     84)
makeTab("Settings", "Settings", 122)

------------------------------------------------------------
-- UI ХЕЛПЕРЫ
------------------------------------------------------------
local function makeSectionLabel(parent, text, y)
	local row = Instance.new("Frame")
	row.Size = UDim2.new(1, -10, 0, 20)
	row.Position = UDim2.new(0, 5, 0, y)
	row.BackgroundTransparency = 1
	row.Parent = parent

	local dot = Instance.new("Frame")
	dot.Size = UDim2.new(0, 5, 0, 5)
	dot.Position = UDim2.new(0, 0, 0.5, -2)
	dot.BackgroundColor3 = Color3.fromRGB(80, 220, 130)
	dot.BorderSizePixel = 0
	dot.Parent = row

	local dc = Instance.new("UICorner")
	dc.CornerRadius = UDim.new(1, 0)
	dc.Parent = dot

	local lbl = Instance.new("TextLabel")
	lbl.Size = UDim2.new(1, -12, 1, 0)
	lbl.Position = UDim2.new(0, 12, 0, 0)
	lbl.BackgroundTransparency = 1
	lbl.Text = string.upper(text)
	lbl.TextColor3 = Color3.fromRGB(200, 200, 215)
	lbl.Font = Enum.Font.GothamBold
	lbl.TextSize = 11
	lbl.TextXAlignment = Enum.TextXAlignment.Left
	lbl.Parent = row
end

local function makeValueRow(parent, text, y, getValue)
	local row = Instance.new("Frame")
	row.Size = UDim2.new(1, -10, 0, 34)
	row.Position = UDim2.new(0, 5, 0, y)
	row.BackgroundColor3 = Color3.fromRGB(28, 28, 36)
	row.BorderSizePixel = 0
	row.Parent = parent

	local rc = Instance.new("UICorner")
	rc.CornerRadius = UDim.new(0, 8)
	rc.Parent = row

	local lbl = Instance.new("TextLabel")
	lbl.Size = UDim2.new(1, -80, 1, 0)
	lbl.Position = UDim2.new(0, 14, 0, 0)
	lbl.BackgroundTransparency = 1
	lbl.Text = text
	lbl.TextColor3 = Color3.fromRGB(220, 220, 230)
	lbl.Font = Enum.Font.Gotham
	lbl.TextSize = 13
	lbl.TextXAlignment = Enum.TextXAlignment.Left
	lbl.Parent = row

	local val = Instance.new("TextLabel")
	val.Size = UDim2.new(0, 60, 1, 0)
	val.Position = UDim2.new(1, -74, 0, 0)
	val.BackgroundTransparency = 1
	val.Text = tostring(getValue())
	val.TextColor3 = Color3.fromRGB(80, 220, 130)
	val.Font = Enum.Font.GothamBold
	val.TextSize = 13
	val.TextXAlignment = Enum.TextXAlignment.Right
	val.Parent = row
end

local function makeModernToggle(parent, text, y, getter, setter)
	local row = Instance.new("Frame")
	row.Size = UDim2.new(1, -10, 0, 34)
	row.Position = UDim2.new(0, 5, 0, y)
	row.BackgroundColor3 = Color3.fromRGB(28, 28, 36)
	row.BorderSizePixel = 0
	row.Parent = parent

	local rc = Instance.new("UICorner")
	rc.CornerRadius = UDim.new(0, 8)
	rc.Parent = row

	local lbl = Instance.new("TextLabel")
	lbl.Size = UDim2.new(1, -80, 1, 0)
	lbl.Position = UDim2.new(0, 14, 0, 0)
	lbl.BackgroundTransparency = 1
	lbl.Text = text
	lbl.TextColor3 = Color3.fromRGB(220, 220, 230)
	lbl.Font = Enum.Font.Gotham
	lbl.TextSize = 13
	lbl.TextXAlignment = Enum.TextXAlignment.Left
	lbl.Parent = row

	local toggle = Instance.new("TextButton")
	toggle.Size = UDim2.new(0, 40, 0, 20)
	toggle.Position = UDim2.new(1, -54, 0.5, -10)
	toggle.BackgroundColor3 = getter() and Color3.fromRGB(80, 220, 130) or Color3.fromRGB(55, 55, 68)
	toggle.Text = ""
	toggle.BorderSizePixel = 0
	toggle.AutoButtonColor = false
	toggle.Parent = row

	local tc = Instance.new("UICorner")
	tc.CornerRadius = UDim.new(1, 0)
	tc.Parent = toggle

	local knob = Instance.new("Frame")
	knob.Size = UDim2.new(0, 16, 0, 16)
	knob.Position = getter() and UDim2.new(1, -18, 0.5, -8) or UDim2.new(0, 2, 0.5, -8)
	knob.BackgroundColor3 = Color3.fromRGB(240, 240, 250)
	knob.BorderSizePixel = 0
	knob.Parent = toggle

	local kc = Instance.new("UICorner")
	kc.CornerRadius = UDim.new(1, 0)
	kc.Parent = knob

	toggle.MouseButton1Click:Connect(function()
		local n = not getter()
		setter(n)
		if n then
			toggle.BackgroundColor3 = Color3.fromRGB(80, 220, 130)
			TweenService:Create(knob, TweenInfo.new(0.18), {Position = UDim2.new(1, -18, 0.5, -8)}):Play()
		else
			toggle.BackgroundColor3 = Color3.fromRGB(55, 55, 68)
			TweenService:Create(knob, TweenInfo.new(0.18), {Position = UDim2.new(0, 2, 0.5, -8)}):Play()
		end
	end)
end

local function makeArrowRow(parent, text, y, options, getIndex, setIndex)
	local row = Instance.new("Frame")
	row.Size = UDim2.new(1, -10, 0, 34)
	row.Position = UDim2.new(0, 5, 0, y)
	row.BackgroundColor3 = Color3.fromRGB(28, 28, 36)
	row.BorderSizePixel = 0
	row.Parent = parent

	local rc = Instance.new("UICorner")
	rc.CornerRadius = UDim.new(0, 8)
	rc.Parent = row

	local lbl = Instance.new("TextLabel")
	lbl.Size = UDim2.new(1, -140, 1, 0)
	lbl.Position = UDim2.new(0, 14, 0, 0)
	lbl.BackgroundTransparency = 1
	lbl.Text = text
	lbl.TextColor3 = Color3.fromRGB(220, 220, 230)
	lbl.Font = Enum.Font.Gotham
	lbl.TextSize = 13
	lbl.TextXAlignment = Enum.TextXAlignment.Left
	lbl.Parent = row

	local leftA = Instance.new("TextButton")
	leftA.Size = UDim2.new(0, 22, 0, 22)
	leftA.Position = UDim2.new(1, -124, 0.5, -11)
	leftA.BackgroundColor3 = Color3.fromRGB(40, 40, 52)
	leftA.Text = "◄"
	leftA.TextColor3 = Color3.fromRGB(200, 200, 215)
	leftA.Font = Enum.Font.GothamBold
	leftA.TextSize = 12
	leftA.BorderSizePixel = 0
	leftA.AutoButtonColor = false
	leftA.Parent = row

	local lac = Instance.new("UICorner")
	lac.CornerRadius = UDim.new(0, 6)
	lac.Parent = leftA

	local val = Instance.new("TextLabel")
	val.Size = UDim2.new(0, 55, 1, 0)
	val.Position = UDim2.new(1, -98, 0, 0)
	val.BackgroundTransparency = 1
	val.Text = options[getIndex()]
	val.TextColor3 = Color3.fromRGB(80, 220, 130)
	val.Font = Enum.Font.GothamBold
	val.TextSize = 13
	val.Parent = row

	local rightA = Instance.new("TextButton")
	rightA.Size = UDim2.new(0, 22, 0, 22)
	rightA.Position = UDim2.new(1, -40, 0.5, -11)
	rightA.BackgroundColor3 = Color3.fromRGB(40, 40, 52)
	rightA.Text = "►"
	rightA.TextColor3 = Color3.fromRGB(200, 200, 215)
	rightA.Font = Enum.Font.GothamBold
	rightA.TextSize = 12
	rightA.BorderSizePixel = 0
	rightA.AutoButtonColor = false
	rightA.Parent = row

	local rac = Instance.new("UICorner")
	rac.CornerRadius = UDim.new(0, 6)
	rac.Parent = rightA

	leftA.MouseButton1Click:Connect(function()
		local n = getIndex() - 1
		if n < 1 then n = #options end
		setIndex(n)
		val.Text = options[n]
	end)

	rightA.MouseButton1Click:Connect(function()
		local n = getIndex() + 1
		if n > #options then n = 1 end
		setIndex(n)
		val.Text = options[n]
	end)
end

------------------------------------------------------------
-- MOVEMENT PAGE
------------------------------------------------------------
makeSectionLabel(movementPage, "Speed Configuration", 44)
makeValueRow(movementPage, "Normal Speed", 68, function() return Settings.WalkSpeed end)
makeModernToggle(movementPage, "Anti Ragdoll", 106,
	function() return Settings.AntiRagdoll end,
	function(v) Settings.AntiRagdoll = v end)

makeSectionLabel(movementPage, "Jump Configuration", 148)
makeModernToggle(movementPage, "Infinite Jump", 172,
	function() return Settings.InfiniteJump end,
	function(v) Settings.InfiniteJump = v end)
makeArrowRow(movementPage, "Jump Mode", 210, InfJumpModes,
	function() return InfJumpMode end,
	function(i) InfJumpMode = i end)

------------------------------------------------------------
-- STEAL PAGE
------------------------------------------------------------
makeSectionLabel(stealPage, "Auto Grab", 44)
makeModernToggle(stealPage, "Auto Grab", 68,
	function() return Settings.AutoGrab end,
	function(v)
		Settings.AutoGrab = v
		if v then showStatusHUD() else hideStatusHUD() end
	end)

local autoGrabInfo = Instance.new("TextLabel")
autoGrabInfo.Size = UDim2.new(1, -10, 0, 40)
autoGrabInfo.Position = UDim2.new(0, 5, 0, 108)
autoGrabInfo.BackgroundColor3 = Color3.fromRGB(24, 24, 32)
autoGrabInfo.BorderSizePixel = 0
autoGrabInfo.Text = "  Мгновенный захват брейнрота\n  при подходе к нему."
autoGrabInfo.TextColor3 = Color3.fromRGB(140, 140, 160)
autoGrabInfo.Font = Enum.Font.Gotham
autoGrabInfo.TextSize = 11
autoGrabInfo.TextXAlignment = Enum.TextXAlignment.Left
autoGrabInfo.TextYAlignment = Enum.TextYAlignment.Top
autoGrabInfo.Parent = stealPage

local agi = Instance.new("UICorner")
agi.CornerRadius = UDim.new(0, 8)
agi.Parent = autoGrabInfo

local agPad = Instance.new("UIPadding")
agPad.PaddingTop = UDim.new(0, 8)
agPad.PaddingLeft = UDim.new(0, 8)
agPad.Parent = autoGrabInfo

------------------------------------------------------------
-- MISC PAGE
------------------------------------------------------------
makeSectionLabel(miscPage, "Performance", 44)
makeModernToggle(miscPage, "Anti Lag", 68,
	function() return Settings.AntiLag end,
	function(v)
		Settings.AntiLag = v
		applyAntiLag()
	end)
makeModernToggle(miscPage, "Anti Die", 106,
	function() return Settings.AntiDie end,
	function(v)
		Settings.AntiDie = v
		applyAntiDie()
	end)

------------------------------------------------------------
-- SETTINGS PAGE
------------------------------------------------------------
makeSectionLabel(settingsPage, "About", 44)

local about = Instance.new("TextLabel")
about.Size = UDim2.new(1, -10, 0, 80)
about.Position = UDim2.new(0, 5, 0, 68)
about.BackgroundColor3 = Color3.fromRGB(24, 24, 32)
about.BorderSizePixel = 0
about.Text = "  LIT ENERGY • TOP 1 SCRIPT\n  discord.gg/q3BKJ2hvY\n  Toggle key: RightShift"
about.TextColor3 = Color3.fromRGB(200, 200, 215)
about.Font = Enum.Font.Gotham
about.TextSize = 12
about.TextXAlignment = Enum.TextXAlignment.Left
about.TextYAlignment = Enum.TextYAlignment.Top
about.Parent = settingsPage

local ab = Instance.new("UICorner")
ab.CornerRadius = UDim.new(0, 8)
ab.Parent = about

local abPad = Instance.new("UIPadding")
abPad.PaddingTop = UDim.new(0, 10)
abPad.PaddingLeft = UDim.new(0, 10)
abPad.Parent = about

switchTab("Movement")

------------------------------------------------------------
-- STATUS HUD
------------------------------------------------------------
local statusGui = Instance.new("ScreenGui")
statusGui.Name = "LitEnergyStatus"
statusGui.ResetOnSpawn = false
statusGui.IgnoreGuiInset = true
statusGui.DisplayOrder = 90
statusGui.Parent = player:WaitForChild("PlayerGui")

local statusFrame = Instance.new("Frame")
statusFrame.AnchorPoint = Vector2.new(0.5, 1)
statusFrame.Size = UDim2.new(0, 320, 0, 42)
statusFrame.Position = UDim2.new(0.5, 0, 1, -80)
statusFrame.BackgroundColor3 = Color3.fromRGB(20, 30, 24)
statusFrame.BackgroundTransparency = 0.15
statusFrame.BorderSizePixel = 0
statusFrame.Visible = false
statusFrame.Parent = statusGui

local sfc = Instance.new("UICorner")
sfc.CornerRadius = UDim.new(0, 10)
sfc.Parent = statusFrame

local sfStroke = Instance.new("UIStroke")
sfStroke.Color = Color3.fromRGB(60, 200, 120)
sfStroke.Thickness = 1
sfStroke.Transparency = 0.4
sfStroke.Parent = statusFrame

local pctLabel = Instance.new("TextLabel")
pctLabel.Size = UDim2.new(0, 60, 0, 22)
pctLabel.Position = UDim2.new(0, 16, 0, 4)
pctLabel.BackgroundTransparency = 1
pctLabel.Text = "0%"
pctLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
pctLabel.Font = Enum.Font.GothamBlack
pctLabel.TextSize = 18
pctLabel.TextXAlignment = Enum.TextXAlignment.Left
pctLabel.Parent = statusFrame

local fpsLabel = Instance.new("TextLabel")
fpsLabel.Size = UDim2.new(0, 120, 0, 22)
fpsLabel.Position = UDim2.new(0, 90, 0, 4)
fpsLabel.BackgroundTransparency = 1
fpsLabel.Text = "FPS 60"
fpsLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
fpsLabel.Font = Enum.Font.GothamBold
fpsLabel.TextSize = 17
fpsLabel.Parent = statusFrame

local pingLabel = Instance.new("TextLabel")
pingLabel.Size = UDim2.new(0, 130, 0, 22)
pingLabel.Position = UDim2.new(1, -140, 0, 4)
pingLabel.BackgroundTransparency = 1
pingLabel.Text = "PING 0ms"
pingLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
pingLabel.Font = Enum.Font.GothamBold
pingLabel.TextSize = 17
pingLabel.TextXAlignment = Enum.TextXAlignment.Right
pingLabel.Parent = statusFrame

local barBg = Instance.new("Frame")
barBg.Size = UDim2.new(1, -32, 0, 6)
barBg.Position = UDim2.new(0, 16, 1, -12)
barBg.BackgroundColor3 = Color3.fromRGB(15, 20, 18)
barBg.BorderSizePixel = 0
barBg.Parent = statusFrame

local bbc = Instance.new("UICorner")
bbc.CornerRadius = UDim.new(1, 0)
bbc.Parent = barBg

local barFill = Instance.new("Frame")
barFill.Size = UDim2.new(0, 0, 1, 0)
barFill.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
barFill.BorderSizePixel = 0
barFill.Parent = barBg

local bfc = Instance.new("UICorner")
bfc.CornerRadius = UDim.new(1, 0)
bfc.Parent = barFill

local fillGradient = Instance.new("UIGradient")
fillGradient.Color = ColorSequence.new({
	ColorSequenceKeypoint.new(0, Color3.fromRGB(255, 255, 255)),
	ColorSequenceKeypoint.new(0.5, Color3.fromRGB(230, 255, 240)),
	ColorSequenceKeypoint.new(1, Color3.fromRGB(255, 255, 255)),
})
fillGradient.Parent = barFill

local dotHolder = Instance.new("Frame")
dotHolder.Size = UDim2.new(1, 0, 1, 0)
dotHolder.BackgroundTransparency = 1
dotHolder.ClipsDescendants = true
dotHolder.Parent = barBg

for i = 1, 10 do
	local dot = Instance.new("Frame")
	dot.Size = UDim2.new(0, 2, 0, 2)
	dot.Position = UDim2.new(math.random() * 0.9, 0, math.random() * 0.6, 0)
	dot.BackgroundColor3 = Color3.fromRGB(120, 255, 160)
	dot.BorderSizePixel = 0
	dot.Parent = dotHolder

	local dc = Instance.new("UICorner")
	dc.CornerRadius = UDim.new(1, 0)
	dc.Parent = dot

	task.spawn(function()
		while true do
			task.wait(math.random(8, 20) / 10)
			TweenService:Create(dot, TweenInfo.new(0.6), {
				Position = UDim2.new(math.random() * 0.95, 0, math.random() * 0.6, 0)
			}):Play()
		end
	end)
end

local statusVisible = false

function showStatusHUD()
	statusFrame.Visible = true
	statusVisible = true
end

function hideStatusHUD()
	statusFrame.Visible = false
	statusVisible = false
end

task.spawn(function()
	local fpsAccum, fpsTime, frames = 0, 0, 0
	local lastTime = tick()

	RunService.RenderStepped:Connect(function(dt)
		frames += 1
		fpsTime += dt
		if fpsTime >= 1 then
			fpsAccum = math.floor(frames / fpsTime)
			frames = 0
			fpsTime = 0
		end

		if statusVisible then
			pctLabel.Text = "100%"
			barFill.Size = UDim2.new(1, 0, 1, 0)

			local pulse = 0.7 + 0.3 * math.sin(tick() * 6)
			barFill.BackgroundTransparency = 1 - pulse

			local now = tick()
			if now - lastTime >= 0.5 then
				lastTime = now
				fpsLabel.Text = "FPS " .. (fpsAccum > 0 and fpsAccum or 60)

				local ok, ping = pcall(function()
					return player:GetNetworkPing() * 1000
				end)
				if ok and ping then
					pingLabel.Text = "PING " .. math.floor(ping) .. "ms"
				end
			end
		end
	end)
end)

------------------------------------------------------------
-- ANTI LAG
------------------------------------------------------------
local savedLighting = {
	GlobalShadows = Lighting.GlobalShadows,
	FogEnd = Lighting.FogEnd,
	Brightness = Lighting.Brightness,
}

local hiddenInstances = {}

local function antiLagON()
	Lighting.GlobalShadows = false
	Lighting.FogEnd = 100000
	Lighting.Brightness = 1

	for _, obj in ipairs(Lighting:GetChildren()) do
		if obj:IsA("PostEffect") or obj:IsA("Atmosphere") or obj:IsA("Sky") then
			pcall(function() obj.Enabled = false end)
			table.insert(hiddenInstances, obj)
		end
	end

	task.spawn(function()
		for _, obj in ipairs(Workspace:GetDescendants()) do
			if obj:IsA("ParticleEmitter") or obj:IsA("Trail") or obj:IsA("Smoke")
			or obj:IsA("Fire") or obj:IsA("Sparkles") or obj:IsA("Beam") then
				pcall(function()
					obj.Enabled = false
					table.insert(hiddenInstances, obj)
				end)
			elseif obj:IsA("PointLight") or obj:IsA("SpotLight") or obj:IsA("SurfaceLight") then
				pcall(function()
					obj.Enabled = false
					table.insert(hiddenInstances, obj)
				end)
			elseif obj:IsA("Decal") or obj:IsA("Texture") then
				pcall(function()
					obj.Transparency = 1
					table.insert(hiddenInstances, obj)
				end)
			end
		end
	end)
end

local function antiLagOFF()
	Lighting.GlobalShadows = savedLighting.GlobalShadows
	Lighting.FogEnd = savedLighting.FogEnd
	Lighting.Brightness = savedLighting.Brightness

	for _, obj in ipairs(hiddenInstances) do
		if obj and obj.Parent then
			pcall(function()
				if obj:IsA("Decal") or obj:IsA("Texture") then
					obj.Transparency = 0
				else
					obj.Enabled = true
				end
			end)
		end
	end
	hiddenInstances = {}
end

function applyAntiLag()
	if Settings.AntiLag then antiLagON() else antiLagOFF() end
end

------------------------------------------------------------
-- ANTI DIE
------------------------------------------------------------
local antiDieConnections = {}

local function clearAntiDieConnections()
	for _, c in ipairs(antiDieConnections) do
		pcall(function() c:Disconnect() end)
	end
	table.clear(antiDieConnections)
end

local function setResetButton(enabled)
	task.spawn(function()
		for _ = 1, 25 do
			local ok = pcall(function()
				StarterGui:SetCore("ResetButtonCallback", enabled)
			end)
			if ok then return end
			task.wait(0.15)
		end
	end)
end

local function enableAntiDieOnCharacter(character)
	local humanoid = character:WaitForChild("Humanoid", 5)
	if not humanoid then return end

	pcall(function()
		humanoid.BreakJointsOnDeath = false
		humanoid.MaxHealth = 1000000000
		humanoid.Health = humanoid.MaxHealth
		humanoid:SetStateEnabled(Enum.HumanoidStateType.Dead, false)
		humanoid:SetStateEnabled(Enum.HumanoidStateType.FallingDown, false)
		humanoid:SetStateEnabled(Enum.HumanoidStateType.Ragdoll, false)
	end)

	table.insert(antiDieConnections, humanoid.HealthChanged:Connect(function(health)
		if Settings.AntiDie and health < humanoid.MaxHealth then
			pcall(function() humanoid.Health = humanoid.MaxHealth end)
		end
	end))
end

function applyAntiDie()
	if Settings.AntiDie then
		clearAntiDieConnections()
		setResetButton(false)
		if player.Character then
			enableAntiDieOnCharacter(player.Character)
		end
	else
		clearAntiDieConnections()
		setResetButton(true)
	end
end

------------------------------------------------------------
-- AUTO GRAB (мгновенный, без полоски)
------------------------------------------------------------
local GRAB_RANGE = 25
local GRAB_COOLDOWN = 0.1
local lastGrab = 0

task.spawn(function()
	while true do
		task.wait(0.02)

		if Settings.AutoGrab then
			local char = player.Character
			local root = char and char:FindFirstChild("HumanoidRootPart")

			if root then
				local now = tick()

				if now - lastGrab >= GRAB_COOLDOWN then
					local myPos = root.Position
					local grabbed = false

					for _, obj in ipairs(Workspace:GetDescendants()) do
						if obj:IsA("ProximityPrompt") and obj.Enabled then
							local p = obj.Parent
							if p and p:IsA("BasePart") then
								if (p.Position - myPos).Magnitude < GRAB_RANGE then
									pcall(function() fireproximityprompt(obj) end)
									grabbed = true
								end
							elseif p and p:IsA("Attachment") and p.Parent then
								local base = p.Parent
								if base:IsA("BasePart") and (base.Position - myPos).Magnitude < GRAB_RANGE then
									pcall(function() fireproximityprompt(obj) end)
									grabbed = true
								end
							end
						end
					end

					for _, obj in ipairs(Workspace:GetDescendants()) do
						if obj:IsA("BasePart") then
							local name = obj.Name:lower()
							if name:find("brainrot") or name:find("collect")
							or name:find("grab") or name:find("cash")
							or name:find("coin") or name:find("brain") then
								if (obj.Position - myPos).Magnitude < GRAB_RANGE then
									local touch = obj:FindFirstChildOfClass("TouchTransmitter")
									if touch then
										pcall(function()
											firetouchinterest(root, touch, 0)
											task.wait()
											firetouchinterest(root, touch, 1)
										end)
										grabbed = true
									end
								end
							end
						end
					end

					if grabbed then
						lastGrab = now
					end
				end
			end
		end
	end
end)

------------------------------------------------------------
-- INFINITE JUMP (Tap)
------------------------------------------------------------
UserInputService.JumpRequest:Connect(function()
	if Settings.InfiniteJump and InfJumpMode == 2 then
		local char = player.Character
		local hum = char and char:FindFirstChildOfClass("Humanoid")
		if hum then
			hum:ChangeState(Enum.HumanoidStateType.Jumping)
		end
	end
end)

------------------------------------------------------------
-- CHARACTER SETUP
------------------------------------------------------------
local function setupChar(char)
	local hum = char:WaitForChild("Humanoid")

	hum.StateChanged:Connect(function(_, new)
		if not Settings.AntiRagdoll then return end
		if new == Enum.HumanoidStateType.FallingDown
		or new == Enum.HumanoidStateType.Ragdoll
		or new == Enum.HumanoidStateType.PlatformStanding then
			hum:ChangeState(Enum.HumanoidStateType.Running)
		end
	end)

	if Settings.AntiRagdoll then
		hum:SetStateEnabled(Enum.HumanoidStateType.FallingDown, false)
		hum:SetStateEnabled(Enum.HumanoidStateType.Ragdoll, false)
		hum:SetStateEnabled(Enum.HumanoidStateType.PlatformStanding, false)
	end

	if Settings.AntiDie then
		task.wait(0.2)
		enableAntiDieOnCharacter(char)
	end
end

------------------------------------------------------------
-- MAIN LOOP
------------------------------------------------------------
RunService.RenderStepped:Connect(function()
	local char = player.Character
	if not char then return end
	local hum = char:FindFirstChildOfClass("Humanoid")
	local root = char:FindFirstChild("HumanoidRootPart")
	if not hum or not root then return end

	if Settings.InfiniteJump and InfJumpMode == 1 then
		hum.Jump = true
	end

	if Settings.Aimbot then
		local closest, dist = nil, math.huge
		local myPos = root.Position

		for _, p in ipairs(Players:GetPlayers()) do
			if p ~= player and p.Character then
				local h = p.Character:FindFirstChildOfClass("Humanoid")
				local hrp = p.Character:FindFirstChild("HumanoidRootPart")
				if h and hrp and h.Health > 0 then
					local d = (hrp.Position - myPos).Magnitude
					if d < dist then
						dist = d
						closest = hrp
					end
				end
			end
		end

		if closest then
			camera.CFrame = CFrame.new(camera.CFrame.Position, closest.Position)
			hum:MoveTo(closest.Position)
			if hum.WalkSpeed < 25 then hum.WalkSpeed = 25 end
		end
	else
		if hum.WalkSpeed > Settings.WalkSpeed then
			hum.WalkSpeed = Settings.WalkSpeed
		end
	end
end)

------------------------------------------------------------
-- ХОТКЕЙ + ЧАТ
------------------------------------------------------------
UserInputService.InputBegan:Connect(function(input, gpe)
	if gpe then return end
	if input.KeyCode == Settings.ToggleKey then
		main.Visible = not main.Visible
	end
end)

openBtn.MouseButton1Click:Connect(function()
	main.Visible = not main.Visible
end)

player.Chatted:Connect(function(msg)
	local m = msg:lower()
	if m == "/menu" or m == "/settings" or m == "/cfg" then
		main.Visible = not main.Visible
	elseif m == "/aim" then
		Settings.Aimbot = not Settings.Aimbot
		updateAimBtn()
	elseif m == "/lag" or m == "/antilag" then
		Settings.AntiLag = not Settings.AntiLag
		applyAntiLag()
	elseif m == "/die" or m == "/antidie" then
		Settings.AntiDie = not Settings.AntiDie
		applyAntiDie()
	elseif m == "/ij" or m == "/infjump" then
		Settings.InfiniteJump = not Settings.InfiniteJump
	elseif m == "/jumpmode" then
		InfJumpMode = InfJumpMode == 1 and 2 or 1
	elseif m == "/grab" or m == "/autograb" then
		Settings.AutoGrab = not Settings.AutoGrab
		if Settings.AutoGrab then showStatusHUD() else hideStatusHUD() end
		print("[LIT ENERGY] AutoGrab: " .. tostring(Settings.AutoGrab))
	end
end)

------------------------------------------------------------
-- СТАРТ
------------------------------------------------------------
if player.Character then
	setupChar(player.Character)
end
player.CharacterAdded:Connect(setupChar)
updateAimBtn()
