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
	Text = "This is An Button",
	Flag = "button",
	Callback = function()
	   print("Clicked")
  end
})
```

## Adding Toggle
```lua
local Toggle = Folder:AddToggle({
	Text = "Toggle",
	Flag = "toggle",
	Callback = function(Value)
	   print("Toggled")
  end
})
```

## Creating an Slider
```lua
local Slider = Folder:AddSlider({
	Text = "FOV",
	Min = 70,
	Max = 170,
	Dual = true,
	Type = "slider",
	Callback = function(Value)
	   print("Slided")
  end
})
```

## Creating an Dropdown
```lua
local Dropdown = Folder:AddList({
    Text = "Pick a Number",
    Values = {"One", "Two", "Three"},
    Open = false,
    Flag = "number_option"
    Callback = function(Value)
        print("Selected number:", Value)
    end
})
```

## Creating an Label
```lua
local Label = Folder:AddLabel({Text = "An Interface Made By Jan & Wally", Type = "label"})
```

## Creating an Bind
```lua
local Keybind = Folder:AddBind({
    Text = "Keybind",
    Key = "LeftControl",
    Hold = false,
    Callback = function()
      print("Keybind had been set")
    end
})
```

## Creating an Colorpicker
```lua
local Colorpicker = Folder:AddColor({
	Text = "Color Picker",
	Flag = "color",
	Type = "color",
	Callback = function(Value)
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
