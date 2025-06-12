# FiveM Case Opening

Standalone, highly customizable case opening resource.

## Features
The resource can be triggered using the "case_opening:openCase" passing 2 arguments
  - case ID (specified in the config.js)
  - callback

Example usage - Server Script
```lua
TriggerEvent("case_opening:server:openCase","caseID",playerID)
RegisterNetEvent("case_opening:server:getReward",function(reward)
    print("Yay! I won",reward)
end)
```

### The resource can handle different specific scenarios 
- If the event gets triggered with an invalid case ID the result will be *false*
- If a case is already opening the result will be *false*

## To-Do
- The resource currently has no sound effects, I'm planning to add some
