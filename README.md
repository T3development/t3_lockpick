# t3_lockpick

A lockpick minigame for use with other scripts

## Installation

> Drag *t3_lockpick* into your server's resources folder and add `ensure t3_lockpick` to your *server.cfg*.

> Configure the options to your liking in *config.lua*.

> In your scripts that use lockpicking add the export `exports["t3_lockpick"]:startLockpick([item or strength], difficulty, pins)`. This export returns true if successful, or false if unsuccessful.

> Restart your server.

## Example

```lua
---@param item string|float?
---@param difficulty number?
---@param pins number?
local success = exports["t3_lockpick"]:startLockpick(item, difficulty, pins)
if success then
    -- Unlock vehicle
else
    -- Remove lockpick
end
```

## Support

Support and updates are offered through our Discord: https://discord.gg/t3dev