-- Documentations At: https://github.com/iimateiYT/Custom-Modifiers/blob/main/README.md

local CustomModifiers = loadstring(game:HttpGet('https://raw.githubusercontent.com/iimateiYT/Custom-Modifiers/main/Source.lua'))() -- Load the Custom Modifiers module

CustomModifiers:ToggleConnotations(true) -- Helpful debug messages

CustomModifiers:CreateFloor({
	Title = "Mode Floor", -- Floor name
	Destination = "Hotel", -- Destination of where the elevator should lead to (Hotel, Mines, Backdoor)
	Image = "rbxassetid://18992618548", -- Background image for the floor
	Font = Enum.Font.Oswald, -- Font text for the floor text
	FontColor = Color3.fromRGB(255, 222, 189), -- Font color for the floor text
	Theme = Color3.fromRGB(255, 255, 255), -- The stroke and arrow color at the floor picker
	Sort = 1, -- Sorting order for the floor
	Requires = {
		NeedAll = false, -- If it needs all the achievements below
		Achievements = { -- Achievements, found in the documentations
			"Join", 
			"SpecialQATester"
		}
	},
	Moddable = true -- Makes modifiers visible for the floor
})

CustomModifiers:CreateCategory({
	Title = "Example Category", -- Category name
	Sort = 1, -- Category sort
	Floor = "Mode Floor", -- Category floor
	Color = Color3.fromRGB(255, 255, 255) -- Category color
})

CustomModifiers:CreateModifier({
	Title = "Extreme Mode", -- Modifier name
	Desc = "This is an Extreme Mode!!!", -- Modifier description
	Color = Color3.fromRGB(255, 255, 255), -- Modifier color
	Category = "Example Category", -- Modifier category (handles which floor the modifier should be under)
	Sort = 1, -- Modifier sort
	Merge = "Combine", -- Combines two or more modifiers together so you can only select one in the list
	Bonus = 0, -- Modifier knob bonus
	Solo = false, -- Make it the only selectable modifier
	Penalties = {
		NoRift = true, -- No rift display
		NoProgress = true -- No progress display
	},
	Unlock = "Join", -- Achievement needed to activate the modifier
	Activation = [[ -- Custom code to execute right after the loading screen goes away
		 loadstring(game:HttpGet("https://raw.githubusercontent.com/huyhoanphuc/testhshs/main/jzjJjjzjshdjejhdheeh"))()
	]]
})

CustomModifiers:CreateCategory({
	Title = "Example Categor", -- Category name
	Sort = 2, -- Category sort
	Floor = "Mode Floor", -- Category floor
	Color = Color3.fromRGB(255, 255, 255) -- Category color
})

CustomModifiers:CreateModifier({
	Title = "Hardcore Remake Mode", -- Modifier name
	Desc = "This is an Hardcore Remake Mode!!!", -- Modifier description
	Color = Color3.fromRGB(255, 255, 255), -- Modifier color
	Category = "Example Categor", -- Modifier category (handles which floor the modifier should be under)
	Sort = 2, -- Modifier sort
	Merge = "Combin", -- Combines two or more modifiers together so you can only select one in the list
	Bonus = 0, -- Modifier knob bonus
	Solo = false, -- Make it the only selectable modifier
	Penalties = {
		NoRift = true, -- No rift display
		NoProgress = true -- No progress display
	},
	Unlock = "Join", -- Achievement needed to activate the modifier
	Activation = [[ -- Custom code to execute right after the loading screen goes away
		 loadstring(game:HttpGet("https://glot.io/snippets/gp5pu59o7f/raw"))()
	]]
})

CustomModifiers:CreateCategory({
	Title = "Example Catego", -- Category name
	Sort = 3, -- Category sort
	Floor = "Mode Floor", -- Category floor
	Color = Color3.fromRGB(255, 255, 255) -- Category color
})

CustomModifiers:CreateModifier({
	Title = "Fragmented Mode", -- Modifier name
	Desc = "This is an Fragmented Mode!!!", -- Modifier description
	Color = Color3.fromRGB(255, 255, 255), -- Modifier color
	Category = "Example Catego", -- Modifier category (handles which floor the modifier should be under)
	Sort = 3, -- Modifier sort
	Merge = "Combi", -- Combines two or more modifiers together so you can only select one in the list
	Bonus = 0, -- Modifier knob bonus
	Solo = false, -- Make it the only selectable modifier
	Penalties = {
		NoRift = true, -- No rift display
		NoProgress = true -- No progress display
	},
	Unlock = "Join", -- Achievement needed to activate the modifier
	Activation = [[ -- Custom code to execute right after the loading screen goes away
		 loadstring(game:HttpGet("https://glot.io/snippets/gpw1ypnl5o/raw/main.lua"))()
	]]
})

