# GrandHubX UI Script

This script is designed to create a customizable and interactive User Interface (UI) for Roblox games using the `GrandHubX` library. The script includes features like buttons, toggles, sliders, dropdowns, textboxes, separators, and lines. Below is a detailed explanation of the script's functionality and usage.

---

## Script Overview

### 1. **Loading the Library**
```lua
local GrandHubX = loadstring(game:HttpGet("https://raw.githubusercontent.com/KingTIM3R/Ui_Final/refs/heads/main/source.lua", true))()
```
This line fetches and executes the `GrandHubX` UI library from the specified URL. It initializes the core functionality needed to build the UI.

---

### 2. **Creating the Main Window**
```lua
local Library = GrandHubX:Window("GrandHubX","","",Enum.KeyCode.RightControl)
```
This creates the main UI window with the following parameters:
- **Name**: `"GrandHubX"` (displayed title of the UI).
- **Game Name**: Left empty (`""`) to automatically detect the current game.
- **Logo**: Left empty (`""`) as no logo is provided.
- **Keybind**: `Enum.KeyCode.RightControl` toggles the UI on/off.

---

### 3. **Adding a Tab**
```lua
Tab1 = Library:Tab("Main")
```
Creates a new tab labeled `"Main"`. Tabs help organize elements within the UI.

---

## UI Elements

### 1. **Button**
```lua
Tab1:Button("Button",function()
    print("hi")
end)
```
- **Label**: `"Button"`.
- **Functionality**: When clicked, it prints `"hi"` to the console.

---

### 2. **Toggle**
```lua
Tab1:Toggle("Toggle",false,function(value)
    print(value)
end)
```
- **Label**: `"Toggle"`.
- **Initial State**: `false` (off).
- **Callback**: Prints the toggle state (`true` or `false`) to the console.

---

### 3. **Slider**
```lua
Tab1:Slider("Slider",1,100,25,function(value)
    print(value)
end)
```
- **Label**: `"Slider"`.
- **Range**: `1` (min) to `100` (max).
- **Default Value**: `25`.
- **Callback**: Prints the slider's current value to the console.

---

### 4. **Dropdown**
```lua
Tab1:Dropdown("Dropdown",{"Sub","To","GrandLegacy(grand_lostsoulz0 on yt)"},function(value)
    print(value)
end)
```
- **Label**: `"Dropdown"`.
- **Options**: `{"Sub", "To", "GrandLegacy(grand_lostsoulz0 on yt)"}`.
- **Callback**: Prints the selected option to the console.

---

### 5. **Separator**
```lua
Tab1:Seperator("Seperator")
```
Adds a visual separator labeled `"Seperator"`. Used for grouping UI elements.

---

### 6. **Line**
```lua
Tab1:Line()
```
Adds a horizontal line for visual clarity.

---

## How to Use

1. Copy the script and paste it into your Roblox script editor.
2. Modify the parameters for buttons, toggles, sliders, dropdowns, and other elements as needed.
3. Run the script to see the UI in action.

---

## Example Output
The script creates a UI similar to the following structure:

- **Main Tab:**
  - Button: Prints `"hi"` when clicked.
  - Toggle: Switches between `true` and `false` states.
  - Slider: Adjusts between a range of `1` to `100`.
  - Dropdown: Allows selection from predefined options.
  - Separator and Line: Improves visual organization.

---

## Notes
- The script uses the `GrandHubX` library, fetched dynamically from the provided URL.
- Ensure you have an active internet connection to load the library.
- Customize the UI labels, default values, and callbacks as per your requirements.

---

