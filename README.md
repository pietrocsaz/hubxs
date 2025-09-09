-- Exemplo básico de Hub de Scripts
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local ScriptButton1 = Instance.new("TextButton")
local ScriptButton2 = Instance.new("TextButton")

ScreenGui.Parent = game.CoreGui
ScreenGui.Name = "MeuScriptHub"

Frame.Parent = ScreenGui
Frame.Position = UDim2.new(0.1, 0, 0.1, 0)
Frame.Size = UDim2.new(0, 200, 0, 300)
Frame.BackgroundColor3 = Color3.fromRGB(30, 30, 30)

ScriptButton1.Parent = Frame
ScriptButton1.Size = UDim2.new(0, 180, 0, 50)
ScriptButton1.Position = UDim2.new(0, 10, 0, 10)
ScriptButton1.Text = "Script 1"
ScriptButton1.MouseButton1Click:Connect(function()
    loadstring(game:HttpGet("https://example.com/seuscript1.lua"))()
end)

ScriptButton2.Parent = Frame
ScriptButton2.Size = UDim2.new(0, 180, 0, 50)
ScriptButton2.Position = UDim2.new(0, 10, 0, 70)
ScriptButton2.Text = "Script 2"
ScriptButton2.MouseButton1Click:Connect(function()
    loadstring(game:HttpGet("https://example.com/seuscript2.lua"))()
end)
# hubxs
