# Galaxy Library
Simple, Clean, Fresh, Friendly Interface By Jan & Wally

## Set-up The Library Loadstring
```lua
local Galaxy = loadstring(game:HttpGet("https://raw.githubusercontent.com/ArzyScripts/Library-UI/main/Galaxy%20Library/LibraryUI.lua", true))()
```

## Creating an Window
```lua
local Window = Galaxy:CreateWindow("Your Title")
```

## Creating an Folder (Tab)
```lua
local Folder = Window:AddFolder("Folder")
```

## Creating an Button
```lua
local Button = Folder:AddButton({
	text = "This is An Button",
	flag = "button",
	callback = function()
	   print("Clicked")
  end
})
```

## Adding Toggle
```lua
local Toggle = Folder:AddToggle({
	text = "Toggle",
	flag = "toggle",
	callback = function(Value)
	   print("Toggled")
  end
})
```

## Creating an Slider
```lua
local Slider = Folder:AddSlider({
	text = "FOV",
	min = 70,
	max = 170,
	dual = true,
	type = "slider",
	callback = function(Value)
	   print("Slided")
  end
})
```

## Creating an Dropdown
```lua
local Dropdown = Folder:AddList({
    text = "Pick a Number",
    values = {"One", "Two", "Three"},
    open = false,
    flag = "number_option"
    callback = function(Value)
        print("Selected number:", Value)
    end
})
```

## Creating an Label
```lua
local Label = Folder:AddLabel({text = "An Interface Made By Jan & Wally", type = "label"})
```

## Creating an Bind
```lua
local Keybind = Folder:AddBind({
    text = "Keybind",
    key = "LeftControl",
    hold = false,
    callback = function()
      print("Keybind had been set")
    end
})
```

## Creating an Colorpicker
```lua
local Colorpicker = Folder:AddColor({
	text = "Color Picker",
	flag = "color",
	type = "color",
	callback = function(Value)
	   print("You have picked a color")
  end
})
```

## Close Library (FUNCTION)
```lua
Galaxy:Close()
```

## Load The Interface (THIS IS REQUIRED OR ELSE THE INTERFACE WONT SHOW)
```lua
Galaxy:Init()
```

### UI Developers: Jan & Wally
