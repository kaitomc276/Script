local ScreenGui = Instance.new("ScreenGui")
local ImageButton = Instance.new("ImageButton")
local UICorner = Instance.new("UICorner")

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

ImageButton.Parent = ScreenGui
ImageButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
ImageButton.BorderSizePixel = 0
ImageButton.Position = UDim2.new(0.10615778, 0, 0.16217947, 0)
ImageButton.Size = UDim2.new(0, 40, 0, 40)
ImageButton.Draggable = true
ImageButton.Image = "http://www.roblox.com/asset/?id=1081002842"

UICorner.CornerRadius = UDim.new(1, 10) 
UICorner.Parent = ImageButton

ImageButton.MouseButton1Down:Connect(function()
    game:GetService("VirtualInputManager"):SendKeyEvent(true, Enum.KeyCode.End, false, game)
end)

local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()
repeat wait() until game:IsLoaded()
local Window = Fluent:CreateWindow({
    Title = "kaitoMC276",
    SubTitle = "kaitoMC276",
    TabWidth = 160,
    Size = UDim2.fromOffset(500, 320),
    Acrylic = true,
    Theme = "135340321174352",
    MinimizeKey = Enum.KeyCode.End
})
local Tabs = {
        Main0=Window:AddTab({ Title="Main" }),
        Main1=Window:AddTab({ Title="Item" }),
        Main2=Window:AddTab({ Title="Quest" }),
        Main3=Window:AddTab({ Title="Dojo" }),
        Main4=Window:AddTab({ Title="Sea Event" }),
        Main5=Window:AddTab({ Title="Setting" }),
        Main6=Window:AddTab({ Title="Race V4" }),
        Main7=Window:AddTab({ Title="Raid" }),
        Main8=Window:AddTab({ Title="Volcanic" }),
        Main8=Window:AddTab({ Title="Misc" }),
}
Tabs.Main0:AddButton({
    Title = "Auto Farm Level",
    Description = "",
    Callback = function()
        print("ditmemay")
    end
})
Tabs.Main0:AddButton({
    Title = "Auto Farm Nearest",
    Description = "",
    Callback = function()
        print("ditmemay")
    end
})
Tabs.Main0:AddButton({
    Title = "Auto Farm Bone",
    Description = "",
    Callback = function()
        print("ditmemay")
    end
})
Tabs.Main0:AddButton({
    Title = "Auto Farm Katakuri",
    Description = "",
    Callback = function()
        print("ditmemay")
    end
})
