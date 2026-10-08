-- Complete Menu GUI Wrapper with Speed Walk, Custom Image, ESP, Reset, Trash, Minimize, and Lock Buttons
local ScreenGui = Instance.new("ScreenGui")
local MainFrame = Instance.new("Frame")
local Title = Instance.new("TextLabel")
local BackgroundImage = Instance.new("ImageLabel") -- خلفية الصورة
local MinimizeButton = Instance.new("TextButton")
local TrashButton = Instance.new("TextButton")
local LockButton = Instance.new("TextButton") -- زر القفل الجديد
local KorbloxButton = Instance.new("TextButton")
local HeadlessButton = Instance.new("TextButton")
local NoclipButton = Instance.new("TextButton")
local InfJumpButton = Instance.new("TextButton")
local EspButton = Instance.new("TextButton")
local SpeedBox = Instance.new("TextBox")
local OkButton = Instance.new("TextButton")
local ResetButton = Instance.new("TextButton")

local UICorner = Instance.new("UICorner")
local UICorner_Title = Instance.new("UICorner")
local UICorner_Min = Instance.new("UICorner")
local UICorner_Trash = Instance.new("UICorner")
local UICorner_Lock = Instance.new("UICorner")
local UICorner_2 = Instance.new("UICorner")
local UICorner_3 = Instance.new("UICorner")
local UICorner_4 = Instance.new("UICorner")
local UICorner_5 = Instance.new("UICorner")
local UICorner_Esp = Instance.new("UICorner")
local UICorner_6 = Instance.new("UICorner")
local UICorner_7 = Instance.new("UICorner")
local UICorner_Reset = Instance.new("UICorner")
local UICorner_8 = Instance.new("UICorner")

-- خصائص الواجهة (ScreenGui)
ScreenGui.Parent = game.CoreGui
ScreenGui.Name = "MenuGui"

-- الإطار الرئيسي (MainFrame)
MainFrame.Parent = ScreenGui
MainFrame.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
MainFrame.Position = UDim2.new(0.5, -110, 0.5, -150)
MainFrame.Size = UDim2.new(0, 220, 0, 310)
MainFrame.Active = true
MainFrame.Draggable = true

UICorner_8.Parent = MainFrame

-- عنوان القائمة (Title)
Title.Parent = MainFrame
Title.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
Title.Size = UDim2.new(0, 220, 0, 35)
Title.Font = Enum.Font.GothamBold
Title.Text = "  Abdullah Al-Otaibi"
Title.TextXAlignment = Enum.TextXAlignment.Left
Title.TextColor3 = Color3.fromRGB(255, 255, 255)
Title.TextSize = 13

UICorner_Title.Parent = Title

-- إعداد صورة الخلفية (قم بتغيير YOUR_IMAGE_ID برقم الـ ID الخاص بصورتك الملكية)
BackgroundImage.Parent = MainFrame
BackgroundImage.BackgroundTransparency = 1
BackgroundImage.Position = UDim2.new(0, 0, 0, 35)
BackgroundImage.Size = UDim2.new(0, 220, 0, 275)
BackgroundImage.Image = "rbxassetid://YOUR_IMAGE_ID" 
BackgroundImage.ImageTransparency = 0.4 
BackgroundImage.ZIndex = 0

-- زر التصغير (-)
MinimizeButton.Parent = MainFrame
MinimizeButton.BackgroundColor3 = Color3.fromRGB(110, 110, 110)
MinimizeButton.Position = UDim2.new(0.54, 0, 0.03, 0)
MinimizeButton.Size = UDim2.new(0, 26, 0, 26)
MinimizeButton.Font = Enum.Font.GothamBold
MinimizeButton.Text = "-"
MinimizeButton.TextColor3 = Color3.fromRGB(255, 255, 255)
MinimizeButton.TextSize = 16
MinimizeButton.AutoButtonColor = true

UICorner_Min.Parent = MinimizeButton

