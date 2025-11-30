# REDz V2
This documentation is for A Stable Release Of REDz V2

## Load REDz V2
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/ArzyScripts/Library-UI/main/REDz%20V2/Library.lua"))()
```

## Creating a REDz V2
```lua
MakeWindow({
  Hub = {
    Title = "REDz Interface Suite",
    Animation = "Made by tlredz"
  },
  Key = {
    KeySystem = false,
    Title = "Key System",
    Description = "This is an Key System",
    KeyLink = "",
    Keys = {"12345"},
    Notifi = {
      Notifications = true,
      CorrectKey = "Key Correct, Loading Interface Suite...",
      Incorrectkey = "Key is Invalid...",
      CopyKeyLink = "Copied to Clipboard"
    }
  }
})
```

## Minimize Button (Toggle)
```lua
MinimizeButton({
  Image = "",
  Size = {40, 40},
  Color = Color3.fromRGB(10, 10, 10),
  Corner = true,
  Stroke = false,
  StrokeColor = Color3.fromRGB(255, 0, 0)
})
```

## Creating a Tab
```lua
local Tab = MakeTab({Name = "Tab 1"})
```

## Creating a Notify
```lua
MakeNotifi({
  Title = "REDz Interface Suite",
  Text = "This is an notification, what would the content be...",
  Time = 5
})
```

## Creating a Section
```lua
local Section = AddSection(Main, {"General"})
```

## Set Section
```lua
SetSection(Section, "New Section")
```

## Creating a Button
```lua
AddButton(Main, {
  Name = "Button",
  Callback = function()
  -- Script Here
  end
})
```

## Creating a Toggle
```lua
local Toggle = AddToggle(Main, {
  Name = "Toggle",
  Default = false,
  Callback = function(Value)
   -- Script Here
  end
})
```

## Creating a Mobile Toggle
```lua
local MobileToggle = AddMobileToggle({
  Name = "Toggle",
  Visible = true,
  Callback = function(Value)
   -- Script Here
  end
})
```

## Creating a Slider
```lua
local Slider = AddSlider(Main, {
  Name = "Slider",
  MinValue = 10,
  MaxValue = 100,
  Default = 25,
  Increase = 1,
  Callback = function(Value)
   -- Script Here
  end
})
```

## Creating a Keybind
```lua
AddKeybind(Main, {
  Name = "Keybind",
  KeyCode = "LeftControl",
  Default = false,
  Callback = function(Value)
   -- Script Here
  end
})
```

## Creating a Textbox
```lua
AddTextBox(Main, {
  Name = "Textbox",
  Default = "Cool UI!",
  PlaceholderText = "Type here...",
  ClearText = true,
  Callback = function(Value)
   -- Script Here
  end
})
```

## Creating a Dropdown
```lua
local Dropdown = AddDropdown(Main, {
  Name = "Dropdown",
  Options = {"1", "2", "3"},
  Default = "1",
  Callback = function(Value)
   -- Script Here
  end
})
```

## Creating a Color Picker
```lua
AddColorPicker(Main, {
  Name = "Colorpicker",
  Default = Color3.fromRGB(255, 255, 0),
  Callback = function(Value)
   -- Script Here
  end
})
```

## Creating a Paragraph
```lua
local Paragraph = AddParagraph(Main, {"Paragraph", "Hey"})
```
## Creating a Set Paragraph 
```lua
SetParagraph(Paragraph, {"Paragraph", "A New Paragraph"})
```

## Creating a Label
```lua
local Label = AddTextLabel(Main, "Made by tlredz")
```

## Creating a Set Label
```lua
SetLabel(Label, "A New Label")
```

## Creating a Image Label
```lua
local Image = AddImageLabel(Main, {
  Name = "Image",
  Image = "rbxassetid://"
})
```

## Set Image
```lua
SetImage(Image, "rbxassetid://4155801252")
```

## Destroy Interface
```lua
DestroyScript()
```

### Update Functions

## Update Toggle
```lua
UpdateToggle(Toggle, true)
```

## Update Slider
```lua
UpdateSlider(Slider, 25)
```

## Update DropDown
```lua
UpdateDropdown(Dropdown, {"Haki", "Fighting", "PVP"})
```
