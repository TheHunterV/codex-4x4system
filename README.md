# CodeX 4x4 System
![codex-4x4system](https://github.com/5M-CodeX/codex-4x4system/assets/112611821/3b10a9ad-e68e-47bb-af42-1177c26ec977)

The CodeX 4x4 System is a script for Grand Theft Auto V (GTA V) that allows players to toggle between 4x4 mode and 2WD (rear-wheel drive) mode in compatible vehicles. This system enhances the off-road and all-terrain capabilities of SUVs, vans, and off-road vehicles by adjusting vehicle handling parameters.

## Usage
To use the CodeX 4x4 System in GTA V, follow these instructions:

In the game, open the chat or console.

Enter the following command to toggle 4x4 mode on/off: `/4x4`

## Configurables
The script provides some configurable parameters at the beginning of the code. These parameters can be adjusted to fine-tune the behavior of the 4x4 system:
```lua
local fourwheelsc = false -- Default to 4x4 off

-- Vehicle class identifiers
local SUVClass = 2
local OffRoadClass = 9
local VanClass = 12
local Class8 = 18
```
fourwheelsc: Determines whether 4x4 mode is initially turned on (true) or off (false) when you start the game.

Vehicle class identifiers: These are used to specify which types of vehicles are compatible with the 4x4 system. By default, it includes SUVs, off-road vehicles, vans, and Class 8 vehicles. You can modify these class identifiers to include or exclude specific vehicle types.

## Features
The script automatically adjusts the handling parameters of compatible vehicles when you enter them.

In 4x4 mode, it increases the front-wheel drive bias, acceleration, and top speed, providing better off-road performance.

In 2WD mode, it shifts the power to the rear wheels, returning the vehicle to its default handling characteristics.

## Notes
If you are not in a compatible vehicle, attempting to toggle 4x4 mode will display an error message.

The script includes an automatic mode that periodically checks if you are in a compatible vehicle and applies the appropriate mode (4x4 or 2WD) based on the current setting.