-- زر القفل (Lock Button) بجانب زر الزبالة
LockButton.Parent = MainFrame
LockButton.BackgroundColor3 = Color3.fromRGB(52, 152, 219)
LockButton.Position = UDim2.new(0.68, 0, 0.03, 0)
LockButton.Size = UDim2.new(0, 26, 0, 26)
LockButton.Font = Enum.Font.GothamBold
LockButton.Text = "🔓"
LockButton.TextColor3 = Color3.fromRGB(255, 255, 255)
LockButton.TextSize = 12
LockButton.AutoButtonColor = true

UICorner_Lock.Parent = LockButton

-- زر سلة المهملات (Trash Button)
TrashButton.Parent = MainFrame
TrashButton.BackgroundColor3 = Color3.fromRGB(231, 76, 60)
TrashButton.Position = UDim2.new(0.82, 0, 0.03, 0)
TrashButton.Size = UDim2.new(0, 26, 0, 26)
TrashButton.Font = Enum.Font.GothamBold
TrashButton.Text = "🗑"
TrashButton.TextColor3 = Color3.fromRGB(255, 255, 255)
TrashButton.TextSize = 14
TrashButton.AutoButtonColor = true

UICorner_Trash.Parent = TrashButton

-- زر Korblox
KorbloxButton.Parent = MainFrame
KorbloxButton.BackgroundColor3 = Color3.fromRGB(0, 170, 255)
KorbloxButton.Position = UDim2.new(0.1, 0, 0.15, 0)
KorbloxButton.Size = UDim2.new(0, 176, 0, 28)
KorbloxButton.Font = Enum.Font.GothamBold
KorbloxButton.Text = "Korblox"
KorbloxButton.TextColor3 = Color3.fromRGB(255, 255, 255)
KorbloxButton.TextSize = 13
KorbloxButton.AutoButtonColor = true
KorbloxButton.ZIndex = 2

UICorner_2.Parent = KorbloxButton

-- زر Headless
HeadlessButton.Parent = MainFrame
HeadlessButton.BackgroundColor3 = Color3.fromRGB(255, 85, 85)
HeadlessButton.Position = UDim2.new(0.1, 0, 0.28, 0)
HeadlessButton.Size = UDim2.new(0, 176, 0, 28)
HeadlessButton.Font = Enum.Font.GothamBold
HeadlessButton.Text = "Headless"
HeadlessButton.TextColor3 = Color3.fromRGB(255, 255, 255)
HeadlessButton.TextSize = 13
HeadlessButton.AutoButtonColor = true
HeadlessButton.ZIndex = 2

UICorner_3.Parent = HeadlessButton

-- زر Noclip
NoclipButton.Parent = MainFrame
NoclipButton.BackgroundColor3 = Color3.fromRGB(46, 204, 113)
NoclipButton.Position = UDim2.new(0.1, 0, 0.41, 0)
NoclipButton.Size = UDim2.new(0, 176, 0, 28)
NoclipButton.Font = Enum.Font.GothamBold
NoclipButton.Text = "Noclip"
NoclipButton.TextColor3 = Color3.fromRGB(255, 255, 255)
NoclipButton.TextSize = 13
NoclipButton.AutoButtonColor = true
NoclipButton.ZIndex = 2

UICorner_4.Parent = NoclipButton

-- زر Infinity Jump
InfJumpButton.Parent = MainFrame
InfJumpButton.BackgroundColor3 = Color3.fromRGB(155, 89, 182)
InfJumpButton.Position = UDim2.new(0.1, 0, 0.54, 0)
InfJumpButton.Size = UDim2.new(0, 176, 0, 28)
InfJumpButton.Font = Enum.Font.GothamBold
InfJumpButton.Text = "Infinity Jump"
InfJumpButton.TextColor3 = Color3.fromRGB(255, 255, 255)
InfJumpButton.TextSize = 13
InfJumpButton.AutoButtonColor = true
InfJumpButton.ZIndex = 2

UICorner_5.Parent = InfJumpButton

