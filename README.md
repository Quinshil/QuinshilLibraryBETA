# QuinshilLibraryBETA
It's really simple to use, soon, hopefully, i will release actual library.


# How to use it?
As i said, really simple, here are some tips:


**Getting Loadsting**
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Unknown56406516401563456/Peacock-Lib/main/src.lua"))()

**Creating UI Library Window**
local Window = Library:CreateLib {
	name = "Name"
}

**Creating Tabs**
local Tab = Window:NewTab({
	name = "Name",
	icon = "rbxassetid://3926305904"
})

**Creating Buttons**
local Button = Tab:NewButton({
	name = "Name"
})
Button:SetCallback(function()
	
end)

**Creating Labels**
local Label = Tab:NewLabel({
	name = "Name"
})

**Creating Sliders**
local Slider = Tab:NewSlider({
	name = "Name",
	min = "16", -- (min 16) to (max 100) min is the lowest max is the highest and default choose to 16 to 100
	max = "100",
	default = "16"
})
Slider:SetCallback(function(v)
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = v -- if you want JumpPower Change the WalkSpeed To JumpPower
end)

**Creating Toggles**
local Toggle = Tab:NewToggle({
	name = "Name"
})
Toggle:SetCallback(function(v)
	print(v)
end)
