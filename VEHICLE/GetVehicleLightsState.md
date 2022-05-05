---
ns: VEHICLE
---
## GET_VEHICLE_LIGHTS_STATE

```c
// 0xB91B4C20085BD12F 0x7C278621
BOOL GET_VEHICLE_LIGHTS_STATE(Vehicle vehicle, BOOL* lightsOn, BOOL* highbeamsOn);
```

## Examples

```lua
local playerPed = PlayerPedId()
local vehicle = GetVehiclePedIsIn(playerPed, false)
local retval, lightsOn, highbeamsOn = GetVehicleLightsState(vehicle)

if retval  == 1 then
    if lightsOn == 1 and highbeamsOn == 1 then
        print('off')
    elseif lightsOn == 0 and highbeamsOn == 0 then
        print('low beam')
    elseif lightsOn == 1 and highbeamsOn == 0 then
        print('high beam'
    end
end
```


## Parameters
* **vehicle**: 
* **lightsOn**: 
* **highbeamsOn**: 

## Return value