-- زر ESP
EspButton.Parent = MainFrame
EspButton.BackgroundColor3 = Color3.fromRGB(230, 126, 34)
EspButton.Position = UDim2.new(0.1, 0, 0.67, 0)
EspButton.Size = UDim2.new(0, 176, 0, 28)
EspButton.Font = Enum.Font.GothamBold
EspButton.Text = "ESP"
EspButton.TextColor3 = Color3.fromRGB(255, 255, 255)
EspButton.TextSize = 13
EspButton.AutoButtonColor = true
EspButton.ZIndex = 2

UICorner_Esp.Parent = EspButton

-- خانة كتابة السرعة (Speed Walk TextBox)
SpeedBox.Parent = MainFrame
SpeedBox.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
SpeedBox.Position = UDim2.new(0.1, 0, 0.80, 0)
SpeedBox.Size = UDim2.new(0, 84, 0, 28)
SpeedBox.Font = Enum.Font.Gotham
SpeedBox.PlaceholderText = "Speed Walk"
SpeedBox.Text = ""
SpeedBox.TextColor3 = Color3.fromRGB(255, 255, 255)
SpeedBox.TextSize = 11
SpeedBox.ZIndex = 2

UICorner_6.Parent = SpeedBox

-- زر التعيين (OK Button)
OkButton.Parent = MainFrame
OkButton.BackgroundColor3 = Color3.fromRGB(241, 196, 15)
OkButton.Position = UDim2.new(0.51, 0, 0.80, 0)
OkButton.Size = UDim2.new(0, 42, 0, 28)
OkButton.Font = Enum.Font.GothamBold
OkButton.Text = "OK"
OkButton.TextColor3 = Color3.fromRGB(255, 255, 255)
OkButton.TextSize = 11
OkButton.AutoButtonColor = true
OkButton.ZIndex = 2

UICorner_7.Parent = OkButton

-- زر إعادة التعيين (Reset Button 🔄)
ResetButton.Parent = MainFrame
ResetButton.BackgroundColor3 = Color3.fromRGB(127, 140, 141)
ResetButton.Position = UDim2.new(0.72, 0, 0.80, 0)
ResetButton.Size = UDim2.new(0, 42, 0, 28)
ResetButton.Font = Enum.Font.GothamBold
ResetButton.Text = "🔄"
ResetButton.TextColor3 = Color3.fromRGB(255, 255, 255)
ResetButton.TextSize = 14
ResetButton.AutoButtonColor = true
ResetButton.ZIndex = 2

UICorner_Reset.Parent = ResetButton

-- منطق زر القفل والفتح (Lock / Unlock Logic)
local isLocked = false
LockButton.MouseButton1Click:Connect(function()
    isLocked = not isLocked
    if isLocked then
        MainFrame.Draggable = false
        LockButton.Text = "🔒"
        LockButton.BackgroundColor3 = Color3.fromRGB(46, 204, 113)
    else
        MainFrame.Draggable = true
        LockButton.Text = "🔓"
        LockButton.BackgroundColor3 = Color3.fromRGB(52, 152, 219)
    end
end)

-- منطق زر التصغير والتكبير (Minimize / Maximize Logic)
local minimized = false
MinimizeButton.MouseButton1Click:Connect(function()
    minimized = not minimized
    if minimized then
        MinimizeButton.Text = "+"
        MainFrame.Size = UDim2.new(0, 220, 0, 35)
        BackgroundImage.Visible = false
        KorbloxButton.Visible = false
        HeadlessButton.Visible = false
        NoclipButton.Visible = false
        InfJumpButton.Visible = false
        EspButton.Visible = false
        SpeedBox.Visible = false
        OkButton.Visible = false
        ResetButton.Visible = false
    else
        MinimizeButton.Text = "-"
        MainFrame.Size = UDim2.new(0, 220, 0, 310)
        BackgroundImage.Visible = true
        KorbloxButton.Visible = true
        HeadlessButton.Visible = true
        NoclipButton.Visible = true
        InfJumpButton.Visible = true
        EspButton.Visible = true
        SpeedBox.Visible = true
        OkButton.Visible = true
        ResetButton.Visible = true
    end
end)

-- منطق زر الحذف (Trash Button)
TrashButton.MouseButton1Click:Connect(function()
    ScreenGui:Destroy()
end)

-- حدث زر Korblox
KorbloxButton.MouseButton1Click:Connect(function()
    pcall(function()
        loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-Korblox-All-145374"))()
    end)
end)

-- حدث زر Headless
HeadlessButton.MouseButton1Click:Connect(function()
    pcall(function()
        loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-Headless-(R6R15)-224493"))()
    end)
end)

-- حدث زر Noclip
local noclipEnabled = false
local runService = game:GetService("RunService")

NoclipButton.MouseButton1Click:Connect(function()
    noclipEnabled = not noclipEnabled
    if noclipEnabled then
        NoclipButton.BackgroundColor3 = Color3.fromRGB(39, 174, 96)
        NoclipButton.Text = "Noclip: ON"
    else
        NoclipButton.BackgroundColor3 = Color3.fromRGB(46, 204, 113)
        NoclipButton.Text = "Noclip"
    end
end)

runService.Stepped:Connect(function()
    if noclipEnabled then
        local character = game.Players.LocalPlayer.Character
        if character then
            for _, part in pairs(character:GetDescendants()) do
                if part:IsA("BasePart") and part.CanCollide then
                    part.CanCollide = false
                end
            end
        end
    end
end)

-- حدث زر Infinity Jump
local infJumpEnabled = false
local userInputService = game:GetService("UserInputService")

InfJumpButton.MouseButton1Click:Connect(function()
    infJumpEnabled = not infJumpEnabled
    if infJumpEnabled then
        InfJumpButton.BackgroundColor3 = Color3.fromRGB(142, 68, 173)
        InfJumpButton.Text = "Infinity Jump: ON"
    else
        InfJumpButton.BackgroundColor3 = Color3.fromRGB(155, 89, 182)
        InfJumpButton.Text = "Infinity Jump"
    end
end)

userInputService.JumpRequest:Connect(function()
    if infJumpEnabled then
        local player = game.Players.LocalPlayer
        if player.Character and player.Character:FindFirstChildOfClass("Humanoid") then
            player.Character.Humanoid:ChangeState(Enum.HumanoidStateType.Jumping)
        end
    end
end)

-- حدث زر ESP
local espEnabled = false
EspButton.MouseButton1Click:Connect(function()
    espEnabled = not espEnabled
    if espEnabled then
        EspButton.BackgroundColor3 = Color3.fromRGB(211, 84, 0)
        EspButton.Text = "ESP: ON"
    else
        EspButton.BackgroundColor3 = Color3.fromRGB(230, 126, 34)
        EspButton.Text = "ESP"
    end
end)

runService.RenderStepped:Connect(function()
    if espEnabled then
        for _, player in pairs(game.Players:GetPlayers()) do
            if player ~= game.Players.LocalPlayer and player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
                local character = player.Character
                if not character:FindFirstChild("Highlight_ESP") then
                    local highlight = Instance.new("Highlight")
                    highlight.Name = "Highlight_ESP"
                    highlight.Adornee = character
                    highlight.Parent = character
                    highlight.FillColor = Color3.fromRGB(255, 0, 0)
                    highlight.OutlineColor = Color3.fromRGB(255, 255, 255)
                    highlight.FillTransparency = 0.5
                end
            end
        end
    else
        for _, player in pairs(game.Players:GetPlayers()) do
            if player.Character and player.Character:FindFirstChild("Highlight_ESP") then
                player.Character.Highlight_ESP:Destroy()
            end
        end
    end
end)

-- حدث زر OK لتغيير السرعة
OkButton.MouseButton1Click:Connect(function()
    local speedValue = tonumber(SpeedBox.Text)
    if speedValue then
        local player = game.Players.LocalPlayer
        if player.Character and player.Character:FindFirstChild("Humanoid") then
            player.Character.Humanoid.WalkSpeed = speedValue
        end
    end
end)

-- حدث زر إعادة التعيين (🔄)
ResetButton.MouseButton1Click:Connect(function()
    SpeedBox.Text = ""
    local player = game.Players.LocalPlayer
    if player.Character and player.Character:FindFirstChild("Humanoid") then
        player.Character.Humanoid.WalkSpeed = 16
    end
end)